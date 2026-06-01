# 🧑‍🏫 Instructor Guide
## Lesson: JIRA Concepts via GitHub Issues & Projects

---

## ⏱️ Suggested Timing
| Section | Time |
|---------|------|
| Introduction & Lecture | 20 min |
| Live Demo | 25 min |
| Student Activity | 40 min |
| Review & Debrief | 15 min |
| **Total** | **~100 min** |

---

## 🛠️ Pre-Class Setup (Do This Before Lesson)

### 1. Create a Demo Repository
- Create a **public** GitHub repo called `project-management-demo` (or similar)
- Add a basic `README.md` describing a fictional project (see suggested project below)

**Suggested Fictional Project:**  
> *"TaskFlow App — A simple to-do list web application. The team is building v1.0 which includes
> user login, task creation, and a dashboard."*

### 2. Pre-Create Issues for Demo
Create the following issues ahead of time so the board isn't empty during the demo:

| # | Title | Type | Label |
|---|-------|------|-------|
| 1 | As a user, I can log in with my email | Story | `enhancement` |
| 2 | As a user, I can create a new task | Story | `enhancement` |
| 3 | Login page crashes on mobile | Bug | `bug` |
| 4 | Design the dashboard layout | Task | `design` |
| 5 | Set up CI/CD pipeline | Task | `infrastructure` |
| 6 | Password reset not sending email | Bug | `bug` |

### 3. Create Labels
Go to **Issues → Labels** and create:
- `bug` (red) — Something isn't working
- `enhancement` (blue) — New feature or request
- `design` (purple) — UI/UX work
- `infrastructure` (orange) — DevOps/backend setup
- `in-review` (yellow) — Ready for code review

### 4. Create a Milestone (= JIRA Epic)
- Go to **Issues → Milestones → New Milestone**
- Name: `v1.0 — User Authentication`
- Due date: 2 weeks from today
- Assign issues #1, #2, #3, #6 to this milestone

### 5. Create a GitHub Project (= JIRA Board)
- Go to your org/profile → **Projects → New Project**
- Choose **Board** template
- Name it: `TaskFlow Sprint Board`
- Add columns: `Backlog`, `To Do`, `In Progress`, `In Review`, `Done`
- Add all 6 issues to the board (start them all in Backlog)
- Create a custom field: **Story Points** (Number type)
- Set up an **Iteration** field named "Sprint" with 2-week sprints

---

## 🎬 Live Demo Script

### Part 1 — Introduce the Concept (Lecture Slides or Whiteboard)

**Say:**
> "In the industry, teams use tools like JIRA to track all the work on a project.
> Every task, bug, and feature lives as a **ticket**. Today we're going to learn
> those same concepts using GitHub — which many companies also use, and which
> works nearly identically to JIRA."

**Draw or show on whiteboard:**
```
JIRA Project  →  GitHub Project Board
JIRA Epic     →  GitHub Milestone  
JIRA Ticket   →  GitHub Issue
JIRA Sprint   →  GitHub Iteration
```

---

### Part 2 — Demo: The GitHub Issues Interface

**Show students:**

1. **Navigate to Issues tab** in your demo repo
   - Point out: Title, Description, Labels, Assignees, Milestones
   - Say: *"This is identical to a JIRA ticket. In JIRA they call it a Story, Task, or Bug — here we just call it an Issue."*

2. **Open Issue #1** ("As a user, I can log in...")
   - Show the **Assignee** field → *"In JIRA this is also called the Assignee"*
   - Show the **Labels** field → *"In JIRA these are called Labels or Components"*
   - Show the **Milestone** field → *"In JIRA, this is your Epic — the big feature this belongs to"*
   - Add a **comment**: type "Starting work on the login form today" → *"In JIRA, teammates comment on tickets to give updates"*
   - Check off a sub-task in the description if you have one, or add a task list:
     ```
     - [ ] Build login form HTML
     - [ ] Connect to backend API
     - [ ] Write unit tests
     ```
   - Say: *"In JIRA, these are Sub-tasks"*

3. **Show Milestones page**
   - Navigate to Issues → Milestones
   - Open `v1.0 — User Authentication`
   - Show the progress bar → *"This is exactly like a JIRA Epic — it shows how much of the work is done"*

---

### Part 3 — Demo: The GitHub Project Board

**Show students:**

1. **Navigate to the Project Board**
   - Switch to **Board view**
   - Say: *"This is your Kanban board — identical to the JIRA board view. Each card is a ticket (Issue)."*
   - **Drag Issue #1** from `Backlog` → `In Progress`
   - Say: *"In JIRA you do the same thing — drag the ticket to update its status. The developer picks it up, drags it to 'In Progress'."*

2. **Show the Table view**
   - Switch to **Table view**
   - Show Story Points field — enter some values (3, 5, 2, 8, 5, 3)
   - Say: *"Story Points estimate how hard a task is. Teams use these in Sprint Planning."*

3. **Show the Roadmap view**
   - Switch to **Roadmap view**
   - Say: *"In JIRA this is the Roadmap — you can see Epics/Milestones on a timeline."*

4. **Simulate a Sprint**
   - Show the **Iteration/Sprint** field
   - Move issues #1 and #2 into Sprint 1
   - Say: *"This is Sprint Planning in JIRA — the team decides what they'll complete in the next two weeks."*

5. **Close an Issue = Complete a Ticket**
   - Open Issue #4 (Design the dashboard layout)
   - Say: *"When a developer finishes their work, they close the ticket."*
   - Click **Close Issue**
   - Go back to the board — it moves to `Done`
   - Say: *"In JIRA you'd transition the ticket to 'Done'. GitHub does this automatically when an issue is closed."*

---

### Part 4 — Bonus: Linking Issues to Code (Autoclose)

**Show in a demo commit or PR description:**

```
Fixes #3
```

- Say: *"When a developer opens a Pull Request, they can reference the Issue number.
  When the PR merges, GitHub automatically closes the Issue and moves it to Done.
  JIRA has the same integration with Git — it's called Smart Commits."*

---

## 🗣️ Key Talking Points

- **"JIRA is just a fancier version of this."** GitHub Projects and JIRA use the same Agile methodology. Skills learned here transfer directly.
- **Tickets = Communication.** Issues aren't just to-do items — they're the paper trail of *why* decisions were made.
- **The board tells the story of a Sprint.** A healthy board has most cards in "Done" by end of sprint.
- **Labels help filter at scale.** On real teams with 100s of tickets, labels/components are how you find things fast.

---

## ✅ Debrief Questions to Ask the Class

1. What is the GitHub equivalent of a JIRA Epic?
2. Why would you assign Story Points to an Issue?
3. What happens to a GitHub Issue when a PR with "Fixes #5" is merged?
4. What's the difference between the Board view and the Table view in GitHub Projects?
5. If you're a new developer joining a team, how would you use the board to understand what needs to be done?