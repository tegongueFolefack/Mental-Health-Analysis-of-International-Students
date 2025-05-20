# 🧠 Mental Health Analysis of International Students

## 📊 Project Objective

This project explores and analyzes mental health diagnostic scores among international students at a Japanese university to determine how **length of stay (stay)** influences mental health outcomes.

The data comes from a 2018 survey and includes tests measuring depression, social connectedness, and acculturative stress. The goal is to assess whether staying longer in a new country impacts these factors.

---

## 🔍 Research Question

**Does the length of stay in a foreign country affect the mental health of international students?**

We focus on three mental health indicators:
- **PHQ-9 test (todep)** → Measures depressive symptoms
- **SCS test (tosc)** → Measures social connectedness
- **ASISS test (toas)** → Measures acculturative stress

---

## 🧬 Dataset Description

The dataset contains anonymized survey responses with the following relevant columns:

| Column Name | Description |
|-------------|-------------|
| `stay`      | Number of years the student has stayed in the country |
| `int`       | International student status (1 = international, 0 = local) |
| `todep`     | PHQ-9 depression score |
| `tosc`      | SCS (social connectedness score) |
| `toas`      | ASISS (acculturative stress score) |

---

## 🛠️ Tools & Technologies

- **PostgreSQL** for querying and analyzing the data
- **Pandas** for final DataFrame manipulation and formatting
- **Jupyter Notebook** for writing and documenting the workflow

---

## 🧾 Methodology

Using SQL, we extracted a summary table for all international students, grouped by length of stay:

- Count of international students (`count_int`)
- Average PHQ-9 depression score (`average_phq`)
- Average SCS score (`average_scs`)
- Average ASISS score (`average_as`)

All averages are **rounded to two decimal places**, and the results are **sorted by length of stay in descending order**.

Example of the expected output format:

| stay | count_int | average_phq | average_scs | average_as |
|------|-----------|-------------|-------------|------------|
| 5    | 12        | 9.25        | 3.88        | 4.12       |
| ...  | ...       | ...         | ...         | ...        |

---

## 📈 Key Insights

- **Longer stays** may correlate with improved mental health in some areas (e.g., higher social connectedness).
- **Acculturative stress** tends to be higher in students with shorter stays.
- **Depression scores** vary and may relate to both personal and environmental factors beyond duration alone.

---

## 📦 Repository Structure

