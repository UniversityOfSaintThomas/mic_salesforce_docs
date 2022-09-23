# Orion JS Services

```bash
src/
    |__ js/
        |__ services/
            |__ admissions.js
            |__ events.js
            |__ lawsearch.js
```

## admissions.js

### APIs:

```
Graduate Program Finder

https://stthomas.force.com/applicantportal/services/apexrest/ustadmissionsrest.json?type=gradprogramfinder

Undergraduate Program Finder

https://stthomas.force.com/applicantportal/services/apexrest/ustadmissionsrest.json?type=ugprogramfinder
```

### Used in:

-   FieldGraduateProgram.vue

### Object example:

```json
{
	"title": "Academic Behavioral Strategist",
	"schoolId": "a0O0a00000IEeXgEAL",
	"school": "School of Education",
	"programMajorCode": "ED_SE_MAT|SPAB",
	"programId": "a0M0a00001e8j3QEAQ",
	"programCode": "ED_SE_MAT",
	"preprofessional": "false",
	"minor": "false",
	"majorId": "a1h0a00000ExvbGAAR",
	"majorConcentration": "false",
	"major": "false",
	"link": "https://education.stthomas.edu/teacher-degrees-licensure/special-education/ma-teaching-initial-licensure/academic-behavioral-strategist/index.html",
	"learningStyle": "Online",
	"keywords": "",
	"interest": "Education",
	"degreeLevel": "Master of Arts in Teaching Special Education",
	"concentration": "false",
	"coMajor": "false"
}
```

---

## events.js

### API:

```
https://stthomas.force.com/applicantportal/services/apexrest/usteventfeed?feedType=eventList
```

### Used in:

-   CasEventFilter.vue
-   EventDetail.vue
-   EventFinder.vue
-   EventListing.vue
-   HealthEventFilter.vue

### Endpoints:

```javascript
feedType = 'eventList',
id = '',
viewStart = '',
viewEnd = '',
audience = '',
filter = '',
sponsor = '',
school = '',
category = '',
displayon = '',
building = '',
type = '',
env = 'production',
```

### Object example:

```json
{
	"title": "Group Visits - Week of August 23-25",
	"start": "2022-08-23T08:00:00.000Z",
	"sponsors": "",
	"longDesc": "",
	"locationType": "St. Paul",
	"locationTitle": "",
	"locationMapLink": "",
	"locationBuilding": "",
	"locationAddress": "",
	"instanceDesc": "",
	"ID": "a345b000003EykDAAS",
	"feedButtonText": "Register",
	"excludeSearchTag": false,
	"eventUrl": "javascript:void(0);",
	"eventClosed": true,
	"end": "2022-08-25T16:00:00.000Z",
	"description": "",
	"className": "eventClosed",
	"capacityTotal": 1,
	"capacityRemaining": 1
}
```

---

## lawsearch.js

### API:

```
Parameter Keys

https://uofstthomas.secure.force.com/services/apexrest/professionaldirectoryfeed?type=parameterkey

Practice Areas

https://uofstthomas.secure.force.com/services/apexrest/professionaldirectoryfeed?type=practice

Directory

https://uofstthomas.secure.force.com/services/apexrest/professionaldirectoryfeed?type=directory

```

### Used in:

-   AdvancedSearch.vue
-   AlumniProfile.vue
-   PracticeAreas.vue
-   SearchResults.vue

### Endpoints:

```javascript
type = 'directory',
practice = '',
language = '',
city = '',
state = '',
admissionstate = '',
country = '',
pagesize = '',
page = '',
first = '',
last = '',
employer = '',
gradyear = '',
keywords = '',
sortby = '',
order = '',
```

### Object example:

```json
{
	"workEmail": "riki.rodriguez@ci.stpaul.mn.us",
	"website": "",
	"title": "Associate Attorney - Criminal Division",
	"specialties": [
		{
			"specialtyPercentage": 100,
			"specialty": "Criminal - Prosecution"
		}
	],
	"picture": "",
	"linkedIn": "",
	"lastName": "Rodriguez",
	"language": "",
	"keywords": "Domestic Assault,,,,",
	"gradYearSelfReported": "2018",
	"gradYear": "2018",
	"genderIdentity": "",
	"firstName": "Riki",
	"ethnicity": "Hispanic or Latino",
	"employerZip": "55102",
	"employerState": "MN",
	"employerPhone": "651-266-8718",
	"employerName": "Saint Paul City Attorney's Office",
	"employerCountry": "United States of America",
	"employerCity": "St Paul",
	"employerAddress": "15 West Kellogg Blvd",
	"degreeAwarded": "J.D.",
	"bio": "",
	"admissionState": "MN",
	"additionalIdentity": ""
}
```
