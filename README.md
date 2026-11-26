# Servicio Médico Juan Pablo II — Portal Web Estático y Normativo

Portal web oficial del **Servicio Médico Juan Pablo II** (Ejido, Municipio Campo Elías, Estado Mérida, Venezuela), diseñado para despliegue estático **100 % gratuito** bajo estándares estrictos de privacidad clínica.

## Características Principales
- **Hero 3D Parallax Multicapa:** basado en `HERO_JPII.jfif` con animación 3D interactiva, capas de fondo con suavizado inercial (`lerp`), brillo especular dinámico y estado de horario en vivo (hora oficial de Venezuela, UTC-4).
- **Botón de Despliegue con Logo Mini Extraído:** acceso rápido flotante (`Menú Clínico`) y botón de cabecera con menú Glassmorphism.
- **Dashboards Bento Grid con Glassmorphism y Gradient Mesh:** degradación cromática derivada directamente del Hero (`#000F35 → #012248 → #01517B → #1EE3FF`).
- **Botones Neumorphism Suaves:** geometría redondeada en el tono de fondo del Hero (`#062D55`) con relieve dual y estado presionado cóncavo.
- **Asistente Privado de Citas (Cero Almacenamiento):** arma el mensaje localmente en el dispositivo del paciente y abre WhatsApp Business (`+58 424-7225404`) sin guardar ningún dato en servidores.

## Stack Open-Source Gratuito y Verificado en GitHub
- [`darkroomengineering/lenis`](https://github.com/darkroomengineering/lenis) (MIT) — Scroll suave inercial (carga progresiva).
- [`Leaflet/Leaflet`](https://github.com/Leaflet/Leaflet) (BSD-2-Clause) + OpenStreetMap — Mapa interactivo gratuito de Ejido, Mérida con fallback SVG offline.
- [`lucide-icons/lucide`](https://github.com/lucide-icons/lucide) (ISC) — Estilo iconográfico SVG inline sin bloqueo de renderizado.
- Metodología y auditoría alineadas con [`github/spec-kit`](https://github.com/github/spec-kit), [`dequelabs/axe-core`](https://github.com/dequelabs/axe-core), [`biomejs/biome`](https://github.com/biomejs/biome) y [`semgrep/semgrep`](https://github.com/semgrep/semgrep).

## Despliegue Gratuito en GitHub Pages
1. Sube esta carpeta a un repositorio en GitHub con rama principal `main`.
2. En **Settings → Pages**, selecciona **Source: GitHub Actions**.
3. El flujo `.github/workflows/deploy-pages.yml` ejecutará la auditoría pre-despliegue y publicará el portal automáticamente.

> Si prefieres desplegar un único archivo sin la carpeta `assets/`, renombra `index-autocontenido.html` a `index.html`.
