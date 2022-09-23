# Capricorn JS Services

Vue components don't all have a services file. Some components call the API directly.

```bash
src/
|__ js/
    |__ services/
        |__ admissions.js
        |__ cape.js
        |__ degrees-certificates.js
        |__ events.js
```

---

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
-   DegreesCertificates.vue
-   ProgramFilter.vue

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
Event List

https://stthomas.force.com/applicantportal/services/apexrest/usteventfeed?feedType=eventList

DFC Group Visits

https://stthomas.force.com/applicantportal/services/apexrest/usteventfeed?eventId=a3s0a000000Av67&viewStart=&viewEnd=&feedType=eventList

DFC Interviews

https://stthomas.force.com/applicantportal/services/apexrest/usteventfeed?eventId=a3s0a0000002eJn&feedType=eventList&viewStart=&viewEnd=
```

### Used in:

-   DfcGroupVisits.vue
-   DfcInterviews.vue
-   Events.vue

### Endpoints:

```javascript
feedType = 'eventList',
env = 'production',
org = '',
id = '',
viewStart = '',
viewEnd = '',
audience = '',
filter = '',
program = '',
school = '',
category = '',
displayon = '',
building = '',
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
