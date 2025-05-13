# Wagtail ATAG audits

> The [Authoring Tool Accessibility Guidelines (ATAG) 2.0](https://www.w3.org/TR/ATAG20/) provides guidelines for designing web content authoring tools that are both more accessible to authors with disabilities (Part A) and designed to enable, support, and promote the production of more accessible web content by all authors (Part B).

For Wagtail, as an authoring tool, ATAG is the most relevant standard to follow.

## Available audits

### Wagtail 7.0

ATAG 2.0, available in multiple formats:

- [HTML – Wagtail 7.0](https://wagtail.github.io/accessibility/audits/atag/atag_wagtail_7.0.html)
- [Markdown (Source) - Wagtail 7.0](https://github.com/wagtail/accessibility/blob/main/audits/atag/atag_wagtail_7.0.md)
- [HTML – Wagtail 7.0, ATAG Report Tool format](https://wagtail.github.io/accessibility/audits/atag/atag_wagtail_7.0_atag-report-tool.html)
- [JSON – Wagtail 7.0, ATAG Report Tool format](./atag_wagtail_7.0_atag-report-tool.json)
- [WAI Authoring Tools List](https://www.w3.org/WAI/tools-list/authoring/)

Here is an overview of audit findings, at the “success criteria” level as per the [W3C ATAG report tool](https://www.w3.org/WAI/atag/report-tool/), pass/fail:

| Conformance Level | Total   | Part A  | Part B  |
| ----------------- | ------- | ------- | ------- |
| Pass              | 28 (+6) | 14 (+2) | 14 (+4) |
| Fail              | 24 (-6) | 15 (-2) | 9 (-4)  |
| Not applicable    | 13      | 4       | 9       |

### Wagtail 6.3

ATAG 2.0, available in multiple formats:

- [HTML – Wagtail 6.3](https://wagtail.github.io/accessibility/audits/atag/atag_wagtail_6.3.html)
- [Markdown (Source) - Wagtail 6.3](https://github.com/wagtail/accessibility/blob/main/audits/atag/atag_wagtail_6.3.md)
- [HTML – Wagtail 6.3, ATAG Report Tool format](https://wagtail.github.io/accessibility/audits/atag/atag_wagtail_6.3_atag-report-tool.html)
- [JSON – Wagtail 6.3, ATAG Report Tool format](./atag_wagtail_6.3_atag-report-tool.json)
- [WAI Authoring Tools List](https://www.w3.org/WAI/tools-list/authoring/)

Here is an overview of audit findings, at the “success criteria” level as per the [W3C ATAG report tool](https://www.w3.org/WAI/atag/report-tool/), pass/fail:

| Conformance Level | Total   | Part A  | Part B  |
| ----------------- | ------- | ------- | ------- |
| Pass              | 28 (+6) | 14 (+2) | 14 (+4) |
| Fail              | 24 (-6) | 15 (-2) | 9 (-4)  |
| Not applicable    | 13      | 4       | 9       |

### Wagtail 5.1

ATAG 2.0, available in multiple formats:

- [HTML – Wagtail 5.1](https://wagtail.github.io/accessibility/audits/atag/atag_wagtail_5.1.html)
- [Markdown (Source) - Wagtail 5.1](https://github.com/wagtail/accessibility/blob/main/audits/atag/atag_wagtail_5.1.md)
- [HTML – Wagtail 5.1, ATAG Report Tool format](https://wagtail.github.io/accessibility/audits/atag/atag_wagtail_5.1_atag-report-tool.html)
- [JSON – Wagtail 5.1, ATAG Report Tool format](./atag_wagtail_5.1_atag-report-tool.json)
- [WAI Authoring Tools List](https://www.w3.org/WAI/tools-list/authoring/)

Here is an overview of audit findings, at the “success criteria” level as per the [W3C ATAG report tool](https://www.w3.org/WAI/atag/report-tool/), pass/fail:

| Conformance Level | Total | Part A | Part B |
| ----------------- | ----- | ------ | ------ |
| Pass              | 22    | 12     | 10     |
| Fail              | 28    | 15     | 13     |
| Not applicable    | 13    | 4      | 9      |

## Generating reports

We manually create an audit report in Markdown, then transpose the results in the [ATAG Report Tool](https://www.w3.org/WAI/atag/report-tool/).
Finally, we report findings in the [WAI Authoring Tools List](https://www.w3.org/WAI/tools-list/authoring/) via [their GitHub repository wai-authoring-tools-list](https://github.com/w3c/wai-authoring-tools-list/pulls?q=sort%3Aupdated-desc+is%3Apr+wagtail+).
