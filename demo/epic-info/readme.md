This demo code is implemented for sandbox [Epic on FHIR](https://fhir.epic.com/Documentation?docId=launching#)
* Account: jonascheng
  registered with jonas_cheng@asus.com
* PWD: 9qZ8Ufx6NB8Tu@8

When a developer registers an app, the website creates an app record in the Epic database and assigns the app production and non-production client IDs. The steps for a user to register an app are:

1. Navigate to the Build Apps page
2. Select "Create My First App”
3. Complete the Create an App form

  * Application name
  * Application Audience: Clinicians or Administrative Users
  * Application access scope:

    * Patient.read (R4)
    * Patient.search (R4)
    * Observation.read (Labs) (R4)
    * Observation.search (Labs) (R4)
    * Observation.read (Vitals) (R4)
    * Observation.search (Vitals) (R4)

  * Redirect Uri = your repl.it url, ex: https://epic.jonascheng1.repl.co
