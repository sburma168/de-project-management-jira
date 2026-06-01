# 🎓 Student Worksheet
## Hands-On Activity: Managing a Project with GitHub Issues & Projects

**Name:** ___________________________  
**Date:** ___________________________

---

## 🎯 Objective
In this activity, you'll act as a member of a software development team managing a project
using GitHub Issues and GitHub Projects — the same workflow used with JIRA in the industry.

---

## 📖 Reference: JIRA ↔ GitHub Cheat Sheet

| What you'd say in JIRA | What it's called in GitHub |
|------------------------|---------------------------|
| Project | GitHub Project (Board) |
| Epic | Milestone |
| Story / Task / Bug | Issue |
| Sub-task | Checklist inside an Issue |
| Sprint | Iteration |
| Ticket Status | Board Column (To Do, In Progress, Done) |
| Story Points | Custom Number Field |
| Assignee | Assignee |
| Reporter | Issue Author |
| Comment | Issue Comment |
| Kanban Board | Board View in GitHub Projects |
| Roadmap | Roadmap View in GitHub Projects |

---

## 🏗️ Scenario

You are part of the development team for **"TaskFlow App"** — a simple to-do list application.
Your team is working on **Sprint 1**, which focuses on user authentication features.

Your Project Board has these columns: `Backlog | To Do | In Progress | In Review | Done`

---

## ✏️ Part 1 — Understanding Issues (Tickets)

Your instructor will show you the Issues tab in the demo repository.

**Answer these questions:**

1. How many issues (tickets) are currently open?  
   `Answer: _______________`

2. Find the issue titled **"Login page crashes on mobile"**.  
   What **label** does it have?  
   `Answer: _______________`  
   What type of ticket is this in JIRA terms?  
   `Answer: _______________`

3. Which **Milestone (Epic)** do most of the authentication issues belong to?  
   `Answer: _______________`

4. Look at any issue. What information does the issue contain?  
   List at least **4 fields** you see:  
   ```
   1. _______________
   2. _______________
   3. _______________
   4. _______________
   ```

---

## ✏️ Part 2 — Create Your Own Issue (Ticket)

In the demo repository, create a new GitHub Issue using the details below.

**Your ticket:**
- **Title:** `As a user, I can reset my password via email`
- **Description** (write a user story):
  ```
  ## User Story
  As a registered user, I want to reset my password via email so that 
  I can regain access to my account if I forget my password.

  ## Acceptance Criteria
  - [ ] User can click "Forgot Password" on the login page
  - [ ] User receives a password reset email within 2 minutes
  - [ ] Reset link expires after 24 hours
  - [ ] User is redirected to login after successful reset
  ```
- **Label:** `enhancement`
- **Milestone:** `v1.0 — User Authentication`
- **Assignee:** Assign it to yourself
- **Story Points:** 5

**After creating your issue, answer:**

5. What is the Issue number GitHub assigned to your ticket?  
   `Answer: #_______________`

6. In JIRA, what would the checklist items under "Acceptance Criteria" be called?  
   `Answer: _______________`

---

## ✏️ Part 3 — Working the Board

Navigate to the **GitHub Project Board** (TaskFlow Sprint Board).

7. How many issues are currently in the **Backlog** column?  
   `Answer: _______________`

8. Find the issue **"Login page crashes on mobile"** on the board.  
   Move it to **"In Progress"**.  
   In JIRA terms, what did you just do to this ticket?  
   `Answer: _______________`

9. Now move the same issue to **"In Review"**.  
   What does this status mean in a real team workflow?  
   `Answer: _______________`

10. Switch to the **Table View** of the project.  
    List two pieces of information that are easier to see in Table View vs Board View:  
    ```
    1. _______________
    2. _______________
    ```

---

## ✏️ Part 4 — Sprint Planning Simulation

Your team is planning **Sprint 1**. You have the following issues in the backlog and
a team capacity of **20 Story Points** for this sprint.

| Issue | Story Points |
|-------|-------------|
| As a user, I can log in with my email | 5 |
| As a user, I can create a new task | 3 |
| Login page crashes on mobile | 2 |
| Design the dashboard layout | 8 |
| Set up CI/CD pipeline | 5 |
| Password reset not sending email | 3 |
| As a user, I can reset my password via email (yours!) | 5 |

11. Which issues would you include in Sprint 1 to stay within 20 points?  
    Write them out and show your total:  
    ```
    Issues selected:
    - _________________________________ (__ pts)
    - _________________________________ (__ pts)
    - _________________________________ (__ pts)
    - _________________________________ (__ pts)
    Total: __ / 20 points
    ```

12. In the Project, assign your selected issues to **Sprint 1** (Iteration 1).

---

## ✏️ Part 5 — Closing the Loop

13. Go back to the issue you created in Part 2.  
    Add a **comment** that says:  
    > "Work complete — implemented password reset flow with 24-hour expiry token. PR opened for review."

    In a real team, why is commenting on tickets important?  
    `Answer: _______________`

14. Now **close your issue**.  
    What column did it move to on the board?  
    `Answer: _______________`

---

## 🧠 Reflection Questions

15. A new developer joins your team. How would they use the GitHub Project Board to
    understand what the team is working on?  
    ```
    _______________________________________________
    _______________________________________________
    _______________________________________________
    ```

16. What is one advantage of linking GitHub Issues directly to Pull Requests  
    (e.g., using "Fixes #5" in a PR)?  
    ```
    _______________________________________________
    _______________________________________________
    ```

17. Name **two ways** GitHub Issues/Projects and JIRA are similar:  
    ```
    1. _______________________________________________
    2. _______________________________________________
    ```

18. Name **one way** JIRA might be more powerful or different from GitHub Projects:  
    ```
    _______________________________________________
    ```

---

## ⭐ Bonus Challenge

Create a second issue for a **bug** you invent yourself for the TaskFlow app.  
Make sure to include:
- A descriptive title
- Steps to reproduce the bug
- Expected vs actual behavior
- The `bug` label
- An estimated Story Point value
- Assignment to the correct Milestone

**Issue # created:** `#_______________`

---

## 📝 Summary

Complete this table based on what you learned today:

| JIRA Term | GitHub Equivalent |
|-----------|-------------------|
| Epic | |
| Story | |
| Sub-task | |
| Sprint | |
| Kanban Board | |
| Story Points | |
| Ticket Status | |