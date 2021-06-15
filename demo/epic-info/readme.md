This demo code is implemented base upon sandbox [Epic on FHIR](https://fhir.epic.com/Documentation?docId=launching#)
* Account: jonascheng
  registered with jonas_cheng@asus.com
* PWD: 9qZ8Ufx6NB8Tu@8

When a developer registers an app, the website creates an app record in the Epic database and assigns the app production and non-production client IDs. The steps for a user to register an app are:

1. Navigate to the Build Apps page
2. Select "Create My First App”

   ![Create My First App](https://fhir.epic.com/Content/images/epiconfhirrequestprocess/buildapp1.png)

3. Complete the Create an App form

  * Application name
  * Application Audience: Clinicians or Administrative Users
  * Application access scope:

    * Patient.read* (R4)
    * Patient.search* (R4)
    * Observation.read* (R4)
    * Observation.search* (R4)
    * Condition.read* (R4)
    * Condition.search* (R4)
    * Procedure.read* (R4)
    * Procedure.search* (R4)
    * DocumentReference.read* (R4)
    * DocumentReference.search* (R4)

  ![Complete the Create an App form](https://fhir.epic.com/Content/images/epiconfhirrequestprocess/buildapp2.png)

  * Redirect Uri = your repl.it url, ex: https://epic.jonascheng1.repl.co

You may follow the [instructions](https://fhir.epic.com/Documentation?docId=launching#) on the web site, and specify *App Launch URL* to test out.

1. Select a patient: Warren McGinnis or Camila Maria (with Vital observations)
2. Choose an app to test with: the app created previously.
3. Enter launch URL to receive the request to your app: https://epic.jonascheng1.repl.co/launch.html

The app retrieves basic information from a single patient as follows.

* FHIR information
* Patient ID
  * patient information
* Encounter ID
  * encounter information
* Condition ID if any
* Procedure ID if any
* DocumentReference ID if any
