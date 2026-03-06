# 03 – Technical Work Breakdown

## 💡 Why this exercise matters
Feasibility beats fantasy. This step translates features into components you can actually build.

## 🎯 Expected Outcomes
- Detailed sub-components for each feature  
- Effort estimates (S 1–2 days / M 3–5 / C 6 +)  
- Risk and dependency map  

Disclaimer: this promt assumes that the solution you want to build is involving prompting an LLM. If that is not your canse you need to change the descrition of the Data/Model part .. to train model & build data pipeline 

---

### 🔧 Prompt – Break Down Each Feature
For every MVP Feature, list technical elements required:

| Area | Description | Effort (S/M/C) | Risks |
|------|---------------|----------------|-------|
| Data / Model | Prompt design or fine-tuning needs |  |  |
| Backend | APIs / endpoints to serve model results |  |  |
| Frontend | Input forms, results display in Lovable |  |  |
| Integration | Link model API → UI → analytics |  |  |
| Analytics | Metrics to track usage / success |  |  |

**Example – Skills Extractor:**  
- Prompt Design (S 1 day)  
- FastAPI `/extract_skills` (M 3 days)  
- Frontend input form (S 1 day)  
- Testing + debugging (S 1 day)
