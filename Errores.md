# Errores

## Día 0 — "flutter no se reconoce como comando"
Qué pasó: al correr `flutter --version` la terminal no reconocía el comando.
Causa: agregué al PATH la ruta C:\dev\flutter\bin, pero yo había extraído
       Flutter en C:\Users\carlo\dev\flutter. El PATH apuntaba a una carpeta
       que no existía.
Solución: corregí la entrada del PATH a la ruta real donde estaba el SDK,
          y reabrí la terminal para que tomara el cambio.

## Día 0 — "fatal: not a git repository"
Qué pasó: al hacer git add/commit me salía ese error fatal.
Causa: estaba parado en C:\Users\carlo en vez de dentro de la carpeta del
       repo (flutter-bootcamp). Git busca un .git en la carpeta actual y
       no lo encontraba.
Solución: entrar con cd a la carpeta del repo antes de usar git. Aprendí a
          correr `git status` primero como brújula.

## Día 0 — Llave SSH / commits en la cuenta de GitHub equivocada
Qué pasó: tenía configurada en Git una cuenta vieja, pero el repo estaba en
          una cuenta nueva.
Causa: ya tenía GitHub en el equipo con otra cuenta/correo de antes.
Solución: reconfiguré git config con el correo de la cuenta nueva y verifiqué
          con ssh -T que GitHub me reconociera como la cuenta correcta.