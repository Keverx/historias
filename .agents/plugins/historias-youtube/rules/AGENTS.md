# Reglas del Proyecto: Guiones de Historias para YouTube

Este espacio de trabajo produce historias de confesión estilo Reddit en español latinoamericano neutro para YouTube (mínimo 2,500 palabras, diseñadas para escucharse con fluidez).

## Reglas obligatorias de comportamiento

1. **Activa siempre el flujo multi-agente (`escribir-historia`):** Cada vez que el usuario pida escribir, crear, reescribir o mejorar una historia en este repositorio, lee y sigue paso a paso la skill `escribir-historia` (`.agents/plugins/historias-youtube/skills/escribir-historia/SKILL.md`).
2. **Orden estricto:**
   - Primero delega el diseño al subagente `arquitecto-trama` (mediante `invoke_subagent`).
   - Luego redacta por bloques en `historias/<slug>-<YYYY-MM-DD>.txt`.
   - Después audita el borrador completo con el subagente `editor-critico` (mediante `invoke_subagent`) hasta que responda `VEREDICTO: APROBADO`.
   - Ejecuta la verificación numérica de palabras (>= 2,500) y lista negra.
3. **Evolución continua sin copiar una historia vieja:** Nunca tomes una historia antigua fija como plantilla de estilo ni repitas el perfil de protagonista, escenario o tono de las últimas historias. Guíate por `historias/_aprendizajes.md` y `historias/_temas-usados.md`.
4. **Sin Git automático:** Nunca ejecutes `git add`, `git commit` ni `git push` al terminar una historia, a menos que el usuario lo pida de forma explícita.

