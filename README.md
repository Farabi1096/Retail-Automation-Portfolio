# Retail Automation Portfolio
**[Your Name] / portfolio** &nbsp; [![Back to Profile](https://img.shields.io/badge/←_Back_to_Profile-FF0000?style=flat-square&logoColor=white)](https://github.com/Farabi1096/portfolio) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/farabi-hsn/)

---

### 🛠️ Expertise
![Automation](https://img.shields.io/badge/Automation-Apps_Script_%7C_VBA-FF0000?style=flat-square&logoColor=white) ![AI Integration](https://img.shields.io/badge/AI_Integration-Gemini_API_%7C_Vision-000000?style=flat-square&logoColor=white) ![Data Architecture](https://img.shields.io/badge/Architecture-Hierarchy_Logic_%7C_SQL-FF0000?style=flat-square&logoColor=white)

---

### ![P7](https://img.shields.io/badge/Project_7-AI_Retail_Display_Audit-FF0000?style=for-the-badge&logo=googlecloud&logoColor=white)
> **Problem:** Manual verification of retail display compliance (shelf talkers, stock availability) is slow and subjective. Field photos are often uploaded without structure, making audit trails nearly impossible to manage.  
> **Solution:** An AI-integrated Web App that validates display modality in real-time, extracts SKU-level data, and automatically organizes assets into a searchable cloud hierarchy.

<p align="center">
  <img src="images/Display_App_Interface.jpg" width="45%" alt="Web App Interface" />
  <img src="images/AI_Audit_Logic.jpg" width="45%" alt="AI Analysis Result" />
</p>

#### 🔑 Key Features
* **Automated Data Capture:** Sales officers upload photos via a custom web portal; the system automatically maps the **Area, Town, DB Code, and DB Name** to a centralized Google Sheet.
* **Vision AI Audit Engine:** Utilizes **Google Gemini API** via Apps Script to perform real-time image analysis:
    * **Modality Check:** Confirms if "Shelf Talkers" and specific branding materials are present.
    * **Product Verification:** Identifies if the correct products are displayed and estimates available quantity.
    * **Image Validation:** Filters out non-retail or duplicate images to ensure data integrity.
* **Dynamic File Hierarchy:** A custom-built **Apps Script** renames and moves images into a structured Drive directory based on business logic:  
  `Root > Area > Town > DB_Code > [Timestamp]_Display.jpg`

---

### 📂 Technical Breakdown

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Frontend** | HTML5 / JavaScript | Responsive mobile interface for field-based uploads. |
| **Logic Layer** | Google Apps Script | Serves as the middleware for API handling and Drive automation. |
| **AI Engine** | Gemini Pro Vision | Processes visual data for compliance and SKU count. |
| **Database** | Google Sheets | Acts as the real-time ledger for all transaction metadata. |

---

### 💡 Impact
* **Eliminated Manual Sorting:** 100% automation of image renaming and filing into the correct regional folders.
* **Instant Compliance Feedback:** Reduced the audit cycle from days to seconds, allowing Sales Officers to correct displays while still on-site.
* **Scalable Reporting:** Created a clean, structured dataset ready for Power BI visualization or SQL analysis.

---
