# Guía Optimizada y Flujo de Trabajo para Google Antigravity (Auditoría GitHub 2026)

> **Propósito:** Directrices de ingeniería agéntica ajustadas y auditadas en tiempo real contra GitHub para construir, verificar y desplegar el portal estático del **Servicio Médico Juan Pablo II** (y futuros proyectos web) usando exclusivamente **repositorios gratuitos, activos y de mayor confianza comunitaria**.

---

## 🔍 Auditoría Real en GitHub del Stack Original

Al verificar los repositorios de la versión previa directamente vía GitHub API (`gh repo view`), se detectaron cambios críticos de mantenimiento:

| Herramienta original | Estado real en GitHub | Diagnóstico | Reemplazo recomendado (100 % gratuito y activo) |
| :--- | :--- | :--- | :--- |
| `gsd-build/get-shit-done` | **Archivado** (`isArchived: true`, mayo 2026, 64.1k ★) | Sin mantenimiento (también se archivó `gsd-2`). | **[`github/spec-kit`](https://github.com/github/spec-kit)** (151.5k ★ · MIT · Activo) |
| `RooCodeInc/Roo-Code` | **Archivado** (`isArchived: true`, mayo 2026, 24.2k ★) | Proyecto archivado. | **[`cline/cline`](https://github.com/cline/cline)** (71.9k ★ · Apache-2.0 · Activo) |
| `abhishekbhakat/ralph-loop-for-antigravity` | Activo, pero solo **67 ★** (último push mar. 2026) | Baja adopción y auditoría comunitaria. | Comandos nativos de Antigravity (`/goal`, `/plan`, `/teamwork`) + bucle automatizado de tests verificables |
| `coderabbit.ai` | SaaS freemium (limitado en repos privados) | No es 100 % open-source local. | **[`The-PR-Agent/pr-agent`](https://github.com/The-PR-Agent/pr-agent)** (16.7k ★ · MIT) + **[`semgrep/semgrep`](https://github.com/semgrep/semgrep)** (18.0k ★) + **[`biomejs/biome`](https://github.com/biomejs/biome)** (26.2k ★) |

---

## 🛠️ Stack Open-Source Gratuito y de Mayor Confianza para la Construcción Web

Todos los repositorios siguientes son gratuitos, de licencia permisiva y alta confianza en GitHub:

### 1. Metodología, Calidad y Auditoría Pre-Commit
- **Especificación y Planificación (SDD):** [`github/spec-kit`](https://github.com/github/spec-kit) — 151.5k ★ · MIT · Desarrollo guiado por especificaciones (*Planificar → Ejecutar → Verificar*).
- **Linting y Formateo ultrarrápido:** [`biomejs/biome`](https://github.com/biomejs/biome) — 26.2k ★ · Apache-2.0/MIT.
- **Seguridad Estática (SAST):** [`semgrep/semgrep`](https://github.com/semgrep/semgrep) — 18.0k ★ · LGPL-2.1.
- **Accesibilidad Clínica (WCAG 2.1 AA):** [`dequelabs/axe-core`](https://github.com/dequelabs/axe-core) — 7.9k ★ · MPL-2.0.
- **Rendimiento y SEO:** [`GoogleChrome/lighthouse`](https://github.com/GoogleChrome/lighthouse) — 31.2k ★ · Apache-2.0.
- **Revisión de PRs Open-Source:** [`The-PR-Agent/pr-agent`](https://github.com/The-PR-Agent/pr-agent) — 16.7k ★ · MIT.

### 2. Construcción Frontend 3D Parallax, Glassmorphism, Mapas e Iconografía
- **Scroll suave inercial (Parallax fluido):** [`darkroomengineering/lenis`](https://github.com/darkroomengineering/lenis) — 17.5k ★ · MIT · Activo.
- **Inclinación 3D y reflejo especular:** [`micku7zu/vanilla-tilt.js`](https://github.com/micku7zu/vanilla-tilt.js) — 4.0k ★ · MIT (y su física `lerp` integrada de forma nativa sin bloqueo).
- **Motor de animaciones ligeras:** [`juliangarnier/anime`](https://github.com/juliangarnier/anime) — 75.1k ★ · MIT · Activo.
- **Mapas interactivos gratuitos (sin API key ni tarjeta):** [`Leaflet/Leaflet`](https://github.com/Leaflet/Leaflet) — 46.0k ★ · BSD-2-Clause · Activo (con tiles gratuitos de OpenStreetMap).
- **Iconografía SVG consistente:** [`lucide-icons/lucide`](https://github.com/lucide-icons/lucide) — 26.0k ★ · ISC · Activo.
- **Despliegue estático 100 % gratuito:** GitHub Pages + GitHub Actions (`actions/deploy-pages`).

---

## 🤖 Instrucciones del Sistema para Antigravity (Versión Ajustada)

*Reglas operativas listas para copiar en el System Prompt / `AGENTS.md` del proyecto:*

```markdown
# Directrices de Ingeniería Autónoma, Calidad y Cumplimiento Clínico

Actúa como un agente de ingeniería de software autónomo siguiendo estrictamente estas 5 reglas operativas:

## 1. Arquitectura Guiada por Especificaciones (Estándar Spec-Kit)
- **Divide y vencerás:** Desglosa cada requerimiento en fases pequeñas, verificables y atómicas.
- **Ciclo obligatorio por fase:**
  1. **Planificar:** Define archivos, contratos de UI y criterios de aceptación antes de editar.
  2. **Ejecutar:** Implementa únicamente el alcance de la fase actual sin romper funcionalidades previas.
  3. **Verificar:** Valida con pruebas reales (sintaxis JS, renderizado desktop/móvil sin overflow, controles interactivos y accesibilidad) antes de avanzar.
- **Higiene de contexto:** Mantén el código modular, documentado y sin dependencias pesadas ni repositorios archivados.

## 2. Continuidad y Resiliencia (Bucle Verificable)
- **Persistencia hasta el objetivo:** Ante errores de renderizado, solapamiento 3D, desbordamiento móvil o fallos de scripts, diagnostica la causa raíz en navegador real, corrige y vuelve a verificar hasta pasar el 100 % de los controles.
- **Degradación elegante (Progressive Enhancement):** Toda librería externa opcional (p. ej. Lenis o Leaflet) debe degradar limpiamente si el entorno es offline o tiene CSP restrictivo, sin generar errores en consola.

## 3. Gestión de Recursos y Rendimiento Web
- Optimiza imágenes en WebP con dimensiones explícitas (`width`/`height`) y evita bloquear el primer renderizado.
- Respeta siempre `prefers-reduced-motion` en animaciones 3D y efectos parallax.
- Prioriza librerías open-source activas, gratuitas y de licencia permisiva (MIT, Apache-2.0, BSD, ISC).

## 4. Auditoría Pre-Commit (Seguridad, Accesibilidad y Calidad)
Antes de concluir cualquier cambio o crear un commit, verifica obligatoriamente:
- **Seguridad:** Cero credenciales expuestas, cero `innerHTML` con entradas no sanitizadas (anti-XSS), `rel="noopener noreferrer"` en todos los enlaces `target="_blank"`, y políticas de privacidad estrictas.
- **Privacidad Clínica (Servicio Médico Juan Pablo II):** Cero almacenamiento de historiales o datos personales/médicos en servidores web; agendamiento exclusivo vía canales directos encriptados (WhatsApp Business) y avisos obligatorios de emergencias visibles en cabecera y pie de página.
- **Accesibilidad (estándar axe-core / WCAG 2.1 AA):** Un único `<h1>`, jerarquía semántica (`header`, `nav`, `main`, `section`, `footer`), `aria-label`/`aria-expanded` consistentes, foco visible por teclado y alto contraste.
- **Calidad visual:** Cero desbordamiento horizontal en 390 px (móvil) y 1440 px (escritorio), cero errores de consola.

## 5. Despliegue Estático Gratuito
- Mantén compatibilidad 100 % con hosting estático gratuito (GitHub Pages / Netlify / Cloudflare Pages), incluyendo flujo CI/CD reproducible (`.github/workflows/deploy-pages.yml`) y soporte PWA básico (`manifest.webmanifest`).
```