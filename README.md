# Data_Science_job_Analysis
It transforms complex datasets into a visual decision-making tool using multi-criteria array formulas and professional data validation.

##**🚀 Key Technical Concepts**
This project demonstrates the ability to manage large datasets and build complex analytical models without relying on external software.

###***1. Advanced Analytical Formulas***
Multi-Criteria Array Logic: Engineered complex nested IF statements within MEDIAN and COUNT functions to perform real-time filtering across Country, Job Title, and Schedule Type.

Example Formula: ```excel
=MEDIAN(IF((jobs[job_country]=A2)(jobs[salary_year_avg]<>0)(jobs[job_title_short]=title), jobs[salary_year_avg]))```

**Robust Data Retrieval**: Implemented XLOOKUP to dynamically fetch job counts and median pay, replacing older, less efficient VLOOKUP methods for better performance.

**Text Analysis**: Used ISNUMBER(SEARCH(...)) logic to categorize job types from messy text strings, enabling a "Search-like" filtering experience.

###**2. Dynamic UI/UX Engineering**
Custom Shape KPIs: Since standard Excel charts are limited, I engineered Shape-based KPIs that link directly to background calculation sheets. These provide a modern, app-like interface for "Median Salary," "Top Platform," and "Job Count."

***Interactive Slicers & Dropdowns***: Integrated Data Validation dropdowns and Slicers to allow users to instantly pivot the entire dashboard view between different job categories.

***Professional Cleanup***: Utilized "View" layer optimizations—removing Gridlines, Headings, and Formula Bars—to create a standalone "Software" feel within Excel.

###***3. Data Integrity & Error Handling***
Outlier Management: Specifically excluded $0 salary entries in array calculations to ensure "Median" values accurately reflect market reality.

Formula Resilience: Handled #NUM! and #VALUE! errors (common in 32k row datasets) using logic-check multipliers (*) to ensure the dashboard never breaks for the end-user.

##**📁 Repository Structure**
Vrinda Store Data Analysis.xlsx: The master engine containing raw data, logic sheets, and the interactive dashboard.

images/: A collection of high-resolution screenshots capturing the dashboard's responsive states and underlying formula logic.

README.md: Project overview and technical documentation.

##**🛠️ Tools Used**
Excel: Advanced Formulas, Pivot Tables, Data Validation, Map Charts.

Git/GitHub: Version control and project documentation.

##**🛠️ How to Use**
1.Download the .xlsx file or view the Live Preview link above.

2.Use the Slicers or Dropdown Menus at the top of the dashboard to filter by Job Title or Country.

3.Observe how the KPIs and Geographic Maps update instantly to reflect the filtered dataset.
