---
title: "App Store Overview"
category: "General Info"
menu_order: 10
description: "Presents an overview of how to find and use content from the Mendix App Store."
tags: ["app store", "widget", "connector", "module", "partner"]
aliases:
    - /community/app-store/app-store-overview.html
    - /developerportal/app-store/app-store-overview.html
---

## 1 Introduction

{{% alert type="info" %}}
As the Mendix App Store is being updated into a dynamic and fully functioning Mendix Marketplace, some documentation pages will refer to "App Store" and some to "Marketplace." The URLs will also be updated during this conversion.
{{% /alert %}}

The [Mendix App Store](https://appstore.home.mendix.com/index3.html) is a vibrant marketplace containing complete sample apps that can be used right away as well as various components (connectors, widgets, and modules) that can be used to build custom apps more quickly. In the Mendix App Store, you can browse all the content, get what you need, and share the content you have created.

This document describes the different sections of the Mendix App Store.

## 2 App Store Home Page {#home}

The home page of the Mendix App Store has three main tabs at the top:

* **Discover** – the home page, where you can browse various component categories and filter what is displayed
* **My Marketplace** – click this to go to [My App Store](#my-app-store)
* **{Your company's private App Store page}** – click this to go to your [company's App Store](#company-content)

![](attachments/app-store-overview/home-page.jpg)

<a name="catalog"></a>It also presents various content catalogs:

| Catalog | Description |
| --- | --- |
| **Get Studio Pro** | All the versions of [Studio Pro](/releasenotes/studio-pro/) available for download. |
| [Widgets](/appstore/widgets/) | Single user-interface elements that can be configured, such as containers, drop-down menus, and buttons. |
| [Connectors](/appstore/connectors/) | Connectors can be used to connect your Mendix app with other systems.  |
| [Modules](/appstore/modules/) | These elements enable new functionality with accompanying domain models and security options. |
| **App Design** | Start building your app based on a [layout](/refguide/layout) that is ready to use with commons structures and widgets or a [theme](/appstore/themes/) that contains styling options you can apply for different elements and devices. |
| **Solutions** | Fully-formed solutions for your apps. |

The following filter options are also available:

* **Tags**
* **Ratings**

## 3 Component Details Page {#details}

Clicking the tile of an App Store component will bring you to its details page with the sections described below.

![](attachments/app-store-overview/component-details.jpg)

### 3.1 Header & Usage

The header for each component presents the following details:

* The name and category of the component
* The review average (in stars) and the number of reviews
* The number of times the component has been downloaded
* <a name="saved"></a>The **Add to Saved** button which, when clicked, will add the component to the list on the [Dashboard](#dashboard) and [Saved](#saved-components) pages
* The **Share** button, which allows you to copy the URL of the component and share it to your networks
* **Download** – click this to download the component
	* This is only available for components that have a file attached (meaning, all shared Studio Pro components, but not promotions)
	* The best practice is to download a component from the App Store that is accessible in Studio Pro, because it then downloads directly into Studio Pro (for details on importing downloaded App Store content into Studio Pro, see [How to Import & Export Objects](/howto/integration/importing-and-exporting-objects))
	

<a name="usage"></a>The **Usage** section presents  the following information (depending on the type of component):

* The latest **Version** number of the component
* The Studio Pro version that the component **Requires** to work
* The type of [license](share-app-store-content#license) for the component

The **Publisher** section presents the name of the company who created the component as well as the **Date** when the component was first published.

The **Developers** section presents the names of the developers who most recently updated the component, with links to their [Mendix Profile](/developerportal/mendix-profile/).

The **Support** section presents the category of support Mendix offers for the component (for more details, see [App Store Content Support](app-store-content-support)).

* A **GitHub** link, which will take you to the GitHub source files of the component

### 3.2 Tabs

The details page for a component presents the following item information tabs:

*  **Overview** – contains the following sections:
	* **Description** – a description of the component
	* **Screenshots** – screenshots of the component
	* **User Reviews** – user reviews of the component; to leave a review for the component, click **Add Review** – a section will open where you can add text, rate the component, and submit the review (your reviews will be listed on your [Reviews](#my-reviews) page)
*  **Documentation** – can include details on typical use cases, features and limitations, dependencies, installation and configuration, and frequently asked questions
	* [Platform-supported](app-store-content-support#category) components are documented in the various categories of this *App Store Guide*
	* Click **Edit documentation** to open a text editor where you can edit the App Store component's documentation
* **Pricing**  – lists the pricing options (only for paid components)
* **Releases** – lists all the versions of the component (any of which can be downloaded by clicking **Download**) along with details like the **Framework version** and the **UUID** (which can be used in the [CreateNewApp operation](/apidocs-mxsdk/apidocs/projects-api#createnewapp) in the *Projects API*): 

## 4 My App Store {#my-app-store}

### 4.1 Dashboard {#dashboard}

The **Dashboard** page presents your App Store activity:

* Your numbers for [Published Content](#content) and [Submitted Reviews](#my-reviews)
* [Notifications](#notifications) on components you created and favorited
* Content [Drafts](#drafts) you have created
* Your content [Favorites](#saved)

![](attachments/app-store-overview/my_app_store.png)

### 4.2 My Content {#content}

On this page, you can see the App Store content for which you have created at least one version:

![](attachments/app-store-overview/my-content.png)

You may see the **Company only** label on a component, which means it is your company's private App Store content (for details on how this is configured, see the [Adding New App Store Content](share-app-store-content#private-app-store) section of *How to Share App Store Content*). This content can be shared with [guests](#guests).

In addition, you may see a label on a component name for the [user group](#user-groups) to which the component is assigned as user group [content](#content).

To see the component's [details](#details) page, click **View**.

#### 4.2.1 Managing a Component {#manage}

Click **Manage** to manage the component:

![](attachments/app-store-overview/content-management.png)

On this page, you will see the following buttons:

* **Create new draft version** – click this to create a new draft version of the component
	* Only one draft version of a component can exist at a time, so when one draft version is in progress, another draft cannot be initiated – if there is a draft version in progress, click **View draft** to see it
	* For more information on creating a draft version, see the [Updating Existing App Store Content](share-app-store-content#updating) section of *How to Share App Store Content*
* **Unpublish** – click this to remove that version from the component
	* If the component is not the protected content of a [user group](#user-groups), you can only unpublish a version that you have published yourself
	* If the component is protected [content](#content) from a user group, a group [member](#members) can unpublish any version
* **Edit** – click this to edit the component (for details on editing, see the [Adding New App Store Content](share-app-store-content#adding) section of *How to Share App Store Content*)

### 4.3 Drafts {#drafts}

This page contains drafts of App Store content you have started:

![](attachments/app-store-overview/drafts.png)

Click the name of an App Store component to be taken to the [DRAFT](share-app-store-content#adding) page, where you can continue editing the component details.

Click **Delete** to delete a draft.

Click **Withdraw** to withdraw the content from the review process after you have [submitted it for approval](share-app-store-content#approval), which will return the content to the draft state:

![](attachments/app-store-overview/draft-withdraw.png)

### 4.4 Shared with Me {#shared-with-me}

This page contains private content shared with you by other companies who have marked you as a [guest](#guests):

![](attachments/app-store-overview/shared-with-me.png)

### 4.5 Reviews {#my-reviews}

This page contains reviews of [Your content](#content) by other users as well as **Your reviews** that you have written of other content:

![](attachments/app-store-overview/your-reviews.png)

### 4.6 Notifications {#notifications}

This page presents a history of notifications on content you have contributed to:

![](attachments/app-store-overview/notifications.png)

### 4.7 Favorites {#saved-components}

This page presents the App Store content you have [favorited](#saved):

![](attachments/app-store-overview/favorites.png)

When the **Subscribe** box is checked next to a favorite component, you will receive email notifications when new versions of that component are published. Clear the check box if you do not want to receive these notifications.

## 5 Your Company's App Store

### 5.1 Company Content {#company-content}

On this page, you can see all the content your company has published:

![](attachments/app-store-overview/company-content.png)

The **Manage** button is available to you if one of the following conditions is true:

* The component is not assigned to any [user groups](#user-groups) (in which case it can be managed by anyone in the company)
* The component is assigned to a user group, and you are a [member](#members) of that group
* You are a Company Admin of the company that published the component

To manage a component, click **Manage** (for more information, see the [Managing a Component](#manage) section above).

To see the component's [details](#details) page, click **View**.

### 5.2 Reviews

This page contains reviews of **Your company's content** as well as **Your company's reviews** that users from your company have written of other content.

![](attachments/app-store-overview/your-company-reviews.png)

### 5.3 User Groups {#user-groups}

You can configure user groups for various levels of access to your company's App Store. The available configuration tabs for each user group page are described in the sections below.

{{% alert type="info" %}}
The **User Groups** menu item and page are visible to all users. However, only [Company Admins](/developerportal/company-app-roles/companyadmin-settings) with the [Can manage Company](/developerportal/company-app-roles/manage-roles#app-store-manager) permission can create and delete user groups. Both [Group Admins](#members) and Company Admins can manage user groups.
{{% /alert %}}

#### 5.3.1 Members Tab {#members}

On this tab, you can enter the email address of a Mendix Platform user from your company and click **Add Member** to add them as a user group member. User group members can manage the [content](#content) assigned to the group.

Once a member is added, you can select their permission level: **Member** or **Group Admin**. A Group Admin can manage the user group.

![](attachments/app-store-overview/members.png)

To remove a member, click **Remove** next to their name.

#### 5.3.2 Guests Tab {#guests}

A guest is a Mendix Platform user from outside your organization who can download the selected private [Content](#content) of this group. To add a guest, enter their email address in the box and click **Add Guest**:

![](attachments/app-store-overview/guests.png)

The guest will receive an email notifying them of access to the private content. They can then see all the private App Store content shared with them in their [Shared with Me](#shared-with-me) page.

{{% alert type="info" %}}
The guest must be a registered Mendix Platform user; otherwise, they will not be able to access the shared content.
{{% /alert %}}

To remove a guest, click **Remove**.

#### 5.3.3 Content Tab {#content}

On this tab, you can assign content to this user group that can only be managed by members of this group. To assign a component to a user group, click **Assign Content** and select a company App Store component from the dialog box:

![](attachments/app-store-overview/group-content.png)

{{% alert type="info" %}}
A Mendix App Store component can only be assigned to one user group at a time. If a component is already assigned to another user group, it will not appear in this dialog box.
{{% /alert %}}

To manage a component assigned to the user group, click **Manage** (for more information, see the [Managing a Component](#manage) section above).

To see the component's [details](#details) page, click **View**.

To remove a component from the user group, click **Remove**.

[Group Admins](#members) and Company Admins can check the **Allow guests to download** box of this component can be downloaded by [guests](#guests).

#### 5.3.4 Settings Tab

On this tab, you can enter a **Name** and **Description** for the user group.

To delete a group, a Company Admin can click **Delete Group**.

## 6 Read More

* [How to Use App Store Content in Studio Pro](app-store-content)
* [How to Share App Store Content](share-app-store-content)
* [App Store Content Support](app-store-content-support)
