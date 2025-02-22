---
title: 'Tutorial: Azure AD SSO integration with Mail Luck!'
description: Learn how to configure single sign-on between Azure Active Directory and Mail Luck!.
services: active-directory
author: jeevansd
manager: CelesteDG
ms.reviewer: celested
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.topic: tutorial
ms.date: 10/11/2021
ms.author: jeedes
---

# Tutorial: Azure AD SSO integration with Mail Luck!

In this tutorial, you'll learn how to integrate Mail Luck! with Azure Active Directory (Azure AD). When you integrate Mail Luck! with Azure AD, you can:

* Control in Azure AD who has access to Mail Luck!.
* Enable your users to be automatically signed-in to Mail Luck! with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

## Prerequisites

To get started, you need the following items:

* An Azure AD subscription. If you don't have a subscription, you can get a [free account](https://azure.microsoft.com/free/).
* Mail Luck! single sign-on (SSO) enabled subscription.

## Scenario description

In this tutorial, you configure and test Azure AD SSO in a test environment.

* Mail Luck! supports **SP** initiated SSO.

## Add Mail Luck! from the gallery

To configure the integration of Mail Luck! into Azure AD, you need to add Mail Luck! from the gallery to your list of managed SaaS apps.

1. Sign in to the Azure portal using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **Mail Luck!** in the search box.
1. Select **Mail Luck!** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.

## Configure and test Azure AD SSO for Mail Luck!

Configure and test Azure AD SSO with Mail Luck! using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in Mail Luck!.

To configure and test Azure AD SSO with Mail Luck!, perform the following steps:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
    1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with B.Simon.
    1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable B.Simon to use Azure AD single sign-on.
1. **[Configure Mail Luck! SSO](#configure-mail-luck-sso)** - to configure the single sign-on settings on application side.
    1. **[Create Mail Luck! test user](#create-mail-luck-test-user)** - to have a counterpart of B.Simon in Mail Luck! that is linked to the Azure AD representation of user.
1. **[Test SSO](#test-sso)** - to verify whether the configuration works.

## Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the Azure portal, on the **Mail Luck!** application integration page, find the **Manage** section and select **single sign-on**.
1. On the **Select a single sign-on method** page, select **SAML**.
1. On the **Set up single sign-on with SAML** page, click the pencil icon for **Basic SAML Configuration** to edit the settings.

   ![Edit Basic SAML Configuration](common/edit-urls.png)

1. On the **Basic SAML Configuration** section, perform the following steps:

    a. In the **Identifier (Entity ID)** text box, type a URL using the following pattern:
    `https://manage<UNITID>.ml-sgw.jp/<TENANT_NAME>/saml/`

	b. In the **Sign on URL** text box, type a URL using the following pattern:
    `https://manage<UNITID>.ml-sgw.jp/<TENANT_NAME>/saml/sign_in`

	> [!NOTE]
	> These values are not real. Update these values with the actual Identifier and Sign on URL. Contact [Mail Luck! Client support team](https://customer.nttpc.co.jp/cgi-bin/form/inquiry_index.cgi) to get these values. You can also refer to the patterns shown in the **Basic SAML Configuration** section in the Azure portal.

1. On the **Set up single sign-on with SAML** page, In the **SAML Signing Certificate** section, click copy button to copy **App Federation Metadata Url** and save it on your computer.

	![The Certificate download link](common/copy-metadataurl.png)

### Create an Azure AD test user

In this section, you'll create a test user in the Azure portal called B.Simon.

1. From the left pane in the Azure portal, select **Azure Active Directory**, select **Users**, and then select **All users**.
1. Select **New user** at the top of the screen.
1. In the **User** properties, follow these steps:
   1. In the **Name** field, enter `B.Simon`.  
   1. In the **User name** field, enter the username@companydomain.extension. For example, `B.Simon@contoso.com`.
   1. Select the **Show password** check box, and then write down the value that's displayed in the **Password** box.
   1. Click **Create**.

### Assign the Azure AD test user

In this section, you'll enable B.Simon to use Azure single sign-on by granting access to Mail Luck!.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **Mail Luck!**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.
1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.
1. In the **Users and groups** dialog, select **B.Simon** from the Users list, then click the **Select** button at the bottom of the screen.
1. If you're expecting any role value in the SAML assertion, in the **Select Role** dialog, select the appropriate role for the user from the list and then click the **Select** button at the bottom of the screen.
1. In the **Add Assignment** dialog, click the **Assign** button.

## Configure Mail Luck! SSO

To configure single sign-on on **Mail Luck!** side, you need to send the **App Federation Metadata Url** to [Mail Luck! support team](https://customer.nttpc.co.jp/cgi-bin/form/inquiry_index.cgi). They set this setting to have the SAML SSO connection set properly on both sides.

### Create Mail Luck! test user

In this section, you create a user called B.Simon in Mail Luck!. Work with [Mail Luck! support team](https://customer.nttpc.co.jp/cgi-bin/form/inquiry_index.cgi) to add the users in the Mail Luck! platform. Users must be created and activated before you use single sign-on.

## Test SSO

In this section, you test your Azure AD single sign-on configuration with following options. 

* Click on **Test this application** in Azure portal. This will redirect to Mail Luck! Sign-on URL where you can initiate the login flow. 

* Go to Mail Luck! Sign-on URL directly and initiate the login flow from there.

* You can use Microsoft My Apps. When you click the Mail Luck! tile in the My Apps, this will redirect to Mail Luck! Sign-on URL. For more information about the My Apps, see [Introduction to the My Apps](../user-help/my-apps-portal-end-user-access.md).

## Next steps

Once you configure Mail Luck! you can enforce session control, which protects exfiltration and infiltration of your organization’s sensitive data in real time. Session control extends from Conditional Access. [Learn how to enforce session control with Microsoft Defender for Cloud Apps](/cloud-app-security/proxy-deployment-aad).
