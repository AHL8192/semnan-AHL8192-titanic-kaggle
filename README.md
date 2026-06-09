<div align="center">
  <h1>🚢 Titanic Survival Prediction 🌊</h1>
  <h3>Machine Learning Final Project - Semnan University</h3>
  <p><i>پروژه نهایی درس یادگیری ماشین - دانشگاه سمنان</i></p>
</div>

---

## 🇬🇧 English Documentation

### 📌 About the Project

This repository contains the complete workflow of a Machine Learning project from scratch, developed as the final project for the Machine Learning course at Semnan University's Faculty of Electrical and Computer Engineering.
The goal is to predict the survival of passengers on the Titanic using classification algorithms.

### 📊 Dataset

- **Name:** Titanic Dataset
- **Size:** 891 rows, 12 columns
- **Target Variable:** `Survived` (Binary: 0 = Died, 1 = Survived)

### 🛠️ Project Workflow

1. **Exploratory Data Analysis (EDA):**
  - Analyzed feature distributions using Histograms, KDE, and Boxplots.
  - Checked for normality using QQ Plots and applied Log Transformation to heavily skewed features like `Fare`.
  - Visualized feature correlations using a Correlation Heatmap.
2. **Data Preprocessing:**
  - Handled missing values (Median for `Age`, Mode for `Embarked`, dropped `Cabin`).
  - Encoded categorical variables (`Sex`, `Embarked`).
  - Split data into Training (80%) and Testing (20%) sets using `random_state=42`.
3. **Modeling:**
  - Algorithm: **Decision Tree Classifier**
  - Hyperparameters: `max_depth=5` (chosen to control tree depth and prevent severe overfitting).
4. **Evaluation:**
  - Plotted the Confusion Matrix using Seaborn heatmaps.
  - Calculated Accuracy, Precision, Recall, and F1-Score.
  - *Note on Recall:* In this specific context, prioritizing Recall ensures we minimize False Negatives (missing actual survivors), which is critical for imbalanced survival datasets.

### 📈 Results & Future Improvements

- The model achieved ~86% training accuracy and ~78% testing accuracy, showing a reasonably controlled level of overfitting.
- **Future suggestions:** Engineering new features like "Family Size" (combining `SibSp` and `Parch`) and applying class weights (`class_weight='balanced'`) to effectively handle class imbalance.

---

## 🇮🇷 مستندات فارسی (Farsi Documentation)

### 📌 درباره پروژه

این مخزن شامل پیاده‌سازی کامل یک پروژه یادگیری ماشین از صفر تا صد است که به عنوان پروژه نهایی درس یادگیری ماشین در دانشکده مهندسی برق و کامپیوتر **دانشگاه سمنان** انجام شده است.
هدف این پروژه، پیش‌بینی بقای مسافران کشتی تایتانیک با استفاده از الگوریتم‌های طبقه‌بندی است.

### 📊 مجموعه داده (Dataset)

- **نام:** مجموعه داده تایتانیک (Titanic)
- **اندازه:** ۸۹۱ سطر و ۱۲ ویژگی (ستون)
- **متغیر هدف:** `Survived` (دو کلاسه: ۰ = جان‌باخته، ۱ = نجات‌یافته)

### 🛠️ مراحل انجام پروژه

۱. **تحلیل اکتشافی داده‌ها (EDA):**

- بررسی توزیع ویژگی‌های عددی با استفاده از هیستوگرام، KDE و Boxplot.
- بررسی نرمال بودن توزیع داده‌ها با QQ Plot و اعمال تبدیل لگاریتمی برای رفع چولگی (مثلاً در ستون `Fare`).
- بررسی همبستگی ویژگی‌ها با رسم ماتریس همبستگی (Heatmap).
  ۲. **پیش‌پردازش داده‌ها:**
- مدیریت مقادیر گمشده (استفاده از میانه برای `Age`، مد برای `Embarked` و حذف ستون `Cabin`).
- کدگذاری متغیرهای دسته‌ای (مانند جنسیت و بندر سوار شدن).
- تقسیم داده‌ها به دو بخش آموزش (۸۰٪) و آزمون (۲۰٪).
  ۳. **مدل‌سازی:**
- الگوریتم انتخابی: **درخت تصمیم (Decision Tree)**
- پارامترها: تنظیم `max_depth=5` برای کنترل عمق درخت و جلوگیری از بیش‌برازش (Overfitting).
  ۴. **ارزیابی مدل:**
- رسم ماتریس درهم‌ریختگی (Confusion Matrix).
- محاسبه معیارهای Accuracy, Precision, Recall و F1-Score.
- *اهمیت Recall:* در این مسئله، تمرکز بر روی Recall به ما کمک می‌کند تا خطای نوع دوم (عدم تشخیص مسافرانی که واقعاً نجات یافته‌اند) را به حداقل برسانیم.

### 📈 نتایج و پیشنهادات بهبود

- دقت مدل روی داده‌های آموزشی حدود ۸۶٪ و روی داده‌های آزمون حدود ۷۸٪ بود که نشان می‌دهد میزان بیش‌برازش با تنظیم عمق درخت به خوبی کنترل شده است.
- **پیشنهادات برای آینده:** استخراج ویژگی‌های جدید مانند "اندازه خانواده" (از ترکیب `SibSp` و `Parch`) و همچنین استفاده از وزن‌دهی کلاس‌ها (`class_weight='balanced'`) برای مدیریت بهتر نامتوازن بودن داده‌ها.

---

*Developed by Ahmadreza Alipouryan*
