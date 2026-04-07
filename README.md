# research-skills-template

Una plantilla de skills de Claude Code para proyectos de investigación en AI safety.

Originalmente compilada para "Technical AI Safety Projects" de [BAISH](https://baish.com.ar/), Abril-Mayo 2026.

## Setup

1. Clonar este repo
2. Abrir el proyecto en Claude Code
3. Los skills en `.claude/commands/` están disponibles automáticamente como slash commands

## Skills disponibles

| Comando | Descripción |
|---------|-------------|
| `/brainstorm` | Explorar direcciones de investigación en AI safety de forma interactiva |
| `/evaluate-idea` | Puntuar y refinar una idea de investigación colaborativamente |
| `/literature-review` | Mapear el panorama de AI safety para un tema |
| `/research-topic` | Analizar papers en un tema específico |
| `/novelty-check` | Verificar si una idea es novedosa |
| `/runpodctl` | Administrar compute en RunPod (pods, templates, etc.) |

## Requisitos

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) instalado
- Cuenta en RunPod con API key (solo para `/runpodctl`)

## Workflow sugerido

1. `/brainstorm` para explorar ideas y constraints del proyecto
2. `/literature-review` para entender qué existe en el área
3. `/evaluate-idea` para formalizar y puntuar la idea
4. `/novelty-check` para verificar que la pregunta esté abierta
5. `/runpodctl` te levanta compute cuando estés listo para jugar