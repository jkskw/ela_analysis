# Project: Analysis of Factors Influencing Graduates' Salaries and Employment

## Table of Contents
- [Research Questions](#research-questions)
- [Model](#model)
- [Charts](#charts)
  - [Jupyter_1. Salaries and Unemployment by Region](#1-salaries-and-unemployment-by-region)
  - [Jupyter_2. Work Experience and its Impact on Employment and Salaries](#2-work-experience-and-its-impact-on-employment-and-salaries)
  - [Jupyter_3. Histogram: Number of Students vs Salaries (done in different notebook)](#3-histogram-number-of-students-vs-salaries-done-in-different-notebook)
  - [Jupyter_4. Education Level vs Salaries](#4-education-level-vs-salaries)
  - [Jupyter_5. Study Mode vs Salaries](#5-study-mode-vs-salaries)
- [Additional Charts](#additional-charts)
  - [1. Changes in Salaries and Unemployment over Time (up to 5 years after graduation)](#1-changes-in-salaries-and-unemployment-over-time-up-to-5-years-after-graduation)
- [Poster](#poster)

---

## Research Questions
1. **Impact of university location** on graduates' salaries and employment — regional differences and university prestige matter for career outcomes?
2. **Work experience during studies** — how does it affect salaries and time to find the first job?
3. **Potential earnings vs. choice of field of study** — do expected salaries influence students' decisions when choosing their major?
4. **Level of education (Bachelor’s, Master’s, or long-cycle Master's programs)** — does it affect future salaries?
5. **Study mode (full-time vs part-time studies)** — does it impact future salaries?

---

## Model
A predictive model will be developed to forecast future salaries of graduates based on their chosen field of study. Created and finetuned in **models/** directory.

---

## Charts

### 1. Salaries and Unemployment by Region
- **f(P_WOJ) = (P_ME_ZAR or P_WWZ) and P_WWB**

**Definitions:**
- `P_WOJ` — Region (province) of the educational institution
- `P_ME_ZAR` — Median of graduates' monthly salaries from all sources after graduation
- `P_WWZ` — Relative Salary Index of graduates after graduation
- `P_WWB` — Relative Unemployment Index of graduates after graduation

---

### 2. Work Experience and its Impact on Employment and Salaries
- **f() = ?**

**Definitions:**
- `P_WWB_DOSW` — Unemployment rate among graduates with prior work experience
- `P_WWB_NDOSW` — Unemployment rate among graduates without prior work experience
- `P_CZAS_PRACA_DOSW` — Average time (in months) to first job for graduates with prior work experience
- `P_CZAS_PRACA_NDOSW` — Average time (in months) to first job for graduates without prior work experience
- `P_ME_ZAR_DOSW` — Median monthly salary for graduates with prior work experience
- `P_ME_ZAR_NDOSW` — Median monthly salary for graduates without prior work experience

#### Additionally:
- **f(Years 1–5) = (P_WWZ_DOSW_PX and P_WWZ_NDOSW_PX) and (P_ME_ZAR_DOSW_PX and P_ME_ZAR_NDOSW_PX)**

**Definitions:**
- `P_ME_ZAR_DOSW_PX` — Median monthly salary in year X after graduation for graduates with prior work experience
- `P_ME_ZAR_NDOSW_PX` — Median monthly salary in year X after graduation for graduates without prior work experience

---

### 3. Histogram: Number of Students vs Salaries (done in different notebook)
- **f(P_N) = P_ME_ZAR**

**Definitions:**
- `P_N` — Number of students (from `students-major-data.csv`)
- `P_ME_ZAR` — Median monthly salary of graduates after graduation

---

### 4. Education Level vs Salaries
- **f(P_POZIOM) = (P_ME_ZAR or P_WWZ)**

**Definitions:**
- `P_POZIOM` — Level of education completed
- `P_WWZ` — Relative Salary Index
- `P_ME_ZAR` — Median monthly salary

---

### 5. Study Mode vs Salaries
- **f(P_FORMA) = (P_ME_ZAR or P_WWZ)**

**Definitions:**
- `P_FORMA` — Study mode (full-time or part-time)
- `P_WWZ` — Relative Salary Index
- `P_ME_ZAR` — Median monthly salary

---

## Additional Charts

### 1. Changes in Salaries and Unemployment over Time (up to 5 years after graduation)
- **f(Months X 1–60) = P_WWZ_MIES_X and P_WWB_MIES_X**

**Definitions:**
- `P_WWZ_MIES_X` — Relative Salary Index in the Xth month after graduation
- `P_WWB_MIES_X` — Relative Unemployment Index in the Xth month after graduation

---

## Poster
![obraz](https://github.com/user-attachments/assets/6013133f-9303-4035-bac4-c496ffb32119)
