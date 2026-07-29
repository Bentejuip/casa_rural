# Casa Salvador — web

Web estática (HTML/CSS/JS) para reservas directas de Casa Salvador, casa rural en Risco Blanco, San Bartolomé de Tirajana, Gran Canaria.

## Antes de publicar, sustituye:

1. **Fotos y vídeo** — reemplaza los bloques `.img-placeholder` en `index.html` por tus imágenes reales dentro de `assets/img/`. Ejemplo:
   ```html
   <div class="img-placeholder"><img src="assets/img/salon.jpg" alt="Salón" style="width:100%;height:100%;object-fit:cover"></div>
   ```
   Para el vídeo de fondo del hero, sustituye el bloque `<svg class="hero__scape">` por:
   ```html
   <video autoplay muted loop playsinline src="assets/img/hero.mp4"></video>
   ```

2. **WhatsApp** — busca `34600000000` en `index.html` (aparece 3 veces) y cámbialo por tu número real, formato internacional sin espacios ni `+`.

3. **Formulario de reservas (Formspree)** — crea una cuenta gratis en [formspree.io](https://formspree.io), crea un formulario y sustituye `TU-ID` en el atributo `action` del `<form>` por el ID que te den.

4. **Google Analytics** — crea una propiedad GA4 en [analytics.google.com](https://analytics.google.com) y sustituye `G-XXXXXXXXXX` (aparece 2 veces en el `<head>`) por tu ID de medición real.

5. **Mapa** — sustituye la URL del `<iframe>` de Google Maps por la de tu ubicación exacta (Google Maps → Compartir → Insertar un mapa).

6. **Reseñas de Google** — el bloque `.reviews-placeholder` está pensado para sustituirlo por un widget (Trustindex/Elfsight) o por tu propia integración con la API de Google Places.

7. **Email de contacto** — cambia `reservas@casasalvador.com` en el footer por tu email real.

## Publicar en GitHub Pages

1. Sube este contenido a un repositorio en GitHub (puede llamarse `casa-salvador` o el nombre que prefieras).
2. En el repo, ve a **Settings → Pages**.
3. En "Source", selecciona la rama `main` y la carpeta `/ (root)`.
4. Guarda — en 1-2 minutos tu web estará en `https://tu-usuario.github.io/casa-salvador/`.
5. Cuando compres un dominio propio, en la misma pantalla de Pages puedes añadirlo en "Custom domain" y configurar los registros DNS que te indique GitHub.

## Aviso de cookies (RGPD)

Como usas Google Analytics, necesitas un banner de consentimiento de cookies. No está incluido todavía — se puede añadir con una librería gratuita como [CookieConsent](https://github.com/orestbida/cookieconsent) cuando quieras.
