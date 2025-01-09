# Wagtail Accessibility Conformance Report

Based on VPAT® 2.4 WCAG 2.1 and Revised Section 508 Edition

## Name of Product/Version
Wagtail 5.2

## Report Dates and Version
- Report Date: 15/12/2023
- Last Modified Date: 22/12/2023
- Version: wagtail-5.2-1

## Product Description
A Django content management system focused on flexibility and user experience

## Contact Information
### Author Information
- Name: Thibaud Colas
- Company: Torchbox

- Email: thibaud.colas@torchbox.com

- Website: https://torchbox.com/
### Vendor Information
- Name: Thibaud Colas
- Company: Wagtail



- Website: https://wagtail.org/

## Notes
Testing based on https://static-wagtail-v5-2.netlify.app/admin/. This report was created based on results of an ATAG 2.0 audit (https://wagtail.org/accessibility/atag-audit/) and WCAG 2.2 audit (https://github.com/wagtail/wagtail/discussions/11180), as well as the public record of accessibility issues identified as of December 2023.

## Evaluation Methods
Auditing conducted with the WCAG-EM methodology. Specific testing tools employed are Accessibility Insights (Axe) and Pa11y (Axe).

Manual tests included:

- Manual keyboard navigation testing
- Manual touch navigation testing
- Manual 400% zoom testing
- Desktop screen readers: VoiceOver macOS, NVDA
- Mobile screen readers: VoiceOver iOS, TalkBack
- Speech recognition: Voice Control
- Magnification with Apple Zoom
- WHCM


## Applicable Standards/Guidelines
This report covers the degree of conformance for the following accessibility standard/guidelines:

| Standard/Guideline | Included In Report |
| --- | --- |
| [Web Content Accessibility Guidelines 2.1](https://www.w3.org/TR/WCAG21/) | <ul><li>Table 1: Success Criteria, Level A</li><li>Table 2: Success Criteria, Level AA</li><li>Table 3: Success Criteria, Level AAA</li></ul> |
| [Revised Section 508 standards published January 18, 2017 and corrected January 22, 2018](https://www.access-board.gov/ict/) | <ul><li>Chapter 3: Functional Performance Criteria (FPC)</li></ul> |

## Terms
The terms used in the Conformance Level information are defined as follows:
- **Supports**: The functionality of the product has at least one method that meets the criterion without known defects or meets with equivalent facilitation.
- **Partially Supports**: Some functionality of the product does not meet the criterion.
- **Does Not Support**: The majority of product functionality does not meet the criterion.
- **Not Applicable**: The criterion is not relevant to the product.
- **Not Evaluated**: The product has not been evaluated against the criterion. This can be used only in WCAG 2.x Level AAA.

## WCAG 2.1 Report

### Table 1: Success Criteria, Level A


Conformance to the 30 criteria listed below is distributed as follows:

- 58 supported
- 13 partially supported
- 0 not supported
- 49 not applicable

| Criteria | Conformance Level | Remarks and Explanations |
| --- | --- | --- |
| [1.1.1 Non-text Content](https://www.w3.org/TR/WCAG21/#non-text-content) | <ul><li>**Web**: Partially Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: Though Wagtail has alt text options for all images by default, and ways for site implementers to adjust to their needs, some of the default options lack a clear way to mark images as decorative.

See ATAG 2.0 audit: https://wagtail.org/accessibility/atag-audit/#b23-assist-authors-with-managing-alternative-content-for-non-text-content</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so none of the images are decorative and all images have appropriate alt text.</li><li>**Authoring Tool**: In the authoring tool, there are a few scenarios in which images’ alt text is present but not programmatically associated with the image.

See ATAG 2.0 audit: https://wagtail.org/accessibility/atag-audit/#a2-editing-views-are-perceivable</li> </ul> |
| [1.2.1 Audio-only and Video-only (Prerecorded)](https://www.w3.org/TR/WCAG21/#audio-only-and-video-only-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul><li>**Web**: There is no built-in audio or video support in Wagtail.</li><li>**Electronic Documents**: There is no audio or video content in Wagtail’s documentation.</li><li>**Authoring Tool**: There is no audio or video content in Wagtail’s user interface.</li> </ul> |
| [1.2.2 Captions (Prerecorded)](https://www.w3.org/TR/WCAG21/#captions-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul><li>**Web**: There is no built-in audio or video support in Wagtail.</li><li>**Electronic Documents**: There is no audio or video content in Wagtail’s documentation.</li><li>**Authoring Tool**: There is no built-in audio or video support in Wagtail.</li> </ul> |
| [1.2.3 Audio Description or Media Alternative (Prerecorded)](https://www.w3.org/TR/WCAG21/#audio-description-or-media-alternative-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul><li>**Web**: There is no built-in audio or video support in Wagtail.</li><li>**Electronic Documents**: There is no audio or video content in Wagtail’s documentation.</li><li>**Authoring Tool**: There is no built-in audio or video support in Wagtail.</li> </ul> |
| [1.3.1 Info and Relationships](https://www.w3.org/TR/WCAG21/#info-and-relationships) | <ul><li>**Web**: Partially Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: All content created with Wagtail rich text supports 1.3.1 Info and Relationships, except for the built-in blockquote formatting, which lacks a way to programmatically define the cite attribute or element within.

See ATAG 2.0 audit: https://wagtail.org/accessibility/atag-audit/#a34-for-the-authoring-tool-user-interface-enhance-navigation-and-editing-via-content-structure and https://wagtail.org/accessibility/atag-audit/#b24-assist-authors-with-accessible-templates</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so all content is correctly structured with semantic elements.</li><li>**Authoring Tool**: There are a few known 1.3.1 issues. See for example https://github.com/wagtail/wagtail/issues/10576, and https://docs.google.com/spreadsheets/d/1l7tnpEyJiC5BWE_JX0XCkknyrjxYA5T2aee5JgPnmi4/edit.</li> </ul> |
| [1.3.2 Meaningful Sequence](https://www.w3.org/TR/WCAG21/#meaningful-sequence) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: All content authored with Wagtail has a matching visual and DOM order, in all languages.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so visual order and semantic order always match.</li><li>**Authoring Tool**: Wagtail has been extensively tested so all content has a visual order matching the semantic order. We are aware of a few issues with layout of admin views for right-to-left languages (https://github.com/wagtail/wagtail/discussions/7793), those issues have ben addressed and the fixes will be released in February 2024 in Wagtail 6.0.</li> </ul> |
| [1.3.3 Sensory Characteristics](https://www.w3.org/TR/WCAG21/#sensory-characteristics) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Authoring Tool**: We are aware of one view in the CMS which relies on sensory characteristics too much: revision comparisons (https://github.com/wagtail/wagtail/issues/10576).</li> </ul> |
| [1.4.1 Use of Color](https://www.w3.org/TR/WCAG21/#use-of-color) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Authoring Tool**: We are aware of one view in the CMS which relies on color too much: revision comparisons (https://github.com/wagtail/wagtail/issues/10576).</li> </ul> |
| [1.4.2 Audio Control](https://www.w3.org/TR/WCAG21/#audio-control) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul><li>**Web**: There is no built-in audio or video support in Wagtail.</li><li>**Electronic Documents**: There is no audio or video content in Wagtail documentation.</li><li>**Authoring Tool**: There is no audio or video content in the Wagtail user interface.</li> </ul> |
| [2.1.1 Keyboard](https://www.w3.org/TR/WCAG21/#keyboard) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: All content created with built-in Wagtail features is keyboard-accessible.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed for keyboard support.</li><li>**Authoring Tool**: We are currently aware of a issues with keyboard support:

- https://github.com/wagtail/wagtail/issues/7366, due to be resolved in Wagtail 6.0 in February 2024
- https://github.com/wagtail/wagtail/issues/5325, with a clear workaround and plans to improve but no due date.</li> </ul> |
| [2.1.2 No Keyboard Trap](https://www.w3.org/TR/WCAG21/#no-keyboard-trap) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [2.1.4 Character Key Shortcuts](https://www.w3.org/TR/WCAG21/#character-key-shortcuts) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul><li>**Electronic Documents**: There are no character key shortcuts in Wagtail documentation.</li><li>**Authoring Tool**: All keyboard shortcuts in the admin interface rely on modifier keys.</li> </ul> |
| [2.2.1 Timing Adjustable](https://www.w3.org/TR/WCAG21/#timing-adjustable) | <ul><li>**Web**: Partially Supports</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: Animated images (GIFs) created with Wagtail currently require extra steps to allow pausing of the content.</li><li>**Electronic Documents**: There is no moving, blinking, scrolling, or auto-updating in Wagtail documentation.</li><li>**Authoring Tool**: Animated images (GIFs) displayed within the CMS currently cannot be paused.

See ATAG 2.0 audit: https://wagtail.org/accessibility/atag-audit/#a33-for-the-authoring-tool-user-interface-help-authors-avoid-flashing-that-could-cause-seizures</li> </ul> |
| [2.2.2 Pause, Stop, Hide](https://www.w3.org/TR/WCAG21/#pause-stop-hide) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Authoring Tool**: The only timing is the session time limit / session cookie expiry, configured to 2 weeks by default.

See ATAG 2.0 audit: https://wagtail.org/accessibility/atag-audit/#a322-timing-adjustable</li> </ul> |
| [2.3.1 Three Flashes or Below Threshold](https://www.w3.org/TR/WCAG21/#three-flashes-or-below-threshold) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Electronic Documents**: There are no flashing elements in Wagtail documentation.</li><li>**Authoring Tool**: There are no flashing elements in the Wagtail admin interface.</li> </ul> |
| [2.4.1 Bypass Blocks](https://www.w3.org/TR/WCAG21/#bypass-blocks) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Skip links can be created for all Wagtail content.</li><li>**Electronic Documents**: All pages of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) provide skip links and navigation &quot;table of content&quot; menus.</li><li>**Authoring Tool**: The Wagtail admin interface provides skip links, direct anchor links to page sections, and a &quot;minimap&quot; component to jump directly to a specific form section.</li> </ul> |
| [2.4.2 Page Titled](https://www.w3.org/TR/WCAG21/#page-titled) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: By default, Wagtail-managed pages have a title as set in the CMS.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so every page has a unique title.</li><li>**Authoring Tool**: All of the CMS interface has been reviewed so every view has a descriptive title.</li> </ul> |
| [2.4.3 Focus Order](https://www.w3.org/TR/WCAG21/#focus-order) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: All Wagtail-created content uses a matching semantic, visual, and focus order.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so all content has a matching semantic, visual, and focus order.</li><li>**Authoring Tool**: The Wagtail admin interface has been extensively reviewed so semantic, visual, and focus order always match.</li> </ul> |
| [2.4.4 Link Purpose (In Context)](https://www.w3.org/TR/WCAG21/#link-purpose-in-context) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail link content is always user-generated so can be created with enough description. By default, Wagtail link text for pages defaults to the page’s title.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed for content considerations like link text.</li><li>**Authoring Tool**: All of the admin interface has been reviewed for content considerations like link text.</li> </ul> |
| [2.5.1 Pointer Gestures](https://www.w3.org/TR/WCAG21/#pointer-gestures) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [2.5.2 Pointer Cancellation](https://www.w3.org/TR/WCAG21/#pointer-cancellation) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Authoring Tool**: The only CMS operation on the down-event is application of rich text formatting options via the toolbar. This is always undo-able.</li> </ul> |
| [2.5.3 Label in Name](https://www.w3.org/TR/WCAG21/#label-in-name) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: All forms created with Wagtail support setting the text of the label element.</li><li>**Authoring Tool**: All interactive elements within the CMS have programmatically-associated text matching the visible label. There is one exception currently identified: https://github.com/wagtail/wagtail/issues/11372.</li> </ul> |
| [2.5.4 Motion Actuation](https://www.w3.org/TR/WCAG21/#motion-actuation) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [3.1.1 Language of Page](https://www.w3.org/TR/WCAG21/#language-of-page) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Page language is managed in the CMS and then reflects on page templates as configured by site implementers.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) reflects the page’s language across the different versions. Developer documentation is currently english-only.</li><li>**Authoring Tool**: Page language is semantically defined based on what language the CMS user has configured.</li> </ul> |
| [3.2.1 On Focus](https://www.w3.org/TR/WCAG21/#on-focus) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [3.2.2 On Input](https://www.w3.org/TR/WCAG21/#on-input) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [3.3.1 Error Identification](https://www.w3.org/TR/WCAG21/#error-identification) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: Forms created with Wagtail use the aria-describedby and aria-invalid attributes to programmatically identify fields with errors, as per how Django 5.0+ operates.</li><li>**Electronic Documents**: There are no form fields that can have input errors in the editor guide or developer documentation.</li><li>**Authoring Tool**: Within the CMS, all form fields use visible error messages, aria-describedby, and aria-invalid – except a specific type of field, which does not currently use aria-invalid. This is tracked here: https://github.com/wagtail/wagtail/issues/10300.</li> </ul> |
| [3.3.2 Labels or Instructions](https://www.w3.org/TR/WCAG21/#labels-or-instructions) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: All forms created with Wagtail have mandatory labels for all fields, and optional help text.</li><li>**Electronic Documents**: There is no content that requires user input in our Editor Guide or developer documentation.</li><li>**Authoring Tool**: All form fields requiring input in the CMS have labels. Some also have help text for instructions.</li> </ul> |
| [4.1.1 Parsing](https://www.w3.org/TR/WCAG21/#parsing) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: To the extent of our knowledge, there are no parsing issues affecting CMS users or website visitors.</li><li>**Electronic Documents**: To the extent of our knowledge, there are no parsing issues affecting documentation users.</li><li>**Authoring Tool**: To the extent of our knowledge, there are no parsing issues affecting CMS users or website visitors.</li> </ul> |
| [4.1.2 Name, Role, Value](https://www.w3.org/TR/WCAG21/#name-role-value) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Authoring Tool**: There are a few components in the CMS where we are aware of needed improvements: https://github.com/wagtail/wagtail/issues/5411, https://github.com/wagtail/wagtail/issues/10228, https://github.com/wagtail/wagtail/issues/10576, https://github.com/wagtail/wagtail/issues/5408, https://github.com/wagtail/wagtail/issues/5411</li> </ul> |


### Table 2: Success Criteria, Level AA


Conformance to the 20 criteria listed below is distributed as follows:

- 49 supported
- 3 partially supported
- 2 not supported
- 26 not applicable

| Criteria | Conformance Level | Remarks and Explanations |
| --- | --- | --- |
| [1.2.4 Captions (Live)](https://www.w3.org/TR/WCAG21/#captions-live) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.2.5 Audio Description (Prerecorded)](https://www.w3.org/TR/WCAG21/#audio-description-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.3.4 Orientation](https://www.w3.org/TR/WCAG21/#orientation) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [1.3.5 Identify Input Purpose](https://www.w3.org/TR/WCAG21/#identify-input-purpose) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: All input fields of Wagtail-generated forms have programmatically-associated labels, and programmatically-associated help text if set.</li><li>**Electronic Documents**: All input fields in documentation have programmatically-associated labels.</li><li>**Authoring Tool**: All input fields of admin interface forms have programmatically-associated labels, and occasionally also have help text.</li> </ul> |
| [1.4.3 Contrast (Minimum)](https://www.w3.org/TR/WCAG21/#visual-audio-contrast-contrast) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so there are no known contrast issues.</li><li>**Authoring Tool**: The admin interface’s color theme has been extensively reviewed for color contrast considerations. We’re currently aware of two text contrast issues:

- https://github.com/wagtail/wagtail/issues/10875
- https://github.com/wagtail/wagtail/issues/5778</li> </ul> |
| [1.4.4 Resize text](https://www.w3.org/TR/WCAG21/#visual-audio-contrast-scale) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so there are no known text resizing issues.</li><li>**Authoring Tool**: To the extent of our knowledge, all text in the admin interface can be resized.</li> </ul> |
| [1.4.5 Images of Text](https://www.w3.org/TR/WCAG21/#visual-audio-contrast-text-presentation) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: There are no images of text created by Wagtail itself.</li><li>**Electronic Documents**: There are no images of text in our Editor Guide or developer documentation.</li><li>**Authoring Tool**: There are no images of text inside the CMS, except for the Wagtail logotype on the login screen, where presentation as per our branding is essential.</li> </ul> |
| [1.4.10 Reflow](https://www.w3.org/TR/WCAG21/#reflow) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li> </ul> |
| [1.4.11 Non-text Contrast](https://www.w3.org/TR/WCAG21/#non-text-contrast) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so there are no known contrast issues.</li><li>**Authoring Tool**: We’re aware of one issue with non-text contrast (https://github.com/wagtail/wagtail/issues/11306).</li> </ul> |
| [1.4.12 Text Spacing](https://www.w3.org/TR/WCAG21/#text-spacing) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so there are text styling issues.</li> </ul> |
| [1.4.13 Content on Hover or Focus](https://www.w3.org/TR/WCAG21/#content-on-hover-or-focus) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Authoring Tool**: Areas of the CMS interface which rely on content on hover or focus, only do so for non-essential information, and the the appearing content is persistent until hover/focus moves away from the component.</li> </ul> |
| [2.4.5 Multiple Ways](https://www.w3.org/TR/WCAG21/#multiple-ways) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail encourages site implementers to reply on tree-based page navigation, and implement search functionality. Pages also have &quot;next sibling&quot; and &quot;previous sibling&quot; capabilities.</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) supports three means of navigation:

- Tree-based menu navigation
- Next page and &quot;previous page&quot; navigation
- Site-wide search</li><li>**Authoring Tool**: The CMS interface supports the following means of navigation:

- Admin search
- Tree-based navigation / main menu navigation
- Breadcrumbs
- Dashboard &quot;latest work&quot; navigation
- &quot;Edit bird&quot; / Wagtail user bar navigation from the live site</li> </ul> |
| [2.4.6 Headings and Labels](https://www.w3.org/TR/WCAG21/#headings-and-labels) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail supports generating headings via rich text, and StreamField</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) has been reviewed so there is appropriate heading density.</li><li>**Authoring Tool**: All forms within the admin interface have been audited to have appropriate heading density.</li> </ul> |
| [2.4.7 Focus Visible](https://www.w3.org/TR/WCAG21/#focus-visible) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li> </ul> |
| [3.1.2 Language of Parts](https://www.w3.org/TR/WCAG21/#language-of-parts) | <ul><li>**Web**: Partially Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail has little to no opinion on web page implementation, so this can be implemented site-by-site. In the future, we intend to support this directly as a core feature (https://github.com/wagtail/wagtail/issues/4694).</li><li>**Electronic Documents**: All of the Wagtail editor guide (https://guide.wagtail.org/) and developer documentation (https://docs.wagtail.org/) avoids mixing content between multiple languages.</li><li>**Authoring Tool**: When mixing content between multiple languages inside the CMS, there is currently no use of the lang attribute to identify language of parts.

See:

- https://github.com/wagtail/wagtail/issues/11375
- https://github.com/wagtail/wagtail/issues/11376</li> </ul> |
| [3.2.3 Consistent Navigation](https://www.w3.org/TR/WCAG21/#consistent-navigation) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li> </ul> |
| [3.2.4 Consistent Identification](https://www.w3.org/TR/WCAG21/#consistent-identification) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li> </ul> |
| [3.3.3 Error Suggestion](https://www.w3.org/TR/WCAG21/#error-suggestion) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail makes any suggestions upon input error available via Django’s form validation mechanism, with a relevant error message based on the specific error.</li><li>**Electronic Documents**: There is no form validation within Wagtail documentation.</li><li>**Authoring Tool**: Wagtail’s admin interface makes any suggestions upon input error available via Django’s form validation mechanism, with a relevant error message based on the specific error.</li> </ul> |
| [3.3.4 Error Prevention (Legal, Financial, Data)](https://www.w3.org/TR/WCAG21/#error-prevention-legal-financial-data) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: All Wagtail-generated forms support data validation.</li><li>**Electronic Documents**: There are no forms with validation needed within documentation.</li><li>**Authoring Tool**: Wagtail implements multiple ways to prevent those errors:

1. All content entry in the CMS is automatically validated for correctness
2. For page content and opt-in for other content types, all editing actions are reversible
3. For page content and opt-in for other content types, all editing actions can go through a multi-step publication workflow with reviews (https://guide.wagtail.org/en-latest/how-to-guides/configure-workflows-for-moderation/).

For legal and financial requirements specifically, Wagtail supports turning on different publication workflows for different pages or sections of a site.</li> </ul> |
| [4.1.3 Status Messages](https://www.w3.org/TR/WCAG21/#status-messages) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail does not mandate the use of status messages in Wagtail-created content, but supports creating them as needed.</li><li>**Electronic Documents**: The live search in the Wagtail editor guide documentation lacks programmatically-identifiable status messages.</li><li>**Authoring Tool**: Wagtail’s status messages use the role attribute</li> </ul> |


### Table 3: Success Criteria, Level AAA


Conformance to the 28 criteria listed below is distributed as follows:

- 45 supported
- 6 partially supported
- 19 not supported
- 42 not applicable

| Criteria | Conformance Level | Remarks and Explanations |
| --- | --- | --- |
| [1.2.6 Sign Language (Prerecorded)](https://www.w3.org/TR/WCAG21/#sign-language-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.2.7 Extended Audio Description (Prerecorded)](https://www.w3.org/TR/WCAG21/#extended-audio-description-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.2.8 Media Alternative (Prerecorded)](https://www.w3.org/TR/WCAG21/#media-alternative-prerecorded) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.2.9 Audio-only (Live)](https://www.w3.org/TR/WCAG21/#audio-only-live) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.3.6 Identify Purpose](https://www.w3.org/TR/WCAG21/#identify-purpose) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail only uses semantic HTML elements as part of its web page output.</li> </ul> |
| [1.4.6 Contrast (Enhanced)](https://www.w3.org/TR/WCAG21/#contrast-enhanced) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Does Not Support</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Electronic Documents**: We target lower contrast levels than this SC requires.</li><li>**Authoring Tool**: We target lower contrast levels than this SC requires. There are simple ways to create custom color themes for the admin interface should this be a must have.</li> </ul> |
| [1.4.7 Low or No Background Audio](https://www.w3.org/TR/WCAG21/#low-or-no-background-audio) | <ul><li>**Web**: Not Applicable</li><li>**Electronic Documents**: Not Applicable</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Not Applicable</li> </ul> | <ul> </ul> |
| [1.4.8 Visual Presentation](https://www.w3.org/TR/WCAG21/#visual-presentation) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li> </ul> |
| [1.4.9 Images of Text (No Exception)](https://www.w3.org/TR/WCAG21/#images-of-text-no-exception) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Partially Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Electronic Documents**: The Wagtail logotype present in the documentation would fail this.</li><li>**Authoring Tool**: The Wagtail logotype present in the login screen would fail this.</li> </ul> |
| [2.1.3 Keyboard (No Exception)](https://www.w3.org/TR/WCAG21/#keyboard-no-exception) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: See 2.1.1 Keyboard</li><li>**Electronic Documents**: See 2.1.1 Keyboard</li><li>**Authoring Tool**: See 2.1.1 Keyboard</li> </ul> |
| [2.2.3 No Timing](https://www.w3.org/TR/WCAG21/#no-timing) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [2.2.4 Interruptions](https://www.w3.org/TR/WCAG21/#interruptions) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Electronic Documents**: There are no interruptions in the editor guide or developer documentation.</li><li>**Authoring Tool**: Though the admin interface occasionally contains server updates or other kinds of  system-driven notifications, none of them will interrupt the user’s activities.</li> </ul> |
| [2.2.5 Re-authenticating](https://www.w3.org/TR/WCAG21/#re-authenticating) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail does not enforce any specific authentication behavior on website pages.</li><li>**Electronic Documents**: There is no authentication in the documentation.</li> </ul> |
| [2.2.6 Timeouts](https://www.w3.org/TR/WCAG21/#timeouts) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Authoring Tool**: The default is 2 weeks of inactivity to lose data. If the timeout is lower, Wagtail is missing a warning on data loss. See https://github.com/wagtail/wagtail/issues/2199.</li> </ul> |
| [2.3.2 Three Flashes](https://www.w3.org/TR/WCAG21/#three-flashes) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [2.3.3 Animation from Interactions](https://www.w3.org/TR/WCAG21/#animation-from-interactions) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific styles in its output that would affect this SC.</li><li>**Authoring Tool**: All of the animation can be disabled with the prefers-reduced-motion media query,  but there is no CMS setting.</li> </ul> |
| [2.4.8 Location](https://www.w3.org/TR/WCAG21/#location) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Partially Supports</li> </ul> | <ul><li>**Authoring Tool**: Wagtail uses breadcrumb components across the admin interface but not all of it: https://github.com/wagtail/wagtail/issues/11366</li> </ul> |
| [2.4.9 Link Purpose (Link Only)](https://www.w3.org/TR/WCAG21/#link-purpose-link-only) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTML in its output that would affect this SC.</li><li>**Electronic Documents**: A number of links don’t have an understandable purpose without context.</li><li>**Authoring Tool**: A number of links don’t have an understandable purpose without context.</li> </ul> |
| [2.4.10 Section Headings](https://www.w3.org/TR/WCAG21/#section-headings) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTM in its output that would affect this SC.</li><li>**Electronic Documents**: All pages contain headings.</li><li>**Authoring Tool**: All pages contain headings where sub-sections are present.</li> </ul> |
| [2.5.5 Target Size](https://www.w3.org/TR/WCAG21/#target-size) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific CSS in its output that would affect this SC.</li><li>**Electronic Documents**: There are a number of interactive elements that are smaller than the target.</li><li>**Authoring Tool**: There are a number of interactive elements that are smaller than the target.</li> </ul> |
| [2.5.6 Concurrent Input Mechanisms](https://www.w3.org/TR/WCAG21/#concurrent-input-mechanisms) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul> </ul> |
| [3.1.3 Unusual Words](https://www.w3.org/TR/WCAG21/#unusual-words) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTML in its output that would affect this SC.</li><li>**Electronic Documents**: A high number of unusual words aren’t defined currently.</li><li>**Authoring Tool**: Mechanisms to annotate text can be built, but this isn’t built-in functionality.</li> </ul> |
| [3.1.4 Abbreviations](https://www.w3.org/TR/WCAG21/#abbreviations) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTML in its output that would affect this SC.</li><li>**Electronic Documents**: A high number of abbreviations aren’t defined currently.</li><li>**Authoring Tool**: Mechanisms to annotate text can be built, but this isn’t built-in functionality.</li> </ul> |
| [3.1.5 Reading Level](https://www.w3.org/TR/WCAG21/#reading-level) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTML in its output that would affect this SC.</li><li>**Electronic Documents**: A high number of content hasn’t been assessed for reading level.</li><li>**Authoring Tool**: Mechanisms to assess text can be built, but this isn’t built-in functionality.</li> </ul> |
| [3.1.6 Pronunciation](https://www.w3.org/TR/WCAG21/#pronunciation) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Does Not Support</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTML in its output that would affect this SC.</li><li>**Electronic Documents**: A high number of content hasn’t been assessed for reading level.</li><li>**Authoring Tool**: Mechanisms to annotate text can be built, but this isn’t built-in functionality.</li> </ul> |
| [3.2.5 Change on Request](https://www.w3.org/TR/WCAG21/#change-on-request) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail doesn’t enforce any specific HTML in its output that would affect this SC.</li> </ul> |
| [3.3.5 Help](https://www.w3.org/TR/WCAG21/#help) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Supports</li> </ul> | <ul><li>**Web**: Wagtail’s form builder supports providing HTML for all form fields.</li><li>**Authoring Tool**: All forms in Wagtail provide help text.</li> </ul> |
| [3.3.6 Error Prevention (All)](https://www.w3.org/TR/WCAG21/#error-prevention-all) | <ul><li>**Web**: Supports</li><li>**Electronic Documents**: Supports</li><li>**Software**: Not Applicable</li><li>**Authoring Tool**: Does Not Support</li> </ul> | <ul><li>**Authoring Tool**: Though a large number of authoring actions are reversible, not all are. See https://wagtail.org/accessibility/atag-audit/#a411-content-changes-reversible-minimum</li> </ul> |

## Revised Section 508 Report

### Chapter 3: Functional Performance Criteria (FPC)


Conformance to the 9 criteria listed below is distributed as follows:

- 0 supported
- 3 partially supported
- 0 not supported
- 3 not applicable

| Criteria | Conformance Level | Remarks and Explanations |
| --- | --- | --- |
| [302.1 Without Vision](https://www.access-board.gov/ict/#302.1) | <ul><li>Partially Supports</li> </ul> | <ul><li>Wagtail actively supports all popular screen readers, though there are a small number of known issues.</li> </ul> |
| [302.2 With Limited Vision](https://www.access-board.gov/ict/#302.2) | <ul><li>Partially Supports</li> </ul> | <ul><li>Wagtail supports Windows High Contrast Mode / Contrast themes, though there are a few known issues.</li> </ul> |
| [302.3 Without Perception of Color](https://www.access-board.gov/ict/#302.3) | <ul><li>Partially Supports</li> </ul> | <ul><li>None of the Wagtail admin interface relies on perception of color _except_ for revision comparisons. See https://github.com/wagtail/wagtail/issues/10576.</li> </ul> |
| [302.4 Without Hearing](https://www.access-board.gov/ict/#302.4) | <ul><li>Not Applicable</li> </ul> | <ul><li>With only built-in functionality, there is no audio element to the CMS admin interface, documentation, or website content.</li> </ul> |
| [302.5 With Limited Hearing](https://www.access-board.gov/ict/#302.5) | <ul><li>Not Applicable</li> </ul> | <ul><li>With only built-in functionality, there is no audio element to the CMS admin interface, documentation, or website content.</li> </ul> |
| [302.6 Without Speech](https://www.access-board.gov/ict/#302.6) | <ul><li>Not Applicable</li> </ul> | <ul><li>With only built-in functionality, there is no audio element to the CMS admin interface, documentation, or website content.</li> </ul> |
| [302.7 With Limited Manipulation](https://www.access-board.gov/ict/#302.7) | <ul><li>Not Evaluated</li> </ul> | <ul> </ul> |
| [302.8 With Limited Reach and Strength](https://www.access-board.gov/ict/#302.8) | <ul><li>Not Evaluated</li> </ul> | <ul> </ul> |
| [302.9 With Limited Language, Cognitive, and Learning Abilities](https://www.access-board.gov/ict/#302.9) | <ul><li>Not Evaluated</li> </ul> | <ul> </ul> |












## Repository
https://github.com/wagtail/accessibility

## Feedback
https://github.com/wagtail/accessibility


## Copyright

[OpenACR](https://github.com/GSA/openacr) is a format maintained by the [GSA](https://gsa.gov/). The content is the responsibility of the author.

This content is licensed under a [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/legalcode).
