
🥗 Diet Recommender using Linear Programming (Simplex Method)

This project provides an optimal daily diet plan tailored to gender-specific nutritional needs and a given budget using Linear Programming (Simplex Method) via scipy.optimize.linprog. The goal is to minimize cost while satisfying all essential nutrient requirements.
📌 Features

    ✅ Generates a cost-effective daily diet plan under a user-specified budget.

    ✅ Customizes nutrient constraints based on gender (male/female).

    ✅ Ensures intake of all key nutrients within recommended bounds.

    ✅ Utilizes open-source, validated Indian food composition and dietary guidelines.

🧠 Optimization Approach

The diet is optimized using the Simplex/HiGHS solver to:

    Minimize total cost, subject to:

        Nutrient intake being within recommended lower and upper bounds.

        Total cost ≤ user's specified daily budget.

        Ingredient quantities ≥ 0.

📂 Data Sources

    Nutrient Requirements:
    Compiled from official dietary recommendations as per the National Institute of Nutrition (ICMR-NIN), India:
    🔗 Dietary Guidelines by NIN (May 2024)

    Nutrient Content per Ingredient:
    Extracted from the official Compendium of Indian Food Composition Tables by the Central Council for Research in Homoeopathy (CCRH), Ministry of AYUSH:
    🔗 CCRH Compendium PDF

📊 Sample Output

Given a budget of ₹500/day for a male:

Optimal diet for male with budget ₹500.0:
Finger Millet       : 133.4 g (₹12.00/100g)
Rice                : 189.9 g (₹6.60/100g)
Guava               : 27.2 g (₹10.00/100g)
Coriander Leaves    : 9.6 g (₹2.00/100g)
Garlic              : 41.2 g (₹5.30/100g)
Coconut             : 183.3 g (₹7.80/100g)
Milk                : 388.3 g (₹5.00/100g)
Total daily cost: ₹67.35

Nutrients provided:
Energy (Kcal)            : 2200.00 (bounds: 2200 - 3000)
Protein (g)              : 47.91 (bounds: 40 - 120)
...

📁 Files in this Repository

    diet_optimizer.ipynb: Jupyter Notebook implementing the optimization model.

    I.xlsx: Excel file containing ingredient data and nutrient values.

    README.md: Project overview and documentation (this file).

⚙️ Requirements

    Python 3.8+

    pandas

    numpy

    scipy

    openpyxl (for reading .xlsx files in Jupyter)

Install dependencies:

pip install pandas numpy scipy openpyxl

🔄 Future Improvements

    Add age-specific and activity-level based recommendations.

    GUI integration for better interactivity.

    Calorie tracking and visualization dashboard.
