---
auto_validation: true
title: Custom Analytical Queries Calculated Measures
description: Create a Custom Analytical Queries with Calculated Measures.
format: new
primary_tag: topic>abap-development
tags: [  tutorial>beginner, topic>abap-development, products>sap-business-technology-platform, products>sap-btp\\, kyma-runtime  ]
time: 10
---





## Prerequisites  
- You have [Set Up a BTP Account for Tutorials](group.btp-setup). Follow the instructions to get an account, and then to set up entitlements and service instances for the following BTP services.
    - **SAP Launchpad service**
    - **SAP Business Application Studio**




Now/ Next week
1.	Publish the Entitlements tutorial.
2.	Publish the Service Instances tutorial.

## Prerequisites
- You have managed entitlements for your subaccount and created a service instance for <SERVICE NAME>. If you need help with that, check out [Set up your SAP BTP account](link to mission mentioned above).
- Service-specific requirements.
5.	Authors remove all the steps in their tutorials related to logging on, entitlements, service instances. If there are special instructions for entitlements/service creation, then they create a step to indicate the special steps. They can if they want create a step for checking that all is setup OK.
6.	Check which tutorials still use set up trial account in their missions. If they also apply to enterprise accounts, remove the use to the setup tutorial and include the prerequisites mentioned above.
7.	Once authors say their mission/group works in free tier, label these with "free-tier" tag.








The Business users requires the Role `SAP_BCR_CA_ANA_AQD_PC` to access the Query Designer.
Furthermore `ABAP Customs Analytical Queries` as a tutorial reveals another Prerequisite.

Code &#x2B;

## Details
The Application Custom Analytical Queries characterizes the usage of reporting and analysis.
Raw data from business documents are getting converted into a meaningful grid.
By using Custom Analytical Queries you do not need to understand the technical details.

## LINK

[my link](costcenter.png)

[my link](mytext.png)

[mylink-direct](https://raw.githubusercontent.com/SAPDocuments/Tutorials-Contribution/master/tutorials/aa-test/mytext.txt)


### You will learn  
This tutorial teaches you the creation of a Custom Analytical Query and the addition of a Calculated Measures. You will also be able to edit your calculated Measures and define an Exception Aggregation.

---

### Step name
[ACCORDION-BEGIN [Step 1: ](Open Custom Analytical Queries Application)]
Start the **Custom Analytical Queries** Application by selecting the corresponding tile in the SAP Fiori Launchpad.

![Link text e.g., Destination screen](../aaa-test-conditional/444444.png)

### Header

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 2: ](Select your Analytical Query)]
To edit your analytical query you have to search for it and **select** it.
Furthermore you have to click on the **Edit** button to continue.

![start Custom CDS View App](select.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 3: ](Add Calculated Measures)]
Now you have to switch to the **Display** Tab to add a calculated measure.


[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 4: ](Add Further Calculated Measures)]
Press the **Add** button to add further calculated measures like:

-    **Gross Profit**
-    **Gross Revenue**
-     and **Counter**.

![Select Data Source](further-measures.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 5: ](Edit Calculated Measures)]
Select the measure **`margin`** and click on **Edit** to open the expression editor in a `popup` window.

![Select Data Source](calculated-measures2.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 6: ](Choose Measures)]
You can choose different measures, supported functions and you have content assistance by pressing **`Ctrl`** + **space**.

Select **`"Gross Profit" / "Gross Revenue"`** as an Expression.

![Select Data Source](calculated-measures3.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 7: ](Result of Measures)]

Result:
The new expression for the calculated measure is shown in the text field.

![Select Data Source](calculated-measures4.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 8: ](Define Exception Aggregation)]
For a calculated measure, you can define exception aggregation. Check **Exception Aggregation** and press the value help to add a function. The **`popup`** shows you the supported functions. One or more dimensions can be added to the exception aggregation via the **+** button.

Select following:

-      `COUNT` as `Function`
-      `Controlling Area` as `Dimension`
-       and `Cost Object` as `a further Dimension`.

![Select Data Source](calculated-measures5.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 9: ](Display Hierarchy)]
If a field supports hierarchies, then the hierarchy checkbox is shown in the properties.
**`Checkmark` the hierarchy checkbox** to enable displaying hierarchy for `CostCenter`.
Furthermore select values for `Controlling Area` and `Cost Center Hierarchy`.
![Select Data Source](costcenter.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 10: ](Save the Draft and Show the Preview)]
**Click on Save Draft** to save the query and **click** afterwards on **Preview** to test the query.

![Select Data Source](save.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 11: ](Publish the Query)]
**Click on publish** to publish the query. Published queries are available to be consumed by Key Performance Indicators and Reports.  

After publishing the status will be updated to published on the top right corner.

![Select Data Source](publish.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 12: ](Test yourself)]

Test

[VALIDATE_1]
[ACCORDION-END]
