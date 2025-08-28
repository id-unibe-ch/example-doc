Title: Image handling and usage

----

SubText: This page describes the image handling and usage in the documentation

----

Text:

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

## Example folder structure with images
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