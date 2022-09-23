# MIC Salesforce Documentation

## The following outlines where and how we use Salesforce in RFIs (Request for Information) and APIs.

### Capricorn JS Services

Vue components don't all have a services file. Some components call the API directly.

```
src/
|__ js/
    |__ services/
        |__ admissions.js
        |__ cape.js
        |__ degrees-certificates.js
        |__ events.js
```

### Capricorn Vue Components using SF APIs

```
src/
|__ components/
    |__ cape-filter/
        |__ CapeFilter.vue
    |__ cape-listing/
        |__ CapeListing.vue
    |__ dfc-group-visits/
        |__ DfcGroupVisits.vue
    |__ dfc-interviews/
        |__ DfcInterviews.vue
    |__ events/
        |__ Events.vue
    |__ online-learning/
        |__ DegreesCertificates.vue
    |__ rfi/
        |__ FieldGraduateProgram.vue
        |__ RfiForm.vue
    |__ ProgramFilter.vue

```

---

Vue components don't all have a services file. Some components call the API directly.

### Orion JS Services

```
src/
    |__ js/
        |__ services/
            |__ admissions.js
            |__ events.js
            |__ lawsearch.js
```

```
src/
    |__ components/
        |__ cas-event-filter/
            |__ CasEventFilter.vue
        |__ event-detail
            |__ EventDetail.vue
        |__ event-finder/
            |__ EventFinder.vue
        |__ event-listing/
            |__ EventListing.vue
        |__ health-event-filter/
            |__ HealthEventFilter.vue
        |__ lawyer-search/
            |__ AdvancedSearch.vue
            |__ AlumniProfile.vue
            |__ PracticeAreas.vue
            |__ SearchResults.vue
        |__ rfi/
            |__ FieldGraduateProgram.vue
            |__ RfiForm.vue
```
