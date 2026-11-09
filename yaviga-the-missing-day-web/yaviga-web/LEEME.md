# Página de The Missing Day · YAVIGA

## 1. Conectar Firebase
1. Consola de Firebase → tu proyecto → Configuración → "Tus apps" → agrega una app Web.
2. Copia el `firebaseConfig` y pégalo en `index.html` (busca "PEGA AQUÍ").
3. Authentication → Método de acceso → activa "Correo y contraseña" → pestaña Usuarios → "Agregar usuario" (tu correo y contraseña).
4. Firestore Database → Crear base de datos.
5. Storage → Comenzar (puede pedir plan Blaze; el uso pequeño sigue siendo gratis).
6. Pega el contenido de `firestore.rules` y `storage.rules` en la pestaña "Reglas" de cada uno (cambia TU_CORREO@gmail.com por tu correo) y publica.

## 2. Publicar la página
    npm install -g firebase-tools
    firebase login
    firebase init hosting   (carpeta pública: "."  / no sobrescribir index.html)
    firebase deploy

## 3. Subir el juego (.zip) - elige UNA
- A) Con la página: abre la web → pie de página "Acceso del equipo" → inicia sesión → "Subir zip".
- B) Pon `TheMissingDay.zip` dentro de `downloads/` antes del deploy.
- C) Súbelo a itch.io, GitHub Releases o Google Drive y pega el enlace en el panel.

## 4. Logo e imagen
Ya vienen cargados. Para cambiarlos, entra al panel y usa "Subir logo" / "Subir imagen".

## 5. Visitas y reseñas
- Las visitas (una por sesión) y los clics en "Descargar" se cuentan en `site/stats`; los ves en el panel, en "Estadísticas".
- Las reseñas (nombre, 1-5 estrellas, comentario) se guardan en `reviews`. Tú las quitas desde el panel o la propia página.
- IMPORTANTE: vuelve a pegar `firestore.rules` en Firebase y publica, porque cambió.
