# Android / AdMob

AdMob ya está conectado en el código de Tap Rush.

App ID:
ca-app-pub-8854680295966508~8362422277

Rewarded:
ca-app-pub-8854680295966508/5279954200

Interstitial:
ca-app-pub-8854680295966508/6401464189

Al generar la carpeta Android con Capacitor, añadir bajo <application> en
android/app/src/main/AndroidManifest.xml:

<meta-data android:name="com.google.android.gms.ads.APPLICATION_ID"
android:value="@string/admob_app_id" />

Y en android/app/src/main/res/values/strings.xml:

<string name="admob_app_id">ca-app-pub-8854680295966508~8362422277</string>

Durante pruebas antes de publicar conviene usar anuncios de prueba.
La versión de producción debe incluir la configuración de consentimiento
de Google UMP para usuarios donde corresponda.
