# Exemple de practicien français - Guide d'implémentation FHIR - Mesures de santé v3.2.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Exemple de practicien français**

## Example Practitioner: Exemple de practicien français

Jean Dupont (http://www.acme.org/practitioners#801234567897)

-------

| | |
| :--- | :--- |
| Actif : | true |
| Coordonnées | * ph: 01 70 88 88 64(Work)
* 7 rue Coursier Amiens 80000 (home)
 |



## Resource Content

```json
{
  "resourceType" : "Practitioner",
  "id" : "example-mes-fr-practitionner-001",
  "identifier" : [{
    "system" : "http://www.acme.org/practitioners",
    "value" : "801234567897"
  }],
  "active" : true,
  "name" : [{
    "family" : "Dupont",
    "given" : ["Jean"],
    "prefix" : ["Mr"]
  }],
  "telecom" : [{
    "system" : "phone",
    "value" : "01 70 88 88 64",
    "use" : "work",
    "rank" : 1
  }],
  "address" : [{
    "use" : "home",
    "line" : ["7 rue Coursier"],
    "city" : "Amiens",
    "postalCode" : "80000"
  }]
}

```
