<p align="center">
  <img src="https://is.wuaze.com/static/icon/Icon.png" width="120" alt="AnimeAV1 Logo">
</p>

<h1 align="center">AnimeAV1 API</h1>

<p align="center">
  🎌 Anime API · Jikan/MAL · SUB & DUB · JSON
</p>

<p align="center">
  <a href="https://www.mushoku.eu.cc/">
    <img src="https://img.shields.io/badge/API-Online-ff6b9d?style=for-the-badge" alt="API Online">
  </a>
  <a href="https://www.php.net/">
    <img src="https://img.shields.io/badge/PHP-Native-777bb4?style=for-the-badge&logo=php&logoColor=white" alt="PHP Native">
  </a>
  <img src="https://img.shields.io/badge/License-Custom-ff9f43?style=for-the-badge" alt="Custom License">
</p>

<p align="center">
  <strong>AnimeAV1</strong> es una API ligera de anime creada para proyectos, aplicaciones y sitios relacionados con anime.
</p>

<p align="center">
  <a href="https://www.mushoku.eu.cc/">🌐 API</a> ·
  <a href="https://github.com/iloveddev/mus/tree/main/api">📚 Documentación</a> ·
  <a href="https://github.com/iloveddev/mus/issues">🐛 Reportar problema</a>
</p>

---

# 🎉 AnimeAV1 API v1.0.0

> Primera versión pública de **AnimeAV1 API**, una API no oficial basada en AnimeAV1 - Archivo! 
• @NidivDev 
## 🚀 Características

- 📚 Catálogo de anime
- 🔎 Búsqueda por título
- 🎬 Información detallada de anime
- ▶️ Información de episodios
- 🎧 Soporte para SUB y DUB
- 🍥 Integración con MyAnimeList mediante Jikan
- 🆕 Últimos episodios y animes agregados
- 🔥 Catálogo popular
- 🔤 Navegación A-Z
- 📅 Endpoint de horario
- 🖼️ URLs de posters mediante CDN
- ⚡ Respuestas en formato JSON
- 🛡️ Rate limit por IP

## 📡 Endpoints incluidos

| Endpoint | Descripción |
|:---|:---|
| `/catalogo/` | Catálogo de anime |
| `/buscar/?q=` | Buscar anime |
| `/anime/{slug}/` | Información del anime |
| `/ep/{slug}/E{numero}/` | Información del episodio |
| `/mal/{slug}/` | Datos de MyAnimeList |
| `/ultimos/` | Últimos episodios y animes |
| `/top/` | Anime popular |
| `/az/{letra}/` | Catálogo A-Z |
| `/horario/` | Anime agrupado por día |

## 🧪 Ejemplo rápido

```http
GET /buscar/?q=kimetsu
```

Respuesta:

```json
{
  "ok": true,
  "consulta": "kimetsu",
  "pagina_actual": 1,
  "total_resultados": 1,
  "resultados": [
    {
      "id": 123,
      "titulo": "Kimetsu no Yaiba",
      "slug": "kimetsu-no-yaiba",
      "poster": "https://cdn.animeav1.com/img/media/poster/123.jpg",
      "url": "/anime/kimetsu-no-yaiba/"
    }
  ]
}
```

## ⚙️ Tecnología

- **PHP** — Backend de la API
- **AnimeAV1** — Fuente principal de datos
- **Jikan / MyAnimeList** — Información adicional
- **JSON** — Formato de respuesta
- **Apache / .htaccess** — Routing de endpoints

## 🛡️ Rate Limit

La API incorpora un límite de solicitudes por dirección IP para reducir el abuso y mantener estable el servicio.

> **30 solicitudes por minuto por IP**

## 📚 Documentación

Cada endpoint cuenta con su propia documentación:

```text
/api/
├── catalogo/
├── buscar/
├── anime/
├── ep/
├── mal/
├── ultimos/
├── top/
├── az/
└── horario/
```

## 📦 Estado del Release

**v1.0.0 · Initial Release**

Primera versión pública de **AnimeAV1 API**, incluyendo la estructura inicial de endpoints, sistema de scraping, integración con Jikan y protección mediante rate limiting.

## ⚠️ Aviso

AnimeAV1 API es un proyecto **no oficial** y no está afiliado, patrocinado ni respaldado oficialmente por AnimeAV1, MyAnimeList o Jikan.

Los datos dependen de servicios externos y pueden cambiar sin previo aviso.

---

<p align="center">
  🎌 <strong>AnimeAV1 API v1.0.0</strong><br>
  <sub>Initial Release · API no oficial</sub>
</p>
 
