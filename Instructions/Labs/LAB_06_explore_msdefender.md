
# Lab: Explore Microsoft Defender for Cloud

## Lab scenario
In this lab, you will explore Microsoft Defender for Cloud and learn how Azure Secure Score can be used to improve your organization's security posture.

  

**Estimated Time**: 10-15 minutes

#### Task 1: In this task you will take a brief tour of Microsoft Defender for Cloud.
1.	Open Microsoft Edge. In the address bar enter **portal.azure.com**.

1. Sign in with your admin credentials.
    
    1. In the Sign in window enter **odl_user_XXXXXX@cloudlabsai.com** (where XXXXXX is your unique ID provided on the lab environment page) then select **Next**.    
    1. Enter the admin password which should be provided on the lab environment page. Select **Sign in**.
    1. When prompted to stay signed- in, select **Yes**.
    

1. On the top left corner of the screen, next to where it says Microsoft Azure, select the Show portal menu icon (the three horizontal lines also referred to as hamburger icon) then from the left navigation panel, under Favorites, select **Microsoft Defender for Cloud**.  If it is not listed under favorites, then in the search box, enter **Microsoft Defender for Cloud**, then from the results list, select **Microsoft Defender for Cloud**.

1. Notice the information available on the Microsoft Defender for Cloud overview page.  

1. You may see a blue information box on the top of the page indicating that you may be viewing limited information.  Select **click here**.
    1. To ensure that you get tenant wide visibility, assign yourself the necessary role.  Select **Security Admin** then select **Get access** at the bottom of the page.
    1. You will likely see the message; Root management group dos not exist.  Per the description, the system will create the group for you.  It can take up to 15 minutes to complete (but usually happens faster).  Once the access is granted select **Microsoft Defender for Cloud** on the top-left corner of the page, above where it says Get permissions and then refresh the Microsoft Defender for Cloud overview page.

1. Information on the top of the page includes the number of Azure subscriptions, the number of Assessed resources, the number of active recommendations, and any security alerts.  On the main body of the page there are cards representing Secure score, Regulatory compliance, Insights, and more.  

1. From the top of the page, select **Assessed resources**.  (Note that this is equivalent to having selected Inventory from the left navigation panel of the Microsoft Defender for Cloud home page).
    1. This brings you to the **Inventory** page that shows your Azure pass subscription.  Select **Azure Pass – Sponsorship**.
    1. The Resource health page provides a list of recommendations.  From the available list, select **There should be more than one owner assigned to your subscription**.
    1. Select the drop-down arrow next to Remediation steps. Note how detailed remediation steps are provided along with the option to take action.  
    1. Select **Microsoft Defender for Cloud** from the top-left corner of the screen to return to the Microsoft Defender for Cloud overview page.

1. From the top of the page, select **Active recommendations**.  (Note that this is equivalent to having selected Recommendations from the left navigation panel of the Microsoft Defender for Cloud home page).
    1. The recommendations page shows your Secure Score dashboard.
    1. Below the Secure Score dashboard are a list of controls. Each security control represents a security risk that should be mitigated and also includes information on the maximum score associated with that control, the current score, potential score increase, and resource health status.  
    1. Select one of the controls, such as **Enable MFA**.  Select one of the sub-items, such as **MFA should be enabled on accounts with owner permissions on your subscription**.  In the page that opens, you will see a description, Remediation steps, and affected resources. Exit out this page, by selecting the **X** on top-right corner of the screen.
    1. Exit the recommendations page by selecting the **X** on top-right corner of the screen, to return to the overview page.

1. From the main page, select **Regulatory compliance**. The regulatory compliance page provides a list of compliance controls.  Under each control is a set of assessments that are based on the Azure Security Benchmark which provides recommendations on how you can secure your cloud solutions on Azure.
    1. Select **IM. Identity Management** then select **IM-6 Use strong authentication controls**.  The list shows customer responsibility actions that can be taken to improve compliance posture.
    1. Select the **X** on the top-right corner of the screen to close the page and return to the Microsoft Defender for Cloud Overview page. 
    1. Keep the Microsoft Defender for Cloud overview page open, you will use in the next task.



#### Task 2: In this task you will navigate to Azure Secure score and explore recommendations that can improve your secure score.

> ❗ Important: <br>
> Azure Security Center takes time to populate information such as secure score, compliance, recommendations etc. after enabling the services and enrolling the servers to security center. Sometimes, it can take up to 3 hrs. or even more than that for all the tiles on the overview page to update. if it takes more time, attendees can skip the steps of task 2 & proceed with the Task 3 and can come back later and check on this. We are looking at various approaches to optimize this experience for future workshops.

1. From the Security center overview page, select the **Secure Score** card.

    ![alt text](https://raw.githubusercontent.com/Azure/Azure-Security-Center/main/Labs/Images/asc-overview-secure-score-tile.gif)
    
2. From the recommendations page, select **Manage access and permissions**. Notice that there is one item in that group that is red.
3. Select the item **There should be more than one owner assigned to your subscription**, which shows the resource health status as red. If selecting selecting this item does not work.
    1. From the top-left corner of the page, select **Security Center**, above where it says Recommendations.    
    1. From the left navigation panel, select **Recommendations**.
    1. From the recommendations page, select **Manage access and permissions**. Notice that there is one item in that group that is red.
    1. Select the item **There should be more than one owner assigned to your subscription**, which shows the resource health status as red. 
4. Select the **Azure subscription**.
5. From the top of the Access control (IAM) page, select **+ Add** then from the drop down select **Add role assignment**.
6. In the Role field, enter **Owner**, then select **Owner** from the list below.
7. From the user list, select **odl_user_XXXXXX@cloudlabsai.com**,(where XXXXXX is the unique ID which provided on the environment page) then select **Save** on the bottom of the page.
8. It can take up to 24 hours for the status to be updated, after which your secure score will also be updated as all the items in the Manage access and permissions group are satisfied.
9. From the top-left corner of the page, above where is says Azure Pass, select **Security Center** then select **Overview** to return the security center overview page.
10. Keep this page open for the subsequent task.


#### Task 3:  Recall that Security center is offered in two modes: Azure Defender OFF (free) and Azure Defender ON. In this task you discover how to enable and disable Azure Defender.

1.	From the Security center overview page, select the **Enable Azure Defender** from the Azure Defender card.

2.	Select the **Azure Defender on** box.  Notice how all the defender plans change status to On and notice pricing for reach item, then select **Save** from the top-left corner of the page.
3.	Return to the Security center page, by selecting **Security Center** from the top-left corner of the page.   It may take several minutes for the Azure Defender card to reflect the change.  Refresh the page, if necessary.
4.	To disable Azure Defender, select **Pricing & settings** from the left navigation panel of the security center page, select the **CloudLabsai subscription**.

    ![alt text](https://raw.githubusercontent.com/CloudLabs-MOC/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/prod/Instructions/Images/6-1.png)

5.	From the Azure Defender plans page, select the **Azure Defender off** box, then select **Save** from the top-left corner of the page.

    ![alt text](https://raw.githubusercontent.com/CloudLabs-MOC/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/prod/Instructions/Images/6-2.png)

6.	A pop-up window appears requesting confirmation of the downgrade.  Uncheck the box for Microsoft to contact you and select **Confirm**.
7.	You can now close the browser tab to exit the Azure portal.


#### Review
In this lab, you explored Azure Security Center and learned how Azure Secure Score can be used to improve your organization's security posture.
