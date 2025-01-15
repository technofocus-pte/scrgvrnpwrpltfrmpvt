# **Lab 1: Creating and managing environments using Power Platform Admin Center**

An environment is a space to store, manage, and share your
organization's business data, apps, and flows. It also serves as a
container to separate apps that may have different roles, security
requirements, or target audiences. Power Apps automatically creates a
single default environment for each tenant, which is shared by all users
in that tenant.

### **Task 1: Setting an environment refresh Cadence**

You can indicate how often you would prefer an environment to receive
updates and features to certain Microsoft Power Platform services. You
have two options to choose from after creating an environment.

[TABLE]
Service	               Setting	         Description
Canvas app authoring   Frequent	    Get access the latest updates and newest features multiple times a month.
	                   Moderate	    Get access to updates and features at least once a month.


To set refresh cadence:

1.  Browse to the Power Platform Admin Center
    at +++**https://admin.powerplatform.microsoft.com**+++ and
    sign in with your Office 365 tenant credentials. 

2.  From left navigation pane, select **Manage** > **Environments** and
    then click on the **Dev One** environment.

     ![](./media/image1.png)

3.  Click on **Edit** in details section.

     ![](./media/image2.png)

4.  Under **Refresh cadence**, choose the **cadence** type –
    **Frequent** and then click on **Save** button.

     ![](./media/image3.png)
    
> **Note:**

- By default, environments are automatically in
  the **frequent** cadence; creating and editing canvas apps will
  receive updates once a week. When apps are published, they will
  receive the corresponding runtime version.

- If you've chosen the **moderate** cadence for the environment, all
  creating and editing of canvas apps will receive updates once a month.
  When apps are published, they will receive the corresponding runtime
  version.

### **Task 2: Control who can create and manage environments in the Power Platform Admin Center**

1.  Select the **Gear** icon ![Screenshot](./media/image4.png) in the
    upper-right corner of the **Microsoft Power Platform** site.

     ![A screenshot of a computer Description automatically generated](./media/image5.png)

2.  Select **Power Platform settings**.

     ![A screenshot of a computer Description automatically generated](./media/image6.png)

3.  Select **Add-on capacity assignments.** 

     ![](./media/image7.png)

4.  Select **Only specific admins** and click **Save.**

     ![A screenshot of a computer Description automatically generated](./media/image8.png)

### **Task 3: Administration mode**

You can set a sandbox, production, or trial (subscription-based)
environment in administration mode so that only users with System
Administrator or System Customizer security roles will be able to sign
in to that environment. Administration mode is useful when you want to
make operational changes and not have regular users affect your work,
and not have your work affect end users (non-admins)

1.  From the left-side menu, select **Manage** > **Environments**, and
    then select your **Dev One** environment.

     ![](./media/image1.png)

2.  On the **Details** page, click on **Edit**.

     ![A screenshot of a computer Description automatically generated](./media/image2.png)

3.  Under **Administration mode**, toggle **Disabled** to **Enabled**
    and then select **Save**.

     ![A screenshot of a computer Description automatically generated](./media/image9.png)

4.  On the **Details** page, click on **Edit**. Disable Administrative
    mode and **Save** it.

     ![A screenshot of a computer Description automatically generated](./media/image10.png)

### **Task 4 - Create a new custom security role that only has access to "Security Role" table**

1.  Open a new tab and navigate
    to +++**https://make.powerapps.com**+++ . If
    required, sign in with your Office 365 tenant credentials.

2.  Select your **Dev One** environment.

     ![A screenshot of a computer Description automatically generated](./media/image11.png)

3.  Select your environment and click on **Settings** > **Advanced
    Settings**.

     ![A screenshot of a computer Description automatically generated](./media/image12.png)

4.  **Dynamics 365** opens in separate tab. Click on **Settings \>
    Options.**

     ![A screenshot of a computer Description automatically generated](./media/image13.png)

5.  In the **General** tab, scroll down to the bottom and select
    the **user information** link.

     ![](./media/image14.png)

6.  On the user information page select the different tabs, such
    as **Summary**, **Details**, or **Administration** to see details
    about your profile.

     ![](./media/image15.png)

7.  Go back to **Power Platform Admin Center** tab and click on your
    environment and then click on **Settings** on top menu bar.

     ![A screenshot of a computer Description automatically generated](./media/image16.png)

8.  Click on **Users + permissions > Security roles**.

     ![A screenshot of a computer Description automatically generated](./media/image17.png)

9.  Click on **New role**.

     ![A screenshot of a computer Description automatically generated](./media/image18.png)

10. In the **Role Name** field, enter a name for the new role -
    **Security update**. In the **Business unit** field, select the
    business unit the role belongs to. Select **Save**.

    ![A screenshot of a computer Description automaticallygenerated](./media/image19.png)

11. Scroll down to the **Table** list and set the **Security
    Role** table privileges as follows. Click on **Save and
    Close** button

[TABLE]
    ![A screenshot of a computer Description automatically generated](./media/image20.png)

### **Task 5: Assign the new security role to an administrative user**

1.  Click on **Settings** on top navigation.

     ![A screenshot of a computer Description automatically generated](./media/image21.png)

2.  Click on **Users + permissions - \> Users**.

     ![A screenshot of a computer Description automatically generated](./media/image22.png)

3.  Select an administrative user - **MOD Administrator** and then
    choose **Manage Security roles**.

     ![A screenshot of a computer Description automatically generated](./media/image23.png)

4.  Select the new security role which was created above and
    then **Save** it.

     ![A screenshot of a computer Description automatically generated](./media/image24.png)

5.  Click on **Save** to confirm the role assignment.

     ![A screenshot of a computer error Description automatically generated](./media/image25.png)
