# Create Custom Actions for Standard Operations.md

# Table of Contents
- [Prerequisites](#Prerequisites)
- [How to download vRO Client ?](#How-to-download-vRO-Client-?)
- [Add New Price](#Add-New-Price)
	- [Fixed Fare Strategy](#Fixed-Fare-Strategy)
	- [Rate Based Fare Strategy](#Rate-Based-Fare-Strategy)
- [Edit Price](#Edit-Price)
	- [Fixed Fare Strategy](#Fixed-Fare-Strategy)
	- [Rate Based Fare Strategy](#Rate-Based-Fare-Strategy)
- [View Details](#View-Details)
- [Import Pricing Plan](#Import-Pricing-Plan)
- [Download All pricing Plans for selected service](#Download-All-pricing-Plans-for-selected-service)
- [Delete All Pricing Plans for a Service](#Delete-All-Pricing-Plans-for-a-Service)


## Prerequisites
  1. User should have vRA / vRO access.
  2. User should have access to vRO Client (Standalone / Java Based)
  3. In case, user is going to provide already written vRO workflows, then make sure user has correct permissions to access, execute workflows.


## How to download vRO Client ?
  Please follow the link : How to download vRO Client ? https://confluence.gravitant.net/pages/viewpage.action?pageId=427460645


## View All Pricing Plans
1. Select Provider name from the Select Provider dropdown list.
![selectprovider.png](/media/pricingconfigurator/selectprovider.png)
2. Select service name from the Select Service dropdown list.
![selectservice.png](/media/pricingconfigurator/selectservice.png)
3. View the pricing plans for a service as shown below.
![listofservices.png](/media/pricingconfigurator/listofservices.png)

## Add New Price

### Fixed Fare Strategy
1. Click **Add New Price** to create a new price.
![adnewpricebuttton.png](/media/pricingconfigurator/adnewpricebuttton.png)
2. In the Pricing Plan Details section, provide the inputs for Plan Name, Fare Strategy as Fixed, and Base Charge Applicable, and then click **Next**.
	- Plan Name:
		input: free input text ( you can see this plan name in BOM section in the Store app)
	- Fare Strategy:
		input: Dropdown values
		values: Fixed, Rate Based
	- Base Charge Applicable:
		input: Dropdown Values
		values: Yes, No
![new-pricingplandetails.png](/media/pricingconfigurator/new-pricingplandetails.png)
![new-pricingplandetails-next.png](/media/pricingconfigurator/new-pricingplandetails-next.png)
3. In the Pricing Plan Configuration section, select Configurations is Optional. If you need to define the configuration driven price, select configuration and respective value listed in Pricing Plan Configuration Section, and click **Next**. ![new-pricingplanconfig-fixed.png](/media/pricingconfigurator/new-pricingplanconfig-fixed.png) ![new-pricingplanconfig-fixed-next.png](/media/pricingconfigurator/new-pricingplanconfig-fixed-next.png)
4. In the Define Price(s) section, provide the inputs for One Time Charge, Frequency, Frequency value, Recurring Amount and Currency Code, and click **Create Pricing Plan**.
	- One Time Charge:
input type: Number Input (for example, 80.20)
validation: One Time Charge Amount should Accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Frequency:
input type: Dropdown values
values : Month, Hour
	- Frequency value: this not an editable text field. The value should always be 1.
	- Recurring Amount:
input type: Number Input (for example, 20.12)
validation: Recurring Amount should Accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Currency Code: this not an editable text field. The value should always be USD. ![new-defineprices-fixed.png](/media/pricingconfigurator/new-defineprices-fixed.png) ![new-defineprices-fixed-createplan.png](/media/pricingconfigurator/new-defineprices-fixed-createplan.png)

5. After Creating Pricing Plan, navigate to the Pricing Plan Success Message section.
	- To download the pricing plan JSON you created, click **Click here for Pricing Plan JSON** and then click **Download**.
	- To navigate to the pricing configurator Listing Page, click **Return to pricing Configurator Main Page**. ![new-pricesuccessfullmessage.png](/media/pricingconfigurator/new-pricesuccessfullmessage.png) ![new-pricesuccessfullmessage-download.png](/media/pricingconfigurator/new-pricesuccessfullmessage-download.png) ![new-pricesuccessfullmessage-returnhome.png](/media/pricingconfigurator/new-pricesuccessfullmessage-returnhome.png)
6. Now you can view the newly created plan on the pricing configurator listing page. ![listofservices-newprice.png](/media/pricingconfigurator/listofservices-newprice.png)

### Rate Based Fare Strategy
1. Click **Add New Price** to create a new price. ![new-rate-addnewprice-button.png](/media/pricingconfigurator/rate/new-rate-addnewprice-button.png)
2. In the Pricing Plan Details section, provide the inputs for Plan Name, Fare Strategy as Rate Based, and Base Charge Applicable, and then click **Next**.
	- Plan Name:
input: free input text (you can see this plan name in BOM section in the Store app)
	- Fare Strategy:
input: Dropdown values
values: Fixed, Rate Based
	- Base Charge Applicable:
input: Dropdown Values
values: Yes, No
![new-rate-pricingplandetails.png](/media/pricingconfigurator/rate/new-rate-pricingplandetails.png)
![new-pricingplandetails-next.png](/media/pricingconfigurator/rate/new-rate-pricingplandetails-next.png)
3. In the Pricing Plan Configuration section, select configuration and a respective value, and then click **Next**.
![new-rate-pricingconfig.png](/media/pricingconfigurator/rate/new-rate-pricingconfig.png)
![new-rate-pricingconfig-nextbutton.png](/media/pricingconfigurator/rate/new-rate-pricingconfig-nextbutton.png)
4. In the Define Price(s) section, provide the inputs for One Time Charge, Frequency, Frequency value, Usage Charge Amount, and Currency Code, and then click **Create Pricing Plan**.
	- One Time Charge:
input type: Number Input (for example, 80.20)
validation: One Time Charge Amount should accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Frequency:
input type: Dropdown values
values: Month, Hour
	- Frequency value: This is not an editable text field. The value should always be 1.
	- Usage Charge Amount:
input type: Number Input (for example, 20.12)
validation: Recurring Amount should Accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Currency Code: This is not an editable text field. The value should always be USD.
![new-rate-defineprice.png](/media/pricingconfigurator/rate/new-rate-defineprice.png)
5. After Creating Pricing Plan, navigate to the Pricing Plan success message.
	- To download the pricing plan JSON, click **Click here for Pricing Plan JSON**, and then click **Download**.
	- To navigate to the Pricing Configurator Listing page, click **Return to pricing Configurator Main Page**.
![new-rate-sucessfull.png](/media/pricingconfigurator/rate/new-rate-sucessfull.png)
![new-rate-download.png](/media/pricingconfigurator/rate/new-rate-download.png)
![new-rate-success-returnhome.png](/media/pricingconfigurator/rate/new-rate-success-returnhome.png)
6. Now you can view the newly created plan on the Pricing Configurator listing page.
![new-rate-listofservices.png](/media/pricingconfigurator/rate/new-rate-listofservices.png)

## Edit Price

### Fixed Fare Strategy
1. In the Pricing Plans table, select **Over flow menu** in the ACTIONS column for the selected plan, and click **Edit** from the **Overflow** menu.
![editprice-button.png](/media/pricingconfigurator/editprice-button.png)
2. In the Pricing Plan Details section, the fields have been pre-populated with existing data. If needed, edit the fields Plan Name and Fare Strategy, and then click **Next**.
	- Plan Name:
input: Free input text (view the plan name in the BOM section of the Store app)
	- Fare Strategy:
values: Fixed, Rate Based
	- Base Charge Applicable: Cannot modify the Base Charge in Edit flow
![edit-pricingplandetails.png](/media/pricingconfigurator/edit-pricingplandetails.png)
![edit-pricingplandetails-next.png](/media/pricingconfigurator/edit-pricingplandetails-next.png)
3. In Pricing Plan Configuration, note that the configurations have been pre-populated with existing configurations. To modify the existing configurations, select the configuration that you want to change, and then click **Next**.
![edit-pricingplanconfig.png](/media/pricingconfigurator/edit-pricingplanconfig.png)
![edit-pricingplanconfig-next.png](/media/pricingconfigurator/edit-pricingplanconfig-next.png)
4. In the Define Price(s) section, note that all details have been pre-populated with existing data. The fields One Time Charge, Frequency, and Recurring Amount can be edited if needed. Update Pricing Plan by clicking **Update Pricing Plan**.
	- One Time Charge
input type: Number Input (for example, 80.20)
validation: One Time Charge Amount should accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Frequency:
input type: Dropdown values
values: Month, Hour
	- Frequency value: This is not an editable text field. The value should always be 1.
	- Recurring Amount:
input type: Number Input (for example, 20.12)
validation: Recurring Amount should accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Currency Code: this is not an editable text field. The value should always be USD.
![edit-defineprices.png](/media/pricingconfigurator/edit-defineprices.png)
![edit-defineprices-updateprice.png](/media/pricingconfigurator/edit-defineprices-updateprice.png)
5. After updating Pricing Plan, you will navigate to the Pricing Plan Updated success message.
- To download the updated pricing plan JSON, click **Click here for Pricing Plan JSON**, and then click **Download**.
- To navigate to the pricing configurator Listing Page, click **Return to pricing Configurator Main Page**.
![edit-pricesuccesfullmessage-updateplan.png](/media/pricingconfigurator/edit-pricesuccesfullmessage-updateplan.png)
![edit-pricesuccesfullmessage-updateplan-download.png](/media/pricingconfigurator/edit-pricesuccesfullmessage-updateplan-download.png)
![edit-pricesuccesfullmessage-updateplan-returnhome.png](/media/pricingconfigurator/edit-pricesuccesfullmessage-updateplan-returnhome.png)
6. Now you can view the updated pricing plan on the pricing configurator listing page.
![listofservices-editprice.png](/media/pricingconfigurator/listofservices-editprice.png)

### Rate Based Fare Strategy
1. On the Pricing Plans table select **Over flow menu** in the ACTIONS column for the selected plan, and then click **Edit** on the Over Flow menu.
![edit-rate-button.png](/media/pricingconfigurator/rate/edit-rate-button.png)
2. In the Pricing Plan Details section, note that the fields have been pre-populated with existing data. The fields Plan Name and Fare Strategy can be edited if needed. Click **Next**.
	- Plan Name:
input: Free input text (view the plan name in the BOM section of the Store app)
	- Fare Strategy:
input: Dropdown values
values: Fixed, Rate Based
	- Base Charge Applicable: Cannot modify the Base Charge in Edit flow
![edit-rate-pricingplandetails.png](/media/pricingconfigurator/rate/edit-rate-pricingplandetails.png)
![edit-rate-pricingplandetails-next.png](/media/pricingconfigurator/rate/edit-rate-pricingplandetails-next.png)
3. In the Pricing Plan Configuration, note that the configurations have been pre-populated with existing options. If you want to modify the existing configurations on a price, select a different one that you want to change and click **Next**.
![edit-rate-pricingconfig-.png](/media/pricingconfigurator/rate/edit-rate-pricingconfig-.png)
4. In the Define Price(s) section, all details are pre-populated with existed data. The fields One Time Charge, Frequency, and Usage Charge Amount can be edited if needed. Update Pricing Plan by clicking **Update Pricing Plan**.
	- One Time Charge
input type: Number Input (for example, 80.20)
validation: One Time Charge Amount should accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Frequency:
input type: Dropdown values
	values: Month, Hour
	- Frequency value: This not an editable text field. The value  should always be 1.
	- Usage Charge Amount:
input type: Number Input (for example, 20.12)
validation: Recurring Amount should accept only numbers (should be 9 + 1 for decimal point and 2 places after decimal)
	- Currency Code: This is not an editable text field. The value should always be USD.
![edit-rate-defineprices.png](/media/pricingconfigurator/rate/edit-rate-defineprices.png)
![edit-rate-defineprices-createbutton.png](/media/pricingconfigurator/rate/edit-rate-defineprices-createbutton.png)
5. After updating the Pricing Plan, navigate to the Pricing Plan Updated success message.
	- To download the pricing plan JSON, click **Click here for Pricing Plan JSON**, and then click **Download**.
	- To navigate to the Pricing Configurator Listing page, click **Return to pricing Configurator Main Page**.
![edit-rate-sucessmessage.png](/media/pricingconfigurator/rate/edit-rate-sucessmessage.png)
![edit-rate-download.png](/media/pricingconfigurator/rate/edit-rate-download.png)
![edit-rate-success-returnhome.png](/media/pricingconfigurator/rate/edit-rate-success-returnhome.png)
6. View the updated pricing plan on the Pricing Configurator Listing page.
![edit-rate-lists.png](/media/pricingconfigurator/rate/edit-rate-lists.png)

## View Details
1. In the Pricing Plans table, select **Over flow menu** in the ACTIONS column for the selected plan, and then click **View Details** from the Over Flow menu.
![viewdetails-button.png](/media/pricingconfigurator/viewdetails-button.png)
2. Now you can view all of the price details in read mode.
![viewdetails.png](/media/pricingconfigurator/viewdetails.png)

## Import Pricing Plan
1. Click **Import pricing plan**.
![importpricingplan-button.png](/media/pricingconfigurator/importpricingplan-button.png)
2. Click **Choose File**, and then select the pricing JSON file that you want to upload.
![importpricingplan-button.png](/media/pricingconfigurator/importpricingplan-button.png)
![import-choosefile-button.png](/media/pricingconfigurator/import-choosefile-button.png)
![import-selectedfile-view.png](/media/pricingconfigurator/import-selectedfile-view.png)
![import-createplan-button.png](/media/pricingconfigurator/import-createplan-button.png)
![import-plan-sucess-message.png](/media/pricingconfigurator/import-plan-sucess-message.png)

## Download All pricing Plans for Selected Service
1. Click **Download** to download the JSON for all of the pricing plans.
![download-allplans-button.png](/media/pricingconfigurator/download-allplans-button.png)

## Delete All Pricing Plans for a Service
1. Click **Delete** to delete all of the pricing plans for a service.
![delete-allplans-button.png](/media/pricingconfigurator/delete-allplans-button.png)
2. Confirm or decline the delete by clicking **Yes** or **No**.
![delete-allpnas-confirmation.png](/media/pricingconfigurator/delete-allpnas-confirmation.png)
