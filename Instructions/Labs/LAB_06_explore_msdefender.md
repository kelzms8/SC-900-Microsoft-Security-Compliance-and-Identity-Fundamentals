
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
    

1. In the blue search bar enter **Microsoft Defender for Cloud**, then from the results list, select **Microsoft Defender for Cloud**.

1. If this is the first time you enter Microsoft Defender for Cloud with your subscription you may land on the Getting started page, and may be prompted to upgrade.  Scroll to the bottom of the page and select **Remind me later** (or **Skip**).  You'll be taken to the Overview page.

1. Click on the **Getting started (1)** from the left pane. Click on the **Upgrade (2)** tab, select your **subscription (3)** and click **Upgrade (4)**.

   > **Note:** If you are not able to see subscription then it means your subscription is already upgraded, in this case you can skip step 2, 3 and continue from step 4.

   ![alt text](https://raw.githubusercontent.com/CloudLabsAI-Azure/AIW-Security-Immersion/main/Labs/Images/get-started-1.png)

   ![alt text](https://raw.githubusercontent.com/CloudLabsAI-Azure/AIW-Security-Immersion/main/Labs/Images/get-started.png)
   
1. Click on **Install agents**. 

   ![alt text](https://raw.githubusercontent.com/CloudLabsAI-Azure/AIW-Security-Immersion/main/Labs/Images/installagents.png)
   
   > **Note:** If the button is greyed out, then it's already set to **On** and agents are already installed in this case you can move on to the next step.

   ![alt text](https://raw.githubusercontent.com/CloudLabsAI-Azure/AIW-Security-Immersion/main/Labs/Images/installagents1.png)
   
1. Return to Microsoft Defender for Cloud blade. Notice the information available on the Security center overview page.  

    ![alt text](https://raw.githubusercontent.com/Azure/Azure-Security-Center/main/Labs/Images/asc-dashboard-overview.gif)

1. Information on the top of the page includes the number of Azure subscriptions, the number of Assessed resources, the number of active recommendations, and any security alerts.  On the main body of the page there are cards representing Secure score, Regulatory compliance, Insights, Azure Defender, and more.  
1. From the top of the page, select **Assessed resources**.  This brings you to the inventory page that shows the resources under the subscription. Select **Resource Type - Virtual Machine**

    ![alt text](https://raw.githubusercontent.com/Ritu786/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/stag/Instructions/Images/T1%20S8.png)

1. The Resource health page provides a list of recommendations.  From the available list, select **Management ports of virtual machine should be protected with just-in-time network access control**. 

    ![alt text](https://raw.githubusercontent.com/Ritu786/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/stag/Instructions/Images/T1%20S9.png)

1. Select the drop-down arrow next to Remediation steps. Note how detailed remediation steps are provided along with the option to take action.  

    ![alt text](https://raw.githubusercontent.com/Ritu786/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/stag/Instructions/Images/T1%20S10.png)

1. Select **Microsoft Defender for Cloud** from the top-left corner of the screen to return to the Microsoft Defender for Cloud overview page.
1. From the top of the page, select **Active recommendations**.

    ![alt text](https://raw.githubusercontent.com/Ritu786/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/stag/Instructions/Images/16.png)

1. The recommendations page shows specific actions that can be taken on their potential secure score increase.  Exit the recommendations page by selecting the **X** on top-right corner of the screen.
1. From the main page, select **Regulatory compliance**.
1. The regulatory compliance page provides a list of compliance controls.  Under each control is a set of assessments that are based on the Azure Security Benchmark which provides recommendations on how you can secure your cloud solutions on Azure.

    ![alt text](https://raw.githubusercontent.com/Ritu786/SC-900-Microsoft-Security-Compliance-and-Identity-Fundamentals/stag/Instructions/Images/17.png)

1. Select the **X** on the top-right corner of the screen to close the page and return to the Security Center Overview page. 
1. Keep the Security center overview page open, you will use in the next task.


###


#### Task 2: In this task you will navigate to Azure Secure score and explore recommendations that can improve your secure score.

> ❗ Important: <br>
> Azure Security Center takes time to populate information such as secure score, compliance, recommendations etc. after enabling the services and enrolling the servers to security center. Sometimes, it can take up to 3 hrs. or even more than that for all the tiles on the overview page to update. if it takes more time, attendees can skip the steps of task 2 & proceed with the Task 3 and can come back later and check on this. We are looking at various approaches to optimize this experience for future workshops.

1. From the Microsoft Defender for Cloud overview page, select the **Secure posture** card.

    ![alt text](https://raw.githubusercontent.com/Azure/Azure-Security-Center/main/Labs/Images/asc-overview-secure-score-tile.gif)
 
1. From the left navigation panel, select **Recommendations**.  (Note that this is equivalent to having selected Active recommendations from the top of the Microsoft Defender for Cloud overview page).

1. Verify,the **All recommendations** tab is selected (underlined).  Note the dashboard view that shows Active recommendations by severity, Resource health, and more.

1. Note that some items show up as unhealthy resources, as depicted by the red bar on the right of the line item.  From the list, select any unhealthy resource.  In the page that opens, you'll see a description, Remediation steps, and affected resources. Exit out this page, by selecting the **X** on top-right corner of the screen.


#### Task 3:  Recall that Security center is offered in two modes: Azure Defender OFF (free) and Azure Defender ON. In this task you discover how to enable and disable Azure Defender.

1. From the Microsoft Defender for Cloud overview page, select the **Environment settings** from the left navigation panel.
1. Select  the **Expand all** box then select the **Subscription--Azure HOL** subscription listed next to the yellow key icon.
1. On the Defender plans page, notice how you can select Enable all or select individual Defender plans. 
    1. Verify that CSPM status is set to **On**, if not, set it now.  
    1. Enable the plan for Servers.  Select **On** for the Servers line item, then select **Save** from the top of the page.
1. Close all the open browser tabs.

### Review

In this lab, you explored Microsoft Defender for Cloud.

