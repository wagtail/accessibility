# VPAT reports

> A [Voluntary Product Accessibility Template (VPAT®)](https://www.section508.gov/sell/vpat/) is a document that explains how information and communication technology (ICT) products such as software, hardware, electronic content, and support documentation meet (conform to) the Revised 508 Standards for IT accessibility.

Wagtail uses VPATs to report on the accessibility of the Wagtail admin interface, as this format is widely recognised in a procurement context.

## Available reports

### Wagtail 5.2

VPAT® 2.4 WCAG 2.1 and Revised Section 508 Edition (the current best practice standard in the United States of America), available in multiple formats:

- [HTML – Wagtail 5.2](https://wagtail.github.io/accessibility/audits/vpat/vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.html)
- [HTML (source) – Wagtail 5.2](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.html)
- [Markdown (source) – Wagtail 5.2](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.md)
- [YAML (source) – Wagtail 5.2](./vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.yaml)

## Generating reports

We use the [OpenACR Editor](https://gsa.github.io/openacr-editor/) to generate the YAML and HTML, combined with the [OpenACR CLI](https://github.com/GSA/openacr/blob/main/docs/CLI.md) to generate the Markdown:

```bash
./node_modules/.bin/ts-node src/openacr.ts output -f vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.yaml -c catalog/2.4-edition-wcag-2.1-508-en.yaml -o ./vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.md
```