Title: File naming and handling

----

SubText: This page describes the file naming conventions and handling of multilingual content

----

Text:
Files need to be named by the template they are used in, for example `docs/doc.md` for the `markdown` template (= doc.php).

## Multilingual files
For multilingual files, use the language code as a suffix, for example `docs/doc.de.md` for the German version of the `markdown` template. As German is the default language for the platform and is used as fallback, you will need to have a file having the German language code suffix.  
  
Even if your documentation consists of only one language, English as for example, you will need to have a file with the German language code suffix.  
In this case create a file named `docs/doc.de.md` and add the English content in it. There is no need to create a file named `docs/doc.en.md` in this case.

## Example file names
- **doc.de.md:** Used for a combination of Markdown, Markdown Extra and KirbyText content.
- **doc.en.md:** Used for a combination of Markdown, Markdown Extra and KirbyText content in English.

An example of a multilingual page can be found [here](./multilingual-page/).  

!!! tip "Additional information"

    You can find more information about the different syntaxes here:
    - [Markdown syntax reference](https://getkirby.com/docs/reference/text/markdown)
    - [Markdown Extra syntax reference](https://michelf.ca/projects/php-markdown/extra/)
    - [KirbyText syntax reference](https://getkirby.com/docs/reference/text/kirbytags)
