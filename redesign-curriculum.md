# Task 2: Curriculum Audit and Redesign
**Programme:** B.Tech in Computer Science & Engineering (Section 4.7.6)
**Institution / source:** IFHE (ICFAI Foundation for Higher Education), Student Handbook 2023-24, p. 30
**Branch:** CSE | **Admission batch:** 2023 (assumed from handbook year) | **Curriculum version:** Handbook 2023-24
**Audit date:** 23 Oct 2026

> **Source note.** The only official document available was the handbook page (course codes, L-T-P-C, semester totals). Full course syllabi and the IFHE academic regulations were not available to me, so course content is inferred from titles. Regulatory checks use the AICTE model curriculum (160-credit framework under NEP 2020) as the benchmark. Confirm batch and regulations with the department before submitting.

---

## 1. Current map: courses and credits by semester

Credit rule used to check each row: **C = L + T + P/2**.

| Sem | Courses (credits) | Handbook total | Recomputed |
|---|---|---|---|
| I | MA101 Lin. Algebra & ODE (3), EG101 English (3), MT101 Digital Fabrication (3), PH101 Physics (5), CH101 Chemistry (4), CS101 Computer Programming (4), HS101 Indian Traditional Knowledge (0, audit) | 22 | 22 |
| II | MA102 Higher Calculus (3), EG102 Prof. Communication (3), EC101 Basic Electronics (4), DS101 Intro to DS & AI (3), CH102 Environmental Sciences (2), CS102 Data Structures (4), MT102 Engineering Graphics (3) | 22 | 22 |
| III | EC201 Intro to IoT (3), CS201 OOP (4), MA201 Integral Transforms & Prob/Stats (3), CS202 Theory of Computation (3), CS203 DAA (3), MG201 Engg. Economics & Mgmt (3), MA202 Discrete Maths (3), CR201 Power Skills I (1) | 23 | 23 |
| IV | EC102 Signal Processing (3), CS204 Computer Org. & Arch. (3), HSXXX Digital Humanities Elective (3), CS205 Web Technologies (Web 3.0) (4), DS202 Industry Coding Practice Python/R (3), DS203 Data Science (3), CS206 DBMS (4), CR202 Power Skills II (1) | 23 | **24** |
| Summer | IP201 Internship Program I | 3 | 3 |
| V | CS301 Cryptography (3), CS302 OS (4), CS303 Compiler Construction (3), DS304 Machine Learning (4), CS304 Software Engineering (3), CSXXX Elective (3), CR301 Power Skills III (1) | 21 | 21 |
| VI | CS305 Computer Vision (3), CS306 Computer Networks (4), DS307 Big Data Systems (3), CS307 Cloud Computing (4), CSXXX Elective (3), SP301 Special Project (3), CR302 Power Skills IV (1) | 21 | 21 |
| VII | IP401 Internship/Research **or** TS401 Thesis & Seminar + 2 Electives + 2 Prof./Discipline + 1 DH Elective | 15 | 15 |
| VIII | Same structure as VII | 15 | 15 |
| **Total** | | **163** | **166** (or 162 if summing stated semester totals and excluding IP201) |

### Audit findings in the official document
1. **Semester IV does not add up.** The eight courses sum to 24 credits, not the stated 23. Every L-T-P row is internally consistent, so the error is in the total.
2. **Programme total cannot be reproduced.** Stated semester totals give 162; adding IP201 gives 165; using the recomputed Sem IV gives 166. None equals the stated 163.
3. **Sem VII/VIII structure is ambiguous.** The table implies IP401 and TS401 + electives are alternatives worth 15 each, but does not say whether a student does internship in one semester and coursework in the other.
4. **Code inconsistency.** EC102 (a 100-level code) sits in Semester IV.
5. **"Web 3.0" title** suggests a blockchain/decentralised-web focus that none of the three job descriptions below asks for.

These are worth raising with the department regardless of the redesign.

---

## 2. Benchmark: three real, dated job descriptions

| # | Role | Employer / location | Date | Key asks |
|---|---|---|---|---|
| JD1 | Software Engineer (Universal Print), Job ID 200047364 | Microsoft, Hyderabad (hybrid) | Posted 14 Aug 2026 | CS degree; coding in C/C++/C#/Java/JS/Python; preferred: REST APIs, Git workflows, unit testing and software quality |
| JD2 | Systems Software Engineer, AI and Cloud, New College Grad 2026 (JR2025458) | NVIDIA, Santa Clara | Applications open until at least 10 Oct 2026 | Python and JavaScript; DS&A and software design; basic C++; cloud-native systems on Kubernetes; LLM inference (vLLM, Triton); API design |
| JD3 | Software Engineer, Graduates 2026 | Zycus, Mumbai | Listed on Glassdoor, Oct 2026 | B.Tech 2026 grads; use AI tools for coding, debugging, testing, docs; AI-assisted workflows; cloud, Docker, Kubernetes a plus |
| Ref. | Cloud AI Engineer (experienced, stretch reference) | Google, Bengaluru/Hyderabad/Gurugram/Pune | Oct 2026 | GenAI apps, agents, RAG; security, governance and compliance |

**Pattern across all three:** the fundamentals this curriculum already teaches well (DS&A, OS, networks, DBMS, programming) are still the baseline. The gaps are in **engineering practice** (testing, Git, APIs, containers) and **applied AI** (using AI tools responsibly, building with LLMs).

---

## 3. Proposed changes: KEEP / UPDATE / REDUCE / ADD

### KEEP (unchanged)
MA101, MA102, MA201, MA202, EG101, EG102, CS101, CS102, CS201, CS202, CS203, CS204, CS206, CS302, CS303, CS306, DS101, DS203, DS307, EC101, EC201, MG201, CH102 (mandatory EVS), HS101, HSXXX, Power Skills I-IV, IP201, IP401/TS401, SP301, electives.
Rationale: DS&A, OS, networks, DBMS and programming are named or implied in all three JDs.

### UPDATE (same credits, new content): 18 credits
| Course | Cr | Change | JD link |
|---|---|---|---|
| CS304 Software Engineering | 3 | Re-structure 3-0-0 to 2-0-2. Add Git workflows, unit testing, CI/CD, code review, AI-assisted development policy | JD1, JD3 |
| CS307 Cloud Computing | 4 | Make Docker and Kubernetes the lab core; add serverless and cost basics | JD2, JD3 |
| DS304 Machine Learning | 4 | Add a final unit on transformer/LLM fundamentals and model evaluation | JD2, Ref. |
| CS205 Web Technologies (Web 3.0) | 4 | Retitle "Web & API Engineering": JavaScript, REST API design, auth; blockchain becomes one week, not the theme | JD1, JD2 |
| DS202 Industry Coding Practice | 3 | Python-first with Git, testing and packaging; R moves to DS203 | JD1, JD2, JD3 |

### REDUCE: 15 credits touched, 6 credits freed
| Course | From | To | Note |
|---|---|---|---|
| PH101 Physics | 5 (3-1-2) | 4 (3-0-2) | Drop tutorial hour; keep lab |
| CH101 Chemistry | 4 (3-0-2) | 3 (3-0-0) | Drop lab for CSE branch |
| MT102 Engineering Graphics | 3 (2-0-2) | 2 (1-0-2) | Keep CAD lab, trim lecture |
| EC102 Signal Processing | 3 | 0 core (moves to elective pool) | Also fixes the Sem IV overload |

### ADD: 6 credits
| New course | Sem | L-T-P-C | JD link |
|---|---|---|---|
| Responsible AI & Technology Ethics | IV | 2-0-0-2 | Ref. (governance, compliance), JD3 |
| **AI-Assisted Engineering Lab** (Task 1 workflow, see §6) | V | 0-0-4-2 | JD3, JD1 (testing), JD2 |
| LLM Applications & Evaluation | VI | 1-0-2-2 | JD2, Ref., JD3 |

### Credit impact
| Category | Credits touched |
|---|---|
| UPDATE | 18 |
| REDUCE | 15 |
| ADD | 6 |
| **Total touched** | **39 of 163 = 23.9%** (target 20-25%) |

**Balance:** −6 reduced, +6 added. Programme total unchanged.

| Sem | Old | New |
|---|---|---|
| I | 22 | 20 |
| II | 22 | 21 |
| III | 23 | 23 |
| IV | 24 (stated 23) | 23 |
| V | 21 | 23 |
| VI | 21 | 23 |
| VII / VIII | 15 / 15 | 15 / 15 |

Load moves from first year (heavy on general science) to the third year, where students have the prerequisites to use it. Sem IV goes from an actual 24 to 23, so the published number becomes correct.

---

## 4. Ten reasons for the changes
1. **All three JDs ask for engineering practice the curriculum does not name.** Git, unit testing and REST APIs (JD1) appear nowhere in course titles.
2. **AI-assisted coding is now a stated job requirement, not a bonus.** JD3 lists using AI for coding, debugging, testing and docs as a core duty. No course teaches doing this well or safely.
3. **Containers are the default deployment target.** Kubernetes appears in JD2 and JD3; CS307 should teach it hands-on, not survey it.
4. **LLMs appear in the NVIDIA and Google roles.** DS304 ends at classical ML; one unit plus a Sem VI lab closes the gap without displacing fundamentals.
5. **"Web 3.0" mismatches demand.** None of the JDs mentions blockchain; all of them involve APIs.
6. **First-year science is heavier than the AICTE comparator.** A comparable AICTE/NEP CSE structure allots about 20 basic-science credits; this programme has about 23 (maths, physics, chemistry and EVS). Trimming 2 brings it to about 21, still above that comparator.
7. **Signal processing is a narrow need.** Only CS305 Computer Vision depends on it; MA201 already covers integral transforms.
8. **The handbook has arithmetic errors.** Rebalancing Sem IV fixes a real inconsistency, not just a preference.
9. **Responsible AI is under-served.** Students will use AI tools from Sem V onward; ethics, data privacy and attribution should come before that, not after.
10. **The changes reuse existing capacity.** Every UPDATE keeps its credits and slot, so timetabling and faculty load change little.

---

## 5. Prerequisites and regulatory notes
| Change | Prerequisite / regulatory check |
|---|---|
| EC102 to elective | CS305 Computer Vision needs convolution and filtering. Add a 2-week signals module to CS305; MA201 already supplies Fourier/Laplace. |
| CH101 lab removed | CH102 Environmental Sciences (AICTE mandatory) is untouched. Check that IFHE's basic-science minimum is still met (~21 BS credits after change). |
| PH101 tutorial removed | Lab kept, so experimental component remains. |
| AI-Assisted Engineering Lab (Sem V) | Requires CS201 OOP, CS203 DAA, DS202. Must follow Responsible AI (Sem IV). |
| LLM Applications (Sem VI) | Requires DS304 ML (Sem V) and CS307 Cloud running in parallel. |
| Total credits | Stays at 163, above the AICTE 160 minimum. |
| Approval path | As a deemed university, IFHE changes go through the Board of Studies and Academic Council. Apply to a new batch, not mid-programme, to protect students' credit requirements. |

---

## 6. Task 1 workflow as a lab: AI-Assisted Engineering Lab (Sem V, 0-0-4, 2 credits)

> I don't have your Task 1 deliverable. The structure below assumes Task 1 produced a repeatable AI-assisted workflow (prompt, generate, verify, log). Swap in your exact steps.

**Weekly loop (12 weeks):**
1. **Spec.** Student writes the problem and acceptance tests *before* prompting.
2. **Prompt and log.** Record model, date, prompt and raw output (same template as §7).
3. **Verify.** Run tests, compare against a reference or brute-force solution, check edge cases.
4. **Critique.** Note what the AI got wrong or omitted (see Ex5: correct RSA math, no warning about missing padding).
5. **Commit.** Push to Git with the log in the PR; peer code review.

**Assessment:** 40% verification quality, 30% logged critique, 20% final mini-project, 10% peer review. Grading rewards catching AI errors, not just working code.
**Capstone path:** strong students carry the workflow into SP301 Special Project (Sem VI) with no extra credits.

---

## 7. AI-assisted exercise log (five subjects)

**Model:** Claude Opus 5.5 (`claude-opus-5-5`) | **Date:** 23 Oct 2026 | **Verification:** independent Python scripts run in a sandbox the same day.

| # | Subject | Prompt (summarised) | AI output | How I verified it | Result |
|---|---|---|---|---|---|
| 1 | MA101 Linear Algebra & ODE | "Solve y'' + 3y' + 2y = 0 with y(0)=1, y'(0)=0." | y(t) = 2e^(−t) − e^(−2t) | Numerical RK4 integration (h = 0.001) to t = 3, compared with closed form | Match: 0.0970953846 both; error 9.3e-16 |
| 2 | CS102 Data Structures | "Write an O(1) LRU cache in Python with get/put." | OrderedDict class using move_to_end and popitem | Randomised differential test against a slow list-based reference: 200 caches, 20,000 operations, capacities 1-5 | 0 mismatches |
| 3 | CS203 DAA | "Write a DP for edit distance and state its complexity." | Standard O(mn) table DP | Compared with exhaustive recursion on 500 random short strings; checked kitten/sitting | 0 mismatches; kitten/sitting = 3 (known answer) |
| 4 | CS206 DBMS | "SQL for the second-highest distinct salary in each department." | Two versions: correlated subquery and DENSE_RANK window | Ran both in SQLite on a hand-built table with ties and a 1-employee department; compared with hand-computed answer | Both correct: A→90, C→60, B correctly absent (tie at 90 handled) |
| 5 | CS301 Cryptography | "Toy RSA with p=61, q=53, e=17: give n, d and encrypt 65." | n = 3233, d = 2753, c = 2790 | Recomputed d as modular inverse of e mod φ; round-tripped every m < n | All 3,233 messages round-trip. **Gap:** output did not warn that textbook RSA without padding is insecure |

**Takeaway:** all five outputs were mathematically correct, but Ex5 shows why the lab grades critique: a correct answer can still teach a bad habit. Verification methods (numerical check, differential testing, brute-force oracle, hand-built test data, exhaustive round-trip) are themselves the skill the lab should teach.

---

## 8. Faculty / graduate feedback
I could not obtain feedback for this draft: I have no contact with IFHE faculty or alumni, and there was no time to arrange a voluntary review before submission. To close this, send these three questions to one CSE faculty member and one recent graduate:
1. Does the Sem IV / total-credit discrepancy match the current regulations, or was it corrected after 2023-24?
2. Would trimming the Chemistry lab and moving Signal Processing to an elective conflict with any IFHE basic-science or engineering-science minimum?
3. Which tool or skill did you most need in your first job or internship that the curriculum did not teach?

---

## 9. Interactive credit calculator
Attached as **`curriculum_calculator.html`** (open in any browser). It lists every course with old vs. proposed credits, filters by semester and by KEEP / UPDATE / REDUCE / ADD, lets you toggle each proposed change on or off, and recalculates semester totals, programme total and the % of credits touched live.

---

## Sources
- IFHE Student Handbook 2023-24, §4.7.6 B.Tech CSE, p. 30 (provided PDF)
- AICTE/NEP 160-credit comparator structure: [DRIEMS University B.Tech CSE Structure 2024-25](https://www.driems.ac.in/wp-content/uploads/2024/04/1.-B.TECH_CSE-Structure_2024-25.pdf)
- JD1: [Microsoft Software Engineer 2026, Hyderabad (via FreshersHunt)](https://freshershunt.in/microsoft-software-engineer-2026-aug/)
- JD2: [NVIDIA Systems Software Engineer, AI and Cloud, NCG 2026](https://nvidia.wd5.myworkdayjobs.com/en-US/NVIDIAExternalCareerSite/job/Systems-Software-Engineer---AI-and-Cloud---New-College-Grad-2026_JR2025458)
- JD3: [Zycus Software Engineer, Graduates 2026 (Glassdoor listing)](https://www.glassdoor.co.in/Job/india-new-grad-software-engineer-jobs-SRCH_IL.0,5_IN115_KO6,32.htm)
- Ref.: [Google Cloud AI Engineer, India 2026 (Jobscoupe)](https://www.jobscoupe.com/google-recruitment-2026-cloud-ai-engineer-jobs-india/)
