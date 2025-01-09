# Wagtail Accessibility Conformance Report / VPAT

> An [Accessibility Conformance Report](https://www.section508.gov/sell/acr/) or Voluntary Product Accessibility Template (VPAT®) is a document that explains how information and communication technology (ICT) products such as software, hardware, electronic content, and support documentation meet (conform to) the Revised 508 Standards for IT accessibility.

Wagtail documents the accessibility of the Wagtail admin interface with ACR / VPAT® reports, as this format is widely used in a procurement context, particularly in the United States of America.

## Available reports

To view our latest report in HTML format, go to [wagtail.org/vpat/](https://wagtail.org/vpat/). All of our past reports are listed here in multiple formats.

### Wagtail 6.3

#### VPAT 2.5 WCAG 2.2 and Revised Section 508 Edition

- [HTML – Wagtail 6.3](https://wagtail.github.io/accessibility/audits/vpat/vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.html)
- [HTML (source) – Wagtail 6.3](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.html)
- [Markdown (source) – Wagtail 6.3](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.md)
- [YAML (source) – Wagtail 6.3](./vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.yaml)

Report based ased on [ITI VPAT®](https://www.itic.org/policy/accessibility/vpat) templates, November 2023 update, with the latest [WCAG 2.2](https://www.w3.org/TR/WCAG22/) (December 2024), and [Revised Section 508](https://www.access-board.gov/ict/) (January 2017). Built with [OpenACR version 0.3.8](https://github.com/gsa/openacr).

### Wagtail 5.2

#### VPAT 2.5 WCAG 2.2 and Revised Section 508 Edition

- [HTML – Wagtail 5.2](https://wagtail.github.io/accessibility/audits/vpat/vpat_wagtail_5.2_2.5-edition-wcag-2.2-508-en.html)
- [HTML (source) – Wagtail 5.2](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_5.2_2.5-edition-wcag-2.2-508-en.html)
- [Markdown (source) – Wagtail 5.2](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_5.2_2.5-edition-wcag-2.2-508-en.md)
- [YAML (source) – Wagtail 5.2](./vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.yaml)

Documents based on [ITI VPAT®](https://www.itic.org/policy/accessibility/vpat) templates, September 2023 update, with the latest [WCAG 2.2](https://www.w3.org/TR/WCAG22/) (October 2023), and [Revised Section 508](https://www.access-board.gov/ict/) (January 2017). Built with [OpenACR version 0.3.7](https://github.com/gsa/openacr).

#### VPAT 2.4 WCAG 2.1 and Revised Section 508 Edition

- [HTML – Wagtail 5.2](https://wagtail.github.io/accessibility/audits/vpat/vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.html)
- [HTML (source) – Wagtail 5.2](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.html)
- [Markdown (source) – Wagtail 5.2](https://github.com/wagtail/accessibility/blob/main/audits/vpat/vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.md)
- [YAML (source) – Wagtail 5.2](./vpat_wagtail_5.2_2.4-edition-wcag-2.1-508-en.yaml)

Documents based on [ITI VPAT®](https://www.itic.org/policy/accessibility/vpat) templates, September 2023 update, with the latest [WCAG 2.1](https://www.w3.org/TR/WCAG21/) (October 2023), and [Revised Section 508](https://www.access-board.gov/ict/) (January 2017). Built with [OpenACR version 0.3.7](https://github.com/gsa/openacr).

## Other formats

Looking for a VPAT® in another format? Please [request it in GitHub issues](https://github.com/wagtail/accessibility/issues).
VPAT® templates also exist for [EN 301 549](https://en.wikipedia.org/wiki/EN_301_549), and in an "INT" international variant that covers both Section 508 and EN 301 549. We can consider providing those documents on request.

## Generating reports

Either start from an existing report, or use the [OpenACR Editor](https://acreditor.section508.gov/) to generate the YAML. Then use the [OpenACR CLI](https://github.com/GSA/openacr/blob/main/docs/CLI.md) to generate the HTML and Markdown:

```bash
# Update all with absolute paths:
openacr output -f vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.yaml -t openacr-markdown-0.1.0.handlebars -c 2.5-edition-wcag-2.2-508-en.yaml -o ./vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.md
openacr output -f vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.yaml -t openacr-html-0.1.0.handlebars -c 2.5-edition-wcag-2.2-508-en.yaml -o ./vpat_wagtail_6.3_2.5-edition-wcag-2.2-508-en.html
```

Note the default HTML output relies on external files which we don’t want to include, and has a few bugs. See commit ae2d51b for necessary changes.
