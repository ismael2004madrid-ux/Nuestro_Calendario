# Nuestro Calendario

Web mobile-first para recuerdos compartidos. Publicada con GitHub Pages y conectada al proyecto Supabase de Nuestro Jardín.

## Estructura prevista

- `index.html`: calendario, álbumes, modal, gestión privada y carrusel de recuerdos florales.
- `assets/calendar-background.png`: fondo original.
- `assets/kirby-sunset.gif`, `assets/kirby-headphones.gif`, `assets/kirby-pink.gif`: GIF originales de Kirby.

## Supabase

Usa las tablas `calendar_albums` y `calendar_photos`, y el bucket público `calendar-photos`. La lectura es pública; la gestión requiere una cuenta autenticada. No se incluye ninguna clave secreta en el frontend.

Para habilitar la gestión, crea las dos cuentas autorizadas desde Supabase Authentication. No actives el registro público desde la web.

## Publicación

En GitHub: Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
