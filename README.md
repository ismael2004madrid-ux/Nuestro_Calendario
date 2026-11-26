# Nuestro Calendario

Web mobile-first para recuerdos compartidos. Publicada con GitHub Pages y conectada al proyecto Supabase de Nuestro Jardín.

## Funcionamiento

- La página muestra un calendario mensual y los álbumes asociados a cada fecha.
- Cualquier visitante que conozca la dirección de GitHub Pages puede consultar los recuerdos y añadir fotografías sin iniciar sesión.
- El acceso habitual se realiza desde el enlace de WordPress, cuya entrada está restringida por separado.
- La restricción de WordPress no bloquea el acceso directo a la dirección pública de GitHub Pages.

## Estructura

- `index.html`: calendario, álbumes, modal, formulario de subida y carrusel de recuerdos florales.
- `assets/Plataforma estelar entre nubes doradas copia.png`: fondo original.
- `assets/289b8d2dad2ec024807e4cab0375d405.gif`
- `assets/6723f53890d821aefdd3f3c2a4ed4c09.gif`
- `assets/163328.gif`: GIF originales utilizados en la página.

## Supabase

La página utiliza:

- Tablas `calendar_albums` y `calendar_photos`.
- Bucket público `calendar-photos`.
- Clave publicable de Supabase en el frontend; no se incluye ninguna clave secreta.

La lectura y la subida están habilitadas para visitantes anónimos. El bucket admite imágenes JPEG, PNG, WebP y GIF, con un límite de 15 MB por archivo. No se requiere crear cuentas ni iniciar sesión.

**Importante:** la dirección de GitHub Pages es pública. La restricción de acceso configurada en WordPress no se hereda en GitHub Pages ni en Supabase.

## Publicación

En GitHub: Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
