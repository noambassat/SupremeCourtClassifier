
# Supreme Court Appeals Outcome Prediction

This project builds on a larger initiative (https://github.com/noambassat/VIrtual_Machine_Crawler) where we develeped **web crawler**  to scrape all Supreme Court cases in Israel from 1997. The focus here is to predict the outcomes of criminal appeal cases (both direct appeals and requests for appeal) brought before the Supreme Court.


## Project Highlights

1. **Dataset Preparation**:
   - Extracted and processed appeal cases from the scraped data.
   - Used **Legal He BERT** embeddings for text vectorization to handle Hebrew documents.

2. **Handling Imbalanced Data**:
   - The dataset was imbalanced, with the minority class representing successful appeals.
   - Applied **undersampling** with a 60:40 ratio for class 0 (unsuccessful appeals) to class 1 (successful appeals).
   - Assigned a weight of 3:1 to the minority class during model training.

3. **Model and Techniques**:
   - Used **Logistic Regression** for classification.
   - Evaluated performance using **5-fold cross-validation**.
   - Metrics calculated: accuracy, precision, recall, and F1-score.

4. **Key Results**:
   - **Mean Accuracy**: 97.31%
   - **Mean Precision for Class 1**: 97.50%
   - **Mean Recall for Class 1**: 95.28%
   - **Mean F1 Score for Class 1**: 96.32%
   - **Confusion Matrix**:
     ```
     [[70  1]
      [ 2 41]]
     ```
     - **True Negatives (TN)**: 70
     - **False Positives (FP)**: 1
     - **False Negatives (FN)**: 2
     - **True Positives (TP)**: 41

5. **Conclusion**:
   - The model demonstrated excellent performance, achieving high precision and recall for predicting successful appeals.
   - The preprocessing steps, including the embedding generation and data balancing techniques, contributed to the model's success.

---



# חיזוי תוצאות ערעורים לבית המשפט העליון

פרויקט זה ממשיך יוזמה רחבה יותר (https://github.com/noambassat/VIrtual_Machine_Crawler) שבמסגרתה פיתחנו **Web Crawler** לאתר את כל פסקי הדין מבית המשפט העליון בישראל משנת 1997. מטרת הפרויקט היא לחזות את תוצאות הערעורים הפליליים (ערעורים רגילים ובקשות רשות לערער) שהוגשו לבית המשפט העליון.

## עיקרי הפרויקט

1. **עיבוד הנתונים**:
   - חילוץ וניתוח תיקי ערעור מתוך הנתונים שנגרדו.
   - שימוש ב-**Legal He - BERT** ליצירת embedding מותאם למסמכים בעברית.

2. **התמודדות עם חוסר איזון בנתונים**:
   - הנתונים היו לא מאוזנים, כאשר המקרים שבהם הערעור התקבל היוו את המיעוט.
   - יישום **undersampling** ביחס של 60:40 לטובת כיתה 0 (ערעורים שנדחו).
   - מתן משקל של 3:1 לטובת המיעוט במהלך אימון המודל.

3. **מודל ושיטות**:
   - שימוש ב-**Logistic Regression** למודל סיווג.
   - הערכת הביצועים באמצעות **קרוס-ולידציה של 5 קפלים**.
   - חישוב מדדים: דיוק (Accuracy), דיוק עבור הכיתה הקטנה (Precision), רגישות (Recall), ו-F1.

4. **תוצאות עיקריות**:
   - **דיוק ממוצע**: 97.31%
   - **דיוק ממוצע עבור כיתה 1**: 97.50%
   - **רגישות ממוצעת עבור כיתה 1**: 95.28%
   - **מדד F1 ממוצע עבור כיתה 1**: 96.32%
   - **מטריצת בלבול**:
     ```
     [[70  1]
      [ 2 41]]
     ```
     - **True Negatives (TN)**: 70
     - **False Positives (FP)**: 1
     - **False Negatives (FN)**: 2
     - **True Positives (TP)**: 41

5. **מסקנות**:
   - המודל הפגין ביצועים מצוינים, עם דיוק ורגישות גבוהים בחיזוי ערעורים שהתקבלו.
   - שלבי העיבוד המקדימים, כולל יצירת embedding ושיטות לאיזון הנתונים, תרמו להצלחת המודל.
