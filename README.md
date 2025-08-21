# NYC Public Schools SAT Performance — Exploratory Data Analysis

Every year, American high school students take the SATs, standardized tests with three sections (Reading, Math, Writing), each worth up to **800 points**. These scores are critical for college admissions and provide valuable insights into education quality.

This project explores SAT performance data for New York City (NYC) public schools, focusing on identifying top schools and borough-level trends.

---

## Dataset

* **File:** `schools.csv`
* **Columns:**

  * `school_name`: Name of the school
  * `borough`: NYC borough where the school is located
  * `average_math`: Average math score
  * `average_reading`: Average reading score
  * `average_writing`: Average writing score

---

## Objectives

We addressed three main questions:

1. **Which NYC schools have the best math results?**

   * Defined as schools where the average math score is **≥ 640 (80% of the max score)**.
   * Results sorted in descending order of average math.

2. **What are the top 10 performing schools based on combined SAT scores?**

   * Total SAT score = `average_math + average_reading + average_writing`.
   * Identified the top 10 schools with the highest totals.

3. **Which borough has the largest variation (standard deviation) in SAT scores?**

   * Grouped by borough and calculated:

     * `num_schools`: Number of schools
     * `average_SAT`: Mean combined SAT score
     * `std_SAT`: Standard deviation of combined SAT score
   * Found the borough with the largest `std_SAT`.

---

## Tools & Libraries Used

* **Python 3**
* **pandas** → for cleaning, grouping, and aggregation
* **numpy** → for calculations and handling missing data

---

## Insights & Learnings

* Identified high-performing schools in math (≥ 640 average score).
* Ranked the **Top 10 schools** across NYC based on total SAT performance.
* Determined which **borough** has the widest spread in SAT scores, highlighting differences in school performance within that borough.

---

## Possible Extensions

* Visualize the distribution of SAT scores across boroughs.
* Compare performance between public and charter schools (if data available).
* Analyze correlations between borough demographics and SAT performance.

---

## Acknowledgments

* Exercise inspired by **DataCamp**.
* NYC SAT dataset provided with the exercise prompt.
