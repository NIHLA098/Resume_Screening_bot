# Resume Screening Bot (UiPath)

## 📝 Project Overview

This project automates the process of *screening resumes* using *UiPath*.  

The bot performs the following tasks:
- Extracts *skills, experiences, and other relevant details* from resumes
- Scores resumes based on their match with target keywords or job descriptions
- Outputs all structured data into an *Excel workbook*

This automation significantly reduces manual effort in recruitment workflows.

---

## 💼 Key Features

✅ *Automated Resume Extraction*
- Reads resumes in *PDF* or *DOCX* format
- Extracts:
  - Candidate Name 
  - Skills
  - Work experience
  - Education and certifications

✅ *Keyword Matching & Scoring*
- Compares extracted skills and experiences against a *predefined list of keywords*
- Calculates and assigns a *relevance score*

✅ *Excel Report Generation*
- Writes extracted data and scores into a structured Excel file

✅ *Batch Processing*
- Processes multiple resumes in one run

---

## ⚙ Tools & Technologies

- *UiPath Studio*
  - Document Understanding activities
  - Regex-based data extraction
  - Data Tables for structured processing
  - Excel Application Scope and Write Range
- *Microsoft Excel*
  - For reporting outputs

---

## 🚀 Workflow Overview

1. *Input Folder*
   - Resumes are placed in a specified directory (e.g., \Resumes\Input)

2. *Extraction*
   - Bot loops through each resume
   - Uses:
     - *Regex* and *String Manipulation* to extract relevant fields
     - Document Understanding if needed for PDFs

3. *Scoring*
   - Compares extracted skills to a *list of keywords* stored in an Excel or variable
   - Counts matches and calculates a relevance score

4. *Output*
   - Writes all extracted details and the score into an *Excel workbook*

---

## 📂 Project Components

- Main.xaml – Main workflow file
- Config.xlsx – Configuration file containing target keywords
- /Resumes/Input/ – Folder containing resumes to be processed
- /Resumes/Output/ – Folder for processed files and reports
- README.md – Project documentation

---

## ✨ Example Use Case

A recruiter wants to shortlist candidates for a *Data Analyst* role with key skills:
- Python
- SQL
- Tableau

The bot processes all resumes in the input folder, identifies which candidates have these skills, and scores them accordingly.

---

---

## 📄 License

This project is shared for educational and demonstration purposes.
