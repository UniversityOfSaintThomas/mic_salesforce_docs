# Orion JS Services

```
src/
    |__ js/
        |__ services/
            |__ admissions.js
            |__ cape.js
            |__ events.js
            |__ lawsearch.js
```

## admissions.js

Example API:

```
https://stthomas.force.com/applicantportal/services/apexrest/ustadmissionsrest.json?type=gradprogramfinder
```

### Used in:

-   FieldGraduateProgram.vue

Example Object:

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

## cape.js

```
https://stthomas.force.com/applicantportal/services/apexrest/capefeed
```

## events.js

```
https://stthomas.force.com/applicantportal/services/apexrest/usteventfeed
```

## lawsearch.js

```
https://uofstthomas.secure.force.com/services/apexrest/professionaldirectoryfeed
```
