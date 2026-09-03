# Chat Público en Tiempo Real

Aplicación web sencilla de chat público. Cualquier persona puede entrar usando solamente un nombre.

## Importante

GitHub Pages puede publicar el HTML, pero **no puede funcionar como servidor de chat en tiempo real por sí solo**. Esta versión usa **Firebase Firestore** como backend.

## Configuración

1. Entra a Firebase Console y crea un proyecto.
2. Crea una aplicación web.
3. Activa **Firestore Database**.
4. Copia la configuración de Firebase que te proporciona Firebase.
5. Abre `index.html` y reemplaza los valores de `firebaseConfig`.
6. Configura las reglas de Firestore para permitir lectura y escritura del chat.
7. Sube `index.html` a un repositorio de GitHub.
8. Activa GitHub Pages desde Settings → Pages.

## Comportamiento

- No hay registro ni contraseña.
- Cada visitante escribe un nombre cualquiera.
- Todos ven los mensajes en tiempo real.
- Los mensajes antiguos se eliminan de la pantalla cuando se desplaza hacia arriba.
- Se mantienen como máximo 60 mensajes visibles en cada navegador.
- Los mensajes siguen almacenados en Firestore hasta que configures una política de borrado.

## Seguridad

Para una aplicación pública real conviene añadir límites anti-spam, moderación y reglas de Firestore más estrictas. No pongas claves privadas de servidor dentro del HTML.
