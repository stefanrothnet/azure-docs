﻿---
title: 'Tutorial: Azure Active Directory integration with Evidence.com | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and Evidence.com.
services: active-directory
documentationCenter: na
author: jeevansd
manager: mtillman
ms.reviewer: joflore

ms.assetid: f9a7cb7c-ff67-40dc-872c-1fa35f9dd03b
ms.service: active-directory
ms.component: saas-app-tutorial
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 07/25/2017
ms.author: jeedes

---
# Tutorial: Azure Active Directory integration with Evidence.com

In this tutorial, you learn how to integrate Evidence.com with Azure Active Directory (Azure AD).

Integrating Evidence.com with Azure AD provides you with the following benefits:

- You can control in Azure AD who has access to Evidence.com.
- You can enable your users to automatically get signed-on to Evidence.com (Single Sign-On) with their Azure AD accounts.
- You can manage your accounts in one central location - the Azure portal.

If you want to know more details about SaaS app integration with Azure AD, see [what is application access and single sign-on with Azure Active Directory](../manage-apps/what-is-single-sign-on.md).

## Prerequisites

To configure Azure AD integration with Evidence.com, you need the following items:

- An Azure AD subscription
- A Evidence.com single sign-on enabled subscription

> [!NOTE]
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

## Scenario description
In this tutorial, you test Azure AD single sign-on in a test environment. 
The scenario outlined in this tutorial consists of two main building blocks:

1. Adding Evidence.com from the gallery
1. Configuring and testing Azure AD single sign-on

## Adding Evidence.com from the gallery
To configure the integration of Evidence.com into Azure AD, you need to add Evidence.com from the gallery to your list of managed SaaS apps.

**To add Evidence.com from the gallery, perform the following steps:**

1. In the **[Azure portal](https://portal.azure.com)**, on the left navigation panel, click **Azure Active Directory** icon. 

	![The Azure Active Directory button][1]

1. Navigate to **Enterprise applications**. Then go to **All applications**.

	![The Enterprise applications blade][2]
	
1. To add new application, click **New application** button on the top of dialog.

	![The New application button][3]

1. In the search box, type **Evidence.com**, select **Evidence.com** from result panel then click **Add** button to add the application.

	![Evidence.com in the results list](./media/evidence-tutorial/tutorial_evidence.com_addfromgallery.png)

## Configure and test Azure AD single sign-on

In this section, you configure and test Azure AD single sign-on with Evidence.com based on a test user called "Britta Simon".

For single sign-on to work, Azure AD needs to know what the counterpart user in Evidence.com is to a user in Azure AD. In other words, a link relationship between an Azure AD user and the related user in Evidence.com needs to be established.

In Evidence.com, assign the value of the **user name** in Azure AD as the value of the **Username** to establish the link relationship.

To configure and test Azure AD single sign-on with Evidence.com, you need to complete the following building blocks:

1. **[Configure Azure AD Single Sign-On](#configure-azure-ad-single-sign-on)** - to enable your users to use this feature.
1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with Britta Simon.
1. **[Create a Evidence.com test user](#create-a-evidencecom-test-user)** - to have a counterpart of Britta Simon in Evidence.com that is linked to the Azure AD representation of user.
1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable Britta Simon to use Azure AD single sign-on.
1. **[Test single sign-on](#test-single-sign-on)** - to verify whether the configuration works.

### Configure Azure AD single sign-on

In this section, you enable Azure AD single sign-on in the Azure portal and configure single sign-on in your Evidence.com application.

**To configure Azure AD single sign-on with Evidence.com, perform the following steps:**

1. In the Azure portal, on the **Evidence.com** application integration page, click **Single sign-on**.

	![Configure single sign-on link][4]

1. On the **Single sign-on** dialog, select **Mode** as	**SAML-based Sign-on** to enable single sign-on.
 
	![Single sign-on dialog box](./media/evidence-tutorial/tutorial_evidence.com_samlbase.png)

1. On the **Evidence.com Domain and URLs** section, perform the following steps:

	![Evidence.com Domain and URLs single sign-on information](./media/evidence-tutorial/tutorial_evidence.com_url.png)

    a. In the **Sign-on URL** textbox, type a URL using the following pattern: `https://<yourtenant>.evidence.com`

	b. In the **Identifier** textbox, type a URL using the following pattern: `https://<yourtenant>.evidence.com`

	> [!NOTE] 
	> These values are not real. Update these values with the actual Sign-On URL and Identifier. Contact [Evidence.com Client support team](https://communities.taser.com/support/SupportContactUs?typ=LE) to get these values. 

1. On the **SAML Signing Certificate** section, click **Certificate(Base64)** and then save the certificate file on your computer.

	![The Certificate download link](./media/evidence-tutorial/tutorial_evidence.com_certificate.png) 

1. Click **Save** button.

	![Configure Single Sign-On Save button](./media/evidence-tutorial/tutorial_general_400.png)

1. On the **Evidence.com Configuration** section, click **Configure Evidence.com** to open **Configure sign-on** window. Copy the **Sign-Out URL, SAML Entity ID, and SAML Single Sign-On Service URL** from the **Quick Reference section.**

	![Evidence.com Configuration](./media/evidence-tutorial/tutorial_evidence.com_configure.png) 

1. In a separate web browser window, login to your Evidence.com tenant as an administrator and navigate to **Admin** Tab

1. Click on **Agency Single Sign On**

1. Select **SAML Based Single Sign On**

1. Copy the **SAML Entity ID**, **SAML Single Sign-On Service URL** and **Sign-Out URL** values shown in the Azure portal and to the corresponding fields in Evidence.com.

1. Open your downloaded Certificate(Base64) file in notepad, copy the content of it into your clipboard, and then paste it to the **Security Certificate** box. 

1. Save the configuration in Evidence.com.

> [!TIP]
> You can now read a concise version of these instructions inside the [Azure portal](https://portal.azure.com), while you are setting up the app!  After adding this app from the **Active Directory > Enterprise Applications** section, simply click the **Single Sign-On** tab and access the embedded documentation through the **Configuration** section at the bottom. You can read more about the embedded documentation feature here: [Azure AD embedded documentation]( https://go.microsoft.com/fwlink/?linkid=845985)
> 

### Create an Azure AD test user

The objective of this section is to create a test user in the Azure portal called Britta Simon.

   ![Create an Azure AD test user][100]

**To create a test user in Azure AD, perform the following steps:**

1. In the Azure portal, in the left pane, click the **Azure Active Directory** button.

    ![The Azure Active Directory button](./media/evidence-tutorial/create_aaduser_01.png)

1. To display the list of users, go to **Users and groups**, and then click **All users**.

    ![The "Users and groups" and "All users" links](./media/evidence-tutorial/create_aaduser_02.png)

1. To open the **User** dialog box, click **Add** at the top of the **All Users** dialog box.

    ![The Add button](./media/evidence-tutorial/create_aaduser_03.png)

1. In the **User** dialog box, perform the following steps:

    ![The User dialog box](./media/evidence-tutorial/create_aaduser_04.png)

    a. In the **Name** box, type **BrittaSimon**.

    b. In the **User name** box, type the email address of user Britta Simon.

    c. Select the **Show Password** check box, and then write down the value that's displayed in the **Password** box.

    d. Click **Create**.
 
### Create a Evidence.com test user

For Azure AD users to be able to sign in, they must be provisioned for access inside the Evidence.com application. This section describes how to create Azure AD user accounts inside Evidence.com

**To provision a user account in Evidence.com:**

1. In a web browser window, log into your Evidence.com company site as an administrator.

1. Navigate to **Admin** tab.

1. Click on **Add User**.

1. Click the **Add** button.

1. The **Email Address** of the added user must match the username of the users in Azure AD who you wish to give access. If the username and email address are not the same value in your organization, you can use the **Evidence.com > Attributes > Single Sign-On** section of the Azure portal to change the nameidenitifer sent to Evidence.com to be the email address.

### Assign the Azure AD test user

In this section, you enable Britta Simon to use Azure single sign-on by granting access to Evidence.com.

![Assign the user role][200] 

**To assign Britta Simon to Evidence.com, perform the following steps:**

1. In the Azure portal, open the applications view, and then navigate to the directory view and go to **Enterprise applications** then click **All applications**.

	![Assign User][201] 

1. In the applications list, select **Evidence.com**.

	![The Evidence.com link in the Applications list](./media/evidence-tutorial/tutorial_evidence.com_app.png)  

1. In the menu on the left, click **Users and groups**.

	![The "Users and groups" link][202]

1. Click **Add** button. Then select **Users and groups** on **Add Assignment** dialog.

	![The Add Assignment pane][203]

1. On **Users and groups** dialog, select **Britta Simon** in the Users list.

1. Click **Select** button on **Users and groups** dialog.

1. Click **Assign** button on **Add Assignment** dialog.
	
### Test single sign-on

In this section, you test your Azure AD single sign-on configuration using the Access Panel.

When you click the Evidence.com tile in the Access Panel, you should get automatically signed-on to your Evidence.com application.
For more information about the Access Panel, see [Introduction to the Access Panel](../user-help/active-directory-saas-access-panel-introduction.md). 

## Additional resources

* [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](tutorial-list.md)
* [What is application access and single sign-on with Azure Active Directory?](../manage-apps/what-is-single-sign-on.md)

<!--Image references-->

[1]: ./media/evidence-tutorial/tutorial_general_01.png
[2]: ./media/evidence-tutorial/tutorial_general_02.png
[3]: ./media/evidence-tutorial/tutorial_general_03.png
[4]: ./media/evidence-tutorial/tutorial_general_04.png

[100]: ./media/evidence-tutorial/tutorial_general_100.png

[200]: ./media/evidence-tutorial/tutorial_general_200.png
[201]: ./media/evidence-tutorial/tutorial_general_201.png
[202]: ./media/evidence-tutorial/tutorial_general_202.png
[203]: ./media/evidence-tutorial/tutorial_general_203.png

