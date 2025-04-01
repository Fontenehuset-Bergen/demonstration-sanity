# Sanity studio
Sanity er et content management system (CMS) som gjør det veldig lett å ligge inn, og hente ut data. Sanity tillater enkel behandling av data når oppsettet er ferdig, dette er veldig kjekt for brukere som ikke er kjent eller god til koding.

## Registrer en konto hos sanity.io
Aller først må vi sitte opp en konto hos [sanity.io](https://www.sanity.io) som du kan bruke til å holde styr på dine prosjekter og studioer. Hvis du ikke allerede har en sanity konto kan du registrere en her: https://www.sanity.io/login/sign-up

> [!NOTE]
> Hvis du bruker social logins så husk at du har forskjellig bruker utifra hvilken provider du velger, husk å bruk samme provider senere!

## Installer Sanity Studio lokalt
Vi begynner først med å installere Sanity Studio i en tom mappe, hvor `.` på slutten sier at vi ønsker å bruke aktiv mappe som installasjon mål.
```console
npm create sanity@latest .
```

![alt text](docs/sanity-install.png)

Etter dette får du valget om å logge inn i sanity med credentials du satte opp din sanity.io konto med.

![alt text](docs/sanity-login-provider.png)

Videre kan du velge å bruke et eksisterende prosjekt (henter ned detaljer automatisk) eller lage et nytt prosjekt. I dette eksempelet lager jeg et nytt prosjekt

![alt text](docs/sanity-project-create.png)

Hvis du velger å lage et nytt prosjekt får du valget om å knytte dette mot en organisasjon, eller på din egen bruker. Anbefaler å bare bruke din egen bruker hvis den eksisterer.

![alt text](docs/sanity-project-organisation.png)

Hvis du valgte nytt prosjekt må du også fortelle sanity hva hoved databasen din skal hete, i eksempelet bruker vi `production` som er default

![alt text](docs/sanity-project-dataset.png)



Etter du har kjørt disse kommandoenene så vill du se at mange dependencies og mapper blir opprettet (Fil forklaring [her](https://www.sanity.io/docs/project-structure)). Sanity Studio genererer også en React prosjekt som vi gjør at vi kan redigere data på en enklere måte i nettleseren.
Det er mulig å kunne sende [API requests](https://www.sanity.io/docs/http-api) for å lage, lese, endre og slette (CRUD), men vi kommer til å forholde oss til websiden for all redigering i dette eksempelet.

Etter du har installert Sanity Studio får du også tilgang til [Sanity CLI](https://www.sanity.io/docs/cli)

> [!NOTE]
> Du kan finne mer grunndig informasjon om installerings prosessen på [sanity.io/docs](https://www.sanity.io/docs/installation)