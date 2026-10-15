# Financial Services Glossary for Instructors

*Neueda / Fidelity Investments new-hire programme: Systems Analyst and Engineering tracks. Draft for review.*

## Before you use this glossary

Never go past a word you don't fully understand. When a student goes blank or loses the thread, look back for a word they skipped over, and clear it up before you move on. That rule applies to us as instructors too: this programme is built on a trading platform, and it uses many words that have an everyday meaning, a software meaning, and a different financial meaning.

This glossary defines the financial-industry terms used in the course materials, plus a few standard industry terms the course does not use but students may still ask about. Each entry gives:

- **The definition**, written to stand on its own.
- **Where it shows up:** the first place the term appears in each track, in teaching order (week, module, slide). "M03 handout: LEAP BRS" is the Business Requirements Specification SA students read in Week 1, Module 03; Engineering students first receive it at the Week 1 Friday joint kickoff. "Not in course materials" marks these added terms.
- **Course note**, where the course uses the term in a narrower, non-standard or inconsistent way, or where the same word means something else elsewhere in the course.

## 0-9

**401(k):** In the US, an employer-sponsored retirement savings plan, named after a section of the tax code, in which employees contribute part of their pay, often matched by the employer, and choose from a set of investment options.

- *Where it shows up:* Not in course materials
- *See also:* Workplace pension, IRA (Individual Retirement Account)

**88 level (condition name):** In COBOL, a data entry with level number 88 that gives a name to one or more specific values of a field, so a program can test a readable condition (for example IF ACCOUNT-CLOSED) instead of comparing the raw value.

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 7
- *See also:* COBOL (Common Business-Oriented Language), PIC clause, Record layout (copybook)

## A

**Account:** An arrangement between a customer and a financial firm, identified by an account number, under which the firm holds the customer's cash and investments and records every transaction made on the customer's behalf. One client can hold several accounts.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 6; Engineering track: Wk 3, M02 OO Principles in Practice, slide 7
- *Course note:* The course also uses 'account' for AWS, tool and login accounts; make the distinction explicit when both senses appear.
- *See also:* Client, Brokerage account, Account status, Cash balance

**Account status:** A recorded state of an account, such as active, restricted (suspended) or closed, that determines which activity the firm allows. A firm may restrict an account, for example for a compliance review or a trading violation, blocking new trades.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 7
- *Course note:* The course uses ACTIVE, SUSPENDED and CLOSED; a suspended account is blocked from trading, for example by Compliance. Real firms use more varied statuses and partial restrictions.
- *See also:* Account, Client onboarding

**Advised dealing (advised service):** A service in which the firm gives the client a personal recommendation, suited to the client's circumstances, on whether to buy or sell an investment before the client decides to trade. The firm is responsible for the suitability of that advice.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Discretionary dealing, Retail trading platform, Dealer

**Algorithmic trading (automated trading strategy):** Trading in which a computer program automatically generates and submits orders according to predefined rules, such as price, timing, or volume conditions, without a person deciding each individual trade.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *See also:* Order, Trade signal, Execution

**AML (Anti-Money Laundering):** The laws, controls and procedures that financial firms use to detect and prevent criminals from disguising illegally obtained money as legitimate funds. A firm's AML program includes verifying client identity, monitoring transactions and reporting suspicious activity to authorities.

- *Where it shows up:* Not in course materials
- *See also:* KYC (Know Your Customer), Identity verification, Compliance

**Ask (offer):** The lowest price at which a seller is currently willing to sell a security, and so the price at which a buyer can buy immediately. The ask is normally higher than the bid.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 6
- *See also:* Bid, Bid-ask spread, Quote

**Asset class:** A category of investments that share similar characteristics and behave in similar ways in the market. Stocks (equities), bonds and cash are the traditional main asset classes; others include real estate, commodities, currencies and crypto assets.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course treats FX and crypto as asset classes alongside equities, and uses 'instrument class', 'trade type' and an asset_class field loosely as near-synonyms.
- *See also:* Instrument (financial instrument), Equity (share, stock), Bond, FX (foreign exchange)

**Audit trail:** A chronological, tamper-resistant record of the actions taken on a piece of data or a transaction, showing what happened, who did it and when. Regulated firms keep audit trails so that orders and records can be reconstructed and checked later.

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 9; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course's BRS uses it narrowly for the permanent record of an order from submission to outcome. It is also used in the security sense (for example, logging of Kafka access-control changes).
- *See also:* Record-keeping (regulatory), Books-and-records rules (SEC Rule 17a-4), Control (control environment)

## B

**Back office:** The operations and support functions of a financial firm that handle work after a trade is executed, such as confirmation, settlement, record-keeping, reconciliation and client account servicing. It does not deal with clients or make trading decisions.

- *Where it shows up:* SA track: Wk 3, M10 handout: 10-ProcessMappingWorkshop
- *See also:* Front office, Middle office, Settlement, Reconciliation

**Basis point:** One hundredth of one percentage point (0.01%), used to state small changes in interest rates, yields, and fees precisely. A rise from 5.00% to 5.25% is 25 basis points, often written 25 bps.

- *Where it shows up:* Not in course materials

**Batch processing (batch job):** Running a program without user interaction to process a large volume of records in one scheduled run, often overnight or at the end of the business day, rather than one transaction at a time in real time. A single scheduled run is a batch job.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 10; Engineering track: Wk 3, M13 Mission Build, slide 5
- *Course note:* Aliases Control-M and IBM Workload Scheduler are commercial job schedulers that run batch jobs in order and on time.
- *See also:* Batch window, JCL (Job Control Language), Mainframe, Extract file

**Batch window:** The scheduled period, usually overnight when online activity is low, in which batch jobs must run and finish, often under a service level agreement. Online changes to the affected data are typically restricted during the window.

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 11; Engineering track: Wk 7, M11 Accessing Data Through APIs, slide 10
- *See also:* Batch processing (batch job), Mainframe, Extract file

**Best execution:** A broker's duty to use reasonable diligence to get the most favorable terms reasonably available for a client's order, considering price and factors such as speed and likelihood of execution. In the US it is set out in FINRA Rule 5310.

- *Where it shows up:* Not in course materials
- *See also:* FINRA (Financial Industry Regulatory Authority), Regulation NMS (National Market System)

**Bid:** The highest price a buyer is currently willing to pay for a security, and so the price at which a holder can sell immediately. The bid is normally lower than the ask.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 6
- *See also:* Ask (offer), Bid-ask spread, Quote

**Bid-ask spread:** The difference between the bid price (the highest price a buyer will pay) and the ask price (the lowest price a seller will accept) for a security at a given moment. A narrow spread usually indicates high liquidity.

- *Where it shows up:* Not in course materials
- *See also:* Bid, Ask (offer), Liquidity, Quote

**Blotter:** A chronological record of orders or trades, typically showing for each one the instrument, side, quantity, price, time, and status. US broker-dealers must keep blotters as records of original entry for all purchases and sales.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 7; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses a client-facing blotter (a client's own order history). In industry a blotter is usually a trader's, desk's, or firm's log.
- *See also:* Order, Trade, Order status

**Bollinger Bands:** A technical-analysis indicator made of two lines plotted a set number of standard deviations above and below a simple moving average of price, most commonly 2 standard deviations around a 20-period average. The bands widen as prices become more volatile.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *Course note:* Appears in the project spec as 'Bollinger-band triggers', i.e. conditions based on price touching or crossing a band.
- *See also:* Moving-average crossover, Volatility

**Bond:** A debt security in which the investor lends money to an issuer, such as a government or company, for a set period. The issuer pays interest and repays the principal (face value) when the bond reaches maturity.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5; Engineering track: Wk 2, M20 RDBMS Modelling Part 1, slide 7
- *Course note:* Bond prices in the engineering dataset are quoted as a percentage of face value (e.g. 98.50), not in currency per unit.
- *See also:* Security (financial), Corporate bond, US Treasury (UST), Gilt

**Book (trading book):** A set of positions and trades that belong to, and are managed by, a particular trader, desk, or business. In banking, the trading book means positions held for short-term trading profit or to hedge other trading positions.

- *Where it shows up:* Engineering track: Wk 3, M01 Core Java Refresher, slide 14
- *Course note:* In the Java module, 'TradeBook' is a collection class holding trade records, which is closer to a list of trades than the industry sense of a set of positions.
- *See also:* Trade, Closing a position, Blotter

**Booking:** The recording of an executed trade in a firm's systems, which updates the trade record, the account's positions and its cash balance. A trade is "booked" once it is officially recorded against the correct account.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 6
- *See also:* Trade capture, Trade lifecycle, Ledger (debit and credit), System of record

**Books-and-records rules (SEC Rule 17a-4):** The US rules that require broker-dealers to create and preserve records of their business, such as orders, trades, account records and communications. Rule 17a-3 says which records to make; Rule 17a-4 sets how long and in what form to keep them, often six years.

- *Where it shows up:* Not in course materials
- *See also:* Record-keeping (regulatory), Audit trail, SEC (Securities and Exchange Commission)

**Broker:** A firm or individual in the business of buying and selling securities on behalf of customers, usually for a commission or fee. A firm that trades for its own account is a dealer, and one that does both is a broker-dealer.

- *Where it shows up:* SA track: Wk 2, M09 Normalisation, slide 15; Engineering track: Wk 8, M05 Hands On Standing Up Kafka, slide 2
- *Course note:* False friend: in the engineering Kafka week, 'broker' means a Kafka server that stores and serves message streams, not a financial intermediary.
- *See also:* Broker-dealer, Counterparty, Exchange (stock exchange)

**Broker trade feed:** A file or electronic message stream from an external broker listing the trades it executed for a firm or its clients, sent so the receiving firm can record and reconcile them. It is usually delivered on a schedule, such as daily.

- *Where it shows up:* SA track: Wk 2, M09 Normalisation, slide 15
- *See also:* Trade capture, Reconciliation, Control totals, Custodian

**Broker-dealer:** A firm in the business of buying and selling securities both for customers (as a broker) and for its own account (as a dealer). In the US, broker-dealers must generally register with the SEC and become members of FINRA.

- *Where it shows up:* Not in course materials
- *See also:* Broker, Counterparty

**Brokerage account:** An account at a broker-dealer through which an investor buys, sells and holds investments such as stocks, bonds and funds. The two main types are cash accounts, where purchases are paid in full, and margin accounts, where the firm lends money for purchases.

- *Where it shows up:* Not in course materials
- *See also:* Account, Self-directed investor, Cash balance, IRA (Individual Retirement Account)

**Business day:** A day on which financial markets and institutions are open for business, normally Monday to Friday excluding public holidays. Settlement dates, payment deadlines and processing schedules are counted in business days, not calendar days.

- *Where it shows up:* SA track: Wk 6, M01 How the Platform Is Built, slide 11
- *See also:* Settlement cycle (T+1, T+2), Trade date, Cut-off

**Buy and hold:** An investment strategy of buying securities and keeping them for a long period, regardless of short-term market movements, rather than trading frequently. It aims to benefit from long-term growth while keeping trading costs and taxes low.

- *Where it shows up:* Engineering track: Wk 7, M07 Exploratory Data Analysis, slide 10
- *See also:* Trader, Security (financial)

## C

**Cash balance:** The amount of uninvested money held in an account at a given time, available to pay for purchases or to withdraw. In US brokerage accounts, uninvested cash is called a free credit balance and may be swept into a bank deposit or money market fund.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course treats cash balance simply as money on the platform available to pay for buys; sweep programs and settlement timing are not modeled.
- *See also:* Cash movement, Account, Portfolio, Deposit and withdrawal

**Cash movement:** Any transfer of money that changes an account's cash balance, such as a deposit, a withdrawal, the payment for a purchase, the proceeds of a sale, or a dividend or interest payment. Each movement is recorded as a debit or credit.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 9; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Cash balance, Deposit and withdrawal, Account, Statement (client statement)

**CASS (Client Assets Sourcebook):** In the UK, the part of the FCA Handbook that sets rules for how investment firms hold and protect client money and client assets. It requires firms to keep client holdings separate from their own and to reconcile their records against them regularly.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4
- *See also:* FCA (Financial Conduct Authority), Regulation (regulator), Record-keeping (regulatory)

**CICS (Customer Information Control System):** An IBM transaction server for z/OS mainframes that runs online applications, often written in COBOL, processing many short user or system requests in real time. It is the online counterpart to overnight batch processing.

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 9
- *See also:* Mainframe, COBOL (Common Business-Oriented Language), Batch processing (batch job)

**Clearing:** The process after a trade and before settlement in which the obligations of buyer and seller are confirmed and calculated, often netted, so the right securities and cash can be exchanged. It is usually carried out through a clearing house.

- *Where it shows up:* Not in course materials
- *See also:* Clearing house (central counterparty), Settlement, Trade lifecycle

**Clearing house (central counterparty):** An organization that stands between the buyer and seller of a trade, becoming the counterparty to each, and guarantees the trade will complete even if one side defaults. In US equities this role is performed by the National Securities Clearing Corporation (NSCC).

- *Where it shows up:* Not in course materials
- *See also:* Clearing, Settlement, Settlement failure

**Client:** A person or organization that receives services from a financial firm, such as holding accounts, trading or receiving advice. Brokerage rules often use the term customer with the same meaning.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 6; Engineering track: Wk 1, M09 Introduction to GenAI in Engineering At Fidelity, slide 4
- *Course note:* In the course a client links to an advisor, accounts and model portfolios. The word is also used for database clients (psql, pgAdmin).
- *See also:* Account, Retail client (retail investor), Financial advisor, Client onboarding

**Client onboarding:** The process of taking on a new client and opening an account, which includes collecting and verifying identity and financial information, completing know-your-customer and anti-money-laundering checks, and setting up the account records.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course's data-quality module validates raw client intake data as part of onboarding.
- *See also:* Client, Account, Risk profile, Account status

**Client redress:** Compensation or other remedial action that a financial firm provides to clients who suffered loss because the firm broke rules or made an error. It can be ordered by a regulator or offered by the firm, and may include refunds, interest or corrected account terms.

- *Where it shows up:* SA track: Wk 8, M01 Software Quality and the Analyst, slide 6
- *See also:* Regulatory breach, Compliance, Regulation (regulator)

**Client segment:** A group of clients who share characteristics such as wealth, age, account type or investing behavior, defined so that a firm can analyze, serve or market to each group differently. Segments are usually set by the firm's own business rules.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Wealth management

**Closing a position:** Making a trade that brings a holding in an instrument back to zero, for example selling all the shares of a stock you own, or buying back shares you previously sold short.

- *Where it shows up:* SA track: Wk 3, M14 handout: 14-AIRequirementsPack
- *See also:* Short selling, Trade, Take-profit order

**Closing price:** The last price at which a security trades during a market's regular trading session on a given day. For most US stock markets the session ends at 4:00 p.m. Eastern Time, and after-hours trades do not change the official close.

- *Where it shows up:* SA track: Wk 2, M12 Data Quality Dimensions, slide 4
- *See also:* Trading hours (market hours), Mark-to-market, Market data

**COBOL (Common Business-Oriented Language):** A compiled, English-like programming language created in 1959-60 for business data processing. It handles decimal arithmetic precisely and still runs much of the core batch and transaction logic in banking and investment firms' mainframe systems.

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 9
- *See also:* COBOL divisions, PIC clause, COMP-3 (packed decimal), Mainframe

**COBOL divisions:** The four sections that every COBOL program is divided into: Identification (program name), Environment (runtime and file settings), Data (field and record definitions) and Procedure (the executable logic).

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 2
- *See also:* COBOL (Common Business-Oriented Language), Record layout (copybook), PIC clause

**COMP-3 (packed decimal):** A COBOL numeric storage format that packs two decimal digits into each byte, with the sign held in the last half-byte. It stores exact decimal values compactly, so it is common for money fields, but must be unpacked before other systems can read it.

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 7
- *See also:* PIC clause, COBOL (Common Business-Oriented Language), Record layout (copybook), Extract file

**Compliance:** Meeting the laws, regulations and internal policies that apply to a firm. In a financial firm, the compliance function is the team that interprets those rules, advises the business, and monitors that obligations such as record retention and access controls are met.

- *Where it shows up:* SA track: Wk 1, M02 handout: 02-SARole-SDLCMapping; Engineering track: Wk 4, M05 Contract First Design with OpenAPI, slide 4
- *See also:* Risk and compliance (function), Three lines of defense, Control (control environment), Regulation (regulator)

**Compliance risk:** The risk of regulatory sanctions, fines, penalties, or financial loss that a firm faces when it fails to comply with the laws, rules, regulations, and supervisory requirements that apply to it.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *See also:* Conduct risk, Operational risk, Risk (financial)

**Conduct risk:** The risk that a financial firm's behavior causes poor or unfair outcomes for its customers or harms the integrity of financial markets.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *Course note:* The course sometimes groups it as 'conduct and compliance risk'. They overlap: compliance risk is about breaking rules, conduct risk about customer and market outcomes.
- *See also:* Compliance risk, Risk (financial)

**Consumer Duty:** In the UK, an FCA rule that requires firms serving retail customers to act to deliver good outcomes for them. It covers four areas: product design, price and value, customer understanding, and customer support.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4
- *See also:* FCA (Financial Conduct Authority), Suitability (Regulation Best Interest), Risk warning

**Control (control environment):** A control is a policy, procedure or system check that a firm uses to reduce a risk, such as a required approval or an automated validation. The control environment is the full set of controls a firm operates and the culture that supports them.

- *Where it shows up:* SA track: Wk 1, M01 handout: 01-KickOff-SkillsSelfAssessment
- *Course note:* The course uses "control" in this compliance sense, not the software or UI sense. Handouts refer to "control scenarios" meaning situations where a control should act.
- *See also:* Preventive control, Detective control, Four-eyes principle, Compliance

**Control totals:** Counts and sums, such as the number of records or the total of an amount field, calculated when data is sent and recalculated when it is received, to confirm that nothing was lost, duplicated or altered in transfer.

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 7
- *See also:* Reconciliation, Broker trade feed, End-of-day processing (EOD)

**Corporate action:** An event initiated by a company that affects its securities and the people who hold them, such as a dividend, stock split, merger, rights offering or name change. Firms must adjust holders' positions, cash and records to reflect it.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *See also:* Custodian, Reference data (instrument reference data), Market value (valuation)

**Corporate bond:** A bond issued by a company to raise money, for example to build facilities or grow the business. The company pays interest, typically semiannually, and repays the principal at maturity; it usually carries more credit risk than a government bond.

- *Where it shows up:* Engineering track: Wk 8, M04 Kafka Fundamentals, slide 6
- *Course note:* Sample event data uses 'CORPB1', which appears to be a fictional corporate bond identifier.
- *See also:* Bond, US Treasury (UST), Gilt

**Cost basis (average cost):** The original cost of an investment, including commissions and fees, used to calculate the gain or loss when it is sold. Average cost is one method of calculating it: the total cost of all shares held divided by the number of shares.

- *Where it shows up:* SA track: Wk 2, M05 Relational Database Fundamentals, slide 9; Engineering track: Project spec (timing not fixed)
- *Course note:* The course uses cost basis to mean the average price paid for a position, used to compute P&L. US tax rules also allow other methods, such as first-in first-out.
- *See also:* Realized and unrealized P&L, Position, Holding (holdings)

**Counterparty:** The other party to a financial transaction, such as the buyer when you are the seller. Each counterparty relies on the other to deliver the securities or pay the cash agreed.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *See also:* Credit risk, Settlement risk

**Credit risk:** The risk that a counterparty or borrower will not meet its financial obligations in full when due, for example by failing to pay for or deliver securities or by defaulting on a loan.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *Course note:* The course pairs it with settlement risk ('credit and settlement risk'). Settlement risk is the trade-specific case of a failure at the moment of exchange.
- *See also:* Counterparty, Settlement risk, Market risk

**Cryptocurrency (crypto asset):** A digital asset that is created, issued or transferred using a blockchain or similar distributed ledger network, such as Bitcoin or Ether. The SEC uses 'crypto asset' as the umbrella term for tokens, coins, virtual currencies and digital assets.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course treats crypto as one of the platform's three instrument classes, alongside equities and FX.
- *See also:* Asset class, Instrument (financial instrument)

**Currency:** The unit of money in which cash, prices, or an instrument are denominated, such as the US dollar (USD), euro (EUR), or pound sterling (GBP). Amounts in different currencies cannot be added together without first converting them at an exchange rate (FX).

- *Where it shows up:* SA track: Wk 1, M04 Ways of Working, slide 6; Engineering track: Wk 4, M07 Persistence with My Batis, slide 7
- *Course note:* One course dataset sums USD and GBP amounts without conversion; the course flags this as an anomaly.
- *See also:* Market data

**CUSIP:** A nine-character code that identifies a security issued in the US or Canada, such as a stock, bond or municipal bond. It identifies both the issuer and the specific issue, and forms the core of US ISINs.

- *Where it shows up:* Not in course materials
- *See also:* ISIN (International Securities Identification Number), Ticker (symbol)

**Custodian:** A financial institution, typically a bank or broker-dealer, that holds and safeguards securities and cash on behalf of clients, keeps records of those holdings and processes settlements and corporate actions. Holding assets this way is called custody.

- *Where it shows up:* SA track: Wk 6, M16 Webhook and DECAPIs, slide 11; Engineering track: Wk 8, M07 Batch Loading in Practice, slide 4
- *See also:* Settlement, Corporate action, Reconciliation, Back office

**Cut-off:** A deadline by which instructions, payments or data must be received to be processed in the current cycle or business day. Anything received after the cut-off time is processed in the next cycle.

- *Where it shows up:* SA track: Wk 6, M01 How the Platform Is Built, slide 11
- *See also:* Business day, End-of-day processing (EOD), Settlement

## D

**Data residency:** The geographic location where data is physically stored and processed. Laws, regulators or client contracts may require that certain data, such as client personal data, stay within a specific country or region.

- *Where it shows up:* SA track: Wk 6, M09 Cloud Awareness, slide 9; Engineering track: Wk 10, M02 AWS Account Setup IAM, slide 4
- *See also:* Personal financial information (client data), UK GDPR, Regulated firm

**Dealer:** A person or firm in the business of buying and selling securities for its own account, acting as principal. The word is also used informally for a firm employee who takes client orders and places trades on the client's behalf.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses the second sense: an employee who takes client orders (for example by phone) and places them, applying judgment.
- *See also:* Advised dealing (advised service), Order channel, Order

**DEC API (Digital Experience Capability):** An API layer that sits between digital channels, such as websites and mobile apps, and core back-end APIs, shaping and combining data into the form those user interfaces need.

- *Where it shows up:* SA track: Wk 6, M16 Webhook and DECAPIs, slide 2
- *Course note:* Fidelity-specific term; the slide advises confirming scope with the programme contact.
- *See also:* Mainframe, Recordkeeping system

**Deposit and withdrawal:** A deposit is money paid into an account; a withdrawal is money taken out. A transfer between accounts is a withdrawal from one and a deposit to the other, and both sides must be recorded together or not at all.

- *Where it shows up:* Engineering track: Wk 2, M09 OWASP Top 10, slide 16
- *Course note:* Appears in the engineering track (OWASP module) as an example of an operation that must be atomic.
- *See also:* Cash movement, Cash balance, Account

**Derivative:** A financial contract whose value is derived from the performance of an underlying asset, security, index or rate. Options, futures, forwards and swaps are common derivatives, used to hedge risk or to speculate.

- *Where it shows up:* Engineering track: Wk 3, M07 SOLID Principles Part 1, slide 6
- *Course note:* Used only as an example of how the design could be extended; derivatives are not part of the course's platform or data.
- *See also:* Instrument (financial instrument), Security (financial)

**Detective control:** A control designed to find errors, fraud or policy breaches after they have occurred, so they can be corrected. Examples include reconciliations, exception reports and log reviews. It complements a preventive control, which stops the problem in advance.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 7
- *See also:* Preventive control, Control (control environment), Audit trail

**Discretionary dealing:** A service in which the firm, under a mandate agreed with the client, decides what to buy and sell and places trades in the client's account without asking the client to approve each trade.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Advised dealing (advised service), Retail trading platform

**Dividend:** A payment made by a company to its shareholders out of its profits, usually in cash and often on a regular schedule such as quarterly. Some funds also pass dividends from their holdings on to their investors.

- *Where it shows up:* Engineering track: Wk 2, M15 Postgres Essentials and Environment Setup, slide 9
- *Course note:* Recorded in the course data as one type of account transaction, alongside buys, sells, deposits and withdrawals.
- *See also:* Equity (share, stock), Transaction (financial), Growth and income (investment styles)

**Duplicate order:** An order, or a trade or fill resulting from it, that is submitted or recorded more than once by mistake, for example after a double click or a retried message. It can make a client buy or sell twice the intended amount.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 13; Engineering track: Wk 4, M04 RESTAPI Design Principles, slide 8
- *See also:* Order, Fill, Trade

## E

**End-of-day processing (EOD):** Scheduled batch processing run after the business day closes that consolidates the day's transactions, updates balances and positions, and produces reports and statements. It typically runs overnight within a fixed batch window.

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 4; Engineering track: Wk 8, M02 Data Movement At Enterprise Scale, slide 8
- *See also:* Business day, Cut-off, Control totals, System of record

**Equity (share, stock):** A security that represents part ownership of a company, giving the holder a claim on a proportional share of its assets and profits and usually voting rights. The words stock and share are used interchangeably.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Security (financial), Dividend, Ticker (symbol), Asset class

**Estate (technology estate):** The complete set of an organization's technology: its applications, infrastructure, data systems and networks. It has no connection to estate planning or real estate.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 2
- *Course note:* Used in the welcome material; students could misread it as estate planning or real estate.

**ETF (exchange-traded fund):** A pooled investment fund whose shares trade on a stock exchange throughout the day at market prices, like a company's stock. Most ETFs hold a basket of stocks, bonds or other assets, often chosen to track an index.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5; Engineering track: Wk 7, M06 Data Cleaning Preparation, slide 6
- *See also:* Fund (mutual fund), Equity (share, stock), Security (financial)

**Exchange (stock exchange):** An organized, regulated marketplace where buyers and sellers trade securities or other instruments under common rules, and where prices are formed and published. In the US, stock exchanges such as the NYSE and Nasdaq register with the SEC as national securities exchanges.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5
- *Course note:* The course also says 'venue', 'trading venue', and 'crypto venue' for any place an instrument is traded or priced, including crypto trading platforms, which are generally not registered securities exchanges.
- *See also:* LSE (London Stock Exchange), Trading hours (market hours), Market data, Broker

**Exchange suffix (.L):** A code added after a dot to a ticker symbol, in Refinitiv (formerly Reuters) Instrument Code (RIC) format, to show which exchange a listing trades on. The suffix '.L' denotes the London Stock Exchange.

- *Where it shows up:* Engineering track: Wk 3, M11 J Unit, slide 6
- *Course note:* Used in engineering test data (e.g. AZN.L, BP.L, HSBA.L) without explanation.
- *See also:* LSE (London Stock Exchange), Exchange (stock exchange), Market data

**Execution:** The carrying out of an order in the market, when it is matched with a counterparty and completed at a specific price and quantity. Brokers must seek the most favorable terms reasonably available for client orders (best execution).

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 9; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The word also appears in non-finance senses in the course (test execution, SQL execution plans); make the trading sense explicit.
- *See also:* Fill, Execution price, Order

**Execution price:** The price at which an order, or part of an order, is actually carried out. It can differ from the price quoted when the order was placed, especially for market orders in fast-moving markets.

- *Where it shows up:* SA track: Wk 2, M03 Data Fluency for Analysts, slide 7
- *See also:* Execution, Fill, Market order

**Exposure:** The amount of money a firm or investor has at risk to a particular instrument, counterparty, market, or risk factor, usually measured as the current market value of the related positions. Total exposure to an instrument is the sum of all positions held in it.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* Mostly used in the non-finance security sense (exposure of personal or sensitive data). The project spec uses the financial sense: the firm's aggregate positions per instrument.
- *See also:* Risk limit, Mark-to-market, Market risk, Credit risk

**Extract file:** A file, usually produced by a scheduled batch job, containing a selected subset of data copied from a system of record so that other downstream systems can load or process it. Mainframe extracts are often fixed-width records described by a copybook.

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 10
- *See also:* Batch processing (batch job), Batch window, Record layout (copybook), Recordkeeping system

## F

**FCA (Financial Conduct Authority):** The UK regulator responsible for the conduct of financial services firms and the integrity of UK financial markets. Its objectives are protecting consumers, keeping markets sound, and promoting competition.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4
- *See also:* SEC (Securities and Exchange Commission), FINRA (Financial Industry Regulatory Authority), Regulation (regulator)

**Fee (commission):** A charge a broker makes for handling a client's trade. A commission is typically a flat amount per trade or a percentage of the trade value (an ad valorem fee); other fees may cover account services.

- *Where it shows up:* Engineering track: Wk 3, M02 OO Principles in Practice, slide 8
- *Course note:* In the ENG code, the test named 'equityFeeIsOnePercent' actually computes 0.1%, a useful discrepancy to point out.
- *See also:* Trade value (notional), Trade

**Fill:** The execution of all or part of an order at a particular price, resulting in a trade that changes the client's holdings and cash. An order may receive one fill or several partial fills.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 7; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Partial fill, Execution, Trade, Order

**Fill rate:** The proportion of an order's quantity, or of a set of orders, that is actually executed, usually expressed as a percentage. It is a common measure of execution quality.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *Course note:* Non-standard in the course: measures filled orders against rejected orders, not filled quantity against ordered quantity.
- *See also:* Fill, Partial fill, Order rejection

**Finance (function):** The department of a firm responsible for managing its money: accounting, financial reporting, budgeting and planning, treasury (cash management) and financial risk. It is typically led by the chief financial officer (CFO).

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* In the course, Finance is a stakeholder that consumes reporting on trading activity and cash movement.
- *See also:* P&L (profit and loss)

**Financial advisor:** A professional who gives individuals advice on investments and other financial matters and may manage their accounts. It is a general job title, not a legal category; in the US such people are usually registered as investment advisers or broker representatives.

- *Where it shows up:* Engineering track: Wk 2, M15 Postgres Essentials and Environment Setup, slide 8
- *Course note:* In the course each client is assigned exactly one advisor (advisors table / advisors.csv).
- *See also:* Client, Relationship manager, Self-directed investor

**FINRA (Financial Industry Regulatory Authority):** The self-regulatory organization for the US brokerage industry. Under SEC oversight, it writes and enforces rules for broker-dealers and their registered representatives, examines firms, and licenses individuals.

- *Where it shows up:* Not in course materials
- *See also:* SEC (Securities and Exchange Commission), Regulation (regulator), Best execution

**Firm commitment:** In US securities, an underwriting arrangement in which the underwriter agrees to buy an entire new issue of securities from the issuer and resell it, bearing the risk of any unsold securities. The phrase is also used loosely for an order a firm has accepted and is bound to honor.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses it only in the loose sense: a client order accepted and recorded as binding before execution. Industry would more often say 'accepted order'.
- *See also:* Order, Order status, Order confirmation

**Four-eyes principle:** A control that requires a second, independent person to review and approve an action before it takes effect, such as a payment, a data change or a code change. It is also called maker-checker and is a form of segregation of duties.

- *Where it shows up:* Engineering track: Wk 1, M07 Advanced Git Pull Requests and Repo Hygiene, slide 4
- *Course note:* In the engineering track it appears as the required approving review on a pull request.
- *See also:* Preventive control, Control (control environment), Audit trail

**Fractional share:** Ownership of less than one full share of a stock or other security, for example 0.1 of a share. Fractional shares let investors invest a set dollar amount rather than buy whole shares.

- *Where it shows up:* SA track: Wk 8, M08 handout: 08-AICoverageReview
- *See also:* Order, Trade value (notional)

**Front office:** The client-facing and revenue-generating functions of a financial firm, such as sales, trading and investment management, that deal with clients and make trading decisions.

- *Where it shows up:* Not in course materials
- *See also:* Middle office, Back office, Trading desk (dealing desk)

**FTSE All-World Index:** A global stock market index, run by UK-based FTSE Russell (part of the London Stock Exchange Group), that tracks about 4,000 large and mid-sized companies across developed and emerging markets. Funds and ETFs use it as a benchmark for global equities.

- *Where it shows up:* SA track: Wk 2, M05 Relational Database Fundamentals, slide 3
- *Course note:* Appears as the index tracked by the Vanguard FTSE All-World ETF (ticker VWRL), a London-listed fund.
- *See also:* LSE (London Stock Exchange)

**Fund (mutual fund):** A pooled investment vehicle that collects money from many investors and invests it in a portfolio of securities managed by professionals. A mutual fund's shares are bought from and sold back to the fund at end-of-day net asset value, not traded on an exchange.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5; Engineering track: Wk 2, M20 RDBMS Modelling Part 1, slide 8
- *Course note:* The course uses 'fund' generically for pooled vehicles and defines an ETF as 'a fund traded like a share'.
- *See also:* ETF (exchange-traded fund), Security (financial), Model portfolio

**FX (foreign exchange):** The trading of one currency for another, or the global market where this happens. Currencies are quoted in pairs such as EUR/USD, where the first (base) currency is priced in units of the second (quote) currency.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course treats an FX pair (e.g. GBP/USD) as a tradable instrument, one of the platform's three instrument classes.
- *See also:* Asset class, Instrument (financial instrument)

## G

**Gilt:** A bond issued by the UK government through HM Treasury, denominated in pounds sterling and listed on the London Stock Exchange. The name comes from 'gilt-edged', reflecting its reputation as a very safe investment.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5; Engineering track: Wk 8, M04 Kafka Fundamentals, slide 6
- *Course note:* Course example: GILT30 / 'UK Gilt 2030', a gilt maturing in 2030.
- *See also:* Bond, US Treasury (UST)

**Growth and income (investment styles):** Two broad investment approaches. A growth style targets capital appreciation by holding companies expected to grow faster than average, usually paying little or no dividend; an income style targets regular cash payments from dividend-paying stocks and bonds.

- *Where it shows up:* Engineering track: Wk 7, M09 Pandas Deeper Dive, slide 6
- *Course note:* Used as labels for advisor teams (Growth team, Income team) in a data-analysis example.
- *See also:* Dividend, Equity (share, stock), Model portfolio

## H

**Holding (holdings):** A specific investment that an account owns, such as a quantity of a particular stock or fund. An account's holdings together make up its portfolio.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses holding as a synonym for position; the holding quantity is what a sell order is checked against.
- *See also:* Position, Portfolio, Cost basis (average cost)

## I

**Identity verification:** The process of confirming that a new client is who they claim to be, by collecting details such as name, date of birth, address and a government identification number and checking them against documents or trusted data. It is a core part of KYC.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* KYC (Know Your Customer), AML (Anti-Money Laundering)

**Impact tolerance:** In UK operational resilience rules, the maximum level of disruption to an important business service that a firm can tolerate before it causes intolerable harm to clients or markets. Firms usually express it as a maximum outage time.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4
- *See also:* Operational resilience, FCA (Financial Conduct Authority)

**Indicative price:** A price shown for information only, indicating roughly where an instrument could be bought or sold, with no commitment from the quoting party to trade at it. It differs from a firm quote, which the quoting party must honor.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Quote, Pricing, Slippage

**Instrument (financial instrument):** A contract or asset that can be owned and traded, such as a stock, bond, fund share, currency pair, derivative or crypto asset. In accounting terms it is any contract creating a financial asset for one party and a liability or equity interest for another.

- *Where it shows up:* SA track: Wk 1, M01 handout: 01-KickOff-SkillsSelfAssessment; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The BRS defines an instrument as 'an equity, a foreign exchange pair, or a crypto asset', but training data also holds ETFs and bonds.
- *See also:* Security (financial), Asset class, Equity (share, stock), FX (foreign exchange)

**Insufficient funds:** A condition in which an account does not have enough available cash to pay for a purchase and its fees. Firms normally check for it before accepting a buy order and reject the order if the cash is not there.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses this name for the whole pre-trade check, covering both cash for buys and holdings for sells.
- *See also:* Insufficient holdings, Order rejection

**Insufficient holdings:** A condition in which a client tries to sell more of an instrument than the account holds. Where short selling is not allowed, the firm rejects such a sell order.

- *Where it shows up:* SA track: Wk 5, M06 Specifying UI States, slide 6; Engineering track: Project spec (timing not fixed)
- *See also:* Insufficient funds, Short selling, Order rejection

**Internal audit:** An independent function within a firm that gives objective assurance to the board on whether risk management, controls and governance are working. It is the third line in the three lines model and reports to the board rather than to business management.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 6
- *See also:* Three lines of defense, Control (control environment), Compliance

**Investment lifecycle:** The full sequence of stages an investment passes through, from the investment decision and order, through execution and settlement, to ongoing holding, servicing (such as corporate actions and valuation) and eventual sale.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 9; Engineering track: Wk 1, M00 Welcome and Introduction, slide 5
- *See also:* Trade lifecycle, Settlement, Corporate action, Market value (valuation)

**IRA (Individual Retirement Account):** In the US, a tax-advantaged retirement account that an individual opens and funds personally, up to annual IRS contribution limits. Main types are traditional IRAs (tax-deferred) and Roth IRAs (tax-free qualified withdrawals).

- *Where it shows up:* Not in course materials
- *See also:* 401(k), Workplace pension, Brokerage account

**ISIN (International Securities Identification Number):** A 12-character code, defined by the ISO 6166 standard, that uniquely identifies a security worldwide. It is a two-letter country code, a nine-character national identifier (such as a CUSIP) and a check digit.

- *Where it shows up:* Not in course materials
- *See also:* CUSIP, Ticker (symbol), Security (financial)

## J

**JCL (Job Control Language):** The set of statements used on IBM z/OS mainframes to tell the operating system what work to perform: which programs a batch job runs (EXEC), which data sets they use (DD), and how the job is identified (JOB).

- *Where it shows up:* SA track: Wk 2, M14 Data Integration and Mainframe Recordkeeping, slide 9
- *See also:* Batch processing (batch job), Mainframe, Return code

## K

**KYC (Know Your Customer):** The process by which a financial firm verifies a client's identity and gathers the essential facts about them, such as financial situation and who may act on the account. It supports anti-money-laundering checks and suitable advice. In the US, see FINRA Rule 2090.

- *Where it shows up:* Not in course materials
- *See also:* Identity verification, AML (Anti-Money Laundering), Suitability (Regulation Best Interest)

## L

**Ledger (debit and credit):** A set of accounting records in which every financial transaction is recorded as equal debit and credit entries, so the books always balance. The general ledger is a firm's master set of accounts, from which its financial statements are produced.

- *Where it shows up:* SA track: Wk 6, M01 How the Platform Is Built, slide 9; Engineering track: Wk 2, M09 OWASP Top 10, slide 16
- *See also:* Booking, System of record, Reconciliation

**Limit order (limit price):** An order to buy or sell a security at a specified price (the limit price) or better: a buy executes only at or below the limit, a sell only at or above it. The order may not execute at all.

- *Where it shows up:* SA track: Wk 1, M05 Jira Confluence, slide 15
- *Course note:* The course is inconsistent on whether the platform takes limit orders, market orders, or both; confirm the intended rule before teaching.
- *See also:* Market order, Order type, Stop-loss order

**Liquidity:** How easily and quickly an asset can be bought or sold without significantly moving its price. A liquid stock trades often and in size with a narrow bid-ask spread; an illiquid one may be hard to sell without accepting a lower price.

- *Where it shows up:* SA track: Wk 10, M03 Validating the Deployed Platform, slide 7
- *See also:* Bid-ask spread, Trading volume, Slippage

**LSE (London Stock Exchange):** In the UK, the main stock exchange, based in London and owned by the London Stock Exchange Group (LSEG). Its Main Market trades on business days from 8:00 a.m. to 4:30 p.m. UK time.

- *Where it shows up:* SA track: Wk 2, M06 SQL Fundamentals, slide 5
- *See also:* Exchange (stock exchange), Exchange suffix (.L), Trading hours (market hours)

## M

**Mainframe:** A large, highly reliable central computer, typically an IBM system running z/OS, that businesses use to host core databases, transaction servers and batch applications needing very high security, availability and throughput. Many financial firms keep their core records on mainframes.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 2
- *See also:* COBOL (Common Business-Oriented Language), CICS (Customer Information Control System), JCL (Job Control Language), Recordkeeping system

**Mark-to-market:** The practice of valuing positions or holdings at current market prices rather than at the price originally paid. It shows what each position is worth today and its unrealized gain or loss.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *See also:* Closing price, Market data, Exposure, Pricing

**Market data:** Price and trading information published by exchanges and data vendors, such as current bid and ask quotes, last trade prices and sizes, and trading volume. Firms receive it through real-time or scheduled data feeds to value positions and make trading decisions.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 10; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course names its price source 'Fauxnance' (Fauxnance API). Treat it as the course's market-data feed, not a real industry product.
- *See also:* Quote, Bid, Ask (offer), Trading volume

**Market order:** An order to buy or sell a security immediately at the best price currently available. It is almost certain to execute, but the execution price is not guaranteed and may differ from the last quoted price.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 10
- *Course note:* The course is inconsistent on whether the platform takes limit orders, market orders, or both; confirm the intended rule before teaching.
- *See also:* Limit order (limit price), Order type, Execution price

**Market risk:** The risk of losses caused by movements in market prices, such as share prices, interest rates, exchange rates, or commodity prices, moving against a position.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *See also:* Volatility, Exposure, Credit risk, Risk (financial)

**Market value (valuation):** The current worth of a security or holding at the price it could be bought or sold for now. For a position, it is the quantity held multiplied by the current market price. Updating values this way is called marking to market.

- *Where it shows up:* SA track: Wk 3, M06 handout: 06-AIDraftCriticalReview; Engineering track: Wk 3, M11 J Unit, slide 20
- *See also:* Reference data (instrument reference data), Corporate action

**Master file:** A file holding the current, authoritative records for a business entity, such as client accounts or holdings. It is updated periodically, often by a batch job that applies a separate file of transactions to it.

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 4
- *See also:* Recordkeeping system, Batch processing (batch job), Record layout (copybook)

**Middle office:** The functions of a financial firm that sit between the front office and the back office, such as risk management, compliance, trade validation and profit and loss reporting. Its role is to check and control trading activity.

- *Where it shows up:* Not in course materials
- *See also:* Front office, Back office, Trading operations

**Model portfolio:** A predefined mix of investments, each with a target weight, designed by an adviser or investment firm to meet a stated goal or risk level. Client accounts follow the model and are rebalanced when their holdings drift from it.

- *Where it shows up:* Engineering track: Wk 2, M19 Data Quality, slide 3
- *Course note:* In the course, clients 'subscribe' to named models (e.g. Adventurous Growth, Balanced Growth, Income Focus).
- *See also:* Target weight, Portfolio drift, Wealth management

**Moving-average crossover:** A technical-analysis signal that occurs when a shorter-term moving average of price (the average over a rolling number of recent periods) crosses a longer-term one. An upward cross is read as a possible uptrend, a downward cross as a possible downtrend.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *See also:* Bollinger Bands, Volatility

## O

**Operational resilience:** A firm's ability to prevent, adapt to, respond to, recover from and learn from operational disruption, such as a system outage or cyber attack, while keeping its most important services running for clients.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4; Engineering track: Project spec (timing not fixed)
- *See also:* Impact tolerance, FCA (Financial Conduct Authority), Regulated firm

**Operational risk:** The risk of loss from inadequate or failed internal processes, people, or systems, or from external events. Examples include duplicate or lost trades, data-entry errors, system outages, and fraud.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *See also:* Compliance risk, Settlement risk, Risk (financial)

**Order:** An instruction from a client to a broker to buy or sell a specified quantity of a particular instrument, possibly with conditions on price or timing. An order becomes one or more trades only when it is executed.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses order, trade, and fill loosely; also appears as SQL ORDER BY.
- *See also:* Trade, Fill, Order type, Order lifecycle

**Order cancellation:** The withdrawal of an order, at the client's or firm's request, before it has been executed. Only the unexecuted part of an order can be canceled; any quantity already filled stands.

- *Where it shows up:* SA track: Wk 3, M14 handout: 14-AIRequirementsPack; Engineering track: Project spec (timing not fixed)
- *Course note:* The course allows cancellation only of open orders in NEW status, before any fill.
- *See also:* Working order (open order), Partial fill, Order status

**Order channel:** The route by which an order reaches a firm, such as an online platform, a mobile app, or a phone call to staff. Firms record the channel because checks, fees, and rules can differ by channel.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses two channels: WEB (client self-service) and DESK (entered by staff).
- *See also:* Order, Dealer, Retail trading platform

**Order confirmation:** A notice to the client that an order has been received or, once executed, a record of the trade showing details such as price, quantity, fees, and settlement date. US brokers must send trade confirmations at or before completion of each transaction.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses the term for both an order acknowledgement and a trade confirmation; in industry these are different messages.
- *See also:* Order, Trade, Execution

**Order expiration:** The automatic ending of an unexecuted order when the period it was set to remain active (its time-in-force) runs out, for example at the end of the trading day for a day order. Any unfilled quantity is no longer working.

- *Where it shows up:* SA track: Wk 6, M05 Reading Code Without Writing It, slide 8
- *See also:* Working order (open order), Order status, Order cancellation

**Order history:** A chronological record of a client's or account's past orders and their outcomes, including fills, cancellations and rejections. A firm-wide chronological record of orders and trades is often called a blotter.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Trade reconstruction, Trade dispute, Trade event

**Order lifecycle:** The sequence of states an order passes through from receipt to completion, typically received, accepted (open), partially or fully filled, and then filled, canceled, rejected, or expired, followed by settlement of any resulting trades.

- *Where it shows up:* SA track: Wk 3, M07 Process Modelling in Mermaid, slide 8; Engineering track: Wk 3, M00 Java Week Introduction, slide 4
- *Course note:* Course states: Received, New, Filled/Rejected/Cancelled, Settled. Strictly, settlement applies to the resulting trade, not the order.
- *See also:* Order status, Order, Fill

**Order rejection:** The refusal of an order by a firm or trading venue, usually during checks before execution, for a stated reason such as insufficient funds, an unknown instrument, or a closed market. A rejected order is never executed.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Insufficient funds, Insufficient holdings, Order status

**Order status:** The current state of an order in its lifecycle, such as new, partially filled, filled, canceled, rejected, or expired. Systems update it as events occur so clients and staff can see what has happened to the order.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* Status names differ across the BRS, the project spec, and weeks (submitted/accepted/NEW/FILLED...); agree one list with students.
- *See also:* Order lifecycle, Blotter, Working order (open order)

**Order ticket:** The record or entry form that captures an order's details, such as account, instrument, side, quantity, order type, price, and time received. US broker-dealers must keep such a record of each order and any change or cancellation.

- *Where it shows up:* SA track: Wk 5, M01 User Centred Design, slide 7; Engineering track: Wk 5, M00 Angular Week Introduction, slide 4
- *Course note:* The course uses it for the order entry screen, which also shows an estimated cost.
- *See also:* Order, Side (buy/sell), Order type

**Order type:** The kind of order, which determines how, when, and at what price it may be executed, for example a market order, a limit order, or a stop order.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 10
- *Course note:* The course is inconsistent about which order types the platform supports (market, limit, or both); confirm the intended rule before teaching.
- *See also:* Market order, Limit order (limit price), Stop-loss order

## P

**P&L (profit and loss):** The gain or loss made over a period. For investments it is the change in value of positions: realized P&L comes from positions already sold, and unrealized P&L from the current value of positions still held. For a company, the P&L is its income statement.

- *Where it shows up:* SA track: Wk 3, M06 handout: 06-AIDraftCriticalReview; Engineering track: Project spec (timing not fixed)
- *Course note:* The course uses P&L for gains or losses on client positions, not company income statements.
- *See also:* Finance (function), Transaction (financial)

**Partial fill:** Execution of only part of an order's quantity, for example 60 of 100 shares, leaving the remaining quantity still working until it is filled, canceled, or expires.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 6
- *See also:* Fill, Working order (open order), Order status

**Personal financial information (client data):** Information about a client that identifies them or describes their finances, such as name, account numbers, balances and transaction history. Financial privacy laws limit how firms may share it and require them to keep it secure.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, M09 Introduction to GenAI in Engineering At Fidelity, slide 4
- *See also:* UK GDPR, Data residency, Regulatory breach

**PIC clause:** The COBOL PICTURE (PIC) clause, which defines a field's type and size using symbols: 9 for a digit, X for any character, S for a sign and V for an implied decimal point. For example, PIC 9(5)V99 holds five digits, then two decimal places.

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 7
- *See also:* COBOL (Common Business-Oriented Language), COMP-3 (packed decimal), Record layout (copybook), 88 level (condition name)

**Portfolio:** The combined set of investments, such as stocks, bonds and funds, and usually cash, held by an individual or institution. It may span one account or several.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Holding (holdings), Position, Cash balance, Account

**Portfolio drift:** The gradual divergence of a portfolio's actual holdings from its target weights, caused by some investments rising or falling in value faster than others. Drift is corrected by rebalancing, which buys and sells to restore the target mix.

- *Where it shows up:* Engineering track: Wk 2, M20 RDBMS Modelling Part 1, slide 8
- *See also:* Model portfolio, Target weight

**Position:** The amount of a particular security or instrument that an account holds (a long position) or owes (a short position). A client's position in a stock is their current holding of that stock.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* Course treats position and holding as synonyms and ignores short positions. The 'legal position' in BR-14 is an unrelated meaning.
- *See also:* Holding (holdings), Portfolio, Cost basis (average cost)

**Pre-trade check (order validation):** An automated control that tests an order against set rules before the order is accepted or sent to market, and rejects it if a rule fails. Typical checks cover sufficient cash or holdings, credit or trading limits, and prices or sizes that look erroneous.

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 9; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course calls these the firm's 'trading rules' an order must pass before acceptance, e.g. sufficient cash or holding and the instrument being tradable. US broker-dealers with market access must have such controls under SEC Rule 15c3-5.
- *See also:* Risk limit, Quote, Stale price (stale quote)

**Preventive control:** A control designed to stop an error, fraud or policy breach before it happens. Examples include input validation, access restrictions and requiring a second approval. It complements a detective control, which finds problems after they occur.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 7
- *See also:* Detective control, Four-eyes principle, Control (control environment)

**Pricing:** The process of setting the price at which an instrument is valued or an order is executed, usually by taking a current market quote. In order processing it is the step where an order is assigned a price before it is filled (executed).

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course treats pricing as a named stage of the order lifecycle, where the order is valued at a current quote before it is filled.
- *See also:* Quote, Market data, Mark-to-market, Slippage

## Q

**Quote:** The current price at which an instrument can be bought or sold, usually shown as a bid (the price to sell at) and an ask (the price to buy at). A quote may be firm (the quoting party will trade at it) or indicative.

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 10; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* In the course's BRS glossary. The platform uses a single quote price and makes no bid/ask distinction.
- *See also:* Bid, Ask (offer), Bid-ask spread, Indicative price

## R

**Realized and unrealized P&L:** Profit and loss (P&L) on investments. Realized P&L is the gain or loss locked in when an investment is sold; unrealized P&L is the change in value of investments still held, measured against their cost basis.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *See also:* Cost basis (average cost), Position, Portfolio

**Reconciliation:** The process of comparing two sets of records that should agree, such as a firm's positions against its trade fills or against a custodian's statement, and investigating any differences. An unexplained difference is called a break.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4; Engineering track: Wk 2, M27 Capstone Extending the Schema, slide 6
- *Course note:* The course also uses "reconciliation" in a non-finance sense for a domain model reconciliation session.
- *See also:* Control totals, Custodian, Trading operations, System of record

**Record layout (copybook):** A field-by-field description of a fixed-format record, giving each field's name, position, length and data type. In COBOL it is usually kept in a copybook, a shared source file that programs include with the COPY statement.

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 2
- *See also:* PIC clause, COMP-3 (packed decimal), Extract file, COBOL divisions

**Record-keeping (regulatory):** A regulated firm's obligation to create, keep and be able to produce accurate records of its business, such as client accounts, orders, trades and communications, for set retention periods. These records are often called the firm's books and records.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 9; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses two senses: regulatory record retention, and "recordkeeping" systems (often mainframe) that hold the official account records. Point out which one a slide means.
- *See also:* Books-and-records rules (SEC Rule 17a-4), Audit trail, Compliance

**Recordkeeping system:** The system that holds a firm's official, authoritative records of each client's accounts, holdings, cash and transactions. Other systems treat it as the source of truth; it is also called the book of record or system of record.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 12
- *Course note:* The course means Fidelity's mainframe systems of record. Do not confuse with regulatory record-keeping, the rules on what records firms must keep and for how long.
- *See also:* Master file, Mainframe, Position, Extract file

**Reference data (instrument reference data):** Relatively static descriptive data that transactions are checked against, such as each security's identifier, name, type, currency and trading market, and account or client details. A central store of instrument details is often called a security or instrument master.

- *Where it shows up:* SA track: Wk 2, M13 Profiling and Validation Rules, slide 4; Engineering track: Wk 2, M15 Postgres Essentials and Environment Setup, slide 9
- *See also:* System of record, Market value (valuation), Corporate action

**Regulated firm:** A firm that must be authorized or registered by a financial regulator and is supervised by it, such as a broker-dealer or investment adviser. Its rules affect how the firm runs its business, including its technology, data storage and outsourcing choices.

- *Where it shows up:* SA track: Wk 6, M09 Cloud Awareness, slide 10
- *See also:* Regulation (regulator), Compliance, Data residency

**Regulation (regulator):** Regulation is the body of legally binding rules that govern how financial firms operate, for example how they trade, treat clients and keep records. A regulator is the public authority or self-regulatory organization that makes and enforces those rules.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 2; Engineering track: Wk 1, M00 Welcome and Introduction, slide 5
- *Course note:* The course speaks of regulation generically and does not name a specific regulator or rule.
- *See also:* SEC (Securities and Exchange Commission), FINRA (Financial Industry Regulatory Authority), FCA (Financial Conduct Authority), Regulated firm

**Regulation NMS (National Market System):** A set of SEC rules, adopted in 2005, that govern how US stock trading venues are linked. Its main rules require trading centers to avoid executing trades at prices worse than displayed quotes elsewhere, give fair access to quotes, and set standards for market data.

- *Where it shows up:* Not in course materials
- *See also:* Best execution, SEC (Securities and Exchange Commission)

**Regulatory breach:** A failure by a firm to meet a legal or regulatory obligation, such as exposing client data or failing to report trades. Serious breaches usually must be reported to the regulator and can lead to fines or client redress.

- *Where it shows up:* SA track: Wk 8, M11 Severity Priority and Triage, slide 5
- *Course note:* The course's example is a breach of client confidentiality.
- *See also:* Client redress, Compliance, Personal financial information (client data)

**Regulatory reporting:** The mandatory submission of data by a regulated firm to its regulators, such as reports of executed trades, financial condition or client assets, in a set format and on a set schedule.

- *Where it shows up:* SA track: Wk 6, M01 How the Platform Is Built, slide 9; Engineering track: Wk 2, M14 Data Systems Concepts, slide 5
- *Course note:* The course mostly means transaction reports sent to regulators.
- *See also:* Transaction reporting, Record-keeping (regulatory), Compliance

**Relationship manager:** A firm employee assigned to look after a client relationship, serving as the client's main contact and coordinating the services the firm provides to them. In wealth management the role may include advice and placing trades for the client.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 3; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* In the course a relationship manager is a named employee who places trades on the client's behalf.
- *See also:* Financial advisor, Client

**Retail client (retail investor):** An individual who invests their own money rather than on behalf of an institution. Regulators give retail clients the highest level of protection because they are assumed to have the least market expertise.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Client, Self-directed investor, Risk profile

**Retail trading platform:** An online system through which individual (retail) investors place their own orders to buy and sell securities, view their holdings and cash, and track their orders, usually without advice from the firm.

- *Where it shows up:* Both tracks: Wk 1, M00 Welcome and Introduction, slide 2
- *See also:* Advised dealing (advised service), Order channel, Order ticket

**Return code:** A number a program or job step sets on finishing to report its outcome; on IBM mainframes, 0 usually means success, and higher values such as 4, 8 or 12 signal warnings or errors. JCL can test it to decide whether later steps run.

- *Where it shows up:* SA track: Wk 6, M07 COBOL and CICS for Analysts, slide 10
- *See also:* JCL (Job Control Language), Batch processing (batch job), Mainframe

**Risk (financial):** The possibility that a financial outcome, such as an investment's return or a firm's result, differs from what was expected, including the possibility of loss. Firms divide it into types such as market, credit, operational, compliance, and conduct risk.

- *Where it shows up:* SA track: Wk 1, M00 Welcome and Introduction, slide 2; Engineering track: Wk 1, M00 Welcome and Introduction, slide 5
- *Course note:* Also used for the firm's Risk function (the department that oversees risk) and for ordinary project risk in the kickoff risk list.
- *See also:* Market risk, Credit risk, Operational risk, Compliance risk

**Risk and compliance (function):** The departments in a financial firm that oversee risk management and regulatory compliance, setting policies, monitoring the business and challenging it where needed. They form the second line in the three lines model.

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course treats this as the owner of audit, record-keeping and regulatory alignment requirements.
- *See also:* Compliance, Three lines of defense, Internal audit

**Risk limit:** A maximum a firm sets on the risk it or its clients may take, such as caps on position size, exposure to one instrument or counterparty, losses, or number of trades. Activity that would breach a limit is blocked or escalated.

- *Where it shows up:* SA track: Wk 7, M03 handout: 03-ReframingARequest; Engineering track: Wk 3, M01 Core Java Refresher, slide 6
- *Course note:* The course's example is a client-protection control, such as blocking clients from trading more than ten times a day. 'Block trade' in the alias list means blocking, not the industry term for a large negotiated trade.
- *See also:* Exposure, Pre-trade check (order validation), Market risk

**Risk profile:** An assessment of how much investment risk a client is able and willing to take, often expressed as a category, used to check that investments are suitable for them. It combines risk tolerance with factors such as goals and time horizon.

- *Where it shows up:* Engineering track: Wk 2, M16 SQL Fundamentals Refresher, slide 6
- *Course note:* The course uses three categories, Cautious, Balanced and Adventurous, for suitability checks.
- *See also:* Client onboarding, Retail client (retail investor), Portfolio

**Risk warning:** A statement shown to an investor that describes the risks of an investment, such as the possibility of losing money, typically before they buy or when a product is promoted. Regulators require that such information be clear, fair and not misleading.

- *Where it shows up:* SA track: Wk 5, M01 User Centred Design, slide 12
- *See also:* Consumer Duty, Suitability (Regulation Best Interest)

## S

**SEC (Securities and Exchange Commission):** The US federal agency that regulates the securities markets. Its mission is to protect investors, maintain fair and orderly markets, and facilitate capital formation, and it oversees brokers, dealers, investment advisers, exchanges and public company disclosure.

- *Where it shows up:* Not in course materials
- *See also:* FINRA (Financial Industry Regulatory Authority), FCA (Financial Conduct Authority), Regulation (regulator)

**Security (financial):** A tradable financial instrument such as a stock, bond or fund share that represents ownership in, or a debt owed by, an issuer. In the US, securities are a legal category whose issue and trading the SEC regulates.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 6; Engineering track: Project spec (timing not fixed)
- *See also:* Instrument (financial instrument), Equity (share, stock), Bond

**Self-directed investor:** An investor who makes their own investment decisions and places their own trades without advice from a financial professional. The firm executes the orders but does not recommend them.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 10; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Retail client (retail investor), Financial advisor, Brokerage account

**Settlement:** The completion of a trade, when the securities are transferred to the buyer's account and the cash to the seller's account. It happens on the settlement date, after the trade has been executed and cleared.

- *Where it shows up:* SA track: Wk 1, M01 handout: 01-KickOff-SkillsSelfAssessment; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course does not model a settlement cycle; the engineering "Settlement Engine" only reports accepted or rejected orders and fees, which is not settlement in the standard sense.
- *See also:* Settlement cycle (T+1, T+2), Clearing, Custodian, Trade date

**Settlement cycle (T+1, T+2):** The standard number of business days between a trade date (T) and its settlement date. T+1 means settlement one business day after the trade; T+2 means two. Most US securities trades have settled T+1 since May 28, 2024.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 9
- *Course note:* Course training data says bonds settle T+2. In the US, corporate bonds are also T+1 under SEC Rule 15c6-1; T+2 is out of date for US practice.
- *See also:* Trade date, Settlement, Business day

**Settlement failure:** A trade that does not settle on its scheduled settlement date because the seller does not deliver the securities or the buyer does not pay. A seller's failure to deliver securities is called a fail to deliver.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *See also:* Settlement, Settlement cycle (T+1, T+2), Reconciliation, Trading operations

**Settlement risk:** The risk that a trade does not settle as expected, meaning one side fails to deliver the securities or pay the cash on the agreed date. In the worst case one party delivers its side but never receives the other.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *See also:* Counterparty, Credit risk, Operational risk

**Short selling:** Selling a security you do not own, usually shares borrowed through a broker, expecting to buy it back later at a lower price. It creates a negative (short) position and loses money if the price rises.

- *Where it shows up:* Engineering track: Wk 3, M02 OO Principles in Practice, slide 5
- *Course note:* The course's rules implicitly prohibit it: a sell larger than the holding is rejected.
- *See also:* Insufficient holdings, Closing a position

**Side (buy/sell):** The direction of an order or trade: whether it buys or sells the instrument. Not to be confused with 'buy side' and 'sell side', which describe types of firm.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 8; Engineering track: Wk 2, M15 Postgres Essentials and Environment Setup, slide 9
- *Course note:* Also used in the non-finance sense ('both sides of the conversation').
- *See also:* Order, Order ticket

**Slippage:** The difference between the price expected when an order is placed and the price at which it actually executes. It arises when the market moves, or too little volume is available at the quoted price, between decision and execution.

- *Where it shows up:* SA track: Wk 1, M03 handout: 03-Scenario-StakeholderMap
- *See also:* Quote, Stale price (stale quote), Liquidity, Volatility

**Stale price (stale quote):** A price or quote that no longer reflects the current market because it has not been updated recently, for example because a data feed has stopped or trading has paused. Using it to value or execute an order can give the wrong price.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 3
- *Course note:* In the course, a quote that is no longer current at execution time (BR-08).
- *See also:* Quote, Slippage, Market data, Pre-trade check (order validation)

**Statement (client statement):** A periodic report sent to a client showing, for a set period, the account's holdings and their values, cash balances, and transactions. US broker-dealers must send one at least quarterly.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Account, Holding (holdings), Cash movement, Portfolio

**Stop-loss order:** An order to buy or sell once the price reaches a specified level (the stop price), at which point it becomes a market order. Investors often place a sell stop below the current price to limit losses on a holding.

- *Where it shows up:* SA track: Wk 5, M04 AI Wireframe Review Lab, slide 6
- *See also:* Market order, Limit order (limit price), Take-profit order

**Suitability (Regulation Best Interest):** Suitability is a broker's duty to recommend only investments that fit a client's profile, such as goals, risk tolerance and finances. Regulation Best Interest is the SEC rule that raises this for retail clients: the broker must act in the client's best interest and not put its own interests first.

- *Where it shows up:* Not in course materials
- *See also:* KYC (Know Your Customer), Consumer Duty, FINRA (Financial Industry Regulatory Authority), SEC (Securities and Exchange Commission)

**System of record:** The information system designated as the authoritative source for a given set of data, such as a firm's official client holdings. When systems disagree, the system of record's version is treated as correct.

- *Where it shows up:* SA track: Wk 6, M01 How the Platform Is Built, slide 2; Engineering track: Wk 2, M25 Cloud Data Warehouses and Snowflake Overview, slide 4
- *See also:* Reference data (instrument reference data), Ledger (debit and credit), Reconciliation

## T

**Take-profit order:** An order to close a position automatically when the price reaches a specified favorable level, usually a limit order to sell above the current price, so that a gain is realized.

- *Where it shows up:* SA track: Wk 8, M04 handout: 04-TestCasePack
- *Course note:* The course uses 'take profit' more loosely for simply selling a holding to realize a gain, not necessarily a standing order.
- *See also:* Stop-loss order, Limit order (limit price), Closing a position

**Target weight:** The planned percentage of a portfolio's total value allocated to a particular investment or asset class. The target weights in a portfolio add up to 100 percent and are the benchmark used to measure drift and trigger rebalancing.

- *Where it shows up:* Engineering track: Wk 2, M20 RDBMS Modelling Part 1, slide 8
- *See also:* Model portfolio, Portfolio drift, Asset class

**Tax reporting (tax year summary):** The reporting of a client's taxable investment events for a tax year, such as sale proceeds, gains and losses, dividends and interest, to the client and the tax authority. It relies on accurate, settled transaction records.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 12
- *See also:* Settlement, System of record, Corporate action

**Three lines of defense:** A risk governance model that separates three roles: the business that owns and manages its risks (first line), risk and compliance functions that oversee and challenge it (second line), and internal audit that gives independent assurance (third line).

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course mostly refers to the second line (risk and compliance oversight).
- *See also:* Internal audit, Risk and compliance (function), Compliance

**Ticker (symbol):** A short code of letters, and sometimes numbers, that identifies a listed security on a stock exchange, such as AAPL for Apple on Nasdaq. Tickers are exchange-specific and can be reused, so they are not unique global identifiers like ISINs.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5; Engineering track: Wk 2, M20 RDBMS Modelling Part 1, slide 7
- *Course note:* Course examples include London-listed tickers (VOD, HSBA, VWRL) alongside AAPL, MSFT and SPY; no ISIN or CUSIP is used.
- *See also:* ISIN (International Securities Identification Number), CUSIP, Equity (share, stock)

**Tradable status:** Whether an instrument can currently be bought or sold, which depends on factors such as whether its market is open and whether trading in it has been halted or suspended.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 11; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Order rejection, Order

**Trade:** A completed purchase or sale of a quantity of a security at an agreed price between a buyer and a seller, resulting from the execution of an order. One order can produce several trades.

- *Where it shows up:* SA track: Wk 1, M01 handout: 01-KickOff-SkillsSelfAssessment; Engineering track: Wk 1, M00 Welcome and Introduction, slide 3
- *Course note:* The course itself warns that order, trade, fill, and settlement mean different things to different teams.
- *See also:* Order, Fill, Execution

**Trade capture:** The recording of an executed trade's details, such as security, quantity, price, time and account, into a firm's trading systems immediately after execution, so that the trade can be confirmed, booked and settled.

- *Where it shows up:* SA track: Wk 4, M07 AI Sequence Diagram Lab, slide 2; Engineering track: Project spec (timing not fixed)
- *See also:* Booking, Trade lifecycle, Broker trade feed, Trading desk (dealing desk)

**Trade confirmation (contract note):** A document a broker sends to a client after executing a trade, recording its details such as the security, quantity, price, trade date, settlement date, fees and commissions. It is also called a contract note.

- *Where it shows up:* SA track: Wk 7, M06 Ideation and Prioritisation, slide 9; Engineering track: Wk 3, M14 Mission Wrapup, slide 6
- *Course note:* The course uses the term "contract note".
- *See also:* Trade date, Settlement, Trade lifecycle

**Trade correction:** A change made to a previously recorded trade to fix an error, such as a wrong price, quantity or account. Good practice records it as a new entry, often a cancellation plus a replacement, so the original remains visible for audit.

- *Where it shows up:* SA track: Wk 3, M07 Process Modelling in Mermaid, slide 8
- *Course note:* The course models corrections as appended records rather than overwrites, and lists "refund" as an alias, which is not a standard synonym.
- *See also:* Trade reconstruction, Booking, Trade dispute

**Trade date:** The date on which a trade is executed and its price is fixed, written as T. The settlement date, when ownership and cash actually change hands, is counted in business days from the trade date.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 9; Engineering track: Wk 2, M27 Capstone Extending the Schema, slide 5
- *Course note:* The course lists "settlement date" as an alias of trade date; they are different dates.
- *See also:* Settlement cycle (T+1, T+2), Settlement, Business day

**Trade dispute:** A disagreement in which a client challenges a trade, for example claiming it was unauthorized, executed at the wrong price or quantity, or not executed as instructed. Resolving it depends on the firm's records of the order and its execution.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 10; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Trade reconstruction, Order history, Trading operations

**Trade event:** A record or message stating that something happened to an order or trade, such as it being filled, rejected or cancelled. Systems publish these events so other systems can react to and record each change in state.

- *Where it shows up:* SA track: Wk 2, M04 Data Systems Concepts OLTP vs OLAP, slide 7; Engineering track: Wk 8, M00 Kafka Week Introduction, slide 3
- *Course note:* In the course these are messages on a Kafka topic (trade-events).
- *See also:* Order history, Trade lifecycle, Trade reconstruction

**Trade lifecycle:** The sequence of steps a trade passes through from order placement to completion: order, validation, execution, capture, confirmation, clearing, settlement and final recording. Each step is often handled by a different team or system.

- *Where it shows up:* SA track: Wk 1, M01 handout: 01-KickOff-SkillsSelfAssessment; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Investment lifecycle, Trade capture, Clearing, Settlement

**Trade reconstruction:** The ability to rebuild the complete history of a trade from a firm's records, including the order, its timing, pricing, execution and settlement. Regulators require firms to keep records detailed enough to do this.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 11
- *Course note:* The course ties this to a record-keeping business requirement (BR-15).
- *See also:* Order history, Trade dispute, Trade correction, System of record

**Trade signal:** An indication, produced by analysis or by a rule-based model, that an instrument should be bought, sold, or held at a given time. It is an input to a trading decision, not an order.

- *Where it shows up:* Both tracks: Project spec (timing not fixed)
- *See also:* Algorithmic trading (automated trading strategy), Order

**Trade value (notional):** The monetary value of a trade, calculated as quantity multiplied by price, before fees; also called consideration. In derivatives, 'notional' means the reference amount used to calculate payments, which does not itself change hands.

- *Where it shows up:* Engineering track: Wk 3, M01 Core Java Refresher, slide 8
- *Course note:* The course uses 'notional' as a synonym for trade value; in industry 'notional' is mainly a derivatives term.
- *See also:* Fee (commission), Trade, Execution price

**Trader:** A person who buys and sells securities or other instruments to profit from price movements, often over short periods. The term covers individuals trading their own money and professionals trading on behalf of a firm or its clients.

- *Where it shows up:* Engineering track: Wk 5, M00 Angular Week Introduction, slide 4
- *Course note:* The persona for the Angular UI: a user who places buy and sell orders.
- *See also:* Buy and hold, Transaction (financial)

**Trading desk (dealing desk):** The team within a financial firm that executes buy and sell orders in securities, either for clients or for the firm itself. It is also called a dealing desk.

- *Where it shows up:* SA track: Wk 1, M02 SA Role, slide 6; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* In the course scenario the desk is the business stakeholder that owns the trading rules the platform must enforce.
- *See also:* Front office, Trading operations, Trade capture

**Trading hours (market hours):** The times during which a market or trading venue is open to accept and execute orders. Regular US stock market hours are 9:30 a.m. to 4:00 p.m. Eastern Time on business days, with optional extended-hours sessions before and after.

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 11; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* Aliases include '24/7', reflecting crypto venues, which trade continuously, unlike stock exchanges.
- *See also:* Closing price, Exchange (stock exchange), LSE (London Stock Exchange)

**Trading operations:** The team in a financial firm that makes sure executed trades are processed correctly after execution, including confirmation, settlement, reconciliation, fixing breaks and resolving client disputes. Often shortened to "operations" or "ops".

- *Where it shows up:* SA track: Wk 1, M03 Trading Platform Scenario, slide 10; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *See also:* Back office, Middle office, Reconciliation, Settlement failure

**Trading volume:** The quantity of an instrument traded over a period, usually the number of shares or contracts that change hands per day, or their total value. Each trade counts once, not once for the buyer and again for the seller.

- *Where it shows up:* SA track: Wk 1, M03 handout: LEAP BRS; Engineering track: Wk 1, Fri joint kickoff (BRS issued)
- *Course note:* The course uses it loosely for the number and/or value of trades; industry volume usually counts shares or contracts rather than trades.
- *See also:* Liquidity, Market data

**Transaction (financial):** A recorded event that changes the contents or cash balance of an account, such as a purchase or sale of a security, a dividend or interest payment, a deposit or a withdrawal. Not to be confused with a database transaction.

- *Where it shows up:* Engineering track: Wk 2, M09 OWASP Top 10, slide 11
- *Course note:* The course uses both senses: a financial transaction (transactions table in the enterprise schema) and a database transaction (OLTP). Students may confuse them.
- *See also:* Dividend, Trader, P&L (profit and loss)

**Transaction reporting:** In the UK and EU, the requirement for investment firms to send regulators a detailed report of each executed trade in covered instruments, including the instrument, price, quantity, time and parties. Regulators use the reports to detect market abuse.

- *Where it shows up:* SA track: Wk 2, M02 Risk Regulation and Controls, slide 4
- *See also:* Regulatory reporting, FCA (Financial Conduct Authority), Audit trail

## U

**UK GDPR:** The UK's main data protection law, retained from the EU General Data Protection Regulation after Brexit and applied with the Data Protection Act 2018. It governs how organizations collect, use, store and share personal data about individuals.

- *Where it shows up:* SA track: Wk 4, M12 Production Data Querying, slide 2
- *See also:* Personal financial information (client data), Data residency

**US Treasury (UST):** A debt security issued by the US Department of the Treasury and backed by the US government. Treasury bills mature in one year or less, notes in 2 to 10 years and bonds in 20 or 30 years.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 5
- *Course note:* Course example UST10 is presumably a 10-year Treasury note.
- *See also:* Bond, Gilt, Security (financial)

## V

**Volatility:** How much and how quickly the price of an instrument or index moves up and down over a period, usually measured as the standard deviation of its returns. Higher volatility means larger, faster price swings and more uncertainty.

- *Where it shows up:* SA track: Wk 7, M03 handout: 03-ReframingARequest; Engineering track: Project spec (timing not fixed)
- *See also:* Market risk, Bollinger Bands, Liquidity

## W

**Wealth management:** A professional service that combines investment management with financial planning, such as retirement, tax and estate planning, for individuals and families. It is usually aimed at affluent and high-net-worth clients.

- *Where it shows up:* Engineering track: Wk 1, M00 Welcome and Introduction, slide 5
- *See also:* Model portfolio, Client segment

**Working order (open order):** An order that has been accepted but is not yet fully executed, canceled, or expired, so it can still be filled. Limit orders often remain working until the price reaches the limit.

- *Where it shows up:* SA track: Wk 1, M05 Jira Confluence, slide 15; Engineering track: Project spec (timing not fixed)
- *See also:* Order status, Partial fill, Order cancellation, Order expiration

**Workplace pension:** In the UK, a retirement savings plan arranged by an employer, into which a percentage of the employee's pay is paid automatically each payday, usually with an added employer contribution and tax relief.

- *Where it shows up:* SA track: Wk 2, M01 Investment Lifecycle, slide 12
- *See also:* 401(k), IRA (Individual Retirement Account)

## Sources

Each definition was checked against at least one of the sources below, preferring regulators and primary standards bodies (SEC, Investor.gov, FINRA, FCA, IRS, DTCC, ISO/ANNA, IBM documentation). A few entries rest on general industry usage where no authoritative definition exists; these are listed in the separate review notes.

- <https://www.accaglobal.com/us/en/student/exam-support-resources/professional-exams-study-resources/p7/technical-articles/auditing-computer-based-environment2.html>
- <https://www.anna-dsb.com/isin/>
- <https://api-handbook.fca.org.uk/files/sourcebook/CASS.pdf>
- <https://assets.publishing.service.gov.uk/media/67e1612564220b68ed6a7009/SA108-Notes-2025.pdf>
- <https://www.bis.org/committees/bcbs/basel-framework/standard/mar/11/inforce/2022-01-01/published/2019-12-15>
- <https://www.bis.org/committees/bcbs/basel-framework/standard/ope/10/inforce/2023-01-01/published/2024-07-05>
- <https://www.bis.org/committees/bcbs/basel-framework/standard/rbc/25/inforce/2019-12-15/published/2019-12-15>
- <https://www.bis.org/cpmi/glossary.pdf>
- <https://careernavigator.accaglobal.com/gb/en/job-profiles/expert/banking-relationship-manager.selector.Leader.html>
- <https://www.cfainstitute.org/programs/cfa-program/careers/private-wealth-manager>
- <https://chartschool.stockcharts.com/table-of-contents/trading-strategies-and-models/trading-strategies/moving-average-trading-strategies/trading-using-the-golden-cross>
- <https://corporatefinanceinstitute.com/resources/capital_markets/what-is-the-trade-lifecycle/>
- <https://www.deloitte.com/ng/en/services/audit-assurance/perspectives/coso-control-environment.html>
- <https://www.dmo.gov.uk/responsibilities/gilt-market/about-gilts/>
- <https://www.dtcc.com/about/businesses-and-subsidiaries/nscc>
- <https://en.wikipedia.org/wiki/Chief_financial_officer>
- <https://en.wikipedia.org/wiki/Failure_to_deliver>
- <https://en.wikipedia.org/wiki/Foreign_exchange_market>
- <https://en.wikipedia.org/wiki/Income_statement>
- <https://en.wikipedia.org/wiki/Internal_control>
- <https://en.wikipedia.org/wiki/International_Securities_Identification_Number>
- <https://en.wikipedia.org/wiki/Maker-checker>
- <https://en.wikipedia.org/wiki/Market_segmentation>
- <https://en.wikipedia.org/wiki/Middle_office>
- <https://en.wikipedia.org/wiki/Order_(exchange)>
- <https://en.wikipedia.org/wiki/Refinitiv_Identification_Code>
- <https://en.wikipedia.org/wiki/System_of_record>
- <https://www.fca.org.uk/about/what-we-do/the-fca>
- <https://www.fca.org.uk/firms/operational-resilience>
- <https://www.fca.org.uk/firms/regulatory-reporting/notification-fca-pra>
- <https://www.fca.org.uk/firms/risk-warnings-mainstream-investments>
- <https://www.fca.org.uk/markets/transaction-reporting>
- <https://www.fca.org.uk/news/speeches/conduct-risk-briefing>
- <https://www.fca.org.uk/publication/business-plans/fca-risk-outlook-2013.pdf>
- <https://www.fca.org.uk/publication/policy/ps21-3-operational-resilience.pdf>
- <https://www.federalreserve.gov/boarddocs/supmanual/trading/trad_p2.pdf>
- <https://www.federalreserve.gov/newsevents/speech/kroszner20060403a.htm>
- <https://www.federalreserve.gov/supervisionreg/srletters/SR0808.pdf>
- <https://www.fidelity.com/learning-center/smart-money/1099-b>
- <https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/bollinger-bands>
- <https://www.financialresearch.gov/viewpoint-papers/2017/03/27/approach-to-financial-instrument-reference-data/>
- <https://www.finra.org/about>
- <https://www.finra.org/investors/insights/corporate-actions-public-companies-what-you-should-know>
- <https://www.finra.org/investors/insights/cost-basis-basics>
- <https://www.finra.org/investors/insights/defining-value-investment>
- <https://www.finra.org/investors/insights/key-terms-tough-times-vocabulary-stressed-markets>
- <https://www.finra.org/investors/insights/know-your-risk-tolerance>
- <https://www.finra.org/investors/insights/managing-cash-in-brokerage-account>
- <https://www.finra.org/investors/insights/time-parameters-qualifiers-stock-orders>
- <https://www.finra.org/investors/investing/investing-basics/fees-commissions>
- <https://www.finra.org/investors/investing/investment-accounts/brokerage-accounts>
- <https://www.finra.org/investors/investing/investment-products/stocks/order-types>
- <https://www.finra.org/investors/investing/investment-products/stocks/types>
- <https://www.finra.org/investors/investing/working-with-investment-professional/professional-designations-credentials>
- <https://www.finra.org/rules-guidance/guidance/interpretations-financial-operational-rules/sea-rule-15c3-3-and-related-interpretations>
- <https://www.finra.org/rules-guidance/key-topics/algorithmic-trading>
- <https://www.finra.org/rules-guidance/key-topics/aml>
- <https://www.finra.org/rules-guidance/key-topics/books-records>
- <https://www.finra.org/rules-guidance/key-topics/consolidated-audit-trail-cat>
- <https://www.finra.org/rules-guidance/notices/21-15>
- <https://www.finra.org/rules-guidance/notices/95-2>
- <https://www.finra.org/rules-guidance/rulebooks/finra-rules/2090>
- <https://www.finra.org/rules-guidance/rulebooks/finra-rules/2231>
- <https://www.finra.org/rules-guidance/rulebooks/finra-rules/2232>
- <https://www.finra.org/rules-guidance/rulebooks/finra-rules/5110>
- <https://www.finra.org/rules-guidance/rulebooks/finra-rules/5310>
- <https://www.finra.org/sites/default/files/Investors_Guide_to_Securities_Industry_Disputes.pdf>
- <https://www.frbservices.org/about/holiday-schedules/>
- <https://www.frbservices.org/resources/financial-services/wires/operating-hours.html>
- <https://www.ftc.gov/legal-library/browse/rules/financial-privacy-rule>
- <https://www.globalrelay.com/resources/the-compliance-hub/rules-and-regulations/a-guide-to-cass/>
- <https://www.gov.uk/workplace-pensions>
- <https://handbook.fca.org.uk/glossary/G1980>
- <https://handbook.fca.org.uk/glossary/G395>
- <https://handbook.fca.org.uk/glossary/G877>
- <https://handbook.fca.org.uk/handbook/COBS/3/2.html>
- <https://handbook.fca.org.uk/handbook/COBS/3/4.html>
- <https://handbook.fca.org.uk/handbook/cobs11/cobs11s12>
- <https://handbook.fca.org.uk/handbook/conred1>
- <https://handbook.fca.org.uk/handbook/glossary/G1380.html>
- <https://handbook.fca.org.uk/handbook/prin2a>
- <https://handbook.fca.org.uk/handbook/prin2a/prin2as1>
- <https://handbook.fca.org.uk/handbook/sup15/sup15s3>
- <https://handbook.fca.org.uk/handbook/sysc9/sysc9s1>
- <https://www.handbook.fca.org.uk/handbook/glossary/G395.html>
- <https://www.ibm.com/docs/SSLTBW_2.2.0/com.ibm.zos.v2r2.ieab500/iea3b5_Examples_of_COND_return_code_testing_in_a_job.htm>
- <https://www.ibm.com/docs/en/cics-ts/6.x?topic=what-is-cics-transaction-server-zos>
- <https://www.ibm.com/docs/en/cobol-aix/5.1.0?topic=dates-avoiding-problems-packed-decimal-fields>
- <https://www.ibm.com/docs/en/cobol-zos/6.2.0?topic=vc-format-2>
- <https://www.ibm.com/docs/en/cobol-zos/6.4.0?topic=coding-example-using-copy-statement>
- <https://www.ibm.com/docs/en/cobol-zos/6.4.0?topic=entry-picture-clause>
- <https://www.ibm.com/docs/en/cobol-zos/6.4.0?topic=structure-cobol-program>
- <https://www.ibm.com/docs/en/cobol-zos/6.5.0?topic=clause-computational-items>
- <https://www.ibm.com/docs/en/devops-test-workbench/11.0.8?topic=schemas-cobol-copybooks-overview>
- <https://www.ibm.com/docs/en/entirex/11.1.0?topic=mapping-condition-names-level-88-data-items>
- <https://www.ibm.com/docs/en/zos-basic-skills?topic=collection-basic-jcl-concepts>
- <https://www.ibm.com/docs/en/zos-basic-skills?topic=processing-mainframes-working-after-hours-batch>
- <https://www.ibm.com/docs/en/zos-basic-skills?topic=today-what-is-mainframe-its-style-computing>
- <https://www.ibm.com/docs/en/zos/2.5.0?topic=commands-condition-codes>
- <https://www.ibm.com/docs/zosbasics/com.ibm.zos.zconcepts/zconc_whatisbatch.htm>
- <https://www.ibm.com/docs/zosbasics/com.ibm.zos.zmainframe/zconc_batchproc.htm>
- <https://www.ibm.com/products/cics-transaction-server>
- <https://www.ibm.com/think/perspectives/your-it-estate-is-limiting-what-your-organization-can-become>
- <https://www.ibm.com/think/topics/cobol>
- <https://www.ibm.com/think/topics/data-residency>
- <https://www.ibm.com/think/topics/mainframe>
- <https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/personal-information-what-is-it/what-is-personal-data/what-is-personal-data/>
- <https://www.ifrs.org/content/dam/ifrs/publications/html-standards/english/2021/issued/ias32.html>
- <https://www.ig.com/en/trading-strategies/what-are-take-profit-and-stop-loss-orders--how-do-they-work--230605>
- <https://www.inforeachinc.com/fix-dictionary/fix_4_4_fields_ordstatus>
- <https://www.investor.gov/additional-resources/general-resources/publications-research/info-sheets/beginners-guide-asset>
- <https://www.investor.gov/additional-resources/spotlight/crypto-assets>
- <https://www.investor.gov/better-understanding-your-brokerage-account-statement>
- <https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-14>
- <https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-42>
- <https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-73>
- <https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/fractional-share-investing-buying-slice-instead-whole-share>
- <https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/new-t1-settlement-cycle-what-investors-need-know-investor-bulletin>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/401k-plan>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/ask-price>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/asset-classes>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/basis-point>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/bid-price>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/bonds>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/bonds-corporate>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/broker>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/closing-price>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/cusip-number>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/derivatives>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/dividend>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/exchange-traded-fund-etf>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/financial-industry-regulatory-authority-finra>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/freeze-brokerage-account>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/individual-retirement-account-ira>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/investment-adviser>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/liquidity-or-marketability>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/national-securities-exchange>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/portfolio>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/risk>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/risk-tolerance>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/security>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/short-sales>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/stock>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/ticker>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/trading-halts-and-delays>
- <https://www.investor.gov/introduction-investing/investing-basics/glossary/treasury-securities>
- <https://www.investor.gov/introduction-investing/investing-basics/how-stock-markets-work/types-orders>
- <https://www.investor.gov/introduction-investing/investing-basics/investment-accounts/brokerage-accounts>
- <https://www.investor.gov/introduction-investing/investing-basics/investment-products/mutual-funds-and-exchange-traded-funds-etfs/mutual-funds>
- <https://www.investor.gov/introduction-investing/investing-basics/role-sec>
- <https://www.investor.gov/sites/investorgov/files/media/buy-and-hold-investing-infographic.pdf>
- <https://www.irs.gov/faqs/capital-gains-losses-and-sale-of-home/mutual-funds-costs-distributions-etc/mutual-funds-costs-distributions-etc-1>
- <https://www.irs.gov/retirement-plans/individual-retirement-arrangements-iras>
- <https://www.irs.gov/retirement-plans/plan-participant-employee/retirement-plans-definitions>
- <https://www.irs.gov/taxtopics/tc429>
- <https://www.iso.org/iso-4217-currency-codes.html>
- <https://www.law.cornell.edu/cfr/text/17/240.17a-3>
- <https://www.law.cornell.edu/uscode/text/15/78c>
- <https://www.lexisnexis.com/en-gb/legal/glossary/contract-note>
- <https://linfordco.com/blog/detective-controls-security/>
- <https://linfordco.com/blog/importance-of-preventive-controls/>
- <https://www.lseg.com/en/ftse-russell/indices/ftseall-world>
- <https://www.lseg.com/en/media-centre/press-releases/2026/london-stock-exchange-to-launch-lse-24>
- <https://www.marcus.com/us/en/resources/investing/realized-vs-unrealized-gains-losses>
- <https://www.morningstar.com/investing-terms/model-portfolio>
- <https://www.nasdaq.com/glossary/t/trading-volume>
- <https://www.netsuite.com/portal/resource/articles/accounting/debits-credits.shtml>
- <https://www.newyorkfed.org/markets/international-market-operations/foreign-exchange-operations>
- <https://www.oxfordreference.com/display/10.1093/oi/authority.20110803105309343>
- <https://www.sciencedirect.com/topics/computer-science/detective-control>
- <https://www.sciencedirect.com/topics/computer-science/preventative-control>
- <https://www.sec.gov/files/approved-iac-060624-rec-re-self-directed-investors.pdf>
- <https://www.sec.gov/files/corporate_bond_white_paper.pdf>
- <https://www.sec.gov/files/oasb-broker-dealer-building-block.pdf>
- <https://www.sec.gov/files/rules/final/2010/34-63241-secg.htm>
- <https://www.sec.gov/files/rules/sro/iex/2025/34-102663.pdf>
- <https://www.sec.gov/investment/settlement-cycle-small-entity-compliance-guide-15c6-1-15c6-2-204-2>
- <https://www.sec.gov/news/public-statement/lee-open-meeting-statement-120920>
- <https://www.sec.gov/newsroom/press-releases/2019-89>
- <https://www.sec.gov/rules-regulations/2000/06/privacy-consumer-financial-information-regulation-s-p>
- <https://www.sec.gov/rules-regulations/2003/04/customer-identification-programs-broker-dealers>
- <https://www.sec.gov/rules-regulations/2003/05/books-records-requirements-brokers-dealers-under-securities-exchange-act-1934>
- <https://www.sec.gov/rules-regulations/2005/06/regulation-nms>
- <https://www.theiia.org/en/standards/what-are-the-standards/definition-of-internal-audit/>
- <https://www.theiia.org/globalassets/documents/resources/the-iias-three-lines-model-an-update-of-the-three-lines-of-defense-july-2020/three-lines-model-updated-english.pdf>
- <https://www.treasurydirect.gov/marketable-securities/>
