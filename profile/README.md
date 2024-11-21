# Magic Manuscript Maker Typesetting Workflow (under construction)
The Magic Manuscript Maker Typesetting Workflow is a collection of open-source tools and scripts that help to automate the typesetting process of academic articles. The workflow is designed to be used in a Docker container and is part of the [Philosophy and the Mind Sciences](https://philosophymindscience.org/) journal. The workflow consists of the following tools:

- [Typesetting-Container-OS](https://github.com/phimisci/typesetting-container-os)
- [XML2YAML-OS](https://github.com/phimisci/xml2yaml-os)
- [DOC2MD-OS](https://github.com/phimisci/doc2md-os)
- [VerifyBibTeX-OS](https://github.com/phimisci/verifybibtex-os)

These tools are channeled through a web application called the "Magic Manuscript Maker", which allows to create user profiles and projects. The web application will be released in the future. However, the individual tools can also be used independently. In the following sections, you can find a short summary of each tool.

## Typesetting Container OS
The Typesetting Container OS is part of the Magic Manuscript Maker Typesetting Workflow and is used to typeset articles in the journal. The Typesetting Container OS heavily relies on [Pandoc](https://pandoc.org/), which does all the heavy lifting. The container uses pandoc to convert markdown files to various outputs such as PDF, HTML, TEX, and JATS. The container can be used via the command line or in a simple web interface. It comes with a default template that can be adjusted to the needs of the journal. The container is available on GitHub: [Typesetting-Container-OS](https://github.com/phimisci/typesetting-container-os).

## XML2YAML-OS
XML2YAML-OS is an open source CLI program that transforms OJS XML into a YAML format for later use in the Typesetting Container OS. The program is designed to be used in a Docker container, but can also be used locally. Using the OJS XML file to create metdata files for the Typesetting Container OS is a crucial step in the Magic Manuscript Maker Typesetting Workflow, since it allows for a seamless integration of the metadata that is usually already present in the OJS backend. The default metadata fields were selected in view of the default template of the Typesetting Container OS, but can be easily adjusted to your needs. The repository can be found here: [XML2YAML-OS](https://github.com/phimisci/xml2yaml-os)

## DOC2MD-OS
DOC2MD-OS is a CLI program that converts DOCX/ODT files to Markdown, which is the central format of the single source publishing approach of the Magic Manuscript Maker Typesetting Workflow. The program is designed to be used in a Docker container, but can also be used locally. DOC2MD-OS helps to transform initial submissions in DOCX or ODT into a format that can be processed by pandoc during the typesetting workflow. The repository can be found here: [DOC2MD-OS](https://github.com/phimisci/doc2md-os)

## VerifyBibTeX-OS
VerifyBibTeX-OS is a helpful tool that checks the validity of a BibTeX file. In addition, it also checks if the BibTeX file contains all the necessary fields for the Magic Manuscript Maker Typesetting Workflow, such as DOI fields, page numbers, etc. It creates a report that lists all the missing fields and potential errors in the BibTeX file. The repository can be found here: [VerifyBibTeX-OS](https://github.com/phimisci/verifybibtex-os)

## About
The Magic Manuscript Maker Typesetting Workflow is developed by Thomas Jurczyk for Philosophy and the Mind Sciences. If you have any questions, ideas,  or want to report bugs, please contact [thomjur](https://github.com/thomjur).
