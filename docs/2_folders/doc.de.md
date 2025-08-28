Title: Folder naming and handling

----

SubText: This page describes the folder naming conventions and structures

----

Text:
Each page needs to be in its own folder, named after the short-form pagetitle, for example `docs/example/doc.de.md`.  
The folder name may contain only lowercase letters, numbers and hyphens.  
Each folder may contain subfolders, for example `docs/example/sub-page/doc.de.md`.

## Folder states
Each folder can have one of the following states:
- **Draft:** Folder name starts with an underscore, for example `docs/_example/doc.de.md`.
- **Unlisted:** Folder name consists of the folder name only, for example `docs/example/doc.de.md`.
- **Listed:** Folder name with a prefix number, for example `docs/1_example/doc.de.md`.

The number defines the order of the page in the navigation.  
You may also use `1_` as prefix for each page, if you want to have all pages in the navigation but do not care about the order.

## Example folder structure
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