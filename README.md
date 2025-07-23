# Upgrading to Windows 11 24H2 Using Microsoft Intune

This tutorial walks through deploying the **Windows 11 24H2 feature update** to devices using **Microsoft Intune (Endpoint Manager)**.

---

## Technologies Used

- Microsoft 365 Admin Center  
- Microsoft Intune (Endpoint Manager)  
- Feature Update Deployment Profiles

---

## Deployment and Configuration Steps

### 1. Access the Microsoft Intune Admin Center
- Log into the [Microsoft 365 Admin Center](https://admin.microsoft.com).
- On the left-hand menu, click **Show All**, then locate and click on **Endpoint Manager**.

<img width="1094" height="818" alt="image" src="https://github.com/user-attachments/assets/564dacea-cfd6-47cb-ae60-35c38f01245b" />


---

### 2. Navigate to Feature Updates
- In the **Microsoft Intune Admin Center**, go to **Devices** on the left-hand panel.
- Under **By Platform**, click **Windows**.
- Scroll to **Policy** > Click **Windows Updates**.
- Click on the **Feature Updates** tab.

<img width="1478" height="378" alt="image" src="https://github.com/user-attachments/assets/0fbe2dfd-5f8a-4208-b77d-062970542f25" />


---

### 3. Create a New Feature Update Profile
- Click **Create Profile**.
- Enter a **Name** and **Description** (e.g., `Windows 11 24H2 Deployment`).
- The **Feature update to deploy** defaults to **Windows 11, version 24H2**.
- Set **Update Type** to:
  - Required *(forces the install)*  
  - **Available** *(optional for users — selected in this tutorial)*

- Optional: Enable  
  `✔️ When a device isn’t eligible to run Windows 11, install the latest Windows 10 feature update`

<img width="2014" height="1382" alt="image" src="https://github.com/user-attachments/assets/acaf31ab-74af-4e88-ad81-773e1daa5845" />


---

### 4. Set Rollout Options
- Under **Rollout Options**, choose **Make update available as soon as possible**.
- Or set a **specific date** if you want to schedule deployment.

 <img width="872" height="606" alt="image" src="https://github.com/user-attachments/assets/3f89c134-27cc-4b82-8b46-e1c6f42e4c8d" />


---

### 5. Assign the Deployment Profile to a Group
- Click **Next**.
- Under **Assignments**, click **Add Group**.
- Select the group to target (e.g., `Autopilot Devices`) and click **Select**.

<img width="1846" height="1382" alt="image" src="https://github.com/user-attachments/assets/ffc04701-4e85-4a3a-95d4-6cc0bbd3fe05" />


---

### 6. Review and Create the Profile
- Click **Next** to reach the **Review + Create** screen.
- Double-check your settings and click **Create**.
- A notification will confirm the profile was successfully assigned.
- Your new profile will appear under **Feature Updates**.

<img width="1164" height="182" alt="image" src="https://github.com/user-attachments/assets/c6ac1b43-be27-4b71-a656-9a356ef006e1" />


---

## ✅ Verification

- Confirm devices in the assigned group receive the **Windows 11 24H2** update.
- Use **Endpoint Manager** to monitor deployment progress and success rate under **Feature Updates**.

---

Let me know if you found this helpful. Happy deploying! 🚀
