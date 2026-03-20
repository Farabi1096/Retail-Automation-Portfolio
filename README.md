# Retail Automation Portfolio
**Faisal Meah / portfolio** &nbsp; [![Back to Profile](https://img.shields.io/badge/←_Back_to_Profile-FF0000?style=flat-square&logoColor=white)](https://github.com/Farabi1096/portfolio) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/farabi-hsn/)

---

### 🛠️ Expertise
![Automation](https://img.shields.io/badge/Automation-Apps_Script_%7C_VBA-FF0000?style=flat-square&logoColor=white) ![AI Integration](https://img.shields.io/badge/AI_Integration-Gemini_API_%7C_Vision-000000?style=flat-square&logoColor=white) ![Data Architecture](https://img.shields.io/badge/Architecture-Data_Hierarchy-FF0000?style=flat-square&logoColor=white)

---

### ![Project](https://img.shields.io/badge/Project-Retail_Outlet_Display_AI_Audit-FF0000?style=for-the-badge&logo=googlecloud&logoColor=white)

> **Problem:** Retail audit teams struggle with unorganized outlet photos, making it impossible to verify "Shelf Talker" compliance or stock availability in real-time across thousands of unique locations.  
> **Solution:** A centralized pipeline that captures granular outlet data, uses Gemini AI for visual compliance, and organizes images into a strict business hierarchy.

---

#### 🔄 Step-by-Step Implementation

**Step 1: Granular Field Submission (Web App)** Sales officers upload photos via a custom interface. The system ensures every upload is tagged with a complete data string: **Area, Town, DB Code, DB Name, Outlet Code, Outlet Name, and Route**. This eliminates the possibility of "orphan" data.
<p align="center">
  <img src="images/Web%20App.jpg" width="90%" alt="Web App Interface" />
</p>

**Step 2: Intelligent Hierarchy (Apps Script + AI)** Google Apps Script processes the upload and triggers the **Gemini Vision API** to check for "Shelf Talker" presence and SKU quantity. Simultaneously, the script renames and files the image into a deep-folder structure:  
`Root > Area > Town > Route > [Outlet_Code]_[Timestamp].jpg`
<p align="center">
  <img src="images/App%20Script.jpg" width="90%" alt="Apps Script and AI Logic" />
</p>

**Step 3: Automated Ledger (Google Sheets)** The final audit results and metadata are appended to a master database. This structured log allows for instant filtering by **DB Name** or **Route** to identify specific gaps in retail execution.
<p align="center">
  <img src="images/Google%20Sheet.jpg" width="90%" alt="Google Sheet Database" />
</p>

---

#### 📊 Data Schema & Logic
The system maintains a rigid data structure to support advanced MIS reporting:

| Field | Purpose | Logic |
| :--- | :--- | :--- |
| **Area / Town** | Regional Sorting | Directs the file to the correct Drive folder. |
| **DB Code / Name** | Distributor Tracking | Links the audit to the specific distribution point. |
| **Route / Outlet** | Micro-Level Audit | Identifies exactly which shop needs compliance correction. |
| **AI Vision Result** | Compliance Status | Boolean (Yes/No) check for Shelf Talkers via Gemini API. |

#### 💡 Project Impact
* **Structured Asset Management:** Thousands of images are instantly searchable by **Outlet Code** or **Route**.
* **Zero Manual Filing:** 100% of renaming and folder creation is handled by the automation script.
* **Granular Visibility:** Management can now track compliance trends down to the specific **Route** or **Distributor** level.

---
