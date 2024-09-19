# phpDocumentor Test

Issue: Internal links point to external files.

```
git clone git@github.com:natanfelles/phpdoc-test.git
cd phpdoc-test
curl -LO "https://github.com/phpDocumentor/phpDocumentor/releases/download/v3.5.3/phpDocumentor.phar"
php phpDocumentor.phar
```

Open the `build/docs/guide/libraries/bar/index.html` file in your browser.

Hover your mouse over the headings.

Note that the links are created to the `foo` page.

Example: `phpdoc-test/build/docs/guide/libraries/foo/index.html#heading-1`

The correct would be: `phpdoc-test/build/docs/guide/libraries/bar/index.html#heading-1`

Until version `3.3.1` the links were working correctly.

To test:

```
curl -LO "https://github.com/phpDocumentor/phpDocumentor/releases/download/v3.3.1/phpDocumentor.phar"
php phpDocumentor.phar
```

Note that the links point to internal headings.

Thanks!
