Onboard a New User and Add Their Device in Microsoft 365 Admin Center

## Overview
This lab demonstrates the full onboarding process for a new employee in a corporate environment, covering the creation of a Microsoft 365 user account, assignment of licenses, and enrollment of a new Windows device into Intune for management.

## Who / What / Where / When / Why

- **Who:**  
IT Support Specialists at a national consulting firm onboarding new employees.

- **What:**  
Create a Microsoft 365 user account, assign licenses (Office, Intune), set a password, and guide through device enrollment into Intune.

- **Where:**  
Microsoft 365 Admin Center (admin.microsoft.com) and Windows 11 Device.

- **When:**  
During the new hire onboarding process, before the employee receives their computer.

- **Why:**  
To ensure the employee has access to necessary company resources and the new device is secured and managed by corporate policies.

---

# Step-by-Step Instructions

---

## Step 1: Sign in to Microsoft 365 Admin Center

**Instructions:**

1. Open a web browser.
2. Go to [https://admin.microsoft.com](https://admin.microsoft.com).
3. Sign in using Global Admin or User Management Admin credentials.

**Explanation:**  
Access to the Microsoft 365 Admin Center is required to create and manage user accounts. Only authorized roles like Global Administrator or User Management Administrator can perform these tasks.

---

## Step 2: Create a New User Account

**Instructions:**

1. In the left-hand menu, select **Users** > **Active Users**.

![image](https://github.com/user-attachments/assets/839574a7-f930-4a79-b0bc-4a03df9c6e32)

2. Click **Add a user**.

![image](https://github.com/user-attachments/assets/dd887f03-c46f-4d7e-afc1-bd346ac09647)

3. Enter the following:
   - **First name** and **Last name** of the new employee.
   - **Display name** (e.g., John Doe).
   - **Username** (e.g., john.doe@companydomain.com).

4. Choose **Automatically create a password** or **Manually create a password**.
5. Check **Require this user to change their password when they first sign in** (recommended).

**Explanation:**  
Creating a user account provisions the identity needed for the employee to access Microsoft 365 services. Setting an initial password and enforcing a password change upon first login enhances security.

![image](https://github.com/user-attachments/assets/9796a442-14b0-42e0-9201-80af0a68b53d)

---

## Step 3: Assign Product Licenses

**Instructions:**

1. On the same "Add user" page, under **Product licenses**, choose:
   - **Microsoft 365 Business Premium** (includes Office apps, Intune, and other services).
2. If not available, at minimum assign:
   - **Office 365 E3/E5** and **Enterprise Mobility + Security E3/E5** (for Intune access).

**Explanation:**  
Licenses must be assigned to activate the services required for the employee, including email, Office applications, and device management capabilities through Intune.

---

## Step 4: Set Usage Location

**Instructions:**

1. Still under the "Add user" setup, set the **Usage location** (e.g., United States).

**Explanation:**  
Microsoft licensing rules require specifying the country where the services will be used. Without a location, licenses cannot be properly assigned.

![image](https://github.com/user-attachments/assets/12d57c8e-8542-42f2-af4f-f3b2fc7e7958)

2. Fill in the user **Profile Info**

![image](https://github.com/user-attachments/assets/be39b575-9e0d-4288-8023-a0fcb70c8932)

---

## Step 5: Save the User Information

**Instructions:**

1. Review the user details.
2. Click **Finish adding**.
3. Save or copy the temporary password for later device setup.

**Explanation:**  
Finalizing the creation process confirms that the new user is now part of the organization's tenant and will be ready for device enrollment.

![image](https://github.com/user-attachments/assets/efe5f5d0-a501-4af5-8a09-9de318d1b501)

---

## Step 6: Prepare the Device for Enrollment

**Instructions:**

1. Power on a new or reset Windows 11 device.
2. Begin the Windows Out-of-Box Experience (OOBE).
3. On the "Let's set things up for work or school" screen, select **Set up for work or school**.
4. Enter the **new user’s Microsoft 365 email address** created earlier.
5. Sign in using the **temporary password**.
6. Prompt the user to set a new password when required.

**Explanation:**  
Using the Microsoft 365 account during device setup binds the device to Azure AD and automatically triggers enrollment into Intune (if Automatic Enrollment is enabled), ensuring the device is secured and managed right from the start.

![image](https://github.com/user-attachments/assets/8786e53d-310d-4dae-9911-b68cea330dfd)
![image](https://github.com/user-attachments/assets/9087d18f-5bca-4924-92d4-68566f7713a4)
![image](https://github.com/user-attachments/assets/3e7c2a0e-30fd-49f8-9980-e81afa1f856c)
![image](https://github.com/user-attachments/assets/5bf6066d-051d-4876-8f2b-6d630d73efab)
![image](https://github.com/user-attachments/assets/88ba093f-8108-47db-a09b-488073d48e5b)

---

## Step 7: Confirm the Device Enrollment in Intune

**Instructions:**

1. After setup completes, log into the device.
2. Go to **Settings** \u2192 **Accounts** \u2192 **Access work or school**.
3. Confirm that the account is listed under **Connected to Azure AD** and **Managed by Intune**.

**Explanation:**  
This verification step ensures that the device has been properly registered with Azure Active Directory and is managed by Intune. Without this, security policies and application deployments will not apply.

---

## Step 8: Confirm the Device Appears in Microsoft Intune Admin Center

**Instructions:**

1. Open a web browser and go to [https://intune.microsoft.com](https://intune.microsoft.com).
2. Sign in using administrator credentials.
3. In the left-hand menu, select **Devices** \u2192 **All Devices**.
4. Search for the newly enrolled user's device.
5. Confirm that the device is listed with a status of **Enrolled**, and check **Compliance** if applicable.

**Explanation:**  
Verification inside Microsoft Intune ensures the device is enrolled correctly. This is critical for automatic policy enforcement, security baselines, and application deployment within the company's mobile device management (MDM) framework.

---

# Conclusion

By following this lab, a new user is successfully onboarded into Microsoft 365, licensed for core services, and a Windows 11 device is enrolled and visible in Microsoft Intune. This process ensures a secure, policy-driven environment from the moment the employee receives their device, minimizing manual IT intervention and maximizing endpoint security and compliance.
