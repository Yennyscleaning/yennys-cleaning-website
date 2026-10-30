# Sitio web de Yenny's Cleaning, LLC — Netlify + Decap CMS

Sitio estático con panel de edición. La página (`index.html`) lee sus textos de
`content.json`; si ese archivo no carga, muestra los mismos textos incrustados
como respaldo. El logo está en `assets/logo.png`.

## Pasos que faltan para ponerlo en línea

1. **Crear el repositorio en GitHub.** En github.com, crea un repositorio nuevo
   (por ejemplo `yennys-cleaning-sitio`), rama principal `main`, y sube todos
   los archivos de esta carpeta, tal cual, en la raíz del repositorio.
2. **Conectar el repositorio en Netlify.** En netlify.com: Add new site →
   Import an existing project → GitHub → elige el repositorio. No hay comando
   de construcción: publica la carpeta tal cual (sin build command ni carpeta
   de salida especial).
3. **Activar Netlify Identity + Git Gateway.** En el sitio de Netlify:
   Site configuration → Identity → Enable Identity. Luego Identity →
   Services → Git Gateway → Enable Git Gateway. Esto es lo que permite que el
   panel guarde cambios en el repositorio.
4. **Invitar a la usuaria.** En Identity → Invite users, envía la invitación al
   correo del negocio. Al aceptarla, podrá entrar al panel en
   `https://<tu-sitio>.netlify.app/admin` y editar los textos con formularios:
   héroe, franja de confianza, servicios, sección comercial, historia y
   contacto. Cada cambio guardado se publica solo en el sitio.
5. **Cuando esté aprobado, conectar el dominio** (por ejemplo
   yennyscleaningllc.com) desde Netlify: Domain management → Add a domain.
   Hasta entonces, el sitio lleva la franja de "borrador" en la parte superior;
   quita ese texto en `content.json` (campo "Aviso de borrador") cuando ya no
   sea borrador.

## Notas

- No hay sección de misión, visión y valores en esta versión (pendiente de
  decisión de la dueña).
- La frase de la sección comercial sobre move-outs en 48–72 horas viene del
  borrador aprobado; si la dueña prefiere no prometerla en el sitio, se quita
  editando ese punto en el panel.
- El sitio de Wix y el borrador en Muse no se tocan con este proyecto.
