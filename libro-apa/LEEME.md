# Libro en APA 7 (español)

## Subir a Overleaf
1. En Overleaf: **New Project → Upload Project** y selecciona `libro-apa.zip`.
   (O crea un proyecto en blanco y sube estas carpetas y archivos tal cual.)
2. Menú → Compiler: **pdfLaTeX**. Archivo principal: `main.tex`.

## Dónde escribir
| Qué | Archivo |
|---|---|
| Color (`azul` o `verde`) | `main.tex`, línea `\newcommand{\tema}{azul}` |
| Título, ISBN, editorial, año | `datos.tex` |
| Autores y afiliaciones | `preliminares/portadilla.tex` |
| Resumen, Abstract, Prólogo, Agradecimientos | `preliminares/` |
| Capítulos | `capitulos/` (uno por archivo; se agregan en `main.tex`) |
| Referencias | `referencias.bib` |

## APA rápido
- `\textcite{clave}` → Apellido (2024)  ·  `\parencite{clave}` → (Apellido, 2024)
- `\parencite[p.~45]{clave}` → (Apellido, 2024, p. 45)
- Tabla/figura: `\caption{...}` **antes** del contenido y `\nota{...}` al final.
- Cita de 40+ palabras: `\begin{citalarga} ... \end{citalarga}`
- La lista de Referencias se arma sola con las fuentes citadas.

En `capitulos/01-generalidades.tex` hay un ejemplo de cada cosa.
