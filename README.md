# ANSUR II Anthropometric Data vs. Human Body Proportions

## Project Overview

This project will analyze if the commonly known human body proportion ratios are supported by real-world anthropometric measurements. I will be using both the **ANSUR II Male Public Dataset** and the **ANSUR II Female Public Dataset**, these are well known in academic setting and assignments. I will be examining proportional relationships between selected body dimensions and calculating their ratios, both separated by gender and combined datasets.

---
## Dataset Description: ANSUR II

ANSUR II (Anthropometric Survey of U.S. Army Personnel) is based on the results of an extensive anthropometric (body measurement) study conducted by the U.S. Army in 2012.

The **ANSUR II Public Dataset** includes:
* Body measurements such as the head, hand, foot, leg, arm, chest, etc. and ethnicity information of army personnel.
* 93 directly measured anthropometric measurements.
* Male dataset consists of 4,082 samples.
* Female dataset consists of 1,986 samples.
* Together that makes it 6,068 samples in total.
* Standardized physical body measurements (lengths, breadths, circumferences),
* Measurements recorded primarily in **millimeters**.

This makes the dataset well-suited for quantitative analysis of body proportions and dimensional relationships.

---

## Research Questions

Here I will discuss the proportion ratios that the project will focus on.

1. **Arm Span to Stature**: A commonly known body ratio is that arm span is approximately equal to standing height (1:1).

2. **Foot Length to Forearm Length**: Another claim suggests that foot length and forearm length are approximately proportional (1:1).

For each ratio, we ask:

* How close is the calculated average ratio to the commonly cited reference values?
* How much variability exists?
* Does gender play a significant role in variability of the ratios?

---

## Required Measurements and Column Selection

The dataset itself has 93 anthropometric columns, we only select a small subset of columns needed for the analysis. This helps maintain the focus of the project, its readability, and display of information.

### Selected Columns

* `subjectid`
* `stature`
* `span`
* `footlength`
* `forearmhandlength`
* `handlength`

All selected measurements are recorded in millimeters, so ratios are unitless and require no unit conversion.

---

## Measurement Definitions (ANSUR II)

The following definitions are based on official ANSUR II measurement protocols.

* **Arm Span (`span`)**:  The distance between the tips of the middle fingers of horizontally
outstretched arms. 
* **Stature (`stature`)**: The vertical distance from a standing surface to the top of the
head.
* **Foot Length (`footlength`)**: The maximum length of the right foot.
* **Forearm-Hand Length (`forearmhandlength`)**: The horizontal distance between the back of the tip of the right
elbow to the tip of the right middle finger.
* **Hand Length (`handlegth`)**: The length of the right hand between the stylion landmark on the
wrist and the tip of the middle finger.

---

## Project Structure (Jupyter Notebook)

The notebook will be organized as follows:

1. **Data Loading and Initial Inspection**
   * **Column Selection**
2. **Dataset Description**
3. **Ratio 1: Arm Span vs Stature**
   * **Calculating Proportion Ratios**
   * **Statistical Summary**
   * **Visualization of Ratios**
   * **Interpretation and Conclusions**
4. **Ratio 2: Foot Length vs Forearm**
   * **Calculating Proportion Ratios**
   * **Statistical Summary**
   * **Visualization of Ratios**
   * **Interpretation and Conclusions**

Each section includes concise explanations alongside executable code cells.

---