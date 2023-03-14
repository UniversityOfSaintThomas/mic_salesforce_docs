# General Site RFIs

-   https://cas.stthomas.edu/admissions/graduate/request-information/index.html
-   https://business.stthomas.edu/request-for-information/index.html
-   https://dfc.stthomas.edu/admissions-tuition/request-information/index.html
-   https://education.stthomas.edu/admissions/graduate/request-information/index.html
-   https://engineering.stthomas.edu/admissions/graduate/request-information/index.html
-   https://software.stthomas.edu/admissions/request-information/index.html
-   https://health.stthomas.edu/graduate-psychology/admissions/request-information/index.html
-   https://health.stthomas.edu/social-work/admissions/request-information/index.html
-   https://health.stthomas.edu/nursing/admissions/request-information/index.html
-   https://www.stthomas.edu/admissions/graduate/request-information/divinity/index.html
-   https://www.stthomas.edu/admissions/undergraduate/request-information/index.html
-   https://law.aws.stthomas.edu/ethics-compliance/msl/admissions-tuition/request-information/index.html
-   https://law.aws.stthomas.edu/llm-us-law/admissions-tuition/request-information/index.html

# How to build an RFI (Lightning Component)

1. Login to Salesforce EDA Staging: https://uofstthomasmn--edastaging.sandbox.lightning.force.com/lightning/o/RFI_Controller__c/list?filterName=00B4P000009KjScUAK

2. Click on RFI Controllers > All

3. Click New

4. Create the form:

-   Descriptive Name: (ex.) CAS Graduate RFI
-   Lead Owner: Tiana Johnson or Angela Holden
-   Hide Form Title: Checked
-   Lead Source: Check the lead source of the original form
-   Citizenship Type: leave blank
-   Academic Level: Either graduate or undergraduate
-   School/College: Pick from the list
-   Fields to Display: Select all the fields you want added to the form
-   Required Fields: Select the fields that are required
-   Redirect URL: This is the link to the Thank You page
-   Click Save

5. Update the Landing Page spreadsheet: https://uofstthomasmn.sharepoint.com/:x:/r/sites/GroupMIC/_layouts/15/Doc.aspx?sourcedoc=%7BB3486A8B-42C1-43F7-8348-D4BAADAAA42C%7D&file=Campaign-Landing-Pages-Ongoing-List.xlsx&_DSL=1&action=default&mobileredirect=true

6. Embed the form:

-   Create a new page called `eda-rfi`
-   Use a full width module to embed the RFI
-   Uncheck "Include when publishing"
-   Update the rfi_controller number

```javascript
<div id="lightning"></div>

<script type="text/javascript" src="https://uofstthomasmn--edastaging.sandbox.my.salesforce.com/lightning/lightning.out.js"></script>

<script type="text/javascript">
    $Lightning.use("c:requestForInformationApp",
        function () {
            $Lightning.createComponent(
                "c:requestForInformationForm",
                { "rfi_controller": "RFI Controller 0000" }, //replace this number
                "lightning",
                function (cmp) {
                    console.log("LWC Component Created.");
                }
            );
        },
        'https://uofstthomasmn--edastaging.sandbox.my.site.com/Admissions'
    );
</script>
```
