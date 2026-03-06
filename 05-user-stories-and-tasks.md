# 05 – User Stories and Task Mapping

## 💡 Why this exercise matters
This final step connects strategy to execution.  
By breaking features into daily tasks, you create a clear plan for your 3-person team.

## 🎯 Expected Outcomes
- User stories linked to Outcome Goals  
- Deliverables and 1-day tasks for each Epic  
- Optional personal learning goal per member  

---

### 🔧 Prompt – From Goals to Detailed Tasks

For each Outcome Goal / Epic:

1. Write **user stories** with acceptance criteria.
2. Break them into **atomic tasks (≤1 day)** that can be independently verified.
3. For each task, include:
   - **Component / file / API affected**
   - **Input–Output / success condition**
   - **Acceptance criteria**
   - **Dependencies**

| Level | Description | Owner | Est. Effort | Acceptance Criteria |
|--------|--------------|--------|--------------|---------------------|
| **Outcome Goal** | User + learning goal summary | PM | – | – |
| **Epic** | High-level feature | Team | – | – |
| **User Story** | As a [user], I want to [goal] so that [benefit]. | PM | – | Clear before/after user behavior |
| **Deliverables** | Components to build | Dev Leads | – | – |
| **Tasks (≤ 1 day)** | Technical implementation steps (mention file, API, function) | Individual | ≤1d | Clear pass/fail test |
| **Learning Goal (optional)** | What each member practices | Each | – | – |

🧩 **Guideline:**  
Tasks should be small enough to commit and review in a single day (≈2–4 hours focused work).  
Each should end in a *testable change*—a new API route, working UI component, logged metric, etc.


---

### Bonus - Mermaid chart

Once you have your tasks you can prompt ChatGPT to prepare the data for a mermaid chart, for example gantt, and you can specify that you want the tasks to be sorted in the order they should be done, with maximum 3 tasks in paralle and color by epic.. then go to https://mermaid.live

---

### 🧩 Example – *DataPath AI* MVP

**Outcome Goal**  
> In 3 weeks, data analysts will receive AI-generated career matches resulting in 70 % rating them more relevant than current job-search methods,  
> and our team will learn to deploy a complete LLM pipeline end-to-end.

---

#### 🧱 Epic A – Narrative → Skills Extractor  
**Purpose:** Turn free-text project stories into structured skill outputs.

**User Stories**
1. *As a data analyst, I want to paste a project story and get extracted skills so that I can see how AI understands my experience.*  
 **Acceptance Criteria:** Text field (max 800 chars) → “Analyze” button → API returns JSON `{skills:[]}` → tags displayed.
2. *As a user, I want to edit the skills list so that I can correct mistakes.*  
 **Acceptance Criteria:** Tags are editable; “Save” updates local state.

**Deliverables**
- Input Form + Validation  
- `/extract_skills` API endpoint  
- Skill Tag Display Component  

**Tasks**
- [ ] Write and test OpenAI prompt for skill extraction (1 day)  
- [ ] Build FastAPI endpoint (2 days)  
- [ ] Connect frontend form → API (1 day)  
- [ ] Implement editable skill tags (1 day)  
- [ ] Add error handling & logging (1 day)  
- [ ] QA test and fix (0.5 day)

....

✅ **Deliverable:** A 3-week MVP implementation plan that connects user value, feasibility, and team learning.  
