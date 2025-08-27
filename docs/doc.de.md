Title: Example Documentation

----

Read: docs/example

----

Text:

## Source Code
The source code of this documentation is available on GitHub:  
[https://github.com/id-unibe-ch/example-doc](https://github.com/id-unibe-ch/example-doc)

## File naming
Files need to be named by the template they are used in, for example `docs/doc.md` for the `markdown` template (= doc.php).

### Multilingual files
For multilingual files, use the language code as a suffix, for example `docs/doc.de.md` for the German version of the `markdown` template. As German is the default language for the platform and is used as fallback, you will need to have a file having the German language code suffix.  
  
Even if your documentation consists of only one language, English as for example, you will need to have a file with the German language code suffix.  
In this case create a file named `docs/doc.de.md` and add the English content in it. There is no need to create a file named `docs/doc.en.md` in this case.

### Example file names
- **doc.de.md:** Used for a combination of Markdown, Markdown Extra and KirbyText content.
- **doc.en.md:** Used for a combination of Markdown, Markdown Extra and KirbyText content in English.

#### Additional information
You can find more information about the different syntaxes here:
- [Markdown syntax reference](https://getkirby.com/docs/reference/text/markdown)
- [Markdown Extra syntax reference](https://michelf.ca/projects/php-markdown/extra/)
- [KirbyText syntax reference](https://getkirby.com/docs/reference/text/kirbytags)


## Folder structure
Each page needs to be in its own folder, named after the short-form pagetitle, for example `docs/example/doc.de.md`.  
The folder name may contain only lowercase letters, numbers and hyphens.  
Each folder may contain subfolders, for example `docs/example/sub-page/doc.de.md`.

### Folder states
Each folder can have one of the following states:
- **Draft:** Folder name starts with an underscore, for example `docs/_example/doc.de.md`.
- **Unlisted:** Folder name consists of the folder name only, for example `docs/example/doc.de.md`.
- **Listed:** Folder name with a prefix number, for example `docs/1_example/doc.de.md`.

The number defines the order of the page in the navigation.  
You may also use `1_` as prefix for each page, if you want to have all pages in the navigation but do not care about the order.

### Example folder structure
```
docs/
└── _draft/example-draft/
    └── doc.de.md
└── example-unlisted/
    └── doc.de.md
└── 1_example-listed/
    └── doc.de.md
└── 2_example-german-content/
    └── doc.de.md
└── 3_example-english-content/
    └── doc.de.md
└── 4_example-english-and-german-content/
    └── doc.de.md
    └── doc.en.md
    └── 1_sub-page/
        └── doc.de.md
        └── doc.en.md
doc.de.md <= main page
```

## Images
Images need to be stored in the same folder as the documentation file, for example `docs/example/test-image-1.png`.  
  
As Kirby CMS uses its own image handling and routing, images need to be referenced by an absolute path.  

**Allowed image references:**
```
![Example Image](test-image-1.png)
![Example External Image](https://example.org/test-image-1.png)
```

**Not allowed image references:**
```
![Example Image](./test-image-1.png)
![Example Image](/docs/example/test-image-1.png)` <= We will need to adapt our custom image handling for this.
![Example Image](../example/test-image-1.png)
```

### Example folder structure with images
```
docs/
└── 1_example-german-content/
    └── test-image-1.png
    └── test-image-2.jpg
    └── doc.de.md
    └── 1_sub-page/
        └── test-image-1.png
        └── test-image-2.jpg
        └── doc.de.md
        └── doc.en.md
doc.de.md <= main page
```

## Page structure
Each documentation page must have the following structure:  
![File Header](file-header-example.png)

!!! info ""

    Unused sections may be removed, for example if you do not want to have a subtext,
    just remove the whole section including the `----` lines.
