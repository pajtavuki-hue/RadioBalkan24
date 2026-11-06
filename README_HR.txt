RADIOBALKAN24 – KOMPLETAN ANDROID PROJEKT ZA IZGRADNJU APK-a

Ovaj paket sadrži Android modul app, AndroidManifest.xml, MainActivity.java,
RadioPlaybackService.java, Gradle konfiguraciju i GitHub Actions workflow.
Aplikacija otvara postojeću web-stranicu:
https://lighthearted-stardust-37d35c.netlify.app/

VAŽNO
- Verzija projekta: 1.0.1 (versionCode 2). APK još nije potvrđeno izgrađen niti testiran na stvarnom telefonu.
- Ovaj projekt ne mijenja objavljenu Netlify stranicu.
- Web player ostaje aktivan utišan kako bi animacije i heartbeat brojača slušatelja
  nastavili raditi; zvuk preuzima Android Media3 servis.
- Reprodukciju u pozadini, obavijest playera, Bluetooth kontrole i streamove
  treba provjeriti nakon izgradnje i instalacije.
- Nemoj dodavati lozinke, tokene ili druge tajne podatke u repozitorij.

IZGRADNJA APK-a S MOBITELA PREKO GITHUBA
1. Otvori GitHub i napravi novi repozitorij. Ako želiš da kod ne bude javan,
   postavi repozitorij kao Private.
2. Raspakiraj ovaj ZIP. U korijenu repozitorija moraju biti mape app i
   .github te datoteke build.gradle, settings.gradle i gradle.properties.
   Nemoj učitavati samo ZIP kao jednu datoteku.
3. Učitaj cijeli sadržaj raspakiranog projekta u korijen repozitorija.
4. Otvori Actions i odaberi workflow “Build RadioBalkan24 Novi APK”.
5. Pritisni “Run workflow”. Pričekaj da završi.
6. Ako je rezultat zelen (Success), otvori taj run i u odjeljku Artifacts
   preuzmi “RadioBalkan24-Novi-debug-APK”.
7. Raspakiraj preuzeti artefakt i instaliraj app-debug.apk. Android može
   zatražiti dopuštenje za instaliranje aplikacija iz preglednika/datoteka.

AKO BUILD PADNE
Otvori neuspjeli run u Actions, otvori korak “Build debug APK” i pošalji
mi tekst ili snimku greške. Nemoj slati lozinke, tokene ni sigurnosne kodove.
