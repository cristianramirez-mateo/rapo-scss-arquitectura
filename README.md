# RAPO Creative — Arquitectura SCSS

Refactorización completa del sitio académico de RAPO Creative. Todo el diseño nace de archivos .scss; css/style.css es únicamente el resultado de la compilación.

## Sitio publicado

[Ver RAPO Creative](https://rapo-creative-bootstrap.tucenkiconstruccione.chatgpt.site)

## Estructura SCSS

    scss/
    ├── main.scss
    ├── utilities/
    │   ├── _variables.scss
    │   └── _mixins.scss
    ├── base/
    │   ├── _tipografia.scss
    │   └── _base.scss
    ├── layout/
    │   ├── _header.scss
    │   ├── _nav.scss
    │   ├── _main.scss
    │   └── _footer.scss
    ├── components/
    │   ├── _buttons.scss
    │   ├── _cards.scss
    │   ├── _lists.scss
    │   ├── _carousel.scss
    │   └── _accordion.scss
    └── pages/
        └── _responsive.scss

scss/main.scss es el único punto de entrada y utiliza @use para integrar todos los partials.

## Compilación

1. Instalar las dependencias:

       npm install

2. Compilar el SCSS:

       npm run build:css

3. Para trabajar observando cambios:

       npm run watch:css

La compilación genera un único archivo: css/style.css.

## Requisitos cumplidos

- Cero CSS escrito manualmente como fuente del diseño.
- Variables centralizadas para paleta, tipografías, radios, sombras y breakpoints.
- Mixins reutilizables para contenedores, foco, transiciones y media queries.
- Partials organizados en utilities, base, layout, components y pages.
- Uso de nesting y del operador & para estados interactivos.
- main.scss como único archivo maestro con directivas @use.
- Compilación exitosa a un único style.css.
- Bootstrap 5.3.8 conservado en los cinco HTML.
- Diseño responsive conservado para mobile, tablet y desktop.
- Identidad visual oscura, marfil y dorada de RAPO mantenida.

## Tecnologías

- HTML5 semántico.
- SCSS con arquitectura modular.
- CSS3 compilado.
- Bootstrap 5.3.8 mediante CDN.
- Git y GitHub.

