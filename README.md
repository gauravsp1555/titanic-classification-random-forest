## Titanic Survival Prediction — Complete Data Cleaning
1. Fixed duplicate/inconsistent missing-value handling (Age was filled with `mean` first, then again with `median` later) — now it's done only once, using `median` (more robust to outliers than mean).
2. Dropped the `Cabin` column cleanly in one place (the original notebook tried to drop it in two different spots, which caused confusion).
3. Added new features: `IsAlone`, and a `Title` extracted from the Name column (Mr/Mrs/Miss/Master/Rare) — these help improve model accuracy, along with the `Family_size` feature you already had.
4. Added more EDA visuals (survival by Sex, Pclass, Title, and Age).
5. Added Logistic Regression alongside Random Forest, for comparison.
6. Added a feature importance plot to show which features matter most for predictions.
