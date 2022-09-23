# MIC Salesforce Documentation

## The following outlines where and how we use Salesforce

### Capricorn JS Services

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

### Capricorn Legacy Web Apps

```bash
src/
|__ js/
    |__ scripts/
        |__ web-apps/
            |__ locate-counselor.js
        |__ admissions-visit.js
        |__ web-apps.js
```

### Capricorn Vue Components using SF APIs

```bash
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
    |__ ProgramFilter.vue
```

---

### Orion JS Services

```bash
src/
    |__ js/
        |__ services/
            |__ admissions.js
            |__ events.js
            |__ lawsearch.js
```

```bash
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
```
