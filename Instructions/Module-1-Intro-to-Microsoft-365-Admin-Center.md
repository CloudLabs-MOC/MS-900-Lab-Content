# Module 01: Introduction to Microsoft 365 Admin Center

## Lab Scenario
The Microsoft 365 admin center is where you manage your business in the cloud. You can complete tasks such as adding and removing users, changing licenses, and resetting passwords. Here are the features and settings you'll find in the left-hand navigation of the admin center.
  
   - **Home**: This is the landing page in the admin center. Here you will see where to manage users, billing, service health, and reports.
   
   - **Users**: From here you can create and manage users in your organization, like employees or students. You can also set their permission level or reset their passwords.
   
   - **Groups**: Create and manage groups in your organization, such as a Microsoft 365 group, distribution group, security group, or shared mailbox.
   
   - **Resources**: Create and manage resources, like a SharePoint site collection. 
   
   - **Billing**: View purchase or cancel subscriptions for your organization. View past billing statements or view the number of assigned licenses to individual users.
   
   - **Support**: You can view existing service requests or create new ones.
   
   - **Settings**: Manage global settings for apps like email, sites, and the Office suite. Change your password policy and expiration date. Add and update domain names like contoso.com. Change your organization profile and release preferences. And choose whether partners can access your admin center.
   
   - **Setup**: Manage existing domains, turn on and manage multi-factor authentication, manage admin access, migrate user mailboxes to Office 365, manage feature updates, and help users install their Office apps
   
   - **Reports**: See at a glance how your organization is using Microsoft 365 with detailed reports on email use, Office activations, and more.
   
   - **Health**: View the service health at a glance. You can also check out more details and the service health history.
   
   - **Admin centers**: Open separate admin centers for Exchange, Skype for Business, SharePoint, engage, and Microsoft Entra ID. Each admin center includes all available settings for that service.

## Lab objectives

In this lab, you will complete the following tasks:

+ Exercise 1: Admin Experience for User Management
+ Exercise 2: Explore Microsoft 365 Apps

## Estimated Timing: 90 minutes

## Architecture diagram
![](../Instructions/Lab-Scenario-Preview/media/MS-900-LSP-Mod-1.png)

### Exercise 1: Admin Experience for User Management

In this exercise, you will learn how to create users, assign a license to the users, verify custom domains in the tenant, and see how to access other admin centers.
  
#### Task 1: Admin Experience for User Management

In this task, you will learn how to create and manage users from Microsoft Admin Center.

1. Open a new tab inside the browser, and open [Microsoft 365 admin center](https://admin.microsoft.com) page.

1. On the **Microsoft 365 admin center** page, from the left-hand navigation menu, click on the **Users (1)** drop-down and click on **Active users (2)**. This will display the list of active users.

    ![](Images/MS-900-Users.png)

1. From the left-hand navigation menu, click on the **Teams & Groups** icon and click on **Active teams & groups**. This will display a list of all the groups that are created.

1. Now to create a new user, from the left-hand navigation menu click on **Users (1)** and click on **Active users (2)**, and then select **Add a user (3)** icon.

    ![](Images/MS-900-activeuser.png)

1. In the **Set up the basics** page, fill the following details, and then select **Next (7)**.

   - **First name :** **Odl (1)**

   - **Display Name:** **Odl_User-<inject key="DeploymentID" enableCopy="false"/> (2)**

   - **Username:** **Odl (3)**
     
   - **Automatically create a password**: **unselected (4)**

   - **Password**: **<inject key="AzureAdUserPassword"></inject> (5)**.

   - **Require this user to change their password when they first sign in** : **unselected (6)**

     ![](Images/MS-900-basics.png)

1. In the  **Assign product licenses**  pane, choose your location from the **select location (1)** dropdown. In the licenses section, choose **Assign user a product license (2)** and select **office 365 E5 (3)** license. Click **Next (4)**.

    ![](Images/MS-900-License.png)

1. In the **Optional settings**  pane, leave everything as default and click on **Next**.

    ![](Images/MS-900-Optionalsettings.png)

1. In the **Review and Finish** pane, review the new user&#39;s settings and click on **Finish adding**, then **Close**.

    ![](Images/MS-900-Finishadding.png)
   
1. Verify that the user has been created successfully. 

    ![](Images/MS-900-newuser.png)

    >**Note:** If the newly created user does not appear, try refreshing the page until the user shows up.

#### Task 2: Access other admin centers

In this task, you will learn how to access other admin centers from Microsoft Admin Center.

1. On the **Microsoft 365 admin center** page, from the left-hand navigation pane select **Show all**, under **Admin centers (1)** choose **All Admin centers (2)**. It opens a page with a full list of Office 365 admin centers, including admin centers for Teams, Viva Engage, SharePoint, Power Apps, Power BI, and other services.

    ![](Images/MS-900-Mod-1-(admin).png)
   
    ![](Images/MS-900-Mod-1-(alladmin).png)
   
1. On the admin center page, from the left-hand navigation pane select **Exchange**. This will redirect you to the Exchange admin center page. 

      ![](Images/lab1-t3-img04.png)
      
1. From here you can manage email settings for your organization. In the left-hand menu explore through the options available

     - **Recipients**  - View and manage your mailboxes (both user and shared mailboxes), groups, resource mailboxes, and contacts.

     - **Mail flow**   -  Manage remote domains and accepted domains, add connectors, trace messages and manage alert and alert policies.
     
     - **Migration**   -  Migrate mailboxes in batches.
     
     - **Reports**     -  View reports on mail flow and migration batches.
     
     - **Insights**    -  Use the recommendations to discover trends and/or insights, and take actions to fix issues related to mailbox and mail flow.
     
       ![](Images/lab1-t3-img3.png)

1. Switch back to the **Microsoft 365 admin center** page, select **SharePoint**. This will redirect you to the SharePoint admin center page.

    ![](Images/lab1-t3-img4.png)

1. On the **Welcome to your new home page** pop-up, select **Take the tour**.

1. From here you can manage site collections, list and library permissions, file storage and sharing. Explore through the options available in **SharePoint** admin center.

    ![](Images/lab1-t3-img5.png)

1. In the same way you can access and explore through all other admin centers available.
   
### Exercise 2: Explore Microsoft 365 Apps

In the previous exercise, you learn how to create a user and how to assign an office 365 E5 license. In this exercise, you will explore Office 365 apps.

#### Task 1: Explore Outlook

Microsoft Outlook is an application that is used mainly to send and receive emails. It can also be used to manage various types of personal data including calendar appointments and similar entries, tasks, contacts, and notes.

1. Switch back to the **Microsoft 365 admin center** page, select **App launcher (1)** and under Apps, select **Outlook (2)**.

    ![](Images/MS-900-img-1.png)

1. When prompted enter the username **<inject key="AzureAdUserEmail"></inject>** and password:- **<inject key="AzureAdUserPassword"></inject>**.
   
1. On the outlook page, select **New Mail**  to send a new mail. In the **To, Bcc, and Cc** field **enter the username or email address that you created in the Exercise 1 (1)**. In **Subject (2)**, type the subject of the email message. In the **body (3)** of the email message, type the body of the email message. After typing your message, choose **Send (4)**.
    
    ![](Images/MS-900-outlook.png)
    
   
1. From the left-hand menu select **Calendar**. From here you can create appointments, events, organize meetings and view group schedules.

    ![](Images/lab1-E2t1-img4.png)
    
   
1. Now Select **People**, you can use the People page to view, create, edit, find, and delete contacts. You can use your contacts for your reference and can automatically add them as recipients when you compose an email message.

    ![](Images/lab1-E2t1-img5.png)
    
  1. From the left-hand menu you can explore all other options available. 

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - If you receive a success message, you can proceed to the next task.
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide. 
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

<validation step="b8cf10c9-1cd1-4133-b28c-68cbcfb8b75d" />
   
#### Task 2: Explore OneDrive

OneDrive gives you one place to store, share, and sync your work or school files. As part of your organization's Microsoft 365 subscription, you can save your files in OneDrive and then work with them from almost any device, share files with others, give others permission to edit files and work on them at the same time.

1. Now from App launcher under Apps, from here you can manage all your **files**.
   
    ![](Images/MS-900-img-2.png)

1. Now we will try to create a folder and upload files to it. On the OneDrive page click on **+ Add New (1)** and select the **Folder (2)** option, when prompted provide a name **Demo** for your folder, you can also choose the folder color and click on **Create**.
  
    ![](Images/ms-900.lab1.a.png)
   
    > **Note**: Select **My Files**, if you are not able to see your folder refresh the page.

    > **Note:** Before proceeding to the next step, download this [png](https://www.freepnglogos.com/uploads/email-png/email-logo-communications-brands-and-logotypes-gmail-14.png) file and save it inside the C-drive.

1. From the top navigation bar select, **+ Add New (1)** and select **Files upload (2)**, when prompted select the file(s) that you have downloaded.

    ![](Images/ms-900.lab1.1.png)
   
1. Select the checkbox of the new file that you have uploaded, click on the ellipses **...**, this will display the list of actions that can be performed.

    ![](Images/ellipses.png)
   
1. On the **OneDrive** page select the **checkbox of the file or folder (1)** you want to share by selecting the items. Select **Share (2)** at the top of the page.

    ![](Images/MS-900-share.png)

1. Select **Anyone with the link can edit** to customize the link option. Set the options you want on your link, then select **Apply** when you are done.

    ![](Images/anyone.png)

      - **Anyone**: Gives access to anyone who receives this link, whether they receive it directly from you or forwarded from someone else. This may include people outside of your organization.
      
      - **People in (Your Organization)**: Gives access to anyone in your organization who has the link access to the file.
      
      - **People with existing access**: Provides a link that can be used by people who already have access to the file or folder. It does not change the permissions on the item. Use this if you just want to send a link to somebody who already has access.
      
      - **Specific people**: Gives access only to the people you specify, although other people may already have access. 
      
      - **Allow editing**:  select if you want others to be able to edit the file. Uncheck it if you only want others to be able to view the file.
      
      - **Set expiration date**: The link will only work until the date you set. After that, the link will be invalid, and you will need to create a new link for users requiring access to your file or folder.

     - **Set password**: When a user clicks the link, they will be prompted to enter a password before they can access the file. You will need to provide this password separately to users.
     
        ![](Images/lab1-E2t2-img9.png)
       
1. Once you're back at the main **Share** box enter a name or email of users with whom you intend to share the file, click on **Send**. You can also select **Copy Link** to copy the link to your clipboard and share it.
  
1. You can explore through other options available in the **OneDrive**. 

#### Task 3: Explore engage.

With engage people can openly connect across the organization, from here we can discuss ideas, share and collaborate with others.

1. Select **App launcher**, under **Apps** select **Engage**.

    >**Note:** inside the Apps options, if engage is not listed, then select **Explore all your Apps**, on the apps page search and select **engage**.

    >**Note:** If Welcome to the new Viva Engage! pop-up appears, select **Close**.
 
    ![](Images/MS-900-engage.png)

1. From the left-hand pane, select **Communities**, click on **+ Create a community**, enter a name **Management (1)** for your community. In **Members (2)**  search and select the users that you created in Exercise 1. Based on your requirement choose **Public** or **Private** access by click on **Edit (3)**, after this click on **Create (4)**.

    ![](Images/M1E2T3Step2.101.png)  
   
    > **Note**: if you are not able to see your community refresh the page.

1. On the newly created community page, click on **Discussion**. Type the content that you like to post (you can include gifs, files or any website links based on the requirement). Click on **post**.
  
    ![](Images/MS-900-discussion.png)
   
1. Open an Inprivate window, and switch back to the [Engage account](https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiIxNzA3MTUxMTE0MjQifQ/all) of the user whom you added to the group and verify if the user is added to the newly created group and if the posts are visible, and now close the Inprivate window.

1. Navigate back to the **Engage** page.

1. Explore through other options available in engage.

#### Task 4: Explore Microsoft Stream

Microsoft Stream is an Enterprise Video service where people in your organization can upload, view, and share videos securely. You can share recordings of classes, meetings, presentations, training sessions, or other videos that aid your team's collaboration.

1. Select **App launcher**, inside the Apps options, select **Explore all your Apps**, on the apps page search and select **Stream**.

    >**Note:** If **Stream** is not present, then copy and paste this link **https://www.microsoft.com/en-in/microsoft-365/microsoft-stream**, on the **Microsoft Stream** page, select **Sign in**. When prompted enter the username **<inject key="AzureAdUserEmail"></inject>** and password:- **<inject key="AzureAdUserPassword"></inject>**.

1. Before proceeding to the next step, open an another tab, and navigate to this [link](https://www.pexels.com/video/the-sun-illuminating-earth-s-surface-1851190/) and select **Free download** to download this video

1. On the Stream page, select the **Upload** button, and select the file that you have downloaded. Select **Upload** on **Upload to** pop-up.
   
    ![](Images/MS-900-upload.png)

1. It will show you the **Upload complete** pop-up, select **Open**. It will redirect you to the new-browser.

1. Now, click on **Share (1)** button, and again select **Share (2)**.

    ![](Images/MS-900-share1.png)
 
 1. Select **Anyone with the link can edit.**, now select **People you choose (1)** and click on **Apply (2)**, then enter the Username of the user that you created in Exercise 1, and click on **Send**.

    ![](Images/MS-900people.png)
   
1. Open a New InPrivate window and log in to the [Outlook](https://outlook.office.com/mail) with the username on which you have sent the email, now check you have received an email after that click **open** it will open the video that you have shared it from the user you created.

    ![](Images/MS-900-email.png)

1. Close the InPrivate window, and navigate back to the **Microsoft 365 admin center** page.

1. You can explore other options available in Microsoft Stream.

1. To learn more about Microsoft Stream refer to https://docs.microsoft.com/en-us/stream/overview.

#### Task 5: Explore SharePoint

Microsoft SharePoint helps organizations share and manage content, knowledge, and applications to Empower teamwork, quickly find information and seamlessly collaborate across the organization.

1. Select **App launcher**, inside the Apps options, select **SharePoint**.

    >**Note:** If SharePoint is not listed, then select **Explore all your Apps**, on the apps page search and select **SharePoint**.

    >**Note:** On the **News from sites** page, select **Close**.

1. From the top of the SharePoint page, click **+ Create site (1)**  option. A site creation wizard will appear on the right-hand side of the screen. Based on your requirement you can select **Team site** or **Communication site**. For now, select **Team site (2)**. On the **Select a template** page, select any template of your choice and select **Use template**.
   
    ![](Images/img36.png)
   
    - Provide a name for your site:- **Sales-Demo**
    
    - Select **Next**.

    - In the Privacy settings section, choose either **Public - anyone in the organization can access this site** or **Private - only members can access this site** to control who has access to your site.

    -  Select a language for your site and click on **Create site**
    
    - Under **Add members** box, enter the name or email address of the user that you created in Exercise 1 and then click **Finish**.  

        >**Note:** Close **Next steps** pop-up.
    
1. Now let us add and publish a page on the newly created site.

1. On the home page of the site click on **+ New (1)**, and then select **Page (2)**.

    ![](Images/MS-900-salesdemo.png)

    >**Note:** if the **Welcome!** page appears, select **Close**.

1. Choose a page template to start with. For now, you can select **Blank (1)** template and click on **Create page (2)**.

    ![](Images/ms-900-blank.png)

1. Add a page name as **Sales** in the title area. You can customize the title area with an image, a choice of four layouts, text above the title, the ability to change the displayed author, and you can show or hide the published date.

1. Select **Edit web part (1)** icon from here you can select the **layout (2)** of your choice, Set **alignment (3)**, Add text above the title.
  
    ![](Images/ms-900-sales.png)

1. To add an image click on **Browse image** button in the toolbar on the left. 

    ![](Images/Ms-900-browseimage.png)

1. Choose a recent image or get an image from a web search, your site, your computer, or a link. If your organization has specified a set of approved images, you'll be able to choose from that set under Your organization. 

1. You can also add a new section, by clicking on **+** to add content.

1. When done, click **Publish**. This will publish a page on your site.

1. To learn more about SharePoint refer to https://docs.microsoft.com/en-us/sharepoint/introduction.

#### Task 6: Explore Lists

List helps to track information and organize your work. With a list, one can track issues, assets, routines, contacts, inventory and more using customizable views and smart rules and alerts to keep everyone in sync.

1. From the  **App launcher**, under the **Apps** section, select **Explore all your Apps**, on the apps page search and select **Lists**, On **Welcome to Lists** page, select **Close**. 

1. On the home page of **Lists** click on **+ New list**. 

    ![](Images/MS-900-lists.png)

1. From the Create a list page, select **+ Blank list**. 
 
    - Provide a name **Assets (1)** for your list and if needed provide a description.
    
    - Choose a **colour (2)** and icon for your list.
    
    - In **Save to (3)** select a location where you want your list to be saved. Click on **Create (4)**
   
     ![](Images/MS-900-lists-1.png)
    
 1. When your list opens, to add an item to your list, select **+ Add new item**. 
   
     ![](Images/MS-900-addnewitem.png)
 
 1. Under **Title** provide a name for your new item, if needed you can also add attachments. Once done click on **Save**.
 
 1. To add a column, select **+ Add column (1)**. In the dropdown, select the **type of column (2)** you want, and select **Next (3)**.
 
    ![](Images/MS-900-addcolumn.png)
 
 1. In the Create a column panel, in the **Name** field, enter a title or column heading. Enter any other required information. The number of fields will vary with the column type you choose. The above example is for a **Multiple lines of text** field.
 
    ![](Images/img166.png)

1. Select **Save**. In this way, you can add multiple items and columns to your list.

1. To rename a column, select the **column (1)** which you want to rename select **Column settings (2)** and select **Rename (3)**. When prompted provide column name and select **Save**.

    ![](Images/MS-900-rename.png)

1. Now select the item which you have added click on **Show actions (1)** and select **Edit (2)**  from here you can add value against the newly created column, select **Edit all** if you want to edit anything, and select **Save**.

    ![](Images/MS-900-demo.png)

1. To share your list select **Share** near the top of the page.

    ![](Images/MS-900-Share12.png)
    
1. Enter a name or email address of the user that you created in Exercise 1. To change the access permissions, you are granting to people, select **Can edit list** drop-down, then select an option based on requirement, and select **Apply** . 

    ![](Images/MS-900-canedit.png)

1. Select the ellipse **(...) (1)** icon, select **Manage my alerts (2)**.

    ![](Images/MS-900-managealerts.png)

1. Select **Add Alert**.

    ![](Images/img03.png)

1. On **My Alerts on this Site > New Alert** , select the checkbox of your document, and select **Next**.
    
    ![](Images/img04.png)

1. Select a delivery method, choose the types of changes that you want to be notified about, how frequently you want to receive the alert. Once done select **Ok**.

1. Depending on how your site and servers are set up, whenever changes are made the person you created an alert for will be notified.

1. You can explore other options available in Microsoft List.

## Review

Throughout this module, you've gained the knowledge of generating users, allocating licenses through the Microsoft 365 admin center, and acquired the skills to access different admin centers. Additionally, you've navigated and explored various Office 365 applications.

## You have successfully completed the lab.

