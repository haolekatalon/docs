---
title: "Enable Single Sign-On (SSO) for an Organization"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-analytics/docs/sso-settings.html
redirect_from:
    - "/katalon-analytics/docs/accept-sso/"
---

> Requirements:
>
> You need to subscribe to Katalon TestOps Enterprise plan. To request a trial of Katalon TestOps Enterprise, see [TestOps Trial Plans](https://docs.katalon.com/katalon-analytics/docs/trial-plans.html).

## Configure Single Sign-On

> Requirements:
>
> * You must be an **Owner** or **Admin** of an Organization.
>
> * You have configured a Subdomain. See [Configure a Subdomain for an Organization](https://docs.katalon.com/katalon-analytics/docs/subdomain.html).
>
> * You have configured Identity Provider. Your metadata is then automatically encrypted in Katalon's database.

As an Owner or Admin, you can configure SSO by following these steps:

1. Sign in to [Katalon TestOps](https://testops.katalon.io/login).

2. Go to **Settings** > **Organization Management**.

3. Select **Settings** on the left bar, and scroll down to the **Single Sign-On (SSO) Settings** section.

4. Switch **Enable SSO** to **Active**.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/enter-metadata-for-sso.png" width=100% alt="SSO enabled input metadata">

    You then can enter your Metadata.

5. Click **Update**.

## Enable SSO for new members and existing members

After configuring SSO, you can enable SSO for new members when inviting them to your Organization.

You can also enable SSO for the existing members of your Organization.

### For a new User

To enable SSO for a new member, follow these steps:

1. Invite a User to your Organization. See [TestOps User Management](https://docs.katalon.com/katalon-analytics/docs/kt_invite_user_org.html#invite-a-user-to-join-an-organization).

    > Notes:
    >
    > The **Login Settings** section appears on the **Invite User** page once you have configured SSO.

2. Select **Enable SSO** in the **Login Settings** section, then click **Invite**.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/invite-user-page-sso-enabled.png" width=100% alt="enable SSO in Invite user page">

    An invitation is then sent to the User.

### For an existing User

To enable SSO for an existing member, follow these steps:

1. Go to **Settings** > **User Management**.

    The **Manage Users** page appears.

2. Edit a User's account by clicking on the *Pencil* icon.

    The **User's detail** page appears.

3. Select **Enable SSO** as a login option.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/user-detail-page-sso-enabled-blurred.png" width=100% alt="enable sso pending request sent box">

    A request to enable SSO is then sent to the existing User.

> Notes:
>
> * The action is pending until new members accept the invitations and existing members accept the requests.

## View and manage User Authentication

### View pending SSO requests

As an Owner or Admin, you can view the pending invitations and SSO requests on the **Manage Users** page.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/sso-pending-highlight-blurred.png" width=100% alt="pending SSO invitations">

You can withdraw an invitation and request by clicking on the *Trash bin* icon. After confirming your action, the member will no longer be able to access the URLs.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/delete-sso-pop-up-blurred.png" width=100% alt="pending SSO delete box">

### Update authentication methods

There are two login options: **Enable SSO** and **Access Katalon TestOps with username & password**.

You can always switch back to **Access Katalon TestOps with username & password** to change the authentication method.

To update the authentication method for Users, go to the **User's detail** page and update the login option.

## Activate SSO in Katalon Studio

After configuring SSO in Katalon TestOps, you must reactivate Katalon Studio to enable SSO.

Follow these steps:

1. Open Katalon Studio.

2. Click on the *Profile* icon at the top right corner, and select **Deactivate**.

    The **Katalon Studio Activation** box appears as below.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/activate-sso-in-studio.png" width=100% alt="ks activation box">

3. Fill in the required information.

    * **Server URL**: enter the Subdomain you have configured (e.g., https://techwrite.katalon.io).

    * **Email**: enter your registered Katalon account.

    * **Password**: enter an API key generated in Katalon TestOps. See: [API Keys](https://docs.katalon.com/katalon-analytics/docs/ka-api-key.html).

## Enable SSO as a User

If you are not an Owner or Admin of an Organization, you will receive the invitation or SSO request via email.

As a new User, accept the invitation to join the Organization first. See: [TestOps User Management](https://docs.katalon.com/katalon-analytics/docs/kt_invite_user_org.html#as-a-user).

As an existing User, follow these steps:

1. Go to your email and find the *[Katalon TestOps] Verify Single Sign-On (SSO) authentication* email, then click **Click here to confirm** in the email.

    You will be directed to Katalon TestOps and see the below message.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/user-navigate-sso-acceptance-blurred.png" width=100% alt="user accept sso">

    > Notes:
    >
    > If you are a new User, you must accept the invitation to join an Organization first. Then you will receive the authentication email.

2. Check the information, then click **Allow this account to access Organization [...] via SSO** to confirm.

    After accepting the SSO request, you are automatically navigated to the Subdomain.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-sso-settings/subdomain-signin-using-sso-blurred.png" width=100% alt="subdomain sign in using SSO">

3. Click **Sign in using SSO**.
