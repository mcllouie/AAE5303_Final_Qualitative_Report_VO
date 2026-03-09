# AAE5303 Individual Report on Six Qualitative Indicators

## 1. Purpose

This is an **individual** report. Every student submits **their own** Markdown report after the final project presentation.

Although the course project is completed in teams, this report is **not** a team report. The purpose is to document:

- your own technical growth,
- your own use of AI-assisted engineering tools,
- your own engineering judgment,
- your own contribution to the project,
- and your own reflection on what worked, what failed, and what should be redesigned.

The report should be suitable for a GitHub repository and readable as a technical reflection document.

---

## 2. What this report should reflect

This report is designed to match the structure of the course:

- project-based learning around **Visual Odometry / VSLAM**,
- **3D Gaussian Splatting** / 3D reconstruction,
- **2D semantic segmentation** for aerial scenes,
- use of **MARS-LVIG** and **UAVScenes**,
- end-to-end integration,
- benchmarking with metrics such as **RMSE**, **IoU**, and **mIoU**,
- and final reflection on lessons learned.

It is also designed to align with the logic of the pre-class survey, which emphasizes:

- AI literacy,
- prompting and AI co-creation,
- hallucination awareness,
- verification against theory and documentation,
- debugging and troubleshooting,
- reproducibility,
- benchmarking,
- and responsible use of AI in engineering work.

---

## 3. Submission mode: individual, not team

### Required rule
Each student must submit **their own report**, even if the project implementation was completed as a team.

### What this means in practice
You may refer to:

- the **team repository**,
- the **team benchmark results**,
- the **team presentation**,
- and the **team pipeline**,

but you must clearly separate:

1. **Team result**  
2. **My role / my contribution**  
3. **My evidence**  
4. **My reflection / my learning**

### Writing rule
Write mainly in **first person singular**:

- `I configured ...`
- `I verified ...`
- `I changed ...`
- `I compared ...`
- `I found ...`
- `I learned ...`

Use `we` only when you are describing a genuine team-level artifact.

### Important
Do **not** claim team work as personal work unless your own role is clearly identified and traceable.

---

## 4. Deliverable format

### Required deliverable
Submit **one Markdown file**.

Recommended options:

- `README.md`
- `[student_id]_six_indicators_report.md`

### Optional supporting folder
If needed, include an `assets/` folder for figures.

### Recommended GitHub structure
```text
reports/
└── [student_id]_[name]/
    ├── README.md
    └── assets/
        ├── fig1_pipeline.png
        ├── fig2_vo_debug.png
        ├── fig3_reconstruction.png
        └── fig4_segmentation.png
```

### If using a personal repo
```text
README.md
assets/
```

### Formatting rules
- Use **relative paths** for figures.
- Use Markdown tables where possible.
- Use explicit file paths in backticks, for example: `configs/orbslam3/uav.yaml`
- If you reference a result from a specific commit, include the **commit hash**.
- Do not upload large raw datasets into the report folder.
- Do not hide key evidence only in private drives unless your instructor explicitly allows it.

---

## 5. Recommended length

### Main report
- **Recommended length:** 1,800-2,600 words
- **Acceptable range:** 1,500-3,000 words

### What is not counted strictly
The following may be excluded from the word count:

- metadata table,
- summary matrix,
- figure captions,
- benchmark tables,
- references,
- appendix.

### Recommended depth
Each indicator section should usually be about **220-320 words**, plus evidence.

---

## 6. Report logic

The report should answer one core question:

> **How did I develop as an AI-assisted engineering learner through this course, and what evidence shows that growth?**

This means the report should not read like:
- a lecture summary,
- a project advertisement,
- or a team achievement brochure.

Instead, it should read like:
- a personal technical reflection,
- grounded in repository evidence,
- linked to real decisions,
- and honest about limitations.

---

## 7. The six qualitative indicators

This is the recommended six-indicator framework for the report.

| Indicator | What it focuses on | Typical evidence |
|---|---|---|
| 1. Tooling & Reproducible Workflow Readiness | Environment setup, Cursor/Docker/ROS workflow, repo organization, reproducibility | setup commands, screenshots, repo structure, environment files |
| 2. Prompting Strategy & AI Co-Creation | How you learned to prompt, refine prompts, provide context, and collaborate with AI | prompt snippets, before/after prompts, config or code changes |
| 3. Verification, Documentation & Technical Judgment | Cross-checking against theory, notes, docs, trade-offs, rejecting weak AI output | docs links, comparison tables, notes, verification examples |
| 4. Debugging, Iteration & Problem Solving | Diagnosing failures, tuning, step-by-step troubleshooting, improvement cycle | logs, screenshots, commit diffs, before/after metrics |
| 5. Integration & Benchmark-Driven Improvement | Connecting modules, evaluating performance, interpreting metrics, fairness of comparison | pipeline figure, RMSE/IoU table, leaderboard evidence |
| 6. Responsible AI Use, Reflection & Redesign | Hallucination awareness, human oversight, ethics, limitations, redesign priorities | corrected AI output, authenticity statement, redesign plan |

### Rating scale
For each indicator, use a 1-5 self-rating.

| Score | Meaning |
|---|---|
| 1 | Very limited confidence / capability |
| 2 | Basic awareness, but still fragile |
| 3 | Functional in standard cases |
| 4 | Strong and reliable in most cases |
| 5 | Highly confident, reflective, and transferable |

### Before-course rating
You may include an approximate **before-course self-rating** if useful.

Because the pre-class survey was intended as a confidential baseline rather than a graded disclosure, students do **not** need to reproduce their exact original survey answers. A reconstructed estimate is acceptable, and leaving the before-course rating blank is also acceptable unless the instructor later requires it.

---

## 8. Detailed requirements for each indicator

## 8.1 Indicator 1 - Tooling & Reproducible Workflow Readiness

### What this indicator measures
Whether you can use the course toolchain in a stable and reproducible way.

This includes:
- Cursor,
- Docker,
- ROS / ROS bag workflow,
- repo navigation,
- environment setup,
- dependency management,
- and keeping evidence that someone else could follow.

### Must include
- one toolchain task that **you personally completed**,
- one workflow improvement you made,
- one reproducibility practice,
- and one short note on what remained fragile.

### Strong evidence examples
- Docker command or compose snippet,
- environment file,
- setup notes,
- screenshot of successful run,
- repo tree,
- script path,
- issue log,
- commit hash.

### Weak pattern to avoid
- only listing tools without showing how you used them,
- only saying "environment was set up successfully",
- no traceable evidence,
- describing only what the team did.

---

## 8.2 Indicator 2 - Prompting Strategy & AI Co-Creation

### What this indicator measures
Whether you learned how to work with AI actively rather than passively.

This includes:
- giving the AI better context,
- refining prompts,
- using project file references,
- asking for alternatives,
- analyzing why one prompt worked better than another,
- and knowing when prompting is not enough.

### Must include
- one prompt that did **not** work well,
- one revised prompt that improved the output,
- one explanation of what context you added,
- and one reflection on what the AI still could not solve.

### Strong evidence examples
- short prompt snippets,
- before/after prompt pair,
- prompt plus resulting config change,
- prompt plus resulting script change,
- note on using Chat / Composer / Codebase Indexing,
- prompt for ORB-SLAM3 / OpenSplat / U-Net task,
- hyperparameter prompt example.

### Weak pattern to avoid
- "I used Cursor a lot" with no concrete example,
- including only the final good prompt,
- treating prompting like magic,
- not explaining why the revised prompt worked better.

---

## 8.3 Indicator 3 - Verification, Documentation & Technical Judgment

### What this indicator measures
Whether you can verify AI-generated output using engineering reasoning rather than trust it blindly.

This includes:
- checking lecture notes or textbook logic,
- checking official documentation,
- comparing alternative settings,
- understanding coordinate frames / calibration / sensor fusion assumptions,
- recognizing trade-offs,
- and rejecting technically weak suggestions.

### Must include
- one example verified against theory, notes, or official documentation,
- one example of a trade-off,
- one example of a decision you accepted or rejected,
- and one explanation of why that decision was technically justified.

### Strong evidence examples
- ORB-SLAM3 or OpenSplat documentation reference,
- config comparison table,
- note on speed vs accuracy,
- note on visual-only vs visual-inertial trade-off,
- note on UAV viewpoint generalization for segmentation,
- hardware constraint discussion,
- parameter justification.

### Weak pattern to avoid
- reporting the final chosen setting only,
- saying "the AI suggested this so I used it",
- no justification,
- no documentation or theory check.

---

## 8.4 Indicator 4 - Debugging, Iteration & Problem Solving

### What this indicator measures
Whether you can improve a system through structured troubleshooting.

This includes:
- reading logs,
- diagnosing dependency or runtime issues,
- tuning parameters,
- isolating failure causes,
- refining prompts,
- and learning from failed runs.

### Must include
- one concrete failure case,
- a short diagnosis sequence,
- the change you made,
- the result after the change,
- and the lesson learned.

### Strong evidence examples
- ROS compile error log,
- dependency issue,
- drift case in VO,
- image blur / rapid-motion failure analysis,
- reconstruction artifact comparison,
- segmentation failure example,
- before/after screenshot,
- commit pair,
- parameter change list.

### Weak pattern to avoid
- "it failed, then later it worked",
- no causal explanation,
- no evidence of iteration,
- no explanation of why the fix helped.

---

## 8.5 Indicator 5 - Integration & Benchmark-Driven Improvement

### What this indicator measures
Whether you can think beyond one isolated module and evaluate work using evidence.

This includes:
- connecting your work to the larger pipeline,
- understanding how one module affects another,
- using quantitative or structured qualitative evaluation,
- interpreting performance honestly,
- and recognizing the limits of a benchmark.

### Must include
- one system-level connection between your work and another module,
- at least one benchmark table or structured comparison,
- at least one metric or evaluation criterion,
- and one note on what the evaluation does **not** prove.

### Strong evidence examples
- pipeline diagram,
- RMSE / drift table,
- IoU / mIoU table,
- reconstruction artifact comparison,
- leaderboard screenshot or link,
- evaluation script path,
- end-to-end run evidence,
- qualitative comparison with clear criteria.

### Weak pattern to avoid
- only listing numbers with no interpretation,
- discussing modules separately with no integration story,
- claiming improvement without evaluation evidence,
- showing only the best case.

---

## 8.6 Indicator 6 - Responsible AI Use, Reflection & Redesign

### What this indicator measures
Whether you can use AI responsibly and reflect honestly on your engineering growth.

This includes:
- hallucination awareness,
- safety and human oversight,
- academic integrity,
- honest limitation reporting,
- identifying what you can now do better,
- and setting redesign priorities.

### Must include
- one case where AI output was wrong, risky, incomplete, or misleading,
- one honest limitation of your own current work,
- two or three redesign priorities,
- one statement about responsible AI use in coursework.

### Strong evidence examples
- bad AI suggestion plus corrected version,
- authenticity statement,
- AI-use declaration,
- limitation list,
- redesign plan,
- note on safety or deployment readiness,
- note on where human oversight must remain.

### Weak pattern to avoid
- only praising AI,
- writing a generic conclusion,
- hiding failures,
- "need more time" with no specific redesign direction.

---

## 9. Mandatory evidence rules for an individual report

Across the full report, each student **must** include all of the following:

- [ ] **One personal contribution statement**  
      clearly separating `team result` / `my role` / `my evidence`
- [ ] **At least three traceable personal evidence items**  
      such as your commit, script, config, notebook, prompt log, benchmark table, figure, or issue comment
- [ ] **At least one module-specific technical example**  
      from a module you directly worked on  
      (`VSLAM / VO` or `3D reconstruction` or `semantic segmentation`)
- [ ] **At least one integration or system-level example**
- [ ] **At least one benchmark table or structured comparison**
- [ ] **At least one failure case and one corrected case**
- [ ] **At least one prompt example**
- [ ] **At least one documentation / theory cross-check**
- [ ] **One AI-use declaration**
- [ ] **One references section**

### Strongly recommended
- [ ] one screenshot of successful execution,
- [ ] one screenshot of a failure case,
- [ ] one figure showing the pipeline,
- [ ] one note on reproducibility,
- [ ] one note on safety / ethics / academic integrity.

---

## 10. What counts as acceptable personal evidence

Because this is an individual report based on a team project, the following are all acceptable forms of personal evidence:

- your own commit or pull request,
- a config file you edited,
- a script or notebook you ran or modified,
- a benchmark table you created,
- a figure you exported,
- a prompt log or screenshot,
- an issue thread or note authored by you,
- your slide content from the final presentation,
- your own failure analysis note,
- your own reproduction of a team result,
- your own comparison or verification of a team result.

### If the underlying result was team-generated
You must state clearly:

- what the team result was,
- what part you personally handled,
- what evidence proves your role,
- and what you personally learned from it.

---

## 11. What does NOT count as strong evidence

These are weak or unacceptable if used alone:

- a team screenshot with no explanation of your role,
- a metric copied from the team slide deck with no traceable source,
- a general statement such as "I helped with debugging",
- a claim such as "I contributed to integration" with no artifact,
- AI-generated explanation text with no verification,
- polished narrative with no repo evidence.

---

## 12. Recommended report structure

Use the following order.

1. **Title**
2. **Metadata**
3. **Individual Contribution Statement**
4. **Project Snapshot**
5. **Six-Indicator Summary Matrix**
6. **Indicator 1 - Tooling & Reproducible Workflow Readiness**
7. **Indicator 2 - Prompting Strategy & AI Co-Creation**
8. **Indicator 3 - Verification, Documentation & Technical Judgment**
9. **Indicator 4 - Debugging, Iteration & Problem Solving**
10. **Indicator 5 - Integration & Benchmark-Driven Improvement**
11. **Indicator 6 - Responsible AI Use, Reflection & Redesign**
12. **Overall Growth Summary**
13. **GenAI Use Declaration**
14. **References**
15. **Appendix (optional)**

---

## 13. Required metadata block

Use a table near the top.

| Item | Details |
|---|---|
| Course | AAE5303 |
| Report type | Individual Report on Six Qualitative Indicators |
| Student name | |
| Student ID | |
| Team name / group number | |
| Team repo URL | |
| My role in the team | |
| My primary module | VSLAM / 3D reconstruction / segmentation / integration / benchmarking / other |
| Main dataset / scene used | |
| Main tools used | Cursor / Docker / ROS / ORB-SLAM3 / OpenSplat / U-Net / others |
| Main evidence paths | |
| Commit hash(es) / issue / notebook / slide links | |
| Declared AI use | |

---

## 14. Required individual contribution statement

Add this immediately after the metadata.

| Item | Content |
|---|---|
| Team result | [What the team built / evaluated] |
| My specific role | [What I personally handled] |
| My strongest evidence | [commit / script / config / notebook / figure / slide / issue] |
| My main learning focus | [What this report is mainly about] |

---

## 15. Required summary matrix

Put this before the full sections.

| Indicator | Before-course (optional) | End-of-course | Main evidence | Main lesson |
|---|---:|---:|---|---|
| 1. Tooling & Reproducible Workflow Readiness |  |  |  |  |
| 2. Prompting Strategy & AI Co-Creation |  |  |  |  |
| 3. Verification, Documentation & Technical Judgment |  |  |  |  |
| 4. Debugging, Iteration & Problem Solving |  |  |  |  |
| 5. Integration & Benchmark-Driven Improvement |  |  |  |  |
| 6. Responsible AI Use, Reflection & Redesign |  |  |  |  |

---

## 16. Writing pattern for each indicator section

Each indicator section should follow the same mini-structure.

### A. Self-rating
- Before-course confidence *(optional)*: `__/5`
- End-of-course confidence: `__/5`

### B. Situation / task
What task, scenario, or problem is this section about?

### C. What I did
Describe your own action in first person.

### D. Evidence
Provide traceable evidence:
- repo path,
- commit hash,
- figure,
- log,
- prompt snippet,
- metric table,
- notebook,
- or documentation reference.

### E. What this shows
Interpret the evidence. Explain what it demonstrates about your capability or judgment.

### F. Limitation
What is still weak, fragile, incomplete, or uncertain?

### G. Next improvement
State one concrete next step.

---

## 17. Coverage expectations across the course modules

The course project integrates multiple modules. However, because this is an **individual** report, students are not required to claim deep implementation ownership over all modules.

### Required balance
Your report should include:

1. **one technically detailed example** from the module you directly worked on,  
2. **one system-level integration or evaluation example**, and  
3. **some awareness of the larger pipeline** beyond your own narrow task.

### Good examples
- If your main work was VSLAM, you can still discuss how pose quality affected reconstruction or segmentation.
- If your main work was Gaussian Splatting, you can still discuss how upstream pose noise influenced artifacts.
- If your main work was segmentation, you can still discuss how semantic output relates to the geometry pipeline.
- If your main work was benchmarking or integration, you can discuss how you compared outputs from multiple modules.

---

## 18. GitHub writing style guidance

### Good GitHub style
- concise headings,
- explicit evidence links,
- readable tables,
- short paragraphs,
- figures with captions,
- relative paths,
- minimal but meaningful screenshots.

### Avoid
- giant walls of text,
- pasted raw code blocks longer than necessary,
- screenshots of tables that could be written as Markdown tables,
- unexplained figures,
- unlabeled metrics,
- vague language like "many improvements were made."

---

## 19. Academic integrity and authentic evidence rules

This report should make fabrication difficult.

### Therefore
- Every major claim should be traceable.
- If a run failed, say it failed.
- If a number is approximate, label it.
- If a result is team-generated, label it clearly.
- If AI generated part of the code or text, disclose it honestly.
- Do not present AI-generated guesses as verified engineering facts.
- Do not present team-level output as your personal work without attribution.
- Do not claim reproducibility if the repo cannot actually reproduce the result.

### Recommended authenticity statement
> **Authenticity statement:** All claims in this report are based on work that can be traced to repository artifacts, experiment records, project materials, or clearly labeled team outputs. I have not fabricated or misrepresented results.

---

## 20. Recommended GenAI declaration

Include a block like this:

> **GenAI Use Declaration**  
> During this course, I used the following AI tools: `[tool names]`.  
> They were used for `[environment setup / debugging / prompt-based code assistance / language polishing / translation / none]`.  
> All AI-assisted outputs included in this report were checked by me and verified against project requirements, documentation, or experimental evidence before being included.

---

## 21. Optional grading rubric

> Use this only if the report will be graded.  
> If the report is mainly for reflection or pedagogy documentation, this section may be removed.

| Area | Weight |
|---|---:|
| Indicator 1 - Tooling & Reproducible Workflow Readiness | 10 |
| Indicator 2 - Prompting Strategy & AI Co-Creation | 10 |
| Indicator 3 - Verification, Documentation & Technical Judgment | 15 |
| Indicator 4 - Debugging, Iteration & Problem Solving | 15 |
| Indicator 5 - Integration & Benchmark-Driven Improvement | 20 |
| Indicator 6 - Responsible AI Use, Reflection & Redesign | 15 |
| Personal traceability of contribution | 10 |
| Writing clarity, references, and GitHub organization | 5 |
| **Total** | **100** |

### What earns high marks
- clear separation of team result vs personal contribution,
- honest and specific evidence,
- thoughtful interpretation of metrics,
- strong failure analysis,
- theory / documentation cross-checking,
- meaningful reflection,
- responsible discussion of AI use.

---

## 22. Common weak patterns to avoid

Do **not** do the following:

- write only a success story,
- summarize lecture slides without linking to your own work,
- describe the team project without explaining your personal role,
- present figures without interpretation,
- list metrics without explaining what they mean,
- say "AI helped a lot" without a concrete case,
- hide failures,
- write generic conclusions such as "need more time",
- or make claims that cannot be traced to evidence.

---

## 23. Recommended folder and filename conventions

### If collecting all student reports in one course repo
```text
reports/
├── 23012345_chan_tai_man/
│   ├── README.md
│   └── assets/
├── 23012346_lee_siu_ming/
│   ├── README.md
│   └── assets/
└── ...
```

### Recommended filename examples
- `README.md`
- `23012345_six_indicators_report.md`

---

## 24. Ready-to-copy instructor note

You can place this guide directly in the course repository.

### Suggested location
```text
course-repo/
└── docs/
    ├── AAE5303_Individual_Six_Indicators_Report_Guidelines.md
    └── AAE5303_Individual_Six_Indicators_Report_Template.md
```

### Instructor fields to finalize before release
- Due date:
- Submission repo location:
- Whether before-course self-rating is optional or required:
- Whether the rubric is official:
- Citation style:
- Whether appendices are allowed:
- Whether assets must remain inside the repo:
