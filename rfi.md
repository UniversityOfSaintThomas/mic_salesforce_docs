# RFIs

```bash
src/
|__ components/
    |__ rfi/
        |__ FieldGraduateProgram.vue
        |__ RfiForm.vue
```

The part of the RFI that uses a Salesforce API is `FieldGraduateProgram.vue`. That Vue component uses `admissions.js` in both Capricorn and Orion.

This documentation is specific to `RfiForm.vue`. This outlines the additional Salesforce assets needed to power the forms.

## Assets

### oid

```bash
Production

00Dj0000000ITv8

Staging

00Dq0000000Drru
```

### action URL

```bash
Production

https://webto.salesforce.com/servlet/servlet.WebToLead?encoding=UTF-8

Staging

https://test.salesforce.com/servlet/servlet.WebToLead?encoding=UTF-8
```

### scripts

```bash
Chosen

https://static.stthomas.edu/undergraduate-admissions/js/chosen/chosen.ust.1.8.7.jquery.min.js

RFI General

https://static.stthomas.edu/undergraduate-admissions/rfi/new/production/js/rfi.general.js

```

## Cascade RFI Files

### Orion Production RFI Formats

Disregard RFI form formats that live in individual Orion sites. Those don't belong there and are being removed.

```bash
_shared-orion/
|__ _cms/
    |__ formats/
        |__ components/
            |__ <> landing page one
            |__ <> landing page two
            |__ <> rfi form
            |__ <> rfi form cas
            |__ <> rfi form soed
            |__ <> rfi form v2
```

### OPUS DEV Formats

```bash
OPUS DEV/
|__ _shared-orion/
    |__ _cms/
        |__ formats/
            |__ components/
                |__ <> landing page one
                |__ <> rfi form
                |__ <> rfi form v2
```

### Capricorn Production RFI Formats

```bash
University of St. Thomas/
|__ _shared-capricorn/
    |__ formats/
        |__ modules/
            |__ campaign/
                |__ <> rfi-form-v2
            |__ specialized/
                |__ <> rfi-form
```

### STTHOMAS DEV Formats

```bash
STTHOMAS DEV/
|__ _shared-capricorn/
    |__ formats/
        |__ modules/
            |__ campaign/
                |__ <> rfi-form-v2
            |__ specialized/
                |__ <> rfi-form
```
