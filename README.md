# Docs Application Documentation

## Compilation and Execution

### Compilation

To compile the project, use the following command:

```bash
./autobuild.sh all
```

### Clean Build

To clean the existing build, use:

```bash
./autobuild.sh clean
```

### Run

To run the documentation, execute:

```bash
./autobuild.sh run
```

Alternatively, navigate to the _html directory and manually open the index.html file.

## Detailed Overview of the Docs Application

### Diagrams and Documentation Style

* For diagrams and software architecture illustrations, ProcessOn or Visio tools are recommended to ensure consistent visual style (except in special cases).

* Documentation should follow the standard Markdown format, and editing can be done efficiently using the Editor plugin in VS Code.

### Compilation Environment

Ensure the following dependencies are installed:

```bash
pip3 install sphinx
pip3 install recommonmark
pip3 install sphinx_markdown_tables
pip3 install sphinx_rtd_theme
pip3 install sphinx_book_theme
```
### Compilation Process
Use the ./autobuild.sh script for compiling. This script will also package the docs and render settings:
```bash
./autobuild.sh all
```

Alternatively, you can use Sphinx’s native compilation command:
```bash
make html
```
Once the compilation is complete, open the docs/index.html file to view the results.
After submitting changes, verify the rendered webpage to ensure everything is displayed correctly.

### Customization
Custom configurations are managed in the conf.py file. Some additional libraries are required for extended features:

#### Change Style/Theme
The sphinx_rtd_theme is used as an example here, but you can explore other themes online:

```bash
pip install sphinx_rtd_theme
```
Markdown Syntax Support Plugin
Add Markdown support with:

```bash
pip install myst-parser
```
Mermaid Rendering Support Plugin
For rendering diagrams with Mermaid:

```bash
pip install sphinxcontrib.mermaid
```
One-Click Code Block Copy Plugin
To enable a copy button for code blocks:

```bash
pip install sphinx_copybutton
```

#### Editing Recommendations
Use VS Code to edit Markdown files for efficient workflow.
It is highly recommended to install a Markdown preview plugin in VS Code for real-time editing and previewing.

