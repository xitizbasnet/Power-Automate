# 📧 Power Automate

## Automatically Send Email Notification When a File is Updated in OneDrive

**Date:** 9/8/2025

**Prepared By:** Xitiz Basnet

---

# 📑 Table of Contents

* 🔧 Prerequisites
* 📁 Step 1: Prepare the OneDrive Folder
* ⚙ Step 2: Create the Power Automate Flow
* 🧩 Step 3: Configure the Trigger
* ✉ Step 4: Add the Email Notification Action
* 💾 Step 5: Save and Test
* ✅ Success

---

# 📘 Overview

Automatically Send Email Notification When a File is Updated in OneDrive using Power Automate

This guide provides step-by-step instructions to create an automated email notification system using Power Automate. The flow sends an email whenever a new file is added to a specific OneDrive folder — ideal for collaborative team environments such as IT departments.

---

# 🔧 Prerequisites

Before starting, ensure the following requirements are met:

* A Microsoft 365 account with access to OneDrive for Business
* Access to Power Automate: [https://make.powerautomate.com](https://make.powerautomate.com)
* An existing or new OneDrive folder for monitoring

---

# 📁 Step 1: Prepare the OneDrive Folder

1. Log in to your OneDrive for Business account
2. Create a new folder

### 📂 Example Folder Name

```text id="od1"
IT Shared Documents
```

---

# ⚙ Step 2: Create the Power Automate Flow

1. Navigate to Power Automate:
   🔗 [https://make.powerautomate.com](https://make.powerautomate.com)

2. Click:

```text id="od2"
+ Create
```

3. Select:

```text id="od3"
Automated Cloud Flow
```

4. Configure the flow:

* **Flow Name:** `Automated Mail Flow to IT Shared Documents`
* **Trigger:** `When a file is created (OneDrive for Business)`

5. Click **Create**

---

# 🧩 Step 3: Configure the Trigger

After creation, you will be redirected to the flow designer.

1. You may see a warning:

```text id="od4"
⚠ Invalid parameters
```

(This is expected during initial setup)

2. Configure the folder:

* Click folder icon
* Select:

```text id="od5"
/IT Shared Documents
```

---

### ⚙ Advanced Options

* **Include subfolders:** Yes
* **Infer Content Type:** Yes

---

# ✉ Step 4: Add the Email Notification Action

1. Click:

```text id="od6"
+ New step
```

2. Select:

```text id="od7"
Add an action
```

3. Search and choose:

```text id="od8"
Send an email (V2)
```

📌 (Office 365 Outlook)

---

## 📩 Email Configuration

### To

```text id="od9"
Xitizbasnet@gmail.com
```

### Subject

```text id="od10"
File Created - /File Name in IT Shared Documents
```

---

### 📄 Body

```text id="od11"
Dear Account Holder,

This is to inform you that a new file has been created: "/File Name" in the IT Shared Documents folder.

The file is attached here: /File content

Please check it out.

Thank you.
```

---

## 📎 Advanced Options (Attachments)

Enable **Show advanced options** and configure:

* **Attachments Name – 1:** `/File Name`
* **Attachments Content – 1:** `/File Content`

---

# 💾 Step 5: Save and Test

## Save Flow

Click:

```text id="od12"
Save
```

---

## Test Procedure

1. Upload a Word document to:

```text id="od13"
/IT Shared Documents
```

2. Wait **2–3 minutes**
3. Verify email delivery in inbox
4. Confirm attachment is received

---

# ✅ Success

You have successfully created and tested a Power Automate flow that:

* Monitors a OneDrive folder
* Detects new file creation
* Sends automated email notifications
* Attaches the uploaded file

---

# 📌 Conclusion

This automation improves collaboration and ensures real-time notifications for file changes within shared OneDrive environments, making it highly effective for IT teams and enterprise workflows.

---

# 🎉 THE END 
