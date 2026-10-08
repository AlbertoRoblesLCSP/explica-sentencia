# Explica sentencia

**Versión 1.03 · Tercera versión refinada**  
Autoría: [AlbertoRoblesLCSP](https://github.com/AlbertoRoblesLCSP) · Uso no comercial

**Comprender una sentencia con lenguaje claro, rigor jurídico y presentación visual.**

Una skill en español que guía a la IA para explicar qué ocurrió, qué se discutía, cómo razona el tribunal y qué decide. Distingue los hechos, las alegaciones de las partes, la doctrina expresamente formulada y el fallo.

Cuando el entorno permite crear archivos, pide un **informe HTML autocontenido**, con diseño editorial sobrio, tablas, cronologías y esquemas cuando ayudan a comprender. Puede abrirse en un navegador. Si no es posible generar HTML, utiliza Markdown estructurado.

**[Descargar la skill en ZIP](https://raw.githubusercontent.com/AlbertoRoblesLCSP/explica-sentencia/main/explica-sentencia.zip)** · [Leer sus instrucciones](explica-sentencia/SKILL.md)

## Ejemplo: sentencia sobre TRAGSA

**[Ver ejemplo visual: STS 802/2026 sobre TRAGSA](https://albertorobleslcsp.github.io/explica-sentencia/ejemplo-tragsa-STS-802-2026.html)**

Este es el último HTML compartido y revisado en el proceso de refinamiento de la skill: una explicación de la STS 802/2026 sobre el encargo a TRAGSA en Candás. Se conserva el resultado original como ejemplo del diseño y de la estructura de la explicación.

Descarga el archivo y ábrelo con tu navegador para ver su presentación visual. La vista de archivos de GitHub puede mostrar el código HTML en lugar del informe.

## Versión 1.03

Esta es la **tercera versión de la skill**, refinada tras las pruebas realizadas por su autor en ChatGPT. Los ajustes se centran en explicar con fidelidad el contenido y la naturaleza de los pronunciamientos, evitar cautelas doctrinales innecesarias y adaptar la estructura a cada sentencia, manteniendo una presentación visual profesional.

## Qué puedes darle

- Una sentencia en PDF, Word u otro documento.
- Un enlace al texto de la resolución.
- Un ECLI, ROJ, número de sentencia, tribunal u otros datos que permitan intentar localizarla.

La búsqueda de una resolución depende de las herramientas y del acceso a fuentes disponibles en la aplicación donde se utilice.

## Qué aporta

La explicación se organiza alrededor de la propia sentencia:

**Identificación → hechos → debate jurídico → razonamiento → doctrina o interpretación → fallo.**

- Explica con fidelidad el contenido y la naturaleza de cada pronunciamiento.
- Separa lo que sostiene una parte de lo que afirma el tribunal.
- Apoya los puntos relevantes en fundamentos jurídicos, apartados o páginas cuando es posible.
- Adapta la estructura a cada resolución y omite secciones que no aportan valor.
- Evita añadir automáticamente discusiones doctrinales o listas de cosas que la sentencia no dice.
- Da prioridad al rigor y la claridad sobre la decoración.

## Cómo empezar

1. Descarga **explica-sentencia.zip** mediante el enlace superior. Es el paquete de la skill; no necesitas descargar todo el repositorio.
2. Impórtalo desde la opción de añadir o importar skills de tu aplicación, si está disponible. La ubicación y disponibilidad de esa opción pueden variar según la aplicación y la cuenta. Adjuntar el ZIP a una conversación no equivale por sí solo a instalarlo.
3. Activa o selecciona **explica sentencia**, aporta la resolución y formula tu petición.

Por ejemplo:

> Usa la skill explica sentencia con el PDF adjunto. Quiero una explicación visual en HTML, con lenguaje claro y rigor jurídico, que distinga los hechos, el razonamiento, la doctrina y el fallo.

O, si tu aplicación dispone de búsqueda:

> Usa la skill explica sentencia para localizar y explicar la resolución identificada con este ECLI: [pega aquí el ECLI]. Si no accedes al texto íntegro, indícalo.

## Pruebas y compatibilidad

**Probada por su autor en ChatGPT**, incluyendo explicaciones en HTML de una sentencia sobre TRAGSA y posteriores ajustes de las instrucciones.

El núcleo de la skill es un archivo `SKILL.md` con nombre, descripción e instrucciones, siguiendo la estructura de [Agent Skills](https://agentskills.io/home). No incluye scripts ni claves de acceso.

**Esta versión no se ha probado en Claude ni en otras plataformas.** El formato permite su posible reutilización en entornos compatibles, pero la instalación, las herramientas disponibles y los resultados pueden variar. El archivo `agents/openai.yaml` contiene configuración específica de OpenAI.

La skill orienta el trabajo del modelo. La lectura de documentos, la búsqueda y la generación de archivos dependen del entorno donde se ejecute. Conviene contrastar las afirmaciones relevantes con la resolución original.

## Contenido del paquete

```text
explica-sentencia/
├── SKILL.md
├── LICENSE.md
├── VERSION
├── agents/
│   └── openai.yaml
└── assets/
    └── icon.svg
```

El ZIP y la carpeta publicada contienen la misma versión de la skill.

## Licencia

El material original se comparte bajo **Creative Commons Atribución-NoComercial 4.0 Internacional (CC BY-NC 4.0)**: puedes compartirlo y adaptarlo con reconocimiento de la autoría, enlace a la licencia e indicación de los cambios. **La licencia no autoriza el uso comercial.**

Consulta el [aviso de licencia](LICENSE.md) y el [texto legal completo](https://creativecommons.org/licenses/by-nc/4.0/legalcode.es). La licencia se aplica a los derechos que corresponden al autor sobre el material original; no altera el régimen de las resoluciones judiciales citadas ni de otros elementos de terceros.
