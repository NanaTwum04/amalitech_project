

### A. The Executive Summary
* The analysis revealed that the snack market is heavily saturated with high-sugar, low-protein products, while the high-protein, low-sugar segment remains underserved. The biggest opportunity lies in savory and dairy-based snacks delivering 10–20g of protein with less than 5g of sugar per serving. This represents a clear “Blue Ocean” innovation space for a differentiated healthy snacking product line.

### B. Project Links
* **Link to Notebook:** (e.g., Google Colab, etc.). *Ensure sharing permissions are set to "Anyone with the link can view".*
* **Link to Dashboard:** https://snacksdashboard.streamlit.app/
* **Link to Presentation:** [powerpoint](https://1drv.ms/p/c/a4cc64dd6538731e/IQDKHI2oRDbUQ7mBa74ef_-JAWhjHkED2e-MjNmOKBdeGeU?e=D3xssa)

### C. Technical Explanation

## Data Cleaning Approach

To ensure the analysis was based on reliable and biologically plausible data, a structured data cleaning process was applied.

### Filtering Relevant Products  
The dataset was first filtered to include only snack-related products using the `categories_tags` column. This ensured the analysis focused strictly on the snack aisle and aligned with the client’s business objective.

### Handling Missing Text Fields  
Missing values in descriptive fields such as `product_name`, `countries_en`, and `nutriscore_grade` were filled with `"Unknown"` instead of dropping rows. This preserved valuable product records while maintaining consistency for categorical analysis and visualization.

### Removing Biologically Implausible Nutritional Values (Outlier Filtering)  
Domain-specific thresholds were applied to remove invalid or unrealistic nutritional entries caused by data entry errors:

- Energy capped at ≤ 900 kcal/100g and ≤ 4000 kJ/100g  
- Fat, carbohydrates, sugars, and proteins capped at ≤ 100 g/100g  
- Fiber capped at ≤ 40 g/100g  
- Saturated fat constrained to be ≤ total fat  
- Salt capped at ≤ 100 g/100g  
- Fruits/vegetables/nuts estimates capped at ≤ 100%  
- Nutrition score constrained between -15 and 40  

Rows violating these constraints were removed and the dataset index was reset. This produced a clean, biologically plausible dataset suitable for strategic nutritional analysis.

---

## Candidate’s Choice Addition

### Product Type Classification and Commercial Opportunity Analysis  

To extend the analysis beyond the brief, I introduced a **product-type classification framework** that segmented snacks into three strategic groups:

- **Blue Ocean:** High protein and low sugar products  
- **Regular:** Products without strong health positioning  
- **Unhealthy:** Low protein and high sugar products  

This framework allowed clear identification of underserved product spaces aligned with the client’s innovation goals.

### Business Justification  
While the nutrient matrix identified gaps, decision-makers also need insight into **commercial potential**. Therefore, I simulated a price-per-100g metric and compared pricing distributions across product types. This demonstrated that Blue Ocean products have premium pricing potential, translating the nutritional gap into a tangible business opportunity for R&D and product strategy teams.


**Important Note on Code Submission:**
* Upload your `.ipynb` notebook file to the repo.
* **Crucial:** Also upload an **HTML or PDF export** of your notebook so we can see your charts even if GitHub fails to render the notebook code.
* Once you are ready, please fill out the [Official Submission Form Here](https://forms.office.com/e/heitZ9PP7y) with your links

---

## 🛑 CRITICAL: Pre-Submission Checklist

**Before you submit your form, you MUST complete this checklist.**

> ⚠️ **WARNING:** If you miss any of these items, your submission will be flagged as "Incomplete" and you will **NOT** be invited to an interview. 
>
> **We do not accept "permission error" excuses. Test your links in Incognito Mode.**

### 1. Repository & Code Checks
- [✅] **My GitHub Repo is Public.** (Open the link in a Private/Incognito window to verify).
- [✅] **I have uploaded the `.ipynb` notebook file.**
- [✅] **I have ALSO uploaded an HTML or PDF export** of the notebook.
- [✅] **I have NOT uploaded the massive raw dataset.** (Use `.gitignore` or just don't commit the CSV).
- [✅] **My code uses Relative Paths.** 

### 2. Deliverable Checks
- [✅] **My Dashboard link is publicly accessible.** (No login required).
- [✅] **My Presentation link is publicly accessible.** (Permissions set to "Anyone with the link can view").
- [✅] **I have updated this `README.md` file** with my Executive Summary and technical notes.

### 3. Completeness
- [✅] I have completed **User Stories 1-4**.
- [✅] I have completed the **"Candidate's Choice"** challenge and explained it in the README.

**✅ Only when you have checked every box above, proceed to the submission form.**

---
