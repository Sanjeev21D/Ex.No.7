# Ex.No.7 Develop a Prompt-Based Personal Productivity Assistant
**Date:** 14.09.2026  
**Name:** SANJEEV D  
**Register no:** 212223040185  

### Aim:
To design and develop a prompt-based personal productivity application using ChatGPT and modern web technologies (React + Tailwind CSS) to organize daily tasks, showing progression from prompt engineering to functional UI execution.

### AI Tools Required:
* **ChatGPT (GPT-4o):** Prompt engineering, UI/UX architecture design, and React component code generation.
* **Node.js & React Environment:** Frontend execution, state management, and real-time interface rendering.
* **Tailwind CSS & Framer Motion:** Glassmorphism styling, layout animations, and responsive dashboard design.

---

### Explanation:
The objective is to utilize natural language prompt engineering to build a personal productivity web application that parses user intent into actionable tasks, automates reminders, and provides focus tools.

**System Workflow:**
`System Persona Prompt` $\rightarrow$ `Natural Language Parsing` $\rightarrow$ `State Update (Chat, Kanban, Calendar)` $\rightarrow$ `Timer & Wellness Trigger`

---

### Core Prompt:
> *"Build a responsive, modern AI Productivity Dashboard web app using React + Tailwind CSS with a minimal glassmorphism design in purple (#9b5de5), blue (#5d4be3), and dark background (#2a1a40).*  
> *Features: Left Sidebar navigation (Dashboard, Tasks, Calendar, Settings), AI Chat assistant parsing natural language task inputs into reminders, interactive Kanban Board (To Do, In Progress, Done), monthly Calendar view, focus Countdown Timer with circular progress, and a minimalist Music Player."*

---

### Implementation Architecture:

1. **`App.js` / State Store:** Central state for active tab, user session, task list, and reminder queues.
2. **`ChatBot.jsx`:** Parses natural language prompts (e.g., *"Prepare CSE notes before 9 PM today"*) into structured task objects:
   ```json
   {
     "id": 1,
     "title": "CSE notes today",
     "deadline": "Mon, Nov 10, 9:00 PM",
     "category": "study",
     "priority": "medium",
     "status": "In Progress"
   }
   ```
3. **`Dashboard.jsx`:** Two-column layout integrating AI chat, active reminder cards, digital focus timer, and background ambient music player.
4. **`KanbanBoard.jsx`:** Multi-column view organizing tasks by lifecycle status (*To Do*, *In Progress*, *Done*).
5. **`CalendarView.jsx`:** Grid representation synchronizing scheduled tasks across month dates.

---

### Output & Experimental Results:

#### 1. Authentication & Onboarding
* **Sign-in Interface:** Clean glassmorphism authentication card supporting demo login credentials.
* **Daily Inspiration Modal:** Startup motivational quote trigger (`"Begin bold, stay consistent."`) with a dismissal option.

*(Insert Figure 1: Login Screen & Figure 2: Daily Inspiration Modal)*

---

#### 2. Main Dashboard (AI Chat & Focus Center)
* **Natural Language Input:** User types *"Prepare CSE notes before 9 PM today"*.
* **AI Agent Response:** Confirms deadline extraction and instantly pins a reminder card with a 12-hour countdown badge and Snooze/Complete actions.
* **Focus Utilities:** 5-minute countdown timer with circular progress and integrated background music controls.

*(Insert Figure 3: Main Dashboard with AI Chat, Reminders, and Timer)*

---

#### 3. Task Management (Kanban Board)
* Automated transition of natural-language-parsed items into structured cards under the **In Progress** board with metadata tags (`medium`, `study`, `coursework`).

*(Insert Figure 4: Kanban Board Task View)*

---

#### 4. Calendar Scheduling
* Automatic mapping of task deadlines to calendar dates (e.g., November 10–11 timeline).

*(Insert Figure 5: Monthly Calendar Schedule)*

---

### Output Verification & Feature Evaluation:

| Feature | Input / Interaction | System Output | Status |
|---|---|---|---|
| **Natural Language Parsing** | *"Prepare CSE notes before 9 PM today"* | Parsed into title, date, priority, and reminder card | Pass |
| **Active Reminders** | Complete / Snooze trigger | State updated and marked across dashboard tabs | Pass |
| **Focus Countdown Timer** | Minutes input (5:00) $\rightarrow$ Start | Interactive digital timer with circular animation | Pass |
| **Multi-View Sync** | Task added in chat | Instantly visible in Kanban & Calendar views | Pass |

---

### Observation:
Iterative prompt engineering enabled the automatic extraction of dates, task titles, and priority levels directly from conversational English. Designing specialized component prompts ensured proper state synchronization between the chat assistant, Kanban board, and calendar without manual schema configuration.

---

### Conclusion:
A responsive, prompt-driven AI productivity assistant was successfully designed and deployed using LLM-assisted code generation. The application effectively processes free-form text into structured productivity workflows across a clean glassmorphism interface.

---
<img width="1919" height="936" alt="image" src="https://github.com/user-attachments/assets/9246b715-feaf-4beb-94f2-e2528c6b9cb2" />
<img width="1517" height="800" alt="image" src="https://github.com/user-attachments/assets/98cb6e5f-0b05-4635-bf0c-883061fface4" />
<img width="1184" height="694" alt="image" src="https://github.com/user-attachments/assets/8ab96562-4251-48de-bf48-b230f5b37d7c" />
<img width="1909" height="789" alt="image" src="https://github.com/user-attachments/assets/6eb418a1-4eea-40aa-8358-0e0ce32a2aa4" />
<img width="1919" height="918" alt="image" src="https://github.com/user-attachments/assets/a88048ee-81ba-489c-a5d1-a49d4fc2e635" />

### Result:
The prompt-based personal productivity application is developed, verified, and executed successfully.
