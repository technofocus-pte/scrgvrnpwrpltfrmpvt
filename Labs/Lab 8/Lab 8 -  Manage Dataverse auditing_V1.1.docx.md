# **Lab 8: Manage Dataverse auditing**

## Exercise 1: Manage Dataverse auditing

### **Task 1: Start/stop auditing for an environment and set retention policy**

1.  Sign in to the Power Platform admin center using
    **[https://admin.powerplatform.microsoft.com](urn:gd:lg:a:send-vm-keys)**
    with your Office 365 admin tenant credentials.

2.  Select **Manage \>** **Environments** from left navigation.

> ![A screenshot of a computer Description automatically
> generated](./media/image1.png)

3.  Select **Dev One** environment and then select More commands (three
    dots) from above horizontal palette and then select **Settings**.

> ![](./media/image2.png)

4.  Expand **Audit and logs** \> **Audit settings**.

> ![A screenshot of a computer Description automatically
> generated](./media/image3.png)

5.  Select **Start auditing** and **Read log** checkbox. Set the
    retention policy for the logs as **90 days**. Select **Save**.

> ![A screenshot of a computer Description automatically
> generated](./media/image4.png)

[TABLE]

> **Note:** When the audit retention period is set to Forever, logs will
> never be deleted.

6.  You have completed this task, please do not close the browser.
    Proceed ahead with the next task.

### **Task 2: Configure auditing for one or more tables and columns in Power Apps**

1.  Go to **Power Apps** portal
    using [https://make.powerapps.com](https://make.powerapps.com/) and
    sign in with your given Office 365 Admin tenant credentials.

2.  Click on the environment selector and select **Dev One** environment
    that contains a Dataverse database.

> ![A screenshot of a computer Description automatically
> generated](./media/image5.png)

3.  Select Tables from left navigation pane and then click to open
    the **Expense Report** Table.

> ![A screenshot of a computer Description automatically
> generated](./media/image6.png)

4.  Select **Columns** under Schema.

> ![A screenshot of a computer Description automatically
> generated](./media/image7.png)

5.  Locate and click to open the **Expense Report** column.

> ![A screenshot of a computer Description automatically
> generated](./media/image8.png)

6.  Expand the **Advanced options** section. Select the** Enable
    auditing **checkbox and then click on **Save**.

> ![](./media/image9.png)

7.  To go back to Expense Report, select **Expense Report** from the
    path.

> ![](./media/image10.png)

8.  Select **Edit** from the command bar.

> ![A screenshot of a computer Description automatically
> generated](./media/image11.png)

9.  On the command bar, select **Edit table properties**.

> ![A screenshot of a computer Description automatically
> generated](./media/image12.png)

10. Expand **Advanced options**.

> ![](./media/image13.png)

11. Select the **Audit changes to its data** checkbox. Select **Save**.

> ![A screenshot of a computer Description automatically
> generated](./media/image14.png)

12. Select back arrow to go back to the

> ![A screenshot of a computer Description automatically
> generated](./media/image15.png)

13. Select **Advanced** from the command bar and then select **Publish
    table**.

> ![A screenshot of a computer Description automatically
> generated](./media/image16.png)

14. Wait till you see the message as **Publish succeeded**.

> ![A screenshot of a computer Description automatically
> generated](./media/image17.png)

### **Task 3: Test auditing**

1.  Select **Apps** and click to launch the **Expense Tracker
    app** application.

> ![A screenshot of a computer Description automatically
> generated](./media/image18.png)

2.  You can see, you are in the Expense Reports tab, select **Client
    Visit** report.

> ![A screenshot of a computer Description automatically
> generated](./media/image19.png)

3.  Change the name **Client visit** to **Test visit** and then select
    **Save**.

> ![A screenshot of a computer Description automatically
> generated](./media/image20.png)

4.  Click **Related** and select **Audit History**.

> ![A screenshot of a computer Description automatically
> generated](./media/image21.png)

5.  You should see the change history for each of your changes.

> ![](./media/image22.png)
