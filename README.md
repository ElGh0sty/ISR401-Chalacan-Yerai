# Ingeniería de Requerimientos (ISR-401) — Período 2026-2027 SPA

Repositorio personal de actividades y evaluaciones de la asignatura **Ingeniería de Requerimientos**.

## Estructura de `EV-PRAC-01`

```text
├── README.md
└── EV-PRAC-01/
    ├── main.tex
    ├── main.pdf
    └── evidencias/
        ├── hoja-01.jpeg
        ├── hoja-02.jpeg
        └── hoja-03.jpeg
```

## Instrucciones de compilación reproducible (`EV-PRAC-01`)

Para generar el documento `main.pdf` a partir del código fuente LaTeX tras clonar el repositorio:

* **Compilador:** `pdflatex` (distribución TeX Live 2023 o superior / MiKTeX).
* **Archivo principal:** `EV-PRAC-01/main.tex`
* **Paquetes / dependencias requeridas:**
  * `inputenc` (`utf8`)
  * `fontenc` (`T1`)
  * `babel` (`spanish`)
  * `geometry`
  * `tabularx`
  * `booktabs`
  * `graphicx`
  * `float`

### Orden de comandos de ejecución

1. Clonar el repositorio y ubicarse en la carpeta de la evaluación:
   ```bash
   git clone <URL-DEL-REPOSITORIO>
   cd <NOMBRE-DEL-REPOSITORIO>/EV-PRAC-01
   ```
2. Ejecutar `pdflatex` dos veces para resolver las referencias cruzadas y el posicionamiento de figuras:
   ```bash
   pdflatex -interaction=nonstopmode main.tex
   pdflatex -interaction=nonstopmode main.tex
   ```
3. El archivo compilado se generará en `EV-PRAC-01/main.pdf`.
