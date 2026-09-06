# CareerOS AI Starter

Un sistema gratuito y open source para convertir experiencia profesional real en mejores decisiones de carrera, aplicaciones e historias de entrevista con IA.

Creado por [Andrés Castañaza](https://andres.castanaza.com) como recurso público de [AI Career Systems](https://andres.castanaza.com/ai-career-systems).

## Qué incluye

- **Career Profile Builder:** construye un perfil profesional maestro basado en evidencia.
- **Job Fit Analyzer:** compara tu perfil con una vacante y entrega un *estimated fit score*, brechas, keywords y recomendación Apply / Maybe / Skip.
- **STAR Story Builder:** transforma experiencias reales en historias conductuales listas para entrevista.
- [Prompts universales](plugins/careeros-ai-starter/prompts/prompts-universales.md) para usar con la IA que prefieras.
- [Plantillas editables](plugins/careeros-ai-starter/templates/) para perfil, análisis de vacantes, historias STAR y seguimiento de aplicaciones.

CareerOS no promete “ganarle al ATS” ni conseguir entrevistas automáticamente. Su objetivo es ayudarte a decidir y comunicar mejor sin inventar experiencia, métricas o credenciales.

## Usarlo sin instalar nada

1. Descarga el repositorio como ZIP.
2. Abre los [prompts universales](plugins/careeros-ai-starter/prompts/prompts-universales.md).
3. Copia el prompt que necesites en ChatGPT, Codex u otra IA.
4. Sustituye los campos entre corchetes con tu información.
5. Revisa cada afirmación antes de usarla.

[Descargar versión universal](https://github.com/aplus89/careeros-ai-starter/archive/refs/heads/main.zip)

## Instalar como plugin de Codex

El repositorio contiene un marketplace en `.agents/plugins/marketplace.json` y el plugin en `plugins/careeros-ai-starter/`.

### Codex CLI

```bash
codex plugin marketplace add https://github.com/aplus89/careeros-ai-starter
codex plugin add careeros-ai-starter@careeros-ai
```

Después de instalarlo, inicia una conversación nueva y pide una de estas tareas:

- `Build my master professional profile.`
- `Compare my profile with this job.`
- `Turn my experience into STAR stories.`

### ChatGPT Work / equipos

Un administrador puede ir a **Admin → Plugins → Add → Import marketplace**, usar `https://github.com/aplus89/careeros-ai-starter` como Source y dejar Path vacío. La disponibilidad depende del plan y de las políticas del workspace.

## Privacidad y veracidad

Este paquete no incluye servidor, base de datos, analytics ni código de carga de archivos. Tus datos se procesan según las condiciones de la IA donde decidas usarlo. Lee [PRIVACY.md](PRIVACY.md) y evita compartir información sensible innecesaria.

Reglas centrales:

- No inventar experiencia, fechas, métricas, certificaciones, títulos ni herramientas.
- Distinguir hechos confirmados, evidencia faltante y experiencia transferible.
- Presentar el match como estimado, no como el score real de un ATS.
- Revisar humanamente todo resultado antes de aplicarlo.

## Estructura

```text
.agents/plugins/marketplace.json
plugins/careeros-ai-starter/
├── .codex-plugin/plugin.json
├── skills/
│   ├── career-profile-builder/SKILL.md
│   ├── job-fit-analyzer/SKILL.md
│   └── star-story-builder/SKILL.md
├── prompts/prompts-universales.md
└── templates/
```

## Licencia

[MIT](LICENSE). Puedes usar, adaptar y compartir el material conservando el aviso de licencia.

---

## English

CareerOS AI Starter is a free, open-source, evidence-based career workflow. It helps you build a master professional profile, estimate fit for a specific job, and prepare truthful STAR interview stories. The skills work in English or Spanish and never authorize fabricated experience, metrics, or credentials.
