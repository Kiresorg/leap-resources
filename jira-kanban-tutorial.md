# Jira Basics: Plan a Home Project on a Kanban Board

**Goal:** Learn the core Jira workflow by organizing a garage cleanout on a Kanban board.
**Time:** About 20-30 minutes
**You need:** Your free Jira Cloud account, logged in through a web browser

> **A note on terms:** Atlassian has been renaming "issues" to "work items" in Jira. Depending on when you read this, your screen may say either one. They mean the same thing. This tutorial uses "issue."

## Part 1: Get Oriented

1. Log in to your Jira site (it looks like `yourname.atlassian.net`).
2. Take a quick look around the screen:
   - **Left sidebar:** your projects, filters, and other navigation
   - **Top bar:** search box, notifications, and your profile
   - **+ Create button:** creates a new issue from anywhere in Jira
3. Learn four terms in plain English:
   - **Project:** a container for related work (like a folder)
   - **Issue:** a single piece of work (like one to-do item)
   - **Board:** a visual view of issues arranged in columns
   - **Status:** where an issue is in the process (To Do, In Progress, Done)

**What you should see:** Your Jira home page with a sidebar on the left and a **+ Create** button near the top.

## Part 2: Create Your Project

1. In the sidebar, click **Projects**, then click **Create project** (or the **+** next to Projects).
2. Under **Software development**, choose the **Kanban** template.
3. Click **Use template**.
4. If asked to choose a project type, select **Team-managed** (simpler settings, better for learning).
5. Name the project **Garage Cleanout**. Jira will suggest a short **key** like `GC`. Keep it.
6. Click **Create project** (or **Next**, then skip any optional steps).

**What you should see:** An empty board with three columns: **To Do**, **In Progress**, and **Done**. The project name appears at the top left.

> **Why the key matters:** Every issue in this project will be numbered with it, like `GC-1`, `GC-2`. That number is how people refer to issues in conversation.

## Part 3: Add Your Issues

1. Click the **+ Create** button at the top of the screen.
2. In the form:
   - **Project:** Garage Cleanout
   - **Issue type:** Task
   - **Summary:** `Sort tools`
3. Click **Create**.
4. Now add issues the fast way. At the bottom of the **To Do** column, click **+ Create**, type a summary, and press **Enter**. Add these:
   - `Donate old bikes`
   - `Buy shelving`
   - `Sweep the floor`
   - `Haul trash to the dump`
   - `Install shelving`

**What you should see:** Six cards in the **To Do** column, each labeled with a key like `GC-1` through `GC-6`.

## Part 4: Add Details to an Issue

1. Click the **Sort tools** card. A detail panel opens.
2. **Description:** Click the description area and type:
   `Group tools into these piles:`
   Then type `[] ` (left bracket, right bracket, space) to start a checkbox, and add:
   - Hand tools
   - Power tools
   - Garden tools
   - Broken (toss)
   Click **Save**.
3. **Assignee:** Find the **Assignee** field and click **Assign to me**.
4. **Due date:** Find **Due date** (you may need to expand **More fields**) and pick a date this weekend.
5. **Comment:** At the bottom, in the comment box, type `Need more bins before I start this.` and click **Save**.
6. Close the panel.

**What you should see:** The **Sort tools** card now shows your avatar. When you reopen it, you see the description with checkboxes, the due date, and your comment.

**Try it:** Check off one box in the description list. Notice it saves immediately.

## Part 5: Move Work Across the Board

1. **Drag and drop:** Drag the **Sort tools** card from **To Do** into **In Progress**.
2. Drag the **Buy shelving** card all the way to **Done**.
3. **Second way to move work:** Open the **Sweep the floor** card. Near the top of the panel, find the status button (it says **To Do**). Click it and choose **In Progress**. Close the panel.

**What you should see:**
- **To Do:** 3 cards
- **In Progress:** 2 cards (Sort tools, Sweep the floor)
- **Done:** 1 card (Buy shelving), possibly shown with a checkmark or strikethrough on the key

> **Why this matters:** Moving cards is how your team signals progress. Anyone looking at the board can see the state of all work at a glance without asking.

## Part 6: Find and Review

1. **Filter the board:** Above the columns, look for the row of filter controls. Click your **avatar** (or the **Assignee** filter and pick yourself).
2. Notice the board now shows only issues assigned to you. Click your avatar again to clear the filter.
3. **Search the board:** In the board's **Search** box (above the columns), type `shelving`.
4. Notice only the two shelving cards remain. Clear the search box.
5. **Search all of Jira:** Click the main search bar at the very top of the screen and type `GC-1`. Select the result to jump straight to that issue.

**What you should see:**
- Step 1: Only **Sort tools** remains on the board.
- Step 3: Only **Buy shelving** and **Install shelving** remain.
- Step 5: The **Sort tools** issue opens in its own full page.

## Part 7: Wrap-Up

**What you learned:**
- Jira organizes work into **projects**, which hold **issues**
- A **board** shows issues in columns that represent **status**
- Issues can carry details: description, assignee, due date, comments
- You move work by dragging cards or changing status inside the issue
- Filters and search help you find work as the board grows

**Suggested next steps:**
1. Finish the garage project: move every card to **Done** and see the empty board.
2. Try **Tutorial #2: Run a One-Week Mini Sprint** to learn backlogs, epics, and sprints.
3. Try **Tutorial #3: Track a Few Fake Bugs** to learn issue types, linking, and saved filters.
