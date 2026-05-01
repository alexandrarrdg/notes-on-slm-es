# Notes on SLM — edición en castellano

![cadencia](https://img.shields.io/badge/cadencia-mensual-555555)
![ámbito](https://img.shields.io/badge/ámbito-Small%20Language%20Models-555555)
![idioma](https://img.shields.io/badge/idioma-castellano-555555)
[![english edition](https://img.shields.io/badge/english%20edition-notes--on--slm--en-555555)](https://github.com/alexandrarrdg/notes-on-slm-en)
![licencia](https://img.shields.io/badge/licencia-CC%20BY%204.0-555555)

> Notas mensuales curadas sobre **Small Language Models**: papers,
> releases, regulación y explicaciones técnicas, con comentario en
> clave de adopción y gobernanza.
>
> Por **Alexandra Rodríguez**. Parte de *Notes on AI and Data*.

---

## Índice

- [Por qué este repositorio](#por-qué-este-repositorio)
- [Qué hay aquí](#qué-hay-aquí)
- [Cómo se ve una entrada](#cómo-se-ve-una-entrada)
- [Fuentes en el radar](#fuentes-en-el-radar)
- [Ejes temáticos](#ejes-temáticos)
- [Criterio editorial](#criterio-editorial)
- [Cadencia](#cadencia)
- [Cómo seguirlo](#cómo-seguirlo)
- [Sobre la autora](#sobre-la-autora)
- [Sugerencias](#sugerencias)
- [Licencia](#licencia)

---

## Por qué este repositorio

Los Small Language Models cubren cada vez más casos de uso de
producción que antes requerían un modelo frontera. La literatura
relevante está repartida: papers en arXiv y *proceedings* de ACL,
notas de *release* de proveedores, documentación regulatoria europea
y *benchmarks* que envejecen rápido. Mantener el seguimiento mes a
mes consume tiempo, y la mayoría de listados públicos son
agregadores automáticos sin filtro editorial.

Este repositorio resuelve un problema concreto: **una sola página
al mes con tres a cinco lecturas que merecen atención y por qué**,
con cita verificable y un comentario centrado en lo que cambia
para quien tiene que adoptar — no para quien quiere estar al día
del *hype*.

## Qué hay aquí

- **Watches mensuales** (`watches/`) — selección de tres a cinco
  lecturas del mes con comentario propio. Se publica el último día
  laborable del mes.
- **Explicaciones técnicas** (`explainers/`, próximamente) — notas
  de fondo sobre conceptos recurrentes: qué es un SLM, cuándo
  destilar, cómo se evalúan estos modelos y dónde fallan los
  *benchmarks* habituales.
- **Plantillas** (`templates/`) — [`WATCH-template.md`](./templates/WATCH-template.md)
  y [`header-template.svg`](./templates/header-template.svg). Si
  alguien quiere montar su propio watch en otro tema, es libre de
  partir de aquí.

Las noticias relevantes entran en el watch del mes correspondiente.
No hay sección `news/` propia: si una noticia no pasa el filtro
mensual, no entra al repositorio.

## Cómo se ve una entrada

Cada lectura del watch sigue esta estructura fija:

```markdown
### 1. {{Título de la entrada}}

![tipo]    paper · release · regulación · blog
![naturaleza]   real · teórico
![origen]   Europa · EE. UU. · otro
![tema]    evaluación · gobernanza · despliegue · …

**Por qué importa.** {{Tres a cuatro líneas. Comentario propio en
clave de adopción o gobernanza. No resumen del abstract — ángulo.}}

**Para quién.** {{rol 1}} · {{rol 2}} · {{rol 3}}.

<details>
<summary>Cita completa y metadatos</summary>

> {{Apellido, F.; Apellido, F.}} ({{año}}). *{{Título completo}}*.
> {{Venue}}, pp. {{xxx-yyy}}. {{DOI o arXiv}}. <{{URL persistente}}>.

(BibTeX disponible al desplegar.)

</details>
```

La cita completa siempre está disponible al desplegar — la lectura
rápida queda escaneable, el rigor está debajo. Plantilla literal:
[`templates/WATCH-template.md`](./templates/WATCH-template.md).

## Fuentes en el radar

El watch mensual se construye sobre un conjunto curado de fuentes
que reviso semanalmente. No se publica todo lo que aparece — se
publica lo que pasa el filtro editorial.

**Papers y preprints**

- arXiv — categorías `cs.CL` y `cs.LG`, con búsquedas filtradas.
- Hugging Face Papers — selección diaria curada por la comunidad.
- ACL Anthology — *proceedings* de venues principales.
- Papers With Code — sección *Language Models*.

**Industria y laboratorios**

- Microsoft Research blog (familia Phi).
- Hugging Face blog.
- Mistral AI news.
- Meta AI blog.
- Google Research blog.
- Allen Institute for AI — OLMo y derivados.

**Regulación y supervisión europea**

- *EU AI Office* — comunicaciones y *codes of practice*.
- AEPD — guías y publicaciones técnicas.
- ENISA — informes sobre seguridad de IA.
- BOE — alertas filtradas por *inteligencia artificial*.

¿Falta alguna fuente? [Sugerir una fuente](https://github.com/alexandrarrdg/notes-on-slm-es/issues/new?labels=fuente-sugerida&title=Fuente+sugerida%3A+&body=URL+de+la+fuente+primaria%3A+%0A%0AQu%C3%A9+publica+%28papers%2C+releases%2C+blog%2C+regulaci%C3%B3n%29%3A+%0A%0APor+qu%C3%A9+merece+entrar+en+el+radar%3A+).

## Ejes temáticos

Los temas que aparecen recurrentemente en el watch:

- **Evaluación.** Qué miden los *benchmarks* habituales y qué se
  les escapa, especialmente fuera del inglés.
- **Despliegue on-premise.** Coste, latencia, requisitos operativos
  para entornos regulados.
- **Especialización.** *Fine-tuning*, destilación, adaptación a
  dominios verticales.
- **Soberanía tecnológica.** Modelos europeos, alternativas
  *open-source*, dependencia de proveedor.
- **Gobernanza y riesgo.** Controles, evaluación, encaje con AI
  Act, ENS y RGPD.

## Criterio editorial

Cuatro reglas aplicadas a cada entrada:

1. **Cita completa.** Autores, título, venue e identificador
   persistente (DOI, arXiv o URL estable).
2. **Real vs. teórico.** Cada entrada indica si trata sobre un
   modelo desplegado o sobre una propuesta en preprint.
3. **Europa vs. EE. UU.** Se hace explícito el origen del trabajo.
   La asimetría regulatoria entre jurisdicciones cambia el cálculo
   de adopción.
4. **Comentario en clave de adopción.** No resumen del abstract,
   sino ángulo: qué cambia esto para *data leaders*, *compliance
   officers* o arquitectos de IA.

Sin "revolucionario", sin "estado del arte", sin "*must read*".
Sin emojis decorativos.

Cada watch incluye una sección breve sobre lanzamientos del mes
con mucho ruido y poca señal, con explicación corta. Es lo que
distingue una selección editorial de un agregador automático.

## Cadencia

| Pieza | Cuándo |
|---|---|
| Watch mensual | Último día laborable del mes |
| Síntesis semestral | Junio y diciembre, como artículo largo en *Notes on AI and Data* (Medium) |
| Explicaciones técnicas | Cuando el contenido lo justifique |

## Cómo seguirlo

- **GitHub:** botón *Watch* arriba a la derecha → *Custom* →
  *Releases*. Llegan notificaciones sólo cuando hay watch nuevo.
- **LinkedIn:** la última semana del mes publico un post que
  resume el watch y enlaza a esta página.
- **RSS / Atom:** GitHub expone un feed por commits del repositorio
  en `https://github.com/alexandrarrdg/notes-on-slm-es/commits/main.atom`.
- **Notes on AI and Data (Medium):** el contenido largo y las
  síntesis semestrales viven allí.

## Sobre la autora

Trabajo en proyectos de IA aplicada en sectores regulados desde
hace varios años. Escribo mi tesis doctoral sobre gobernanza de
*Small Language Models* con un enfoque basado en riesgos.

Este repositorio es un proyecto personal, sin vínculo con ningún
empleador ni cliente. Las opiniones expresadas son mías.

## Sugerencias

¿Echas en falta una fuente, un paper o un *release* que merezca
estar en el radar?

[**Sugerir una fuente**](https://github.com/alexandrarrdg/notes-on-slm-es/issues/new?labels=fuente-sugerida&title=Fuente+sugerida%3A+&body=URL+de+la+fuente+primaria%3A+%0A%0AQu%C3%A9+publica+%28papers%2C+releases%2C+blog%2C+regulaci%C3%B3n%29%3A+%0A%0APor+qu%C3%A9+merece+entrar+en+el+radar%3A+) — abre un *Issue* con la
etiqueta y la plantilla básica ya rellenadas.

Sin recomendaciones de productos ni servicios.

## Licencia

Texto bajo [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Citas y enlaces a fuentes primarias mantienen su licencia original.
