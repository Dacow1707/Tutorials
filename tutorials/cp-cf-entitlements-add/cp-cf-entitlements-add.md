---
title: Add a New Entitlement to Your Subaccount
description: Each subaccount in your global SAP Cloud Platform account is given a share of the resources through Entitlements. In this tutorial you will add additional entitlements (= resources) to your default subaccount.
auto_validation: true
time: 10
tags: [ tutorial>beginner, products>sap-cloud-platform]
primary_tag: products>sap-cloud-platform-for-the-cloud-foundry-environment
---


## Details
### You will learn
  - Where to find all entitlements of your subaccount
  - How to add a new entitlement to your subaccount

Entitlements are the hearth of all subaccounts in the Cloud Foundry environment. They define which service and runtime artifacts you are able to use. This tutorial will show you how you can set up the entitlements you need to develop success solutions on SAP Cloud Platform Cloud Foundry environment.

---

[ACCORDION-BEGIN [Step: ](Log into SAP Cloud Platform)]


1. Go to <https://account.hanatrial.ondemand.com> and log in to your SAP Cloud Platform cockpit.

2. Click on "Enter Your Access Trial Account" to access the Cloud Foundry environment.

    ![accesstrial](accesstrial.png)

[DONE]
[ACCORDION-END]
[ACCORDION-BEGIN [Step: ](Switch to entitlements view)]

1. Select the tile of the subaccount you want to add entitlements to.

    ![subaccount](selectsubaccount.png)

2. Click on **Entitlements** in the left-hand sidebar.

    ![openentitlements](openentitlements.png)

[DONE]
[ACCORDION-END]
[ACCORDION-BEGIN [Step: ](Add a SAP HANA service entitlement to subaccount)]

In this step we will add a new service plan to a subaccount. Depending on when you created the SAP Cloud Platform account, this entitlement might already be assigned to the subaccount.

1. You can use the filter box if you see too many entries to find the entitlement you are looking for. Click on **Configure Entitlements** to switch the table into edit mode.

    ![findentitlement](findentitlement.png)

2. Click on **Add Service Plans** to see all available entitlements.

    ![addserviceplan](addserviceplan.png)

3. Use the filter bar the search for **`hana`** to reduce the number of available entitlements. Click the checkbox to select the service plans **`hdi-shared`**, **`securestore`**, and **`schema`**. Finally, confirm your selection by clicking on **Add 3 Service Plan**.

    ![addplan](addplan.png)

4. In the table, you can see the quota you are going to assign to the subaccount. As the trial landscape is for free, you can max out all your service plans.

    ![quotamax](quotamax.png)

> If you are not able to increase the quota of a given service plan, you might already consume this service plan in another subaccount. Please make sure to release the quota from other subaccounts, before reassigning it.


[DONE]
[ACCORDION-END]
[ACCORDION-BEGIN [Step: ](Add more entitlements to subaccount)]

Congratulations, you just enabled the SAP HANA service in your Cloud Foundry environment. Depending on what you want to build, you might want to add one of more of the following service plans as well:

| Service | Service Plan | Usage Scenario |
|----|----|----|
|ABAP Trial|shared | For exploring the free trial of the SAP Cloud Platform ABAP environment|
|Application Runtime|MEMORY|Needed to run application on SAP Cloud Platform Cloud Foundry environment. Quota defined the available memory of the Cloud Foundry Application Runtime (CFAR) |
|Connectivity|lite|To use principal propagation between SAP Cloud Platform and on-premise backend systems. |
|Destination|lite|To connect your applications to each other or to third party systems. |
|Enterprise Messaging|dev|Messaging bus for inter-app communication within the Cloud Foundry environment.|
|HTML5 Applications|app-host|To store web applications in the HTML5 Application Repository.|
|Portal|standard|The connect your SAPUI5 components to the Fiori Launchpad.|
|Workflow|lite|To use the SAP Cloud Platform Workflow service within the Cloud Foundry environment.|
> This is an incomplete enumeration.

Follow the instructions from the previous step to add these new entitlements to your subaccount.


[VALIDATE_1]
[ACCORDION-END]
[ACCORDION-BEGIN [Step: ](Save the entitlements)]

Confirm you selection with **Save**.

![save](save.png)


[DONE]
[ACCORDION-END]

---
