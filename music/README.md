# 🎵 Mi Music Player

Reproductor MP3 estático para GitHub Pages.

## Estructura

```text
mi-reproductor/
├── index.html
├── music/
│   ├── cancion1.mp3
│   └── cancion2.mp3
└── covers/
    ├── cancion1.jpg
    └── cancion2.jpg
```

## Agregar canciones

Abre `index.html` y busca:

```js
const songs = [
];
```

Agrega tus canciones así:

```js
const songs = [
  {
    title: "Mi canción",
    artist: "Mi artista",
    file: "music/mi-cancion.mp3",
    cover: "covers/mi-cancion.jpg"
  },
  {
    title: "Otra canción",
    artist: "Otro artista",
    file: "music/otra-cancion.mp3",
    cover: "covers/otra-cancion.jpg"
  }
];
```

La portada es opcional. Puedes quitar `cover` si no tienes imagen.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo.
2. Sube `index.html`, la carpeta `music` y la carpeta `covers`.
3. En GitHub abre **Settings → Pages**.
4. Selecciona `Deploy from a branch`.
5. Elige `main` y `/ (root)`.
6. Guarda.

Después de unos minutos tendrás tu reproductor online.

## Importante

Los MP3 incluidos en el repositorio serán accesibles públicamente. Usa solamente música que tengas derecho a distribuir.
