# 🧭 NorthStar — AI-Powered Career Discovery & Planning

**Find your direction. Build your roadmap. Take your next step.**

NorthStar is an early-stage career guidance platform designed to help college students explore career options, understand their strengths, compare potential career paths, and turn uncertainty into actionable learning plans.

The project focuses on creating a personalized, student-friendly experience that connects career discovery with practical next steps, skill development, and internship preparation.

> **Project status:** Interactive prototype
> **Project type:** Product Management / UI-UX / AI-assisted product concept
> **Target users:** College students and early-career individuals
> **Primary goal:** Help students move from career confusion to informed exploration and action.

---

## 📌 Table of Contents

- [Problem Statement](#-problem-statement)
- [Product Vision](#-product-vision)
- [Target Users](#-target-users)
- [Core Features](#-core-features)
- [User Journey](#-user-journey)
- [Usability and Acceptance Audit](#-usability-and-acceptance-audit)
- [Issues Identified and Proposed Fixes](#-issues-identified-and-proposed-fixes)
- [Acceptance Criteria](#-acceptance-criteria)
- [Accessibility and UX Considerations](#-accessibility-and-ux-considerations)
- [Technology and Tools](#-technology-and-tools)
- [Known Limitations](#-known-limitations)
- [Future Improvements](#-future-improvements)
- [Success Metrics](#-success-metrics)
- [Getting Started](#-getting-started)
- [Disclaimer](#-disclaimer)

## 🚩 Problem Statement

Many college students struggle to choose a career because they lack clear information about different roles, the skills those roles require, and the steps needed to enter them.

Existing career resources can feel overwhelming, disconnected, or too generic. Students may discover a career but still not know what to learn, which projects to build, or how to prepare for internships.

NorthStar aims to bridge this gap by connecting career exploration with personalized planning and progress tracking.

## 💡 Product Vision

Help every student make more informed career decisions through guided discovery, transparent recommendations, and achievable next steps.

NorthStar is designed around three principles:

1. **Discover before deciding:** Students should explore multiple paths rather than feel pressured to choose one career immediately.
2. **Explain recommendations:** Users should understand why a career is suggested and where their skill gaps lie.
3. **Turn insight into action:** Every recommendation should lead to a practical next step.

## 👥 Target Users

### Primary persona: The uncertain college student

- Is exploring career options for the first time.
- Has multiple interests but lacks direction.
- Is unsure which skills to learn.
- Wants to prepare for internships.
- Needs a manageable plan rather than a long list of resources.

### Example scenario

A computer science student enjoys understanding user problems and designing ideas but is unsure whether Product Management or Product Design would be a better fit.

NorthStar helps the student compare both careers, explore their differences, select a path to investigate, create a learning roadmap, and begin preparing for relevant opportunities.

## ✨ Core Features

### 1. Guided Career Assessment

An onboarding flow that collects information about:

- Education and current stage.
- Interests and strengths.
- Work preferences.
- Career priorities.
- Current skills and experience.
- Personal learning goals.

The assessment is intended to support exploration, not make definitive judgments about a user's abilities.

### 2. Career Discovery

Explore career paths such as:

- Product Manager
- Product Designer
- UX Researcher
- Software Engineer
- Data Analyst
- AI/ML Engineer
- Business Analyst
- AI Product Manager

Career cards can communicate role responsibilities, relevant skills, possible entry routes, and suggested first steps.

### 3. Career Comparison

Compare career paths side by side using factors such as:

- Day-to-day responsibilities.
- Technical intensity.
- Creativity and problem-solving.
- Communication and collaboration.
- Required skills.
- Learning effort.
- Beginner-friendly projects.
- Internship preparation.

The goal is to help users make informed decisions based on their priorities rather than rank careers universally.

### 4. Personalized Roadmap

Generate a career exploration plan with:

- Weekly learning goals.
- Skill-building tasks.
- Learning resources.
- Practice exercises.
- Portfolio project milestones.
- Progress indicators.
- Reflection checkpoints.

Users should be able to mark tasks complete and see their progress update.

### 5. Internship Tracker

A dedicated workspace for organizing internship opportunities.

Example application statuses:

`Interested → Preparing → Applied → Interviewing → Offer`

Users can maintain notes, track deadlines, and record follow-up actions. These statuses represent a workflow, not a prediction of application outcomes.

### 6. Progress Dashboard

A central view of the user's career exploration journey, including:

- Roadmap completion.
- Completed learning tasks.
- Skills practiced.
- Career paths explored.
- Internship application activity.
- Upcoming milestones.
- Suggested next actions.

### 7. Contextual Career Assistant

A proposed assistant experience for questions such as:

- Why might this career suit me?
- How do Product Management and Product Design differ?
- What should I learn this week?
- Which beginner project should I build?
- What can I explore if I don't enjoy coding?

Responses should be transparent about uncertainty and distinguish simulated responses from real AI-generated advice.

---

## 🔄 User Journey

The primary user journey follows this sequence:

1. A student opens NorthStar.
2. The student completes the onboarding assessment.
3. NorthStar presents career suggestions with explanations.
4. The student explores Product Manager and Product Designer.
5. The student compares both career paths.
6. The student chooses one path to explore further.
7. The student generates a personalized learning roadmap.
8. The student completes a roadmap task.
9. The dashboard updates progress.
10. The student adds an internship opportunity and updates its application status.

The intended outcome is a clear next step, not a permanent or irreversible career decision.

## 🧪 Usability and Acceptance Audit

### Audit objective

Evaluate NorthStar from the perspective of a first-time student who feels uncertain about their career.

The audit focuses on navigation, task completion, recommendation clarity, state consistency, accessibility, and unnecessary interaction.

**Audit method:** Simulated first-time-user walkthrough and acceptance-test checklist.

**Important:** This document defines the audit scenario and the issues to inspect. It does not claim that automated tests, live usability sessions, or fixes have been executed. Actual results must be recorded after testing the generated prototype.

### Scenario walkthrough

| Step | User action              | Expected behavior                               |
| ---- | ------------------------ | ----------------------------------------------- |
| 1    | Open NorthStar           | Clear introduction and primary CTA              |
| 2    | Complete onboarding      | Selections persist between steps                |
| 3    | View recommendations     | Explanations accompany match indicators         |
| 4    | Explore two careers      | Detailed information is easy to access          |
| 5    | Compare both careers     | Differences and trade-offs are understandable   |
| 6    | Choose a career          | Selection leads to a relevant roadmap           |
| 7    | Generate roadmap         | Tasks match the selected career and skill level |
| 8    | Complete a task          | Completion state and progress update            |
| 9    | Add an internship        | Opportunity appears in the tracker              |
| 10   | Change internship status | Updated status persists and is visible          |

### Issues to inspect

#### 1. Onboarding friction

**Potential issue:** Too many questions may overwhelm students before they experience value.

**Proposed fix:**

- Show a clear progress indicator.
- Group related questions.
- Provide Back and Continue controls.
- Allow users to revise answers.
- Use sensible defaults and optional fields where possible.

**Acceptance test:** A user can complete onboarding, navigate backward, and return without losing previous selections.

#### 2. Misleading career recommendations

**Potential issue:** Match percentages may appear scientifically validated despite being based on simple prototype logic.

**Proposed fix:**

- Label scores as illustrative.
- Explain which preferences influenced each recommendation.
- Display skill gaps and trade-offs.
- Avoid presenting recommendations as definitive career assessments.

**Acceptance test:** Users can understand why a career appears in their recommendations and what the score does and does not mean.

#### 3. Career comparison complexity

**Potential issue:** Comparing too many dimensions can create a dense, difficult-to-scan interface.

**Proposed fix:**

- Limit comparisons to three careers.
- Prioritize the most decision-relevant factors.
- Use consistent labels and concise explanations.
- Preserve selected careers when switching between pages.

**Acceptance test:** The user can compare Product Manager and Product Designer without reselecting them after navigation.

#### 4. Roadmap tasks that do not affect progress

**Potential issue:** Completing a task may update one card but leave dashboard metrics unchanged.

**Proposed fix:**

- Use a shared source of truth for task state.
- Recalculate completion counts and progress indicators consistently.
- Prevent duplicate completion updates.
- Preserve completed tasks when users revisit the roadmap.

**Acceptance test:** Completing a task updates the task card, roadmap progress, and dashboard summary consistently.

#### 5. Internship tracker state inconsistency

**Potential issue:** Application status changes may not persist or appear in summaries.

**Proposed fix:**

- Use a defined set of application statuses.
- Update the tracker immediately after a status change.
- Validate required fields.
- Provide an understandable empty state and confirmation feedback.

**Acceptance test:** Adding an internship and changing its status produces a visible, consistent update across relevant views.

#### 6. Dead buttons and broken navigation

**Potential issue:** Generated screens may contain controls without functional destinations.

**Proposed fix:**

- Audit every primary CTA.
- Connect each navigation item to a valid destination.
- Implement a meaningful result for interactive controls.
- Remove or disable unsupported actions with a clear explanation.

**Acceptance test:** Every primary action has a defined and observable outcome.

#### 7. Lost user state

**Potential issue:** Refreshing or navigating away may reset the user's assessment, bookmarks, or roadmap.

**Proposed fix:**

- Use shared application state.
- Add browser-local persistence where supported.
- Handle missing or invalid saved data gracefully.
- Provide an explicit way to reset demo data.

**Acceptance test:** Saved data survives refreshes where persistence is implemented and supported.

## 🛠️ Issues Identified and Proposed Fixes

The following is the implementation checklist for the usability audit. These are candidate fixes to verify in the running prototype, not claims that each issue has already been observed or resolved.

- [ ] Simplify onboarding and clarify progress.
- [ ] Preserve assessment answers across navigation.
- [ ] Explain recommendation logic and label illustrative scores.
- [ ] Make career comparisons consistent and easy to scan.
- [ ] Connect career selection to roadmap generation.
- [ ] Synchronize task completion across all progress views.
- [ ] Preserve internship status updates.
- [ ] Fix dead buttons and invalid navigation destinations.
- [ ] Add loading, success, error, and empty states where appropriate.
- [ ] Test persistence after refresh.
- [ ] Verify keyboard navigation and visible focus states.
- [ ] Test layouts at desktop, tablet, and mobile widths.
- [ ] Review contrast, labels, and screen-reader accessibility.

Record each finding with severity, reproduction steps, expected behavior, actual behavior, and verification status after testing.

## ✅ Acceptance Criteria

NorthStar's core prototype should satisfy the following criteria before being presented as a working demonstration.

### Core functionality

- [ ] A first-time user can complete onboarding.
- [ ] Assessment answers persist between steps.
- [ ] Career recommendations display explanations.
- [ ] Career detail pages open correctly.
- [ ] Users can save and unsave career paths.
- [ ] Users can compare Product Manager and Product Designer.
- [ ] Selecting a career leads to a relevant roadmap.
- [ ] Users can mark roadmap tasks complete and incomplete.
- [ ] Progress indicators update consistently.
- [ ] Users can add an internship and update its status.
- [ ] Navigation works across all core screens.
- [ ] User state persists after refresh where supported.

### UX and accessibility

- [ ] Primary buttons have clear labels and outcomes.
- [ ] Interactive elements have visible focus states.
- [ ] Forms communicate validation errors clearly.
- [ ] Color is not the only way to communicate status.
- [ ] Text and controls have sufficient contrast.
- [ ] Layouts remain usable on smaller screens.
- [ ] Destructive actions require appropriate confirmation.
- [ ] Recommendations do not imply certainty or guaranteed outcomes.

## ♿ Accessibility and UX Considerations

NorthStar should follow inclusive design practices, using WCAG 2.2 AA as a target for accessibility review.

Key considerations:

- Semantic headings and meaningful page structure.
- Keyboard-accessible navigation and controls.
- Visible keyboard focus.
- Descriptive labels for form inputs.
- Accessible names for icon-only buttons.
- Adequate text and interface contrast.
- Clear validation and error messages.
- Status updates that are not communicated through color alone.
- Responsive layouts and readable text.
- Respect for reduced-motion preferences.
- Plain language that avoids unnecessarily technical career terminology.

Accessibility should be verified in the actual implementation rather than assumed from visual appearance.

## 🧰 Technology and Tools

| Tool          | Intended use                                             |
| ------------- | -------------------------------------------------------- |
| Google Stitch | UI generation and interface prototyping                  |
| Antigravity   | Potential AI-assisted implementation and code refinement |
| Figma         | Optional design refinement and prototyping               |
| GitHub        | Version control, documentation, and project presentation |

The final implementation stack depends on the exported code and the development environment selected.

**Note:** The tools above describe the intended workflow. The exact framework, persistence method, and integrations must be confirmed from the actual project files.

## ⚠️ Known Limitations

As an early-stage prototype, NorthStar may have the following limitations:

- Career recommendations may use sample data or deterministic rules rather than a trained or connected AI model.
- Match percentages may be illustrative rather than empirically validated.
- Salary information may be unavailable or require verified external data.
- Internship listings may be demonstration records rather than live opportunities.
- Persistent storage may be limited to the browser and current device.
- Authentication and multi-user accounts may not be implemented.
- A contextual career assistant may use predefined responses rather than a real language model.
- Automated accessibility and usability testing may not yet have been performed.
- The prototype cannot establish whether the product improves real-world career outcomes without user research.

These limitations should be clearly disclosed during demonstrations.

## 🚀 Future Improvements

Potential next steps include:

1. Conduct usability sessions with college students.
2. Validate the assessment questions and recommendation logic.
3. Add a real AI service with transparent, grounded career guidance.
4. Integrate verified career resources and internship listings.
5. Introduce secure user accounts and cross-device synchronization.
6. Build an editable portfolio-project planner.
7. Add resume and internship-readiness assessments.
8. Track product analytics with appropriate privacy safeguards.
9. Run accessibility checks and automated end-to-end tests.
10. Iterate based on measured user feedback.

## 📊 Success Metrics

NorthStar's effectiveness should be evaluated through measurable user outcomes rather than screen count or visual polish alone.

| Metric                              | What it measures                                         |
| ----------------------------------- | -------------------------------------------------------- |
| Onboarding completion rate          | Percentage of users who finish the assessment            |
| Time to first useful recommendation | How quickly users receive relevant guidance              |
| Career comparison completion        | Whether users can evaluate multiple paths                |
| Roadmap creation rate               | Percentage of users who create a plan                    |
| First-task completion rate          | Whether users take an actionable next step               |
| Internship tracker adoption         | Whether users organize their applications                |
| Task completion consistency         | Whether progress remains synchronized                    |
| User-reported clarity               | Whether users feel more informed after using the product |

Baseline values and targets should be established through research and prototype testing rather than invented in advance.

## 💻 Getting Started

### View the prototype

Open the NorthStar prototype in the environment where it has been generated and verify that its navigation and interactions work.

### Run the project locally

If the prototype has been exported as a web application:

1. Clone the GitHub repository.
2. Review the project files and README for the actual framework and dependencies.
3. Install the dependencies using the appropriate package manager.
4. Configure any required environment variables.
5. Start the development server using the command specified by the project's configuration.
6. Test the primary user journey using the acceptance criteria above.

Example:

```bash
git clone <your-repository-url>
cd <your-project-directory>
```

The installation and startup commands depend on the actual exported project. They should be added once the framework and package configuration are confirmed.

## 📝 Disclaimer

NorthStar is intended to support career exploration and planning. It does not determine a student's ideal career, guarantee employment, or replace professional career counselling.

Users should evaluate recommendations against their own interests, circumstances, research, and experiences.

---

**Built as a product-thinking project:** turning an ambiguous student problem into a structured, testable, user-centered experience.

*NorthStar — Your next step starts here.*
