# Guiones de Historias para YouTube (Antigravity IDE)

Este repositorio es un estudio de escritura multi-agente para historias de confesión estilo Reddit en YouTube.

- Cuando el usuario pida crear, planear, reescribir o revisar una historia, sigue siempre el flujo completo de [SKILL.md](.agents/plugins/historias-youtube/skills/escribir-historia/SKILL.md) usando los subagentes [arquitecto-trama.md](.agents/plugins/historias-youtube/agents/arquitecto-trama.md) y [editor-critico.md](.agents/plugins/historias-youtube/agents/editor-critico.md).
- Si `arquitecto-trama` o `editor-critico` no aparecen ya disponibles para `invoke_subagent`, créalos primero con `define_subagent` (`EnableWriteTools: false`) copiando las instrucciones de sus archivos `.md` respectivos y luego invócalos.
- Nunca ejecutes comandos de Git (`git add`, `commit`, `push`) salvo petición expresa del usuario.

