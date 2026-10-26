# orca

## META
- id: orca
- owner: EduBalderas
- visibility: public
- idioma: en
- estado: estable
- tipo: fork
- nivel: L3
  - L0=gobernanza/política
  - L1=marca/metodología
  - L2=flujo/arquitectura
  - L3=producto ejecutable
  - L4=herramienta
- familia: ninguna
- origen: upstream:https://github.com/stablyai/orca
- experimento: desconocido
- nacido_de: stablyai/orca
- orquestado_por: N/A
- brief_desde: N/A

## OBJETIVO
IDE de escritorio para desarrollo agéntico en paralelo: ejecuta agentes de programación por CLI, cada uno en su worktree, en escritorio, móvil y runtime remoto, con la suscripción del usuario.

## QUE_CONTIENE
- App de escritorio Electron (`electron` 43.7.5) en `src/main`, `src/renderer` y `src/preload`, más el CLI `orca` (`package.json` `bin`, `src/cli`). Versión del paquete: 1.4.214. Descripción del paquete: «Next-gen IDE for parallel agentic development». Autor del paquete: stablyai.
- App móvil `orca-mobile` en `mobile/` (workspace pnpm propio; scripts Expo para iOS y Android).
- Relay que empareja el móvil con el host de escritorio, en `cloud/` (workspace pnpm aparte): `apps/relay`, `apps/push` y contratos en `cloud/packages/`.
- Módulos nativos en `native/`, recursos en `resources/`, documentación en `docs/` (sitio y READMEs traducidos en `docs/readme/`).
- Skills de agente en `skills/`, `skill-guides/` y `skill-stubs/`.
- Tests en `tests/` y scripts de build, lint y typecheck en `config/`.
- Licencia MIT (`LICENSE`); copyright 2026 Lovecast Inc.
- Lenguaje principal según GitHub: TypeScript.

## CARACTERISTICAS
- Orquesta agentes CLI en paralelo, cada uno en un worktree git aislado (README del árbol y `AGENTS.md`).
- Sirve cualquier agente que corra en terminal. El README nombra, entre otros, Claude Code, Codex, Grok, Cursor, GitHub Copilot, OpenCode y Pi, y deja el resto como «any CLI agent».
- Terminales con splits, worktrees remotos por SSH, y flujos de GitHub y Linear dentro de la app (documentados en el README).
- Compañero móvil para seguir agentes y enviar seguimiento; el relay de `cloud/` une móvil y escritorio.
- CLI `orca` para automatizar flujos del propio producto (bin del `package.json`).
- Escritorio en macOS, Windows y Linux (README y `AGENTS.md`).
- El README upstream describe descargas de escritorio, cask de Homebrew `stablyai/orca/orca` y paquete AUR `stably-orca-bin`. Esas descargas apuntan a releases de `stablyai/orca`, no de este fork.

## FUERA_DE_ALCANCE
- Este fork no publica releases ni instaladores (`gh release list` vacío). La distribución citada en el README es la del upstream.
- No incluye suscripciones a modelos ni a agentes: la descripción upstream dice que cada agente corre con la suscripción del usuario.
- No hay en el árbol una lista explícita de exclusiones de producto más allá de eso. N/A.

## RELACIONES
- Fork público de https://github.com/stablyai/orca (`isFork`: true; parent `stablyai/orca`). Creado en GitHub el 2026-10-13.
- Homepage del fork en GitHub: https://onOrca.dev. Homepage en `package.json`: https://github.com/stablyai/orca.
- Descripción del fork en GitHub: entorno de desarrollo agéntico (ADE) para varios agentes en paralelo, en escritorio, móvil y ejecución remota.
- Descripción upstream: flota de agentes (p. ej. Grok Bot, Claude Code) con la suscripción propia del usuario; escritorio, móvil y runtime remoto. Sitio upstream declarado: https://orca.dev.
- Comunidad enlazada en el README: Discord https://discord.gg/fzjDKHxv8Q y X https://x.com/orca_build.
- Topics del upstream `stablyai/orca` (este fork no tiene topics): claude-code, codex, ghostty, terminal, opencode, orchestration, worktrees, pi, ade, mobile-app, agent-ide, ai-agents, yc-backed, automation, bot, grok-bot, hermes-agent, muse, openclaw, runtime.
- Familia sdf, agentability o gentle-ai: no aparece en el repo. N/A.

## ETIQUETAS
- fork
- ide
- electron
- typescript
- agentes-cli
- worktrees
- mit
- desktop
- mobile

## TOPICS_GITHUB
- N/A
