# IHK Project Documentation

> **Note:**  
> This repository is a template for the project documentation for a German IHK (Industrie- und Handelskammer) final project for computer science.  
> The [IHK](https://www.ihk.de/) is the German Chamber of Industry and Commerce and requires a written project documentation as part of vocational training and final exams in Germany.  
> This project is meant as a basic structure.

---

## 🧩 About

This project contains an example structure for a documentation written in **AsciiDoc** and compiled into a **PDF using Asciidoctor PDF**.  
The documentation is modular, with chapters stored in the `chapters/` folder and included into the main `doku.adoc` file.

The PDF supports **syntax highlighting** using Rouge and custom PDF styling with a **theme.yml**.

For styling tips you can look up the offical [documentation](https://docs.asciidoctor.org/pdf-converter/latest/)


---

## ⚙️ Getting Started

To build and work with the documentation locally:

1. Clone the repository.
2. Install Node dependencies:

    ```bash
    npm install
    ```

3. Install Ruby (required for Asciidoctor PDF):

    - Windows: download from [RubyInstaller](https://rubyinstaller.org)  
    - macOS/Linux: install via your package manager

    Verify installation:

    ```bash
    ruby -v
    ```

4. Install Asciidoctor PDF:

    ```bash
    gem install asciidoctor-pdf
    ```

    Verify installation:

    ```bash
    asciidoctor-pdf --version
    ```

5. Install Rouge for syntax highlighting:

    ```bash
    gem install rouge
    ```

6. Start the development watcher, which automatically rebuilds the PDF on file changes:

    ```bash
    npm run dev
    ```

    This will watch:
    - `doku.adoc` (main document)
    - all `.adoc` files in `chapters/`
    - `theme.yml`

---
