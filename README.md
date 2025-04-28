Static archive of the center for reproducible neuroscience website.

Produced with the following wget and bash one liner:

```
wget --recursive --no-clobber --page-requisites --html-extension --convert-links --restrict-file-names=windows --domains reproducibility.stanford.edu --no-parent http://reproducibility.stanford.edu
```

```
find . -name '*.html' -exec sed -i 's|<body[^>]*>|&<div style="background-color: yellow; padding: 10px; text-align: center; font-weight: bold; border: 1px solid red;">This is an archive of the site and is no longer updated. Please address any issues <a href="https://github.com/poldracklab/reproducibility_site_archive/issues">here</a>.</div>|' {} +
```
