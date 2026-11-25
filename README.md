# mobile-qa-app-profiles

Catálogo público de perfiles de app para [mobile-qa-agent](https://github.com/fealfaro/mobile-qa-agent).

Cada carpeta es una app:

```
<app>/
  profile.yaml                              ficha: ids Android/iOS, tiendas, modo de sesión, palabras bloqueadas
  calibration/home-testing.android.yaml     selectores de la pantalla principal, revisados por una persona
  suites/home.yaml                          casos de prueba
```

## Uso

```bash
git clone https://github.com/fealfaro/mobile-qa-agent
cd mobile-qa-agent
git clone https://github.com/fealfaro/mobile-qa-app-profiles profiles
```

## Contribuir un perfil

Desde la consola web de mobile-qa-agent: buscar la app, hacer el levantamiento, revisarlo y presionar "Publicar perfil".

Reglas:
- Solo perfiles generados con un levantamiento sobre la app real y revisados por una persona (`status: reviewed`).
- Sin screenshots, evidencias, credenciales ni datos personales. La herramienta bloquea la publicación si los detecta.
- Las pruebas son de lectura o de navegación no transaccional.
