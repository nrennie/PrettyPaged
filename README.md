# PrettyPaged

Quarto extension for a template to generate a PDF from a paged HTML document with (pretty) styling using `wkhtmltopdf`.

See the template example: [nrennie.rbind.io/PrettyPaged](https://nrennie.rbind.io/PrettyPaged/)

Use `PrettyPaged-pdf` for the format. See [github.com/nrennie/PrettyPDF](https://github.com/nrennie/PrettyPDF) for the LaTeX version of this template and [github.com/nrennie/PrettyTypst](https://github.com/nrennie/PrettyTypst) for the Typst version of this template.

## Installation and use

### `wkhtmltopdf` installation

To use this extension, you must have [wkhtmltopdf](https://wkhtmltopdf.org/) installed on your system. 

### Quarto extension installation

To install the Quarto extension, create a directory, and use the template file:

``` bash
quarto use template nrennie/PrettyPaged
```

To use the extension in an existing project without installing the template file:

``` bash
quarto install extension nrennie/PrettyPaged
```
Note that you will need to update the output format to `format: PrettyPaged-pdf` to enable use of the extension. For book projects, add:

```
project:
  type: PrettyPaged
```
to the `_quarto.yml` file.
