# Module 14 Panel Briefs

Source: Week5-InstructorGuide.docx section 7, expanded with BRS, Module 10 and Module 14 model answers, and the Module 13 deck.

## Facilitator Page (keep this page)

- Each team gets 12 minutes: 8 for the demo, then 4 for challenges. That's room for about two to four challenges, so don't let every panelist ask both of theirs every time. Spread them across teams so each one gets a mix.
- Ask your challenge as written, then follow up once if the first answer is weak. Don't feed teams the answer.
- Behaviours you're scoring (from the slide): **structure, tailoring, evidence, composure, follow-through**. Every challenge should end with an outcome and an owner. "We'll look into it" with no owner loses credit.
- Common mistakes the guide calls out: a feature tour instead of a story, agreeing to stop-loss in the room, and no ask at the end.
- The response the Module 13 deck teaches: **listen, acknowledge, clarify, answer with evidence, agree the next step**.

## Card 1: Programme Sponsor

**Who you are:** Head of Digital Distribution. You own the business case and give final sign-off. You want to launch something impressive, and you're used to people saying yes to you.

**How to play it:** Friendly and senior, but use your authority. Your first challenge is scope pressure. Your second checks whether the team can tie its work to the BRS.

### Challenge 1: "Can we add stop-loss orders before launch?"

- *Push if they hesitate:* "It's a small change, surely. Our competitors all have it."
- *A good response:* Neither agrees nor refuses in the room. Asks what problem a stop-loss would solve for Joanna. Points out that the contract has no order types, so this is an engineering change, not just a screen change. Logs the request in your words and routes it to the product owner with a follow-up date, such as the next sprint review.
- *Red flag:* "Yes, we can add that," or a flat "No, it's out of scope."

### Challenge 2: "How does this meet success criterion 1?"

- *What success criterion 1 says (BRS section 11):* "A client can register, sign in, place an order and see it reflected in their holdings and blotter end to end."
- *A good response:* Walks you through the end-to-end flow in the prototype and shows the order moving to filled. Names any gaps honestly, for example that the holdings update depends on the build, or that live status relies on BR-07.
- *Red flag:* Vague claims with no reference to the BRS, or citing a different requirement as if it were criterion 1.
- *Instructor note:* The model answer links "an order ticket a first-time client can use unaided" to success criterion 1, but that wording is closer to BRS 9.5 (Usability). Accept either answer if the team can show the flow.

**Facts to have ready:** Advised and discretionary dealing are out of scope (BRS 4.2). OrderStatus values are NEW, FILLED, REJECTED and CANCELLED.

## Card 2: Trading Desk (David)

**Who you are:** David, head of trading operations. You don't use the client-facing platform, but you're accountable for every trade it produces. For any trade a client disputes, you need to be able to explain what happened and when without asking engineering to dig through logs.

**How to play it:** Practical and a little impatient. You care about risk and about getting fewer calls to the desk.

### Challenge 1: "Every order must show a risk warning."

- *Push if they cave:* "Every single order. I don't want clients saying they weren't told."
- *A good response:* Acknowledges the concern, then cites the evidence on time to trade: Joanna wants to place a trade in under a minute and has no patience for multi-step confirmations (BRS persona, 9.5). Offers a compromise, such as a warning on the first order only, and routes the decision to **Compliance**, since the wording is theirs. Logs it as "Decision needed," with Compliance as owner.
- *Red flag:* Adds a warning to every order on the spot, or dismisses the concern.

### Challenge 2: "How will I see why an order was rejected?"

- *A good response:* Answers for both audiences. The client sees a plain-language message mapped to each error code (ORD-400, VAL-422, INS-404, ACC-403 and so on), never a raw API message. For you, the permission matrix gives Operations read access to trade lifecycle lookups (BR-15). The strongest teams will also admit the contract gap: the API only allows access to the token's own account, so there is no read-any route for operations yet. That's an open question for the Engineering lead.
- *Red flag:* "The error message will show," with no mapping to the codes, or no answer for David's own view.

**Facts to have ready:** The error codes are ACC-404, ACC-403, INS-404, ORD-400, ORD-409, VAL-422, AUTH-401 (plus AUTH-409 and MKT-503). There is no partial fill.

## Card 3: Risk and Compliance

**Who you are:** Second line of defence. You assume a regulator could inspect the trade records at any time, without notice (BRS 9.4). You're measured and precise, and you notice when someone guesses.

**How to play it:** Calm and probing. You're testing whether teams know the limits of their own knowledge.

### Challenge 1: "Who can see client balances internally?"

- *A good response:* Points to the role and permission matrix and to BRS 9.3 (internal access limited to what the role requires). States the central finding honestly: the contract defines only two roles, CUSTOMER and ADMIN, which can't express least privilege for five business roles. ADMIN is broader than support needs, and Operations and Compliance roles don't exist yet. The role gap goes to the Engineering lead together with Risk and Compliance.
- *Push:* "So today, could a support operator see every client's balance?" Teams should admit yes, ADMIN could, and treat that as an open gap.
- *Red flag:* "Only authorised staff," with no specifics.

### Challenge 2: "Is this accessible to vulnerable customers? Think Consumer Duty."

- *A good response:* Cites the WCAG 2.2 AA findings log from Module 07 (twelve gaps fixed in the spec) and BRS 9.5. Then, crucially, says they can't confirm Consumer Duty compliance themselves and routes it to Compliance with a follow-up date. Module 13 teaches: "never guess about rules or compliance."
- *Red flag:* "Yes, it's fully compliant."
- *Background for you (not in the course materials):* Consumer Duty is the FCA's UK rule (in force since July 2023) requiring firms to deliver good outcomes for retail customers, including customers in vulnerable circumstances. One of its outcomes is consumer understanding. The BRS doesn't mention it, which is exactly why a team shouldn't claim compliance.

**Facts to have ready:** GET /balance returns cash only, and market value comes from portfolio-api.yaml (Sprint 10). A suspended account gets ACC-403, the same code as "not yours."

## Card 4: Engineering Lead

**Who you are:** You'll build what's in the spec. You want nothing left to guess, and you know the API contracts better than anyone in the room.

**How to play it:** Direct and technical. Your challenges catch specs that drift from the contract.

### Challenge 1: "Where does the indicative price come from?"

- *A good response:* Admits it isn't in trade-api.yaml. BR-13 asks for it, but it's only a "Should." Logs it as an open question with you as owner, and marks the indicative price in the field table as "pending data source." That's exactly the model answer's spec change for version 0.3.
- *Red flag:* Invents a source, such as "from the market data feed," without evidence.

### Challenge 2: "Your spec shows a state our API cannot produce."

- *Which state to point to:* Look for "Partially filled" (the API has no partial fill), any status beyond NEW, FILLED, REJECTED or CANCELLED, or a screen that treats a 200 response as done. A 200 can return NEW (Sprint 7).
- *If you can't find one in their spec:* Ask, "Walk me through how your states map to OrderStatus."
- *A good response:* Checks the state diagram against the contract in front of you, agrees to remove the state or mark it as needing a contract change, and logs a versioned spec change.
- *Red flag:* "That's how users think about it," with no plan to reconcile it with the contract.

**Facts to have ready:** OrderStatus values are NEW, FILLED, REJECTED and CANCELLED. Access tokens expire 15 minutes after issue. The only roles are CUSTOMER and ADMIN.
