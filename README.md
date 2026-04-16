\# 🏦 Loan Portfolio Dashboard – Credit Risk Analysis

\# 🏦 داشبورد محفظة القروض – تحليل المخاطر الائتمانية



\---



\## 🧾 Project Overview | نظرة عامة على المشروع



This project presents an Excel-based loan portfolio dashboard built to analyze customer loan data, monitor portfolio performance, evaluate loan status, and segment customers by credit risk.



The dashboard focuses on:

\- Loan portfolio monitoring

\- Loan status distribution

\- Credit status analysis

\- Guarantee type analysis

\- Monthly installment and loan amount comparisons

\- Executive KPI tracking



\---



هذا المشروع عبارة عن داشبورد لتحليل محفظة القروض باستخدام Excel بهدف:



\- متابعة أداء محفظة القروض

\- تحليل حالة القروض

\- تصنيف العملاء حسب الحالة الائتمانية

\- تحليل أنواع الضمانات

\- مقارنة متوسط القروض والأقساط الشهرية

\- عرض مؤشرات أداء رئيسية بشكل تنفيذي



\---



\# 🛠 Tools \& Technologies | الأدوات المستخدمة



\- Excel

\- Pivot Tables

\- Dashboard Design

\- Python (pandas)

\- GitHub



\---



\# 📄 Workbook Structure | مكونات ملف الإكسيل



The workbook includes three main sheets:



\- \*\*Total Facilities\*\* → Raw loan data

\- \*\*Pivots\*\* → Pivot-based analytical layer

\- \*\*Dashboard\*\* → Final dashboard interface



\---



يتكوّن ملف الإكسيل من 3 شيتات رئيسية:



\- \*\*Total Facilities\*\* → البيانات الأساسية

\- \*\*Pivots\*\* → طبقة التحليل باستخدام Pivot Tables

\- \*\*Dashboard\*\* → واجهة الداشبورد النهائية



\---



\# 🧠 Workflow Summary | ملخص خطوات العمل



\### 1. Data Preparation | تجهيز البيانات

\- Organized loan records for customers

\- Structured fields such as branch, funding type, guarantee, loan amount, installment, loan status, and credit score



\### 2. Credit Classification | التصنيف الائتماني

Python was used to classify customers based on their credit scores and support the analysis workflow.



```python

import pandas as pd



\# Load the loan dataset

df = pd.read\_excel("banking\_data.xlsx")



\# Define credit score classification function

def classify\_credit(score):

&#x20;   if score > 750:

&#x20;       return "Satisfactory"

&#x20;   elif score >= 600:

&#x20;       return "High Risk"

&#x20;   else:

&#x20;       return "Unsatisfactory"



\# Apply classification to each customer

df\["Risk\_Category"] = df\["Credit\_Score"].apply(classify\_credit)



\# Save the updated dataset to a new Excel file

df.to\_excel("banking\_data\_with\_risk.xlsx", index=False)

```



\### 3. Pivot-Based Analysis | التحليل باستخدام Pivot Tables

Pivot tables were used to summarize:



\- Loan Status

\- Funding Type

\- Guarantee Type

\- Credit Status

\- Average Loan Amount

\- Average Monthly Installment



\### 4. Dashboard Redesign \& KPI Enhancement | تحسين التصميم وإضافة KPI Cards

The dashboard was visually redesigned to improve clarity and executive presentation.



New KPI cards were added to highlight:



\- Count of Loans

\- Late Rate

\- Total Portfolio Amount

\- Active Loans

\- Closed Loans

\- Late Loans



\---



\# ✅ Credit Classification Logic | منطق التصنيف الائتماني



The credit classification used in this project is based on real, publicly available scoring criteria aligned with Egyptian banking practices and Central Bank of Egypt instructions.



\---



التصنيف الائتماني المستخدم في هذا المشروع مبني على معايير سكور حقيقية ومتاحة للعامة، ومتوافقة مع الممارسات البنكية المصرية وتعليمات البنك المركزي المصري.



\---



\# 📊 Dashboard Insights | أهم التحليلات داخل الداشبورد



The dashboard provides insights into:



\- \*\*Average Loan Amount by Status\*\*

\- \*\*Average Monthly Installment by Status\*\*

\- \*\*Credit Status vs Loan Status\*\*

\- \*\*Guarantee Type vs Loan Status\*\*

\- \*\*Loan Type vs Loan Status\*\*

\- \*\*Executive KPI Overview\*\*

\- \*\*Full Portfolio Dashboard View\*\*



\---



يعرض الداشبورد التحليلات التالية:



\- \*\*متوسط مبلغ القرض حسب الحالة\*\*

\- \*\*متوسط القسط الشهري حسب الحالة\*\*

\- \*\*الحالة الائتمانية مقابل حالة القرض\*\*

\- \*\*نوع الضمان مقابل حالة القرض\*\*

\- \*\*نوع القرض مقابل حالة القرض\*\*

\- \*\*نظرة عامة على مؤشرات الأداء الرئيسية\*\*

\- \*\*عرض كامل للداشبورد\*\*



\---



\# 🎛 Filters | الفلاتر المستخدمة



The dashboard includes interactive filters for:



\- Branch

\- Guarantee

\- Funding Type

\- Monthly Installment

\- Interest Rate (%)



\---



يتضمن الداشبورد فلاتر تفاعلية حسب:



\- الفرع

\- الضمان

\- نوع التمويل

\- القسط الشهري

\- نسبة الفائدة



\---



\# 📈 Key KPIs | المؤشرات الرئيسية



\- \*\*Count of Loans:\*\* 40

\- \*\*Late Rate:\*\* 42.50%

\- \*\*Total Portfolio Amount:\*\* 5,996,877

\- \*\*Active Loans:\*\* 17

\- \*\*Closed Loans:\*\* 6

\- \*\*Late Loans:\*\* 17



\---



\# 📷 Screenshots



\### Full Dashboard View

!\[Full Dashboard View](screenshots/dashboard\_full\_view.png)



\### KPI Cards Overview

!\[KPI Cards Overview](screenshots/kpi\_cards\_overview.png)



\### Average Loan Amount by Status

!\[Average Loan Amount by Status](screenshots/avg\_loan\_amount\_by\_status.png)



\### Average Monthly Installment by Status

!\[Average Monthly Installment by Status](screenshots/avg\_monthly\_installment\_by\_status.png)



\### Credit Status vs Loan Status

!\[Credit Status vs Loan Status](screenshots/credit\_status\_vs\_loan\_status.png)



\### Guarantee Type vs Loan Status

!\[Guarantee Type vs Loan Status](screenshots/guarantee\_vs\_loan\_status.png)



\### Loan Type vs Loan Status

!\[Loan Type vs Loan Status](screenshots/loan\_type\_vs\_loan\_status.png)



\---



\# 📁 Repository Structure



&#x20;   Loan\_Risk\_Analysis\_Dashboard/

&#x20;   ├── dashboard/

&#x20;   │   └── Loan\_Portfolio\_Dashboard.xlsx

&#x20;   ├── screenshots/

&#x20;   │   ├── dashboard\_full\_view.png

&#x20;   │   ├── kpi\_cards\_overview.png

&#x20;   │   ├── avg\_loan\_amount\_by\_status.png

&#x20;   │   ├── avg\_monthly\_installment\_by\_status.png

&#x20;   │   ├── credit\_status\_vs\_loan\_status.png

&#x20;   │   ├── guarantee\_vs\_loan\_status.png

&#x20;   │   └── loan\_type\_vs\_loan\_status.png

&#x20;   ├── scripts/

&#x20;   │   └── credit\_classification.py

&#x20;   ├── .gitignore

&#x20;   └── README.md



\---



\# ⚠️ Limitations | القيود



\- Sample dataset used for demonstration

\- Excel-based dashboard environment

\- No live database connection

\- Static reporting structure



\---



القيود الحالية في المشروع:



\- البيانات تجريبية لغرض العرض

\- الداشبورد مبني داخل Excel

\- لا يوجد اتصال مباشر بقاعدة بيانات

\- التقارير ثابتة وليست متصلة بمصدر حي



\---



\# 🚀 Future Improvements | التطوير المستقبلي



\- Connect the project to SQL Server

\- Rebuild the dashboard in Power BI

\- Improve the credit risk logic

\- Add more advanced KPIs

\- Build a more automated ETL workflow

\- Add date-based trend analysis



\---



التطويرات المستقبلية المقترحة:



\- ربط المشروع بقاعدة بيانات SQL Server

\- إعادة بناء الداشبورد باستخدام Power BI

\- تحسين منطق تصنيف المخاطر الائتمانية

\- إضافة مؤشرات أداء أكثر تقدمًا

\- بناء Workflow أكثر أتمتة للبيانات

\- إضافة تحليل زمني مبني على التواريخ



\---



\# 👨‍💻 Author



\*\*Ahmed Samir Toukhy\*\*  

Data Analyst | Excel, Python, and Dashboard Design  

Cairo, Egypt

