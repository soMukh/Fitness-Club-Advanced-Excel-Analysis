# PowerFit India -- Fitness Club Excel Analysis

## 📌 Project Overview

This project is an **advanced Excel-based analysis** for *PowerFit
India*, a fitness club chain. The goal is to help the management team
better understand their membership base by analyzing:

-   **Retention trends** (how long members stay active)\
-   **Revenue patterns** (by membership type & city)\
-   **Referral performance** (impact of referrals on revenue)\
-   **Attendance behavior** (engagement insights)\
-   **Demographics** (gender & age distributions)

All analysis was conducted in **Excel** using formulas, pivot tables,
conditional formatting, and interactive dashboards.

A supporting Excel file contains the complete analysis and
visualizations.

------------------------------------------------------------------------

## 📂 Dataset Details

-   **Rows:** 3 (sample for demonstration, scalable to larger datasets)\
-   **Columns:** 11

### Column Breakdown

  Column Name       Description
  ----------------- -------------------------------------
  Member_ID         Unique member ID (e.g., M001)
  Full_Name         Member's full name
  Start_Date        Membership start date
  End_Date          Membership end date
  Age               Age in years (19--60)
  Monthly_Fee       Monthly membership fee (₹)
  Membership_Type   Basic, Standard, Premium, or Family
  City              City of residence
  Gender            Male or Female
  Attendance        Days visited in a month (1--30)
  Referred_By       Name of referrer (if any)

------------------------------------------------------------------------

## 🛠️ Analysis Performed

### 1. Membership Duration

-   Added column **Membership_Duration_Months**\

-   Formula:

        =DATEDIF(Start_Date, End_Date, "M")

-   Assumption: 1 month = 30 days

### 2. Referral Impact

-   Created **Referred** column (Yes/No based on `Referred_By`)\
-   Pivot table to compare **average Monthly Fee** for referred vs
    non-referred members

### 3. Revenue Calculation

-   Added **Total_Revenue** column:

        =Monthly_Fee × Membership_Duration_Months

-   Summarized revenue by:

    -   Premium members\
    -   Family membership\
    -   City-wise distribution

### 4. Low Engagement Members

-   Conditional Formatting rule: highlight members with
    -   Attendance `< 10`\
    -   AND Membership_Duration_Months `>= 12`\
-   Flags long-term but inactive users

### 5. Segment Profitability Dashboard

-   Interactive **Pivot Dashboard** built to show:
    -   Most profitable City + Membership Type + Referral combinations\
    -   Average revenue per member per segment\
    -   Insights for marketing & referral strategies\
-   Features: **Slicers & Pivot Charts** for interactivity

### 6. Gender & Age Distribution

-   Pivot table: **Gender-wise member count per city**\
-   Pivot table: **Age distribution across membership types**
    -   18--30 → Youth\
    -   31--45 → Adults\
    -   46+ → Seniors

------------------------------------------------------------------------

## 📊 Deliverables

-   **Excel Workbook**: Contains all analysis, pivot tables, dashboards,
    and visualizations.\
-   **PDF Report**: Assignment summary and problem statement.\
-   **README.md**: Project documentation for GitHub.

------------------------------------------------------------------------

## 🚀 How to Use

1.  Open the Excel file provided in this repo.\
2.  Explore individual sheets for calculations, pivot tables, and
    conditional formatting.\
3.  Use the interactive dashboard (with slicers) to drill into specific
    segments.

------------------------------------------------------------------------

## 📈 Key Insights (Example Outputs)

-   Referrals tend to bring higher-paying members.\
-   Premium memberships generate the highest revenue.\
-   Certain cities show stronger attendance trends, ideal for marketing
    campaigns.\
-   Youth segment dominates in number, while Family memberships provide
    stable long-term revenue.
