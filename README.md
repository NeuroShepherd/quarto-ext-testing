# quarto-ext-testing

Testing what does and doesn't work for a Quarto extension(s) mono-repo.

## Installing


```bash
quarto use template NeuroShepherd/quarto-ext-testing
```

This will install both extensions in the `_extensions/` directory. However, it will only make use of the `project` contributed by the `qtest` extension. 

There is, at the time of writing this, no way to have a single repo with multiple extensions and allow specification of which extension to use for the template. E.g. something like `quarto use template NeuroShepherd/quarto-ext-testing/qtest2` would be practical. Note that I tried running:

```bash
quarto use template NeuroShepherd/quarto-ext-testing/qtest2
```

But the resulting `_quarto.yml` file used `format: qtest` rather than `format: qtest2`.

I think the only option currently is to use separate repos if both extensions are meant to contribute project templates.


## Using

*TODO*: Describe how to use your format.

## Format Options

*TODO*: If your format has options that can be set via document metadata, describe them.

## Example

Here is the source code for a minimal sample document: [example.qmd](example.qmd).
