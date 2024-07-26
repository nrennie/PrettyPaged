# PrettyPaged

Quarto extension for a template to generate a PDF from a paged HTML document with (pretty) styling using Paged.js. Use `PrettyPaged-pdf` for the format. Note that version 1.4 or greater of Quarto is required.

> Note: see [github.com/nrennie/PrettyPDF](https://github.com/nrennie/PrettyPDF) for the LaTeX version of this template and [github.com/nrennie/PrettyTypst](https://github.com/nrennie/PrettyTypst) for the Typst version of this template.

## Installation and use

### Paged.js installation

To use this extension, you must have [Paged.js](https://pagedjs.org/) installed on your system. See the **Command line version** section of [pagedjs.org/documentation/2-getting-started-with-paged.js](https://pagedjs.org/documentation/2-getting-started-with-paged.js/) for instructions.

#### Issues with pandoc and Paged.js on Windows

There are still some issues with getting `pagedjs-cli` to work with pandoc on Windows. See [#8946](https://github.com/quarto-dev/quarto-cli/issues/8946) and [#8061](https://github.com/jgm/pandoc/issues/8061).


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


### Logo

Either replace the `logo.png` file with a new file of your choosing, or change the file path in the YAML to point to a different logo file. Note that the file path is relative to your .qmd file.
