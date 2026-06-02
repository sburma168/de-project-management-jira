# Student Guide: JIRA Concepts with GitHub Issues & Projects

Follow this guide to learn JIRA concepts using GitHub. It's written for learners: clear steps, short tasks, and examples you can follow.

## How long this takes
- Introduction & overview: 20 min
- Live demo / hands-on: 25 min
- Practice activity: 40 min
- Review & reflection: 15 min

## Before you start (do these once)
1. Create a public GitHub repository named `project-management-demo` (or any name).
2. Add a simple `README.md` describing a fictional project (example below).

Suggested project: "TaskFlow App — a basic to-do web app. We're building v1.0: user login, task creation, dashboard."

## Quick setup (follow these steps in your repo)
1. Create these Issues (use Issues → New Issue). Copy titles and add one label each:
   - As a user, I can log in with my email — label: `enhancement`
   - As a user, I can create a new task — label: `enhancement`
   - Login page crashes on mobile — label: `bug`
   - Design the dashboard layout — label: `design`
   - Set up CI/CD pipeline — label: `infrastructure`
   - Password reset not sending email — label: `bug`

2. Add Labels (Issues → Labels): `bug`, `enhancement`, `design`, `infrastructure`, `in-review`.

3. Create a Milestone (Issues → Milestones → New):
   - Name: `v1.0 — User Authentication`
   - Due date: two weeks from today
   - Assign issues: login, create task, mobile crash, password reset

4. Create a Project board (top-right → Projects → New Project):
   - Choose Board template
   - Name: `TaskFlow Sprint Board`
   - Add columns: Backlog, To Do, In Progress, In Review, Done
   - Add the six issues to the board (start them in Backlog)
   - (Optional) Add custom field: Story Points (Number) and an Iteration/Sprint field

## Walkthrough — what to try

1) Inspect an Issue
- Open an issue and note Title, Description, Labels, Assignees, Milestone.
- Add a comment like: "Starting work on the login form today." Practice leaving updates.
- Add a task list in the description:
  - [ ] Build login form HTML
  - [ ] Connect to backend API
  - [ ] Write unit tests

2) Use Milestones as Epics
- Open the `v1.0 — User Authentication` milestone and view its progress bar — this shows percent complete for the epic.

3) Use the Project Board
- Open your Project in Board view. Drag a card from Backlog → In Progress to simulate picking up work.
- Switch to Table view and enter Story Points (e.g., 3, 5, 2, 8, 5, 3) to practice estimating effort.
- Check the Roadmap (if available) to see Milestones on a timeline.

4) Simulate a Sprint
- Assign issues to a two-week Sprint/Iteration and move the selected issues into that Sprint.

5) Close an Issue
- When work is complete, close the issue and verify it moves to Done on the board.

## Bonus: link work to code
When creating a Pull Request, include `Fixes #<issue-number>` in the PR description. When the PR merges, the referenced issue closes automatically.

## Key points to remember
- GitHub Issues = JIRA tickets; Milestones = Epics; Projects = Boards; Iterations = Sprints.
- Issues are the record of work and decisions — use comments and checklists to explain why things changed.
- Labels and Milestones help you filter and group work at scale.

## Reflection questions
1. What is the GitHub equivalent of a JIRA Epic?
2. Why do teams assign Story Points to issues?
3. What happens when a PR with `Fixes #5` is merged?
4. How does the Board view differ from the Table view?
5. As a new team member, how would you use the board to find tasks to work on?

---

Updated: student-facing guide. Follow the Quick setup and Walkthrough to practice.