<!--
PLANTILLA — copiar a /watches/<aaaa-mm>.md y rellenar.
Sustituir todos los {{placeholders}}. Borrar este comentario antes de publicar.
-->

![Notes on SLM — {{Mes AAAA}}](../assets/header-{{aaaa-mm}}.svg)

# Notes on SLM — {{Mes AAAA}}

> **TL;DR del mes.** {{Tres líneas que sintetizan la observación del
> mes. Una tendencia, no un resumen. Si no hay tendencia clara, dilo
> ("Mes disperso, sin patrón claro entre las lecturas").}}

**Contenido:** [Lecturas](#lecturas) · [Lo que no entra](#lo-que-no-entra-este-mes) · [Pregunta abierta](#pregunta-abierta)

---

## Lecturas

### 1. {{Título de la entrada}}

![tipo](https://img.shields.io/badge/tipo-{{paper|release|regulación|blog}}-555555)
![naturaleza](https://img.shields.io/badge/naturaleza-{{real|teórico}}-555555)
![origen](https://img.shields.io/badge/origen-{{Europa|EE.UU.|otro}}-555555)
![tema](https://img.shields.io/badge/tema-{{evaluación|gobernanza|despliegue|...}}-555555)

**Por qué importa.** {{3-4 líneas. Comentario propio en clave de
adopción o gobernanza. No resumen del abstract — ángulo. Sin hype.}}

**Para quién.** {{rol 1}} · {{rol 2}} · {{rol 3}}.

<details>
<summary>Cita completa y metadatos</summary>

> {{Apellido, Inicial.; Apellido, Inicial.}} ({{año}}). *{{Título
> completo}}*. {{Venue, p. ej. Findings of ACL 2026}}, pp.&nbsp;{{xxx-yyy}}.
> {{DOI o arXiv:XXXX.XXXXX}}. <{{URL persistente}}>.

```bibtex
@{{inproceedings|article|misc}}{{{cite-key}},
  author    = {...},
  title     = {...},
  booktitle = {...},
  year      = {{año}},
  url       = {{{URL}}}
}
```

</details>

---

### 2. {{Título de la entrada}}

<!-- mismo formato -->

---

### 3. {{Título de la entrada}}

<!-- mismo formato -->

---

## Lo que NO entra este mes

{{Una o dos líneas sobre lanzamientos con mucho ruido y poca señal,
con explicación corta. Sección breve, no exhaustiva. Es lo que
distingue un watch editorial de un agregador automático.}}

---

## Pregunta abierta

{{Una pregunta concreta para invitar conversación. La misma que cierra
el post LinkedIn asociado al watch del mes.}}

---

<!--
OPCIONAL — diagrama Mermaid sólo cuando el mes tenga cluster temático
real entre las entradas. Si no aporta, borrar este bloque entero.

```mermaid
graph LR
  A[{{tendencia o tema central}}] -->|enfoque empírico| P1[Entrada 1]
  A -->|enfoque comparativo| P2[Entrada 2]
  R1[{{release relacionado}}] -.contexto.-> A
```
-->

*Watch anterior: [{{Mes anterior AAAA}}](./{{aaaa-mm-anterior}}.md)*
*Próximo watch: {{último día laborable del mes siguiente}}*
