#  Creación de un sitio web estático con MkDocs y GitHub Pages


## Materiales para MKdocs
Necesitaremos una estructura de archivos tal como se ve en este esquema
```
.
└── proyecto
    ├── docs
    │   ├── about.md
    │   └── home.md
    └── mkdocs.yml
```
En el yml tendremos algo como esto
```
# Project information
site_name: 'Material for MkDocs'
site_description: 'A Material Design theme for MkDocs'
site_author: 'Martin Donath'
site_url: 'https://squidfunk.github.io/mkdocs-material/'

site_name: IAW

nav:
    - Principal: index.md
    - Acerca de: about.md

# Repository
repo_name: 'squidfunk/mkdocs-material'
repo_url: 'https://github.com/squidfunk/mkdocs-material'

# Copyright
copyright: 'Copyright &copy; 2016 - 2017 Martin Donath'

# Configuration
theme:
  name: 'material'
  language: 'en'
  palette:
    primary: 'indigo'
    accent: 'indigo'
  font:
    text: 'Roboto'
    code: 'Roboto Mono'

# Customization
extra:
  manifest: 'manifest.webmanifest'
  social:
    - type: 'github'
      link: 'https://github.com/squidfunk'
    - type: 'twitter'
      link: 'https://twitter.com/squidfunk'
    - type: 'linkedin'
      link: 'https://www.linkedin.com/in/squidfunk'
```
El nav lo editaremos según los archivos que tengamos en la carpeta docs.

La carpeta docs contendrá, los post que queremos que se reflejen en la pagina.
