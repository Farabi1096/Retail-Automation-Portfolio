# Retail Automation Portfolio
**[Your Name] / portfolio** &nbsp; [![Back to Profile](https://img.shields.io/badge/←_Back_to_Profile-FF0000?style=flat-square&logoColor=white)](https://github.com/Farabi1096/portfolio) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/farabi-hsn/)

---

### 🛠️ Expertise
![Automation](https://img.shields.io/badge/Automation-Apps_Script_%7C_VBA-FF0000?style=flat-square&logoColor=white) ![AI Integration](https://img.shields.io/badge/AI_Integration-Gemini_API_%7C_Vision-000000?style=flat-square&logoColor=white) ![Data Architecture](https://img.shields.io/badge/Architecture-Hierarchy_Logic_%7C_SQL-FF0000?style=flat-square&logoColor=white)

---

### ![P7](https://img.shields.io/badge/Project_7-AI_Retail_Display_Audit-FF0000?style=for-the-badge&logo=googlecloud&logoColor=white)

> **Problem:** Manual verification of retail display compliance (shelf talkers, stock availability) is slow and unorganized. Field photos are often uploaded without structure, making audit trails impossible to manage.  
> **Solution:** An AI-integrated pipeline that validates display modality in real-time, extracts SKU-level data, and automatically organizes assets into a searchable cloud hierarchy.

---

#### 🔄 Step-by-Step Workflow

**Step 1: Field Data Collection (Web App Interface)** The process begins with Sales Officers using a custom mobile-responsive web portal to upload high-resolution display photos directly from the outlet.
<p align="center">
  <img src="images/Web_App.jpg" width="90%" alt="Web App Interface" />
</p>

**Step 2: Intelligent Processing (Apps Script & Gemini AI)** Once uploaded, **Google Apps Script** triggers the **Gemini Vision API**. The AI audits the image for "Shelf Talker" compliance and product availability while a custom script renames the file based on the **Area > Town > DB Code** hierarchy.
<p align="center">
  <img src="images/App_Script_API.jpg" width="90%" alt="Apps Script and AI Logic" />
</p>

**Step 3: Centralized Data Logging (Google Sheets)** All audit results, including AI-generated compliance scores and SKU quantities, are logged into a master Google Sheet. This acts as the "Single Source of Truth" for regional performance tracking.
<p align="center">
  <img src="images/Google_Sheet.jpg" width="90%" alt="Google Sheet Database" />
</p>

---

#### 🔑 Key Technical Features
* **Vision AI Audit Engine:** Automatically detects if branding materials are present and filters out non-retail or duplicate images.
* **Dynamic File Hierarchy:** Images are moved into structured Drive directories:  
  `Root > Area > Town > DB_Code > [Timestamp]_Display.jpg`
* **Real-time Metadata Mapping:** Automatically logs **Area, Town, and DB Name** without manual entry by the officer.

#### 💡 Project Impact
* **100% Automated Renaming:** Eliminated manual file sorting for thousands of field uploads.
* **Instant Compliance Feedback:** Reduced the audit cycle from days to seconds, allowing for immediate on-site corrections.
* **Structured Data Ready:** The clean Google Sheet backend allows for instant connection to **Power BI** for high-level management dashboards.

---
