# 2020-2023 Wagtail accessibility team meeting notes

For notes from past meetings from 2024 onwards, see [Accessibility team: meeting updates](https://github.com/wagtail/wagtail/discussions/11394). Meeting notes previously stored on the [Accessibility team wiki page](https://github.com/wagtail/wagtail/wiki/Accessibility-team) are available below.

## 2023-12-22 – More team members

Attendees: Sherry, Albina, Thibaud, Storm, Ahmed, Damilola, Saptak, Victoria

### **Actions**

- Albina, Storm, Saptak Interview with Ahmed
- Thibaud Review overlap between WCAG 2.2 admin audit & ATAG audit
- Thibaud Share results of ACR
- Thibaud Add accessibility issues from Albina’s audit to backlog
- Thibaud Message Victoria about “design-needed” items in mid-January
- Thibaud Share list of talk ideas
- Saptak & Thibaud Prepare ATAG discussion for FOSDEM
- Saptak Check how to run a BOFs at FOSDEM
- Saptak Share ideas for Django accessibility 😬 Based on Wagtail’s work or otherwise.
- Ahmed Chat with Thibaud about accessibility events
- Sherry Vote / add project ideas on team’s list
- Ahmed Vote / add project ideas on team’s list
- Ahmed, Damilola, Thibaud Organize interviews w/ Storm, Saptak, Albina

### **Actions review**

### **Discussions**

- Introductions
  - Thibaud
  - Albina – our Outreachy intern last year
  - Storm – coming up on five year anniversary
  - Damilola – also our Outreachy intern last year :)
  - Ahmed – Outreachy intern :) Enjoying the mentoring so far
  - Sherry – Outreachy intern :)
  - Saptak – Human rights centered developer
  - Victoria – Design, accessibility interest
- Ideas discussed in the last meeting
  - Triage “design needed” accessibility contributions
  - Outreachy: wagtail.org website accessibility
    - Going great
    - Manual testing of the website
    - Manual spreadsheet: [Wagtail.org | Accessibility audit spreadsheet](https://docs.google.com/spreadsheets/d/1kWb6f9YlT-UA2TC4ioAH40Y5T18hd_Hbt_ncTamabW4/edit)
    - Stacking issue – dark theme
      - Feels like a stacking issue
    - Specific issues are likely to affect other sites
  - Outreachy: accessibility features documentation
    - Understand pain points – interviews
- Plans for 2024
  - Design needed accessibility backlog
  - [WCAG 2.2 AAA\* audit of the Wagtail admin – Nov 2023 #11180](https://github.com/wagtail/wagtail/discussions/11180)
    - Proceed with more auditing in 2024
  - Outreachy projects
  - RFC 89 / ATAG audit
  - ACR – Thibaud
  - Talks
    - Damilola – keen to speak, not sure about accessibility (:
    - Saptak
    - Victoria – already doing this,
    - Thibaud
    - (Albina)
    - Ahmed – talk further to confirm
    - PyCon US May 2024
      - Vince Salvino – accessibility x Wagtail poster
      - Meagen Voss – workshop, based on Scott’s DjangoCon US
    - FOSDEM 2024
    - DjangoCon Europe 2024
    - Wagtail Space US June 2024
    - Wagtail Space NL June 2024
    - Online celebration around [10 years anniversary](https://pypi.org/project/wagtail/#history)
- Django team support / collaboration
  - Thibaud, Saptak, Storm
  - Saptak specific ideas
  - Events – something we could learn from
- Accessible image model by default (current implementation uses filename as title / alt text )
  - 🍎🍈 🍒🍍🍓
  - Approve and implement [RFC 51: Contextual Alt Text](https://github.com/wagtail/rfcs/pull/51) 🍒
  - Package: [https://github.com/newshour/wagtailimagecaptions](https://github.com/newshour/wagtailimagecaptions)
  - First step: how have people done this so far / what works for them.

## 2023-12-01 – Team kickoff

- Welcome & introductions
  - Thibaud – Wagtail accessibility, Django accessibility
    - DSF board director 💥
  - Albina – our Outreachy intern working on the accessibility checker
    - Working at Torchbox on accessibility audits, other things
    - Upcoming: Outreachy project mentoring
  - Ben – Torchbox, Wagtail _AI_
    - Keen to do more open source contributions!
  - Sage – Torchbox, Wagtail core team, Outreachy mentor last year
    - Current work: Universal listings, investigating aria-label
    - Having fun with aria-label and aria-labelledby
  - Storm – from the Netherlands. Contractor working on Wagtail projects
    - Ex Torchbox intern four years ago. Core team since 2021
  - Saptak – Contractor, currently working with Freedom of the Press Foundation
    - OSS maintainer – A11Y Project
    - HTTP Archive Web Almanac Accessibility chapter
  - Scott Cranfill – JPL, Wagtail core team 2020, accessibility team too
    - Help Wagtail users build more accessible websites
  - Victoria!
- Intro to current accessibility efforts – last 12 months
  - **Wagtail 4.2**: [Accessibility checker integration](https://docs.wagtail.org/en/stable/releases/4.2.html)
  - **Wagtail 5.0**: [Accessibility checker improvements](https://docs.wagtail.org/en/stable/releases/5.0.html#accessibility-checker-improvements), [Dark mode](https://docs.wagtail.org/en/stable/releases/5.0.html#dark-mode)
  - **GAAD 2023: **[Wagtail accessibility statistics for GAAD 2023](https://wagtail.org/blog/wagtail-accessibility-statistics-for-gaad-2023/)
  - **Wagtail 5.1**: Accessible “More” dropdown buttons
  - **Wagtail 5.2**: No more invisible buttons
  - **October**: Scott @ DjangoCon US: [Best Practices for Making a Wagtail Website as Accessible as Possible](https://github.com/Scotchester/djangocon-wagtail-accessibility)
  - **November**: [RFC 89 ATAG audit](https://github.com/wagtail/rfcs/pull/89)
  - **December**: [Wagtail CMS Accessibility Webinar](https://wagtail.org/blog/wagtail-cms-accessibility-webinar/) by Scott, Thibaud, Albina
  - Wagtail 6.0 – accessibility
    - In progress – [Accessibility manual audit - WCAG 2.2 #63](https://github.com/wagtail/roadmap/issues/63)
    - In progress – [Accessibility checker in page editor #66](https://github.com/wagtail/roadmap/issues/66)
    - Starting next week – Outreachy: [Accessibility features documentation #69](https://github.com/wagtail/roadmap/issues/69)
    - Outreachy: [Wagtail.org website accessibility #68](https://github.com/wagtail/roadmap/issues/68)
  - Wagtail 6.0 – UI
    - [Universal listings improvements #62](https://github.com/wagtail/roadmap/issues/62)
    - [Polish dark mode #65](https://github.com/wagtail/roadmap/issues/65)
  - Wagtail 6.1: [Admin interface accessibility improvements #71](https://github.com/wagtail/roadmap/issues/71)
  - Beyond
    - [Looking for sponsorship – Accessibility checks for site administrators](https://wagtail.org/blog/looking-for-sponsorship-accessibility-checks-for-site-administrators/)
    - [Fully accessible Wagtail admin interface #27](https://github.com/wagtail/roadmap/issues/27)
    - PyCon US 2024 poster
    - FOSDEM 2024
- How the team works
  - The plan: open membership, 45-min chats every one or two weeks to provide feedback and take actions.
    - Every week or every **two weeks**?
    - Always the same time? Any specific days to avoid? another Doodle?
  - 6 months membership
  - How to contribute as a designer?
    - Lots of ways!
    - Example: [https://github.com/wagtail/wagtail/issues/10576](https://github.com/wagtail/wagtail/issues/10576)
    - Lots of issues in Wagtail that are blocked due to a lack of design expertise / designer availability
      - Ben Enright our designer isn’t always available
- What do we all want to achieve with the accessibility team?

### **Team plans**

Votes: 🥭 Jesse, 🍎 Saptak, 🍐 Jane, 🍒 Scott, 🍋 Thibaud, 🍇 Sage, 🍊Albina, 🍈 Storm 🍍Ben M, 🍓 Victoria,

- Triage “design needed” accessibility contributions 🍒🍋🍍🍊🍓🍎
- Outreachy: wagtail.org website accessibility 🍎🍊🍈🍋🍇🍓
  - Accessibility audits for docs.wagtail.org and guide.wagtail.org🍎🍈🍓
- Work with people using assistive technology to discover areas of improvement 🍎🍋 🍒🍇🍓
  - Or maybe testimonials for Wagtail.org? Wagtail is an accessible CMS!
  - +1 to user testing with assistive tech users
- Accessible image model by default (current implementation uses filename as title / alt text ) 🍎🍈 🍒🍍🍓
  - ❤️Storm w/ Saptak helping 💚
  - Approve and implement [RFC 51: Contextual Alt Text](https://github.com/wagtail/rfcs/pull/51) 🍒
  - Progress is progress (is progress)
    - Anything that’s not using the default title (as-is) is better than status quo
  - Custom image model by default?
  - Power of defaults
- Support Django’s accessibility team with their direction 🍒🍇🍎🍈
- Audit Wagtail design system for accessible contrast as measured by [the new APCA contrast model](https://www.myndex.com/APCA/) (Possibly too early if we’re concerned about it not being an official part of the standard yet?) 🍈🍊🍇🍓
  - (Saptak) I would argue it’s little too early since it’s still not fully ready
  - (Storm) could still be a fun little project, how does Wagtail do with this model?
- Improve how we automatically test Wagtail’s accessibility (add more tests, add better tooling, etc.) to prevent accessibility regressions 🍋🍈🍇 🍒
- Meetup/conference talks related to accessibility work across wagtail 🍎 🍒🍇🍓
- Update Rich Text link modal to include aria-label field 🍋 🍒🍎
- Triage “community management & marketing” accessibility contributions🍋🍓
- VPAT (Voluntary Product Accessibility Template, primarily a Section 508 thing) for Wagtail🍋
- Propose adding a stock Heading Block to Wagtail core, which can implement validation for not skipping levels 🍒
- High-contrast light and dark themes for Wagtail🍋🍊🍓🍍
- Outreachy: accessibility features documentation 🍋 🍒🍓
- Help us look for sponsorships to fund more accessibility checker improvements
- ATAG audit review 🍎🍍🍋
- Updated audit for new WCAG 2.2 rules (also updating the accessibility statement maybe to include that?)
  - (Albina) is it for Wagtail CMS?🍊🍎
- Wagtail websites’ accessibility benchmarking (statistics for GAAD 2024)

## 2023-02-16

Attendees: Albina, Jesse, Thibaud, Storm, Sage

### **Actions**

- Storm Review research visually hidden text

### **Actions review**

- Scott Read & comment on accessibility of Wagtail’s images alt text RFC
  - [https://github.com/wagtail/rfcs/pull/51](https://github.com/wagtail/rfcs/pull/51)

### **Discussions**

- Accessibility checker feedback from RNIB team
  - Key cycling - CTRL+F6 to switch to dialogs
  - “Save draft” -> show accessibility errors
    - Something to opt into?
  - Regular involvement - reviewing other parts of Wagtail
- Visually hidden [https://web-a11y.slack.com/archives/C08J06DKK/p1675785406713029](https://web-a11y.slack.com/archives/C08J06DKK/p1675785406713029)
  - [https://join.slack.com/t/web-a11y/shared_invite/zt-1ngesiobb-N7GWmMzvT3oE4DBhgIRVDQ ](https://join.slack.com/t/web-a11y/shared_invite/zt-1ngesiobb-N7GWmMzvT3oE4DBhgIRVDQ)
- [https://github.com/wagtail/wagtail/issues/10056](https://github.com/wagtail/wagtail/issues/10056)

## 2023-02-03

Attendees: Storm, Scott, Albina, Thibaud, Sage

### **Actions**

- Scott Read & comment on accessibility of Wagtail’s images alt text RFC
  - [https://github.com/wagtail/rfcs/pull/51](https://github.com/wagtail/rfcs/pull/51)

### **Actions review**

- Scott Read & comment on accessibility of Wagtail’s images alt text RFC
  - [https://github.com/wagtail/rfcs/pull/51](https://github.com/wagtail/rfcs/pull/51)
- ✅ Thibaud Contact RNIB accessibility expert

### **Discussions**

- Accessibility checker update
  - Order of results
  - More rules
  - Page editor integration
- GSoC participation: wagtail.org audit
  - [https://wagtail.org/](https://wagtail.org/)
  - [https://www.w3.org/TR/WCAG22/](https://www.w3.org/TR/WCAG22/)
- Speech recognition / voice control
  - macOS has a default

## 2023-01-20 – Accessibility checker demo

Attendees: Saptak, Jesse, Albina, Scott, Thibaud, Storm, Sage,

### **Demo**

- Happy to have made this work after struggling through Sa11y licensing issues
- Axe integration with focus on content
- Userbar error count when there are errors
- Nick’s design
- Dialog with few informations
- Feedback
  - Link to our documentation for possible solutions?
    - Can reuse documentation from Axe for each rule?
  - Surface severity?
    - Possibly useful so people don’t get held up by things that don’t make that much of a difference
  - Order of the results?
    - Right now follow order from Axe
    - Order by severity once we have more
    - Review rules to add based on their severity and easiness to fix by editors
  - False positives – allow ignoring results?

### **Discussion**

Votes: 🥭 Jesse, 🍎 Saptak, 🍐 Jane, 🍒 Scott, 🍋 Thibaud, 🍇 Sage, 🍊Albina, 🍈 Storm

- Potential improvements
  - Checks
    - Turning on more rules 🍋🥭 🍎🍇🍊
    - Wagtail-specific custom rules🍋🍈
      - Avoid image alt text ending in .jpg, .png
    - Project-specific custom rules🍈🍎🍊
    - Configuration by page type
    - Configuration by rule 🍎🥭
    - Configuration by user account type
  - Results
    - Integration with live preview panel 🍒🥭🍊🍋🍇
      - Thoughts on how? (it’s tiny)
    - Annotations on failing elements 🍒🍎🥭🍊🍇
    - Display longer description of error + solution + link to guide.wagtail.org docs?🍈🍋🍊🥭
      - Leverage existing resources where possible
    - Store results & display site-wide report 🍒🥭
    - Prevent publishing a page with errors 🍒
    - Way for editors to ignore certain issues (in case of false positives) 🍈🥭🍎
  - Manual checks
    - [Readability](https://readable.com/readability/) score for full page🍊🍋🍇🍓
    - [Readability](https://readable.com/readability/) score per field
    - Display a document heading outline 🍒🍎🍊
    - Visualise alt text🍎🍓
    - Visualise landmarks
      - (Saptak S) How much control will editors have in this though?
  - Sa11y
    - Separate Sa11y package 🍋🍈🍊
  - Test with editors
    - Ask editors how they experience the axe integration feature🍊🍎🍈🍋🍓
      - Does it help them? Any false positives?
      - Change direction based on insights from editors
      - Jesse can help with testing, Scott colleagues

## 2023-01-19 – cancelled

## 2023-01-06

Attendees: Saptak, Albina, Thibaud, Scott

### **Actions**

- ✅ Thibaud Circulate spreadsheet of Axe rules to turn on by default for feedback
- Scott Read & comment on accessibility of Wagtail’s images alt text RFC
  - [https://github.com/wagtail/rfcs/pull/51](https://github.com/wagtail/rfcs/pull/51)
- Thibaud Contact RNIB accessibility expert

### **Actions review**

- Storm to investigate possibility of Dragon developer licence (or sponsorship?)

### **Discussions**

- Axe issues rendering
  - Try outlining
  - Annotation if possible (see Axe)
- Axe issues
  - Link rendering
  - Link-name
    - For example LinkedImageBlock
- Axe configuration options
- Default alt text
  - RFC discussions
- Features beyond v4.2 release
  - Saptak doing research
  - Torchbox clients interested in this?
    - Sponsorship
  - Do we have feedback like this already?
  - Survey or user research
    - Thibaud contact RNIB contacts
- Extensible checking
  - Custom rules per organisation
  - Inclusive language / org style guide
  - (preamble: custom rules for Wagtail gotchas?)
  - Existing integrations between content checkers and Axe out there?
- Headless support?
  - Userbar should be easier to reuse as a web component
  - In preview panel – injecting Axe only

## 2022-12-22

Attendees: Albina, Jesse, Thibaud, Sage, Josh

### **Actions**

- Thibaud Circulate spreadsheet of Axe rules to turn on by default for feedback

### **Actions review**

- Storm to investigate possibility of Dragon developer licence (or sponsorship?)

### **Discussions**

- Axe rules to turn on by default
- [Sa11y specification options](https://docs.google.com/document/d/1z4z-CmX_5H2eql8heKxK3yM7FBrjta1qM_BhLKhxl_Q/edit#)
- Higher-contrast focus outline
- Color contrast issues based on CSS notation
  - [https://github.com/wagtail/wagtail/issues/9571#issuecomment-1343932716](https://github.com/wagtail/wagtail/issues/9571#issuecomment-1343932716)
  - Albina to investigate
- Button-select
  - [https://github.com/wagtail/wagtail/issues/9838](https://github.com/wagtail/wagtail/issues/9838)

## 2022-12-09

Attendees: Albina, Saptak, Thibaud, Scott, Storm, Kyle

### **Actions**

- Storm to investigate possibility of Dragon developer licence (or sponsorship?)

### **Actions review**

- ✅ Scott to add placeholder items for the accessibility roadmap
- Storm to investigate possibility of Dragon developer licence (or sponsorship?)
- ✅ Jesse to open an issue listing the various Dragon issues Albert showed us

### **Discussions**

- So many new faces! Introductions
- Complete onboarding
  - Add to [wagtail/accessibility team](https://github.com/orgs/wagtail/teams/accessibility) in github
  - Update [accessibility team members wiki](https://github.com/wagtail/wagtail/wiki/Accessibility-team#team-members)
- Accessibility checker project w/ Sa11y
  - Demo of Sa11y / introduction
  - Integration as part of existing userbar
  - Integration as part of preview panel
  - Reaching out to existing maintainers
  - Big questions to answers
  - Show on non-Wagtail pages?
    - Still feels relevant even if content isn’t editable in the CMS
  - Check whole page or only parts of the page editors have control over?
  - Only check things editors can remedy?
    - Frustrating to get reported things you can’t do anything about
    - Different amount of checking for admins vs editors
  - Sa11y as a tool – how does it work?
    - Plugin to install on a site
    - Or bookmarklet in bookmarks bar
    - [https://sa11y.netlify.app/bookmarklet/](https://sa11y.netlify.app/bookmarklet/)
  - Notification badge always visible or within menu?
    - Potentially distracting
    - But also good to be “in your face” 😄
  - False positives?
    - Can at least configure rules that apply, where they apply, via JS API
    - Issues with contrast ratio calculation
  - Reporting on successes
    - Not so useful to click through successes to get to errors
  - Errors reported in bakerydemo
    - What do we do about them?
- Rich text
  - Consider displaying on the left
  - Always visible
  - Heading level indicator in the position of circled plus? Clearer

## 2022-11-11

Attendees: Jesse, Scott, Albert, Storm

### Actions

- ✅ Scott to add placeholder items for the accessibility roadmap
- Storm to investigate possibility of Dragon developer licence (or sponsorship?)
- ✅ Jesse to open an issue listing the various Dragon issues Albert showed us

### Actions review

- ✅ Thibaud Review Jane’s accessibility audit of wagtail.org re-launch over the weekend
- ✅ Scott Review Jane’s accessibility audit of wagtail.org re-launch over the weekend
- Thibaud Raise wagtail.org launch concerns with core team
- ✅ Storm Check with Joey availability for usability testing of Wagtail 4.1
  - Joey is happy to do usability testing with screen magnification.
- Thibaud Check with Steph & Olly re user testing sessions w/ users of assistive tech

### Discussions

- Accessibility Roadmap
  - Discussion started on Slack
  - We’ve had WCAG compliance on the roadmap for a while. When do we consider this complete?
  - Do we keep it on the roadmap
  - We keep it on the roadmap pending an audit
  - We can mention the automated testing issues still open.
  - We can report on manual audits
  - LB commented on roadmap item and asked for the spreadsheet with issues to be shared
  - Generally mention the accessibility goals of Wagtail, link to accessibility statement
  - Scott happy to add placeholder for these items
- Albert demonstrating issues in Wagtail 4 with speech recognition Dragon
  - Activate elements; ‘click link’, ‘click button’.
  - When I try to add a streamfield block, I say click add. Same for click delete.
  - If I don’t know what a button is called, I say ‘click button’.
  - Screenshot of Wagtail 3
  - Then all buttons on the page are numbered and I can say the number.
  - This works fine if all buttons are visible. Many buttons are hidden in Wagtail
  - If I want to publish a page, this does not work. Dragon does not recognize the chevron as button that will open a dropdown
  - Some menu items are labelled as buttons, some are labelled as links. When I say click link only links are highlighted. This does not include all menu items.
  - Breadcrumbs are ‘collapsed’ until hovered over.
  - Can’t engage with minimap – can only be interacted with when hovered over.
  - When I want to collapse a section, I’d say ‘click collapse introduction’ but this collapses all sections on the page.
  - Using Dragon in Wagtail 3 rich text editor, the rich text editor crashes. In Wagtail 4 the rich text editor does not crash but Dragon does not recognize the field as something that can be edited. Dragon calls this a dictation box.
    - Slack does not support dictation boxes. Has to be opened manually. When finished dictating, the text is copied and pasted into the Slack edit field by Dragon.
- Next steps are to open an issue and list these examples.
- Storm to investigate the possibility of getting a Dragon licence for sponsorship.

## 2022-10-27

Attendees: Jane, Albert, Thibaud, Scott, Storm

### Actions

- Thibaud Review Jane’s accessibility audit of wagtail.org re-launch over the weekend
- Scott Review Jane’s accessibility audit of wagtail.org re-launch over the weekend
- Thibaud Raise wagtail.org launch concerns with core team
- ✅ Storm Check with Joey availability for usability testing of Wagtail 4.1
  - Joey is happy to do usability testing with screen magnification.
- Thibaud Check with Steph & Olly re user testing sessions w/ users of assistive tech

### Actions review

- No actions last time

### Discussions

- Welcome Albert!
- Hi Jane!
  - RNIB collab on CMS next year
- Speech recognition software support
  - No expertise in the room :’)
- [https://guide.wagtail.org/](https://guide.wagtail.org/) launch
- wagtail.org launch (preview: [https://wagtail-org-production.herokuapp.com/](https://wagtail-org-production.herokuapp.com/))
  - Jane share audit
  - Hols next week
  - Push back on launch date?
  - Also for packages
- User testing
  - Could we get Joey to help?
  - JPL trialling Fable
  - Videos invaluable to inform our work
    - Screen reader (Musharaf?)
    - Screen magnification (Joey?) / text zooming
    - Speech recognition (Alert?)
    - Assisted digital?
    - Cognitive accessibility
    - Motor
  - Work with community rather than Fable 😄
  - Any examples of videos like this?

## 2022-10-14

Attendees: Storm, Saptak, Jesse, Thibaud

### Actions

### Actions review

- ✅ Thibaud Outreachy accessibility checker project idea
- ✅ Scott Review Outreachy project idea
- ✅ Jesse Review Outreachy project idea

### Discussions

- Figma review Wagtail 4.1dev
- Backlog of issues for 4.2

## 2022-09-16

Attendees: Jesse, Thibaud, Scott

### Actions

- ✅ Thibaud Outreachy accessibility checker project idea
- Scott Review Outreachy project idea
- Jesse Review Outreachy project idea

### Actions review

- Thibaud [Refine Pa11y test results into issues backlog](https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html) (some day)
- Jesse Review Wagtail 4.0 for potential accessibility gotchas (some day)
- ✅ Scott

### Discussions

- Outreachy accessibility project $8’000
  - 23/09 project idea -> 29/09
  - Due soon, main project idea + stretch goals
- Minimap
  - Tab stop after tabs
  - Tab stop for collapse all + minimap toggle? Or single
  - Need better indication of depth w/ SVG lines
  - Also have this on other models editing forms?
    - Snippets / arbitrary models
    - Images and documents meh
    - StreamField navigation menus
      - Someone somewhere mentioned this (Slack)
      - Settings contrib
    - Dev API to exclude sections from minimap
      - Relationship w/ field-level editing permissions
    - Tree collapsing / expanding / file system type nav
- Accessibility reviews as a group
  - [Forms navigation](https://www.figma.com/file/CmvZbE6mBMk2apcuFeyqKP/Wagtail-4.0-forms-navigation?node-id=0%3A1)
    - InlinePanel summarisation feature for collapsed and for minimap
  - [Contrast themes](https://www.figma.com/file/O81E48wieOZ7e6AivvksWn/Contrast-themes%3A-Wagtail-audit?node-id=6901%3A4107)

## 2022-09-01

Attendees: Jesse, Scott, Storm, Thibaud

### Actions

- Thibaud [Refine Pa11y test results into issues backlog](https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html)
- Jesse Review Wagtail 4.0 for potential accessibility gotchas

### Actions review

- ✅ Thibaud, Saptak, Jane, Anuja Refine Contrast themes project plan on a call
- Thibaud [Refine Pa11y test results into issues backlog](https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html)

### Discussions

- [GSoC Contrast Themes](https://github.com/orgs/wagtail/projects/5?query=is%3Aopen+sort%3Aupdated-desc)
  - Running vanilla Pa11y against bakerydemo, opening issues
  - Also trying wagtail-tooling repo to test Wagtail core
  - Learning about Tailwind
  - [https://docs.wagtail.org/en/stable/releases/4.0.html#windows-high-contrast-mode-support-improvements](https://docs.wagtail.org/en/stable/releases/4.0.html#windows-high-contrast-mode-support-improvements)
  - Potentially to pick up after the project: small issues
  - Next big frontier: dark mode for Wagtail admin, & other theming options
- Scrutiny on Wagtail 4.0
  - [https://developer.mozilla.org/en-US/docs/Web/CSS/@media/hover](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/hover)
  - Demo site: [https://wagtaildemo-nightly.herokuapp.com/admin/](https://wagtaildemo-nightly.herokuapp.com/admin/)
    - Usual logins/passwords
- Accessibility reviews as a group
- Accessibility checker – it’s happening soon
- Outreachy accessibility ideas
  - Command palette in Wagtail (for easier navigation?)
  - [https://www.outreachy.org/docs/community/](https://www.outreachy.org/docs/community/)

## 2022-08-19 – cancelled

Cancelled because a lot of people could not make it.

## 2022-08-04

Attendees: Scott, Kyle, Saptak, Thibaud

### Actions

- Thibaud, Saptak, Jane, Anuja Refine Contrast themes project plan on a call
- Thibaud [Refine Pa11y test results into issues backlog](https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html)

### Discussions

- GSoC Contrast Themes
  - [https://docs.wagtail.org/en/latest/releases/4.0.html#windows-high-contrast-mode-support-improvements](https://docs.wagtail.org/en/latest/releases/4.0.html#windows-high-contrast-mode-support-improvements)
- Focus indicator
- Sections collapse
- WCAG 2.2

## 2022-07-22

Attendees: Kyle, Storm, Scott, Thibaud, Anuja, Joey

### Actions

### Discussions

- GSoC: Contrast Themes project+
- Accessibility testing
  - Hover effects for interactive elements
    - Important to have very clear hover effects
    - And consistent mouse pointers
    - Need a way for us to test hover effects on all components
  - RNIB: Borders around icon-only buttons?
    - Some icons are pretty obvious
    - Worth checking for different users - more or less tech-savvy
    - Microsoft Outlook has a text-only mode? As part of Braille support
    - Look at what other software does?
  - [Sa11y](https://sa11y.netlify.app/)
    - Need to think about this more
    - List of all errors at the top
      - Link to the field with the error
    - Saves on a lot of scrolling
  - [New Listings designs](https://www.figma.com/file/3SZAkXYKTo52047weXDvb9/Wagtail-3-UI-Inventory?node-id=6787%3A34720): filters, sort orders
    - Filters aligned with columns: helps a lot visually (less scrolling)
    - No particular issues with sticky header patterns (if it doesn’t cause keyboard issues)
    - Make the reordering controls at least the size of the text
      - Avoid changing zoom level if possible (not that big of a pain but nice not to have to change)
  - Tech-savvy users vs. not tech savvy
    - People who use screen readers generally have to learn the shortcuts
  - Text inputs
    - Problems with gray backgrounds
  - Bulk action checkboxes
    - Darker border
  - Title field
    - Is it clear enough?
    - Hover effect can be missed if you’re zoomed in
    - Bottom border?
    - Should have a border when empty
- RNIB issues
  - Filed 3 in particular that feel ready for us to take on
  - RNIB – advocacy group in the UK for blind & low-vision people

## 2022-07-07

Attendees: Storm, Thibaud, Saptak

### Actions

- ✅ Thibaud Schedule alternative meeting times – Friday
- ✅ Thibaud Create RNIB feedback issues
- Thibaud, Saptak, Jane, Anuja Refine Contrast themes project plan on a call
- ✅Thibaud Check call invite for Saptak
- Thibaud [Refine Pa11y test results into issues backlog](https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html)
- ✅ Jane, Anuja, Thibaud Auditing in high contrast mode

### Discussions

- Pa11y report
  - [https://github.com/thibaudcolas/wagtail-tooling](https://github.com/thibaudcolas/wagtail-tooling)
  - [https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html](https://wagtail-tooling-sample-reports.netlify.app/20220630-pa11y/index.html)
- Contrast themes
  - [https://github.com/garris/BackstopJS](https://github.com/garris/BackstopJS)
- Transparent borders
  - Message / alert at the top of the page [https://github.com/wagtail/wagtail/issues/8836](https://github.com/wagtail/wagtail/issues/8836)
  - Dropdowns & tooltips without backdrops [https://github.com/wagtail/wagtail/issues/8830](https://github.com/wagtail/wagtail/issues/8830)
  - General guideline
    - Thick border so it’s clearer it floats on the page: 10px
  - Border for “ghost” text only
    - Later: Consider adding an underline everywhere?
    - Or an icon?
    - [https://github.com/wagtail/wagtail/issues/8834](https://github.com/wagtail/wagtail/issues/8834)
  - Footer actions (thick border) (experiment, unclear since it’s always on)
  - Login form field borders
- Joey working with Storm
  - User of magnifiers, high contrast mode, screen readers
  - Invited to accessibility team

## 2022-06-23

Attendees: Scott, Thibaud

### Actions

- Thibaud, Saptak, Jane, Anuja Refine Contrast themes project plan on a call
- Thibaud Refine Pa11y test results into issues backlog
- Jane, Anuja, Thibaud Auditing in high contrast mode

### Discussions

- Rich text toolbars
- GSoC Contrast Themes
- Accessibility / UI team expertise requested: [admin confirm before deleting page if contains multiple subpages #8703](https://github.com/wagtail/wagtail/pull/8703#issuecomment-1161885185)
- Feedback from RNIB
  - Tooltips usage
    - “Many icons that exist without visible text on screen such as ‘+’ and ‘x’ icons used for adding and removing sections.”
    - Using `title` attributes in quite a few places
    - Icon sizes? Sometimes icons may be hard to understand because they’re too small
    - Text more important for buttons that can have “arbitrary” icons (vs. places where only one icon is ever used, such as navigation)
    - Tooltips on sidebar “expand sub-menu”? Not sure if needed
    - Tooltips in page explorer would be nice
    - Text-only mode
  - Focus outline
    - “Non-text contrast issues with keyboard focus on key elements”
    - Tweak color to rate higher against APCA (and WCAG 2 if possible?) on white
    - Keep single-tone outline
    - [https://www.myndex.com/APCA/](https://www.myndex.com/APCA/)
    - Title field

## 2022-06-09

Attendees: Jane, Thibaud, Saptak, Jesse, Anuja

### Actions

- Thibaud, Saptak, Jane, Anuja Refine Contrast themes project plan on a call
- Thibaud Refine Pa11y test results into issues backlog
- Jane, Anuja, Thibaud Auditing in high contrast mode

### Discussions

- Introductions
- GSoC Contrast themes
  - Refine backlog on a call – Saptak, Thibaud, Jane, Anuja
  - Based on public issues
  - And automated tests review – Thibaud to refine on his own & add to public issues
- Auditing in high contrast mode - Jane, Anuja, Thibaud
  - All tracking issues in shared sheet
  - Based on tracked Wagtail views
  - Audit in June

## 2022-05-26 – Team kickoff

- Welcome & introductions
  - Jane! Front-end developer & accessibility expert, Torchbox. GSoC project support
  - Jesse. Syracuse University. Get to work on open source, hoping to keep up with accessibility work
  - Scott. GSoC project
  - Saptak. Working with Wagtail a lot. Helps
- Intro to current accessibility efforts
- How the team works
  - Initial plan: open membership, 45-min chats every two weeks to provide feedback and take actions.
    - One week always the same time. Jane: not fridays. Saptak: thursdays
    - 45min every two weeks around this time Thursdays
  - 6months membership
- What do we all want to achieve with the accessibility team?
  - 🥭 Jesse, 🍎 Saptak, 🍐 Jane, 🍒 Scott, 🍋 Thibaud
  - GSoC Contrast themes / Windows High Contrast Mode support 🍒🍐🍎🍋🥭
    - Brief discussion so far. Kickoff / intros soon
    - Open questions on structuring the work & schedule
    - Anuja part of our team
    - Scope: extend towards dark mode, other color themes (under user control within the CMS)
    - Jesse checking with colleagues (can’t all ban Windows!)
    - Saptak has experience. Specific site with theme selector ([https://mxb.dev/](https://mxb.dev/))
  - Sa11y integration 🍎🍐🍋🥭
  - ATAG 2.0 conformance 🍎🍐🥭
  - Benchmarking / HTTP Archive’s Web Almanac 🍋
    - Accessibility chapter Saptak authoring Thibaud analyst-ing
    - See charts like the ones in the Almanac improve
  - SVG icons 🍒
  - Page editor project support 🍒🍎

## 2021-12 – Page editor feedback & design considerations

Designs (for editing): [Wagtail editor 4 (Accessibility team copy)](<https://www.figma.com/file/UTuPx9UV1vzBEXzcaeEqVH/Wagtail-Editor-4-(Accessibility-team-copy)?node-id=2201%3A29434>)

Prototype (with hotspots): [Wagtail Editor 4 prototype](https://www.figma.com/proto/7l3IqiyVZqHT5wrzEAivCe/Wagtail-Editor-4?page-id=225%3A3&node-id=1702%3A21256&starting-point-node-id=1702%3A21256)

[Accessibility bluelines](https://dribbble.com/shots/6269661-Accessibility-Bluelines)

### 2021-12 Saptak feedback

### 2021-12 Thibaud feedback

- Top bar – is it ok to have two tablists? Or do we want tablist + something more bespoke
- Heading navigation
  - Does the title field get preceded with a SR-only <h1>? Or no h1?
  - Do field panels make fieldsets and legends, or sections and headings, or both

### 2021-11-16 Thibaud feedback

This has all been shared with Ben already and taken into account – copying here for reference.

- Title
  - I think it’d be worth trying to have some affordance that the title is editable without relying on hover – when I create a page, can I tell there is a field here?
  - - Potentially having a small "Title" label above this
  - - Or perhaps a character count? That’s something we’ve been keen to have more of anyway
  - - Or something more visually prominent but perhaps only there when the field is empty, say a Material UI - style underline
- Help text
  - With the help text inline, we should provide a recommended "maximum help text length" so it fits in a single line – and perhaps have it truncated above? (expandable on demand)
- Date picker
  - Could we try placing the icon on the right, and having it appear as a focusable button, similar to https://duetds.github.io/date-picker/?
  - This would be important for keyboard and screen reader users, so there is a separate UI element dedicated to triggering the appearance of the date picker.
  - It doesn’t need to be fully recognisable as a button, but it needs to be distinguishable from the decorative icons we have next to labels. And needs to be focusable separately from the field.
- Textarea
  - Could we make it so those text boxes are resizeable by end users? Could also be worthwhile adding a character count on here so we make sure there is space somewhere.
- Asterisk / error message
  - I like the subdued asterisk but wonder if that will work with error message styling – what would they look like?
  - See https://github.com/wagtail/wagtail/pull/7663, which also introduces an icon so error messages are distinguishable with something else than color. I don’t think the icon is necessary to meet any particular accessibility requirement, but it’s an interesting consideration.
- Field grouping icons
  - We might need to review & expand our icon set if we expect people to make use of them for field groupings?
  - Or consider what it’d look like if few / no icons were used?
- Image chooser
  - Nice to have: changing the image chooser preview so the image’s title is displayed somewhere. Right now if you can’t see the imagery well, the only way to know for sure is to click Change or Edit, which takes a lot of time
- StreamField block controls
  - Re our discussion about discoverability of those hoverable controls – a solution could be to have a block "grab handle" on the right-most edge identical to the one we have on the left? This could be the always-on visual indicator there are things happening here, and then the only control that’s not within this group is the "Add".
  - We could also make it so "activating" this grab handle causes all block delimitations to be visible similar to what we’d need for drag'n'drop.
- Sidebar
  - Thinking about this map component a bit more, I really like the idea of having it there to help with keyboard navigation too. Since the page editor is essentially a big form full of rich text & StreamField widgets, it’s very hard to tab through everything to go to a given field.
- Switch control
  - Note if we go for this switch – would be nice for the off and on states to have a bigger difference in luminance than they do at the moment. Currently it feels a bit hard to tell which side is "active" for people who have red-green color blindness unless they’re also aware that "left" is off and "right" is on.
- Inline preview
  - Something we might lose a bit with this inline preview is the ability to add content checks within the preview like https://github.com/neon-jungle/wagtail-accessibility (since there won’t be enough space). Would be nice if there was a place within this inline preview UI to trigger those checks?
- Page history
  - Couple of points here – I think this looks great but I doubt we’d want to build the page history listing this way considering the complexity (unless we used a similar virtualised / fading listing pattern in more valuable places)
  - - The fading-out list pattern is pretty hard to do well in browsers
  - - We’d likely need pagination or "scroll to load" for pages that have lots of entry
- Field groups font size
  - It’d be nice to increase the font size throughout also so we can give Wagtail implementers more heading levels to play with?
  - We have those h2-level styles for top-level field groups, then I can easily see at least one h3-level "group within group", and then h4-type styles for field labels
- Dark mode
  - Have we considered a dark mode version? As well as the cool factor, I understand it’d help with accessibility for people with low vision.

## 2021-11-10 -- Team 6-monthly report

### Membership

- Members:
  - Scott Cranfill ([@Scotchester](https://github.com/Scotchester)), UTC - 4 or 5, since June 2020
  - Thibaud Colas ([@thibaudcolas](https://github.com/thibaudcolas)), UTC + 0 or 1, since June 2020
  - Jesse Menn ([@jessemenn](https://github.com/jessemenn)), UTC - 4 or 5, since February 2021
  - Kyle Bayliss ([@kbayliss](https://github.com/kbayliss)), UTC + 0 or 1, since February 2021
  - Storm Heg ([@Stormheg](https://github.com/Stormheg)), UTC + 1 or 2, since February 2021
  - Saptak Sengupta ([@SaptakS](https://github.com/SaptakS)), since July 2021
- 6 people active during the last 6 months, 4 attending meetings on average
  - Compared to 5 people involved last term, with only 2 attending meetings on average
  - 4 new members this term
  - With Saptak joining us mid-term
  - 3 people on core team
- Met 14 times over 7 months, compared to 9 over 6 months last term

### Recurring themes

- Completing the SVG icons conversion to improve accessibility of icons in the CMS admin
- Testing more of Wagtail – mini audits from Kyle, Jesse, Thibaud
- Accessibility statement
- High-contrast mode support
- Involvement with feature development (slim sidebar, bulk actions, typed table block)
- Outreach

#### Themes from last term

- Completing the SVG icons conversion to improve accessibility of icons in the CMS admin
- Documenting [accessibility considerations](https://docs.wagtail.io/en/stable/advanced_topics/accessibility_considerations.html) for Wagtail sites
- Curating a backlog of accessibility improvements for sites <https://github.com/wagtail/wagtail/projects/10>
- We were also keen to do more automated tests and manual auditing but didn't get around to it.

### Agenda / changes we wanted in the last term

- ✅ Create plan to recruit 5 members
- ❌ Open office hours?
- ✅ Create and publish accessibility audits of Wagtail to have a clear record of our current state
- ✅ Update Wagtail contribution guidance, and PR template, to make it clear individual pull requests should include accessibility testing. Review issue templates as well
- ✅ 45min meetings in the future.
- ❌ Thibaud draft RFC for automated accessibility tests

### Agenda / changes for next 6 months

- Our team
  - Continue Bi-weekly meetings
  - Continue Half a dozen members = at least 3 in attendance
  - Do more outreach – publicising more about a11y efforts that are being taken (e.g. a11y statement, progress in a11y improvements done) to make more people aware and interested to give feedbacks
- CI / automated checks on PR
  - Introduce this for whole admin
  - Prevent UI features with accessibility issues getting released
- Accessibility team reviews
  - Accessibility involvement at design phase rather than code review phase
  - Systematic design reviews for accessibility considerations
  - Recurring item in our team's agenda, so we keep in touch with the core team and set the expectation we're expecting to be reviewing features / designs
  - Keep in mind we don't necessarily want to mandate designs -- it's ok to code first, just want to make sure there is room for accessibility review
- Upcoming work
  - Page editor
  - Windows High Contrast Mode.
  - Continue pushing the SVG icon boulder up the hill :)
  - Low-hanging fruits to tackle
  - Leverage IE11 support removal
  - Triage accessibility issues for new contributors

## 2021-10-15 -- retrospective

Attendees: Scott, Thibaud, Saptak

### Actions

- Saptak Share research on uppercase / capitalized text
- ✅ Thibaud Trial removing all uppercase
- <https://wagtailcms.slack.com/archives/CB7L6L5S6/p1634332413035500?thread_ts=1634249236.029900&cid=CB7L6L5S6>
- ✅ Thibaud Share retrospective with core team

### Discussions

- CI / automated checks on PR
  - Start Set up automated accessibility tests for the whole admin
  - Start/Continue  making stricter a11y related CI checks to prevent UI features with a11y issues getting released?
  - Start implementing automated accessibility testing on PRs.
  - Stop allowing features that involve UI to be merged without meeting some list of accessibility standards.
  - Discussion
    - Check diff from PR?
- Design phase
  - Continue Review of all designs for accessibility considerations
  - Continue paying close attention to editor UI overhaul for accessibility issues.
  - bring up things that need review from a11y team.
  - Continue  implementing a11y at the design phase itself instead of in the review phase for new features?
  - Start UI dev direction on all headline release features at inception
  - Discussion
    - Recurring item in our team's agenda, so we keep in touch with the core team and set the expectation we're expecting to be reviewing features / designs
    - Keep in mind we don't necessarily want to mandate designs -- it's ok to code first, just want to make sure there is room for accessibility review
- Core team
  - Start UI dev team in addition to accessibility
  - Start evolving into the proposed UI Team??
  - Continue paying close attention to editor UI overhaul for accessibility issues.
  - Continue raising awareness of accessibility issues and goals during Core Team discussions.
- Accessibility team
  - Start Systematic review of all UI PRs by either UI dev or accessibility team
  - Start publicising more about a11y efforts that are being taken (e.g. a11y statement, progress in a11y improvements done) to make more people aware and interested to give feedbacks
  - Continue doing meeting biweekly to discuss different things and bring up things that need review from a11y team.
  - Continue having a team of about a half dozen, which usually results in at least 3 people in attendance for regular meetings.
- Current work
  - Continue the great work knocking out the Windows High Contrast Mode issues.
  - Continue pushing the SVG icon boulder up the hill :)
  - Start tackling low-hanging fruit in existing codebase (e.g., capitalized button text issue).
    - Pretty frequent issue
- Misc
  - Continue Triage & curation of accessibility issues backlog, with good first issues in particular
  - Continue Fully remove all IE11 / legacy code so we can leverage more modern browser features
  - Continue Make the styles linting config stricter for common accessibility issues
    - Disallow px units for font-size
    - Disallow hover styles without focus
- Release notes
  - Typed table block release notes / experimental nature
  - High contrast mode

## 2021-10-01

Attendees: Thibaud, Jesse, Saptak, Scott, Kyle

### Actions

- ✅ Thibaud Review draft from Saptak
- Thibaud Blog post about high-contrast mode & Saptak joining our team
- ✅ Thibaud Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
- Add test plan for issue
- ✅ Saptak Add extra notes to accessibility review issue for bulk actions
- ✅ Thibaud Raise accessibility statement at next core team meeting
- ✅ Thibaud Share plan of UI / accessibility work over next 3 months
- ✅ Thibaud Check DjangoCon US plans outside of sprints (not happening)

### Discussions

- Actions review
  - Thibaud Review draft from Saptak
  - Thibaud Review [Fix userbar tabbing behaviour #7507](https://github.com/wagtail/wagtail/pull/7507)
  - Thibaud Look into Squash.io usage
    - ✅Issue with ports fixed: [#7523](https://github.com/wagtail/wagtail/pull/7523)
  - Thibaud Blog post about high-contrast mode & Saptak joining our team
  - ✅ Saptak Add notes from review of bulk actions
  - Thibaud Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
  - Scott Raise accessibility statement at next core team meeting
  - Thibaud will do next week if this hasn't happened
  - ✅Thibaud Review whether there is upcoming work on More dropdown
    - Yes -- from January onwards
  - ✅Storm Triage issues for Hacktoberfest
    - Has happened even if not Storm

## 2021-09-17

Attendees: Saptak, Scott, Jesse, Storm, Thibaud

### Actions

- Thibaud Review draft from Saptak
- Thibaud Review [Fix userbar tabbing behaviour #7507](https://github.com/wagtail/wagtail/pull/7507)
- Thibaud Look into Squash.io usage
  - ✅Issue with ports fixed: [#7523](https://github.com/wagtail/wagtail/pull/7523)
- Thibaud Blog post about high-contrast mode & Saptak joining our team
- Saptak Add notes from review of bulk actions
- Thibaud Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
- Scott Raise accessibility statement at next core team meeting
- Thibaud Review whether there is upcoming work on More dropdown
- Storm Triage issues for Hacktoberfest

### Discussions

- Actions review
  - ✅Saptak Review accessibility statements from other projects & outline of page contents for Wagtail
  - ✅Storm Work on last change for userbar ARIA menu practice
  - [Fix userbar tabbing behaviour #7507](https://github.com/wagtail/wagtail/pull/7507)  - ready for review
    - Scott trying out with squash.io?
  - Thibaud Blog post about high-contrast mode & Saptak joining our team
  - ✅Saptak Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
  - Thibaud Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
- [Accessibility statement](https://docs.google.com/document/u/1/d/1D07GcfmH6R6ZbawomAje5TpcsGASxLi4dz5r_ZirQiA/edit)
- SVG icons
  - Scott & Thibaud
  - One more thing!
    - More dropdown [#6281](https://github.com/wagtail/wagtail/issues/6281)
    - Potentially refactored as part of editor UI?
- Hacktoberfest
  - Good first issues on high-contrast mode
  - Curate ahead of the event?
  - Add to blog post?
  - Issue triage & review of existing Good first PRs ahead of Hacktoberfest

## 2021-09-03

Attendees: Storm, Thibaud, Jesse, Saptak, Scott

### Actions

- Saptak Review accessibility statements from other projects & outline of page contents for Wagtail
- Storm Work on last change for userbar ARIA menu practice
- Thibaud Blog post about high-contrast mode & Saptak joining our team
- Saptak Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
- Thibaud Test bulk-actions work about to be merged, currently in <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>

### Discussions

- Actions review
  - ✅ Thibaud Review high-contrast mode audit from Kyle
    - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
    - Blog post
    - Assistiv Labs
  - ✅ Thibaud Update CONTRIBUTING.md with accessibility opportunities
    - <https://github.com/wagtail/wagtail/pull/7462>
  - Saptak Review accessibility statements from other projects & outline of page contents for Wagtail
    - More work on this over the next week
  - ✅ Thibaud Review & merge <https://github.com/wagtail/wagtail/pull/7408>
  - ✅ Thibaud Update footer actions issue with recommendation for ARIA markup based on review ([https://w3c.github.io/aria-practices/examples/menubar/menubar-navigation.html](https://w3c.github.io/aria-practices/examples/menubar/menubar-navigation.html_)) <https://github.com/wagtail/wagtail/issues/7366>
  - Storm Work on last change for userbar ARIA menu practice
    - Evaluating two different ways to do this
      - Roving tabindex (considering this for now)
      - aria-activedescendants
  - ✅ Thibaud Add Saptak to accessibility team roster & invite to GitHub team
- High-contrast mode -- 20 issues
  - Planning a blog post to spread the word about high-contrast mode, our recent work, Saptak's involvement, and encourage participations from potential users of high-contrast mode.
  - [High-contrast mode: Dashboard icons are hard to see and should use link text color #7325](https://github.com/wagtail/wagtail/issues/7325)
  - [High-contrast mode: SVG icons within links should match link text colour #7326](https://github.com/wagtail/wagtail/issues/7326)
  - [Hamburger menu doesn't work for keyboard and high-contrast mode users #7327](https://github.com/wagtail/wagtail/issues/7327)
  - [High-contrast mode: Breadcrumb separator should match link text colour #7328](https://github.com/wagtail/wagtail/issues/7328)
  - [High-contrast mode: Explorer wagtail icon is hard to see on dark background #7329](https://github.com/wagtail/wagtail/issues/7329)
  - [High-contrast mode: Comments icon should match link colour #7331](https://github.com/wagtail/wagtail/issues/7331)
  - [Collapsible panels in edit UIs are impossible to open or close with keyboards or screen readers #7332](https://github.com/wagtail/wagtail/issues/7332)
  - [High-contrast mode: Success/Warning/Error help-block content needs a border to be more identifiable #7447](https://github.com/wagtail/wagtail/issues/7447)
  - [High-contrast mode: icon buttons with no text appear squashed #7448](https://github.com/wagtail/wagtail/issues/7448)
  - [High-contrast mode: buttons with .disabled class look active in high-contrast mode #7449](https://github.com/wagtail/wagtail/issues/7449)
  - [High-contrast mode: dropdown menu needs custom styles #7450](https://github.com/wagtail/wagtail/issues/7450)
  - [High-contrast mode: Switches do not visually convey their state #7451](https://github.com/wagtail/wagtail/issues/7451)
  - [High-contrast mode: Search form should define a border #7452](https://github.com/wagtail/wagtail/issues/7452)
  - [High-contrast mode: active tab can't be determined #7453](https://github.com/wagtail/wagtail/issues/7453)
  - [High-contrast mode: tag field shouldn't override background #7454](https://github.com/wagtail/wagtail/issues/7454)
  - [High-contrast mode: vertical separation between field panels is lost #7455](https://github.com/wagtail/wagtail/issues/7455)
  - [High-contrast mode: sidebar needs vertical separation with main content #7456](https://github.com/wagtail/wagtail/issues/7456)
  - [High-contrast mode: StreamField block chooser menu buttons do not look like buttons #7457](https://github.com/wagtail/wagtail/issues/7457)
  - [High-contrast mode: comments dropdown needs a border #7458](https://github.com/wagtail/wagtail/issues/7458)
  - [High-contrast mode: Comment buttons should use button text colour #7459](https://github.com/wagtail/wagtail/issues/7459)
- Accessibility time in October
  - UI architecture tech debt: <https://github.com/wagtail/wagtail/issues/3804>
  - Looking for 2-3 people to contribute
- Review accessibility of new checkbox design
  - Raised by Storm (bulk actions mentor)
  - Current unchecked checkboxes don't have a lot of contrast against background.
  - New design (for bulk actions): <https://www.figma.com/file/q6DeuoBXGCtYdf7GdGJs8D/Wagtail-Design-Toolkit?node-id=972%3A53>
  - Bulk actions team requests a11y team expertise: is this new design accessible? Are there any recommendations we should consider when implementing this design?
  - Bulk actions follow-up
    - Running out of time
  - Keen on more thorough
    - Saptak & Thibaud split testing
    - Demo site: <https://wagtaildemo-bulk-actions.herokuapp.com/admin/>
    - Do testing on <https://github.com/wagtail/wagtail/tree/feature/bulk-actions>
    - Report issues on GitHub
- 2.15 release!
  - Bulk actions
  - Wagtail Live
  - New search backends
  - New sidebar -- feature flag
  - Icons PR
    - Monday, Tuesday next week, for Thibaud w/ Scott reviewing

## 2021-08-20

Attendees: Thibaud, Saptak

### Discussions

- CONTRIBUTING.md update [#7462](https://github.com/wagtail/wagtail/pull/7462)
- Accessibility statement

## 2021-08-06

Attendees: Thibaud, Saptak, Scott

### Actions

- Thibaud Review high-contrast mode audit from Kyle
- <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
- Thibaud Update CONTRIBUTING.md with accessibility opportunities
- Saptak Review accessibility statements from other projects & outline of page contents for Wagtail
- Thibaud Review & merge <https://github.com/wagtail/wagtail/pull/7408>
- Thibaud Update footer actions issue with recommendation for ARIA markup based on review (<https://w3c.github.io/aria-practices/examples/menubar/menubar-navigation.html_>) <https://github.com/wagtail/wagtail/issues/7366>
- Storm Work on last change for userbar ARIA menu practice
- Thibaud Add Saptak to accessibility team roster & invite to GitHub team

### Discussions

- Actions review
  - Thibaud Review high-contrast mode audit from Kyle
    - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
  - ✅ Saptak Review proposal for contributor call to action <https://github.com/wagtail/wagtail/pull/7330#pullrequestreview-703416391>
  - ✅ Storm review Jesse's <https://github.com/wagtail/wagtail/pull/7346>
  - ✅ Thibaud review issue <https://github.com/wagtail/wagtail/issues/7333>
  - Storm Work on last change for userbar ARIA menu practice
  - ✅ Thibaud Review recommendations for action menus with mixed links and buttons
  - ✅ Thibaud Check whether we have an open issue for actions menu keyboard & SR support
    - <https://github.com/wagtail/wagtail/issues/7366>
- Accessibility statement & contributing
  - CONTRIBUTING.md update
  - Accessibility statement
    - On the website
    - We care
    - Review other CMSes' statements?
- Icons transition!
  - Change icon source files to use <svg> elements rather than <symbol>
  - Makes the files usable as-is in CSS content attributes (as URLs)
  - Convert to <symbol> elements for sprites in Wagtail core
  - Same for icons added by Wagtail implementers
  - Scott interested in working on this but on holidays soon (7--15 Aug.)
  - 3-4 days on Wagtail for Thibaud in early September (or late September)

## 2021-07-23

Attendees: Saptak, Storm, Scott, Jesse, Thibaud, Kyle

### Actions

- Thibaud Review high-contrast mode audit from Kyle
- <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
- Team Review proposal for contributor call to action <https://github.com/wagtail/wagtail/pull/7330#pullrequestreview-703416391>
- Storm review Jesse's <https://github.com/wagtail/wagtail/pull/7346>
- Thibaud review issue <https://github.com/wagtail/wagtail/issues/7333>
- Storm Work on last change for userbar ARIA menu practice
- Thibaud Review recommendations for action menus with mixed links and buttons
- Thibaud Check whether we have an open issue for actions menu keyboard & SR support

### Discussions

- Actions review
  - ✅ Thibaud Userbar keyboard support blog post / screen recording demo
  - <https://www.youtube.com/watch?v=m6ybdesbaFk>
  - Thibaud Review high-contrast mode audit from Kyle
  - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
  - ✅ Jesse Open ModelAdmin issue (edit unreachable with keyboard only)
  - Storm Work on last change for userbar ARIA menu practice
  - Thibaud Review recommendations for action menus with mixed links and buttons
  - Thibaud Check whether we have an open issue for actions menu keyboard & SR support
- Update on sidebar
  - Not working on this right now, taken over by Karl
  - Storm reviewing
- Keyboard shortcuts for common actions?
  - Right now
    - Ctrl + P for publish
    - Ctrl + M for
    - Common actions: <https://github.com/wagtail/wagtail/issues/3949>
- How to make this happen?
  - Way to register shortcuts?
  - Accessibility or usability thing?
  - Keyboard support is good
- Assistiv Labs for Wagtail -- update next week
- DjangoCon US 2021 -- October 2021
  - <https://2021.djangocon.us/>
  - 21-23 October
  - Keen: Thibaud, Scott, Kyle, Saptak, (Storm?)
- Icons came up in last core team meeting
  - We're not that far from finishing this off
  - There are a lot of icons which will be reworked anyway as part of the sidebar UI overhaul

## 2021-07-09

Attendees: Storm, Saptak, Thibaud, Jesse

### Actions

- Thibaud Userbar keyboard support blog post / screen recording demo
- Thibaud Review high-contrast mode audit from Kyle
- <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
- Jesse Open ModelAdmin issue (edit unreachable with keyboard only)

### Discussions

- On the agenda today
- Hello Saptak!
- Actions review
  - ✅ Thibaud Try out styling overrides fix for userbar ul and li [#6994](https://github.com/wagtail/wagtail/pull/6994)
    - Follow-up [#7290](https://github.com/wagtail/wagtail/issues/7290)
  - ✅ Thibaud Update Figma file with Space key from menu ARIA practices
    - Storm working on the implementation in 2 weeks
  - Thibaud Review high-contrast mode audit from Kyle
    - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
  - Scott Review accessibility of search autocompletes in docs theme -- built-in, and Algolia
  - ✅ Storm Make Scott a maintainer of docs theme package in PyPI
    - And released
  - ✅ Scott Release new version of docs theme & update Wagtail docs to use the new release
- Storm: Google Summer of Code mentor for Wagtail Bulk Actions
- Uses a dropdown menu to decide which action to use
- ModelAdmin -- can't reach edit button
- [#7330 accessibility targets](https://github.com/wagtail/wagtail/pull/7330)
- Launching flagship site on Wagtail

## 2021-06-25

Attendees: Scott, Kyle, Thibaud, Storm

### Actions

- Thibaud Try out styling overrides fix for userbar ul and li [#6994](https://github.com/wagtail/wagtail/pull/6994)
- Thibaud Update Figma file with Space key from menu ARIA practices
- Thibaud Review high-contrast mode audit from Kyle
  - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
- Scott Review accessibility of search autocompletes in docs theme -- built-in, and Algolia
- Storm Make Scott a maintainer of docs theme package in PyPI
- Scott Release new version of docs theme & update Wagtail docs to use the new release
- Kyle Review next-gen editor wireframes / progress
- Storm Review next-gen editor wireframes / progress

### Discussions

- Actions review
  - Thibaud & Storm Follow up on userbar PR progress [#6994](https://github.com/wagtail/wagtail/pull/6994)
    - Done some work. Not yet mergeable
    - Potential styling overrides
  - Thibaud Update Figma file with Space key from menu ARIA practices
  - ✅ Thibaud Talk to users of Transifex (Andy for wagtailmenus) about using it for docs translations
    - Confirmation from core team
    - Not sure when we go through the next steps
  - Thibaud Review high-contrast mode audit from Kyle
    - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
  - ✅ Scott Address low-hanging fruit in docs
    - <https://github.com/wagtail/sphinx_wagtail_theme/pull/109>
    - Some next steps on manual checks
  - Slim sidebar
    - Demo
    - Discuss peeking behavior
  - ARIA landmarks in the admin (@stormheg)
    - [Rework the admin UI's landmark based on established best practices - Issue #5411 - wagtail/wagtail](https://github.com/wagtail/wagtail/issues/5411)
  - Next-gen Wagtail editor
  - Revisit high-contrast mode with slim menu
    - Should be straightforward?
    - Thibaud backlog issues

## 2021-06-11

Attendees: Kyle, Jesse, Thibaud, Storm, Scott

### Actions

- Thibaud & Storm Follow up on userbar PR progress
- Thibaud Update Figma file with Space key from menu ARIA practices
- Thibaud Talk to users of Transifex (Andy for wagtailmenus) about using it for docs translations
- Thibaud Review high-contrast mode audit from Kyle
  - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>

### Actions review

- ✅ Storm PR for userbar recommendations
  - ✅ 👉[Move userbar before navigation in example](https://github.com/wagtail/wagtail/blob/6428820df23b70411a02f1a573f414f480830a16/docs/topics/writing_templates.rst#wagtail-user-bar)
  - 🚧Still need to apply suggestions from code review
- ✅ Thibaud Image upload audit review
  - Jesse & Thibaud also moved findings to [main spreadsheet](https://docs.google.com/spreadsheets/d/1l7tnpEyJiC5BWE_JX0XCkknyrjxYA5T2aee5JgPnmi4/edit)
- ✅ Thibaud Reach out on Twitter for Wagtail high-contrast users
- ✅ Thibaud Ask Torchboxers for high-contrast mode experience
- ✅ Storm & Thibaud Put draft annotations for keyboard support for Simon's work
- ✅ Thibaud Proposal for RTL support for sidebar rewrite
  - <https://github.com/wagtail/wagtail/issues/1240>
  - CSS logical properties
- ✅ Scott Accessibility audit for new docs theme
- ✅ Thibaud Open issue about docs translations in theme repository (or Wagtail?)
- ✅ Kyle High-contrast mode resources / look into what applies to Wagtail
  - Best practices
  - Compare default install

### Discussions

- Menu pattern for Wagtail sidebar
  - Missing Space key
  - <https://dribbble.com/shots/6269661-Accessibility-Bluelines>
- Scott Accessibility audit for new docs theme
  - Started it with WAVE
  - Reported a couple of errors
  - Axe DevTools
- High-contrast mode audit
  - <https://trello.com/c/YOEpYngg/29-comment-buttons-should-use-button-text-colour>
  - Highlights some semantic issues in our markup as well as the contrast issues
- Userbar pull request (@stormheg)
  - Needs a bit of refactoring in a few places
  - How to deal with focus outline
  - [Discussion on Github](https://github.com/wagtail/wagtail/pull/6994#discussion_r646115480)
  - Ensure it is visible against any background
  - Outline provided by browsers not necessarily accessible (e.g. Firefox on Windows)
  - Suggestion -- use the GOV.UK thick yellow? Already used in the Wagtail admin
    - Let's go with thick yellow
  - Research option to use "invert color" feature that might have some browser support?
- ARIA landmarks in the admin (@stormheg)
  - [Rework the admin UI's landmark based on established best practices - Issue #5411 - wagtail/wagtail](https://github.com/wagtail/wagtail/issues/5411)
- We4Authors Cluster project
  - <https://accessibilitycluster.com/main-results/selection-of-features>

## 2021-05-28: skipped (Slack updates)

## 2021-05-14

Attendees: Thibaud, Scott, Jesse, Kyle, Storm

### Actions

- Storm PR for userbar recommendations
- Move userbar before navigation in example
- Thibaud Image upload audit review
- Thibaud Reach out on Twitter for Wagtail high-contrast users
- Thibaud Ask Torchboxers for high-contrast mode experience
- Storm & Thibaud Put draft annotations for keyboard support for Simon's work
- Thibaud Proposal for RTL support for sidebar rewrite
- Scott Accessibility audit for new docs theme
- Thibaud Open issue about docs translations in theme repository (or Wagtail?)
- Kyle High-contrast mode resources / look into what applies to Wagtail
- Best practices
- Compare default install

### Actions review

- ✅ Thibaud userbar PR review [#6994](https://github.com/wagtail/wagtail/pull/6994)
- ✅ Storm PR for userbar recommendations
- ✅ Jesse Audit image upload in Safari VoiceOver <https://bakerydemo-thibaudcolas4.herokuapp.com/admin/images/multiple/add/>
- ✅ Thibaud Share testing site details (admin / changeme)
- ✅ Storm High-contrast mode audit of Dashboard
  - <https://bakerydemo-thibaudcolas4.herokuapp.com/admin/>
  - <https://assistivlabs.com/assistive-tech/display/high-contrast-mode>
- ✅ Thibaud Get in touch with [Assistiv Labs](https://assistivlabs.com/) to get a Torchbox account
- ~~Thibaud Get in touch with Assistiv Labs to get a Wagtail sponsorship~~
- ✅ Scott Review [#7142](https://github.com/wagtail/wagtail/pull/7142)

### Discussions

- Thibaud gave his PyCon talk!
- Got lots of good questions that we should review
- Discuss actions
  - Userbar recommendations
    - Nav then userbar, or userbar then nav?
    - <https://github.com/wagtail/wagtail/pull/6994/files?w=1#diff-bcb0c5f7c94df35f501163b0756512f7a1909f783eaf0d2f1103d286e3c3f4f3>
- Image upload
  - "ADD" Potential fix: [https://css-tricks.com/lets-talk-speech-css/](https://css-tricks.com/lets-talk-speech-css/#the-reality-of-the-situation)
- High-contrast mode audit of Dashboard
  - Logo
  - Search input different color in Edge
  - Different color inheritance for SVG and font icons
  - Interactive Admin menu isn't styled as interactive
  - Jesse different results -- Yellow in Firefox?
  - Which high-contrast modes are meant to be used for testing?
- Assistiv Labs
- Accessibility audit for upcoming sidebar rewrite?
  - <https://paper.dropbox.com/doc/Wagtail-sidebar-rewrite--BKuIZKetNCugApTjr4XzafCJAg-Wn81olplMadAC5eUEokXu>
  - role="menu"
    - A bit daunting but would be the best target
  - Annotate designs with expected accessibility / keyboard behavior?
- Accessibility audit for new docs theme?
  - Most of the markup copied from Typo3 theme
  - Thibaud noted that collapsible sidebar items could not be expanded, had to first load the top level page and then go through the pre-opened menu
  - Version picker KB access should be checked -- Storm thinks provided by ReadTheDocs and may not be able to modify its markup
  - There's no skip link!
  - Open issues at <https://github.com/wagtail/sphinx_wagtail_theme/>

## 2021-04-30

Attendees: Jesse, Scott, Storm, Thibaud

### Actions

- Thibaud userbar PR review [#6994](https://github.com/wagtail/wagtail/pull/6994)
- Storm PR for userbar recommendations
- Thibaud Share draft of automated tests on publish
- Jesse Audit image upload in Safari VoiceOver <https://bakerydemo-thibaudcolas4.herokuapp.com/admin/images/multiple/add/>
- Thibaud Share testing site details (admin / changeme)
- Storm High-contrast mode audit of Dashboard
- <https://bakerydemo-thibaudcolas4.herokuapp.com/admin/>
- <https://assistivlabs.com/assistive-tech/display/high-contrast-mode>
- Thibaud Get in touch with [Assistiv Labs](https://assistivlabs.com/) to get a Torchbox account
- Thibaud Get in touch with Assistiv Labs to get a Wagtail sponsorship
- Scott Review [#7142](https://github.com/wagtail/wagtail/pull/7142)

### Actions review

- ✅ Storm userbar PR [#6994](https://github.com/wagtail/wagtail/pull/6994)
- Thibaud userbar PR review [#6994](https://github.com/wagtail/wagtail/pull/6994)
- Thibaud Share draft of automated tests on publish
- ✅ Thibaud Share draft of accessibility audit formats with expected scope
- ✅ Thibaud Review new switch components
- The issue I had spotted is with all checkboxes in Wagtail, not specific to switch
- ✅ Thibaud Update Wagtail contribution guidance, and PR template, to make it clear individual pull requests should include accessibility testing. Review issue templates as well

### Discussions

- Userbar
- Where should it be on the page?
  - <https://github.com/wagtail/wagtail/blob/9630967e0e3de3469fd858d2cf6fd656be7c491e/docs/topics/writing_templates.rst#L266>
  - Recommend putting it "towards the top, but not first"
- <https://github.com/wagtail/wagtail/pull/7142>
- Audits methodology
  - Thibaud to further define / document ahead of sharing results
  - High level for now? To validate results, but no need to have the whole audit be replicable.
  - Scope of audit: things that are likely to be actionable in the near term.
- PR review methodology
  - Not as controversial as Thibaud thinks :)
  - We strongly encourage™ this.
- PyCon
- [Storybook in Wagtail (#7097)](https://github.com/wagtail/wagtail/pull/7097)
  - Ongoing internal conversations at Torchboxb

## 2021-04-16

Attendees: Storm, Thibaud

### Actions

- Storm userbar PR [#6994](https://github.com/wagtail/wagtail/pull/6994)
- Thibaud userbar PR review [#6994](https://github.com/wagtail/wagtail/pull/6994)
- Thibaud Share draft of automated tests on publish
- Thibaud Share draft of accessibility audit formats with expected scope
- Thibaud Review new switch components
- Thibaud Update Wagtail contribution guidance, and PR template, to make it clear individual pull requests should include accessibility testing. Review issue templates as well

### Discussions

- [SVG icons rework #6107](https://github.com/wagtail/wagtail/issues/6107)
  - [#6998](https://github.com/wagtail/wagtail/pull/6998)
- [Improve userbar accessibility #6994](https://github.com/wagtail/wagtail/pull/6994)
  - Menu + menuitem ARIA implementation
  - Updating docs to mention usage
- Automated accessibility checks as part of publishing pages
  - [Initial review](https://docs.google.com/document/d/12Hrq0EtzoXcqC9U7sFUcmwuQ4TWS9XYZpHE5OH_cBww/edit#)
  - Demo that goes a bit beyond than Tota11y: [Sa11y](https://ryersondmp.github.io/sa11y/)
  - [Axe + WordPress integration](https://docs.google.com/presentation/d/e/2PACX-1vROBCmDyBQI2Zez1hoVBSV1rUp_9Xad6K2J3-KDEr0IbewMqbKePoSwgicLpIHIgnw9v9cgwNu7furx/pub?start=false&loop=false&delayms=3000&slide=id.g2fbab35998_0_62)
  - [ARRM project](https://www.w3.org/WAI/EO/wiki/ARRM_Project_-_Accessibility_Roles_and_Responsibilities_Mapping)
- Accessibility audit
  - Option 1: manual, [Template](https://docs.google.com/spreadsheets/d/1DfqPIVfQYgj2bxxWS4nPs4lrwmWF1wzrtvLwgtVp5kI/edit?usp=sharing)
  - Option2: automated, [Pa11y + Lighthouse demo](https://thibaudcolas.github.io/django_admin_tests/)
- Scope:
  - Dashboard
  - Main menu
  - Pages menu
  - Pages search
  - Both manual and automated

## 2021-03-19 -- new team chat

Attendees: Thibaud, Scott, Storm, Kyle, Jesse

- Welcome & introductions: Thibaud, Scott, Storm, Kyle, Jesse
- Intro to current accessibility effort
  - [Wagtail admin WCAG2.1 AA](https://github.com/wagtail/wagtail/projects/5), [RFC](https://github.com/wagtail/rfcs/pull/37)
  - [WCAG2.1 AA for sites](https://github.com/wagtail/wagtail/projects/10)
  - And docs, one-off projects, etc.
- How the team works
  - Initial plan: open membership, 45-min chats every two weeks to provide feedback and take actions.
  - 6months membership
  - Friday morning, afternoon to evening Europe/Africa
- What do we all want to achieve with the accessibility team?
- Thibaud
  - Another audit of Wagtail
  - Automated accessibility checks as part of publishing pages
  - [SVG icons rework #6107](https://github.com/wagtail/wagtail/issues/6107)
- Scott
  - [SVG icons rework #6107](https://github.com/wagtail/wagtail/issues/6107)
  - [Contextual alt text RFC #51](https://github.com/wagtail/rfcs/pull/51)
  - aria-label on links (give more helpful link text to screen reader users)
    - [Feature: ability to set links as "nofollow" rel via the WYSIWG editor's link chooser #4474](https://github.com/wagtail/wagtail/issues/4474)
  - Being able to use the same link chooser outside of rich text fields
    - [Single interface for choosing links to anything #381](https://github.com/wagtail/wagtail/issues/381)
- Storm
  - [Wagtail userbar is not accessible - Issue #6108](https://github.com/wagtail/wagtail/issues/6108)
  - Review existing accessibility related pull requests.
  - [SVG icons rework #6107](https://github.com/wagtail/wagtail/issues/6107)
  - ["Unpublished" styles in pages listings are very hard / impossible to see - Issue #5370](https://github.com/wagtail/wagtail/issues/5370)
  - [Implement focus management for chooser modals - Issue #5338](https://github.com/wagtail/wagtail/issues/5338)
- Kyle
  - All buttons visible all the time
  - Incorporated as Wagtail customisations in previous agency
  - Look into this further since we know there are people who struggle with this
  - Get up to speed with Wagtail contributions!
  - Read through open issues & raise anything missing
- Jesse
  - Getting up to speed with issues and contributions
- User testing with users of assistive technology
  - Would be good in addition to doing an audit of our own
  - Reach out to Wagtail contributors to use assistive tech
  - Share via Django Newsletter?
  - Share in accessibility communities?
  - Could reach out to <https://makeitfable.com/>
  - Jesse check user testing plan / results from Syracuse University's upcoming Wagtail build
- Another audit
  - Has Wagtail ever been professionally audited?
    - Outline steps to get a more professional audit?
    - Crowdfund :)?
- Jesse check with coworkers for interest in accessibility / Wagtail contributions

## 2021-02-17 -- Team 6-monthly report

- 5 people active during the last 6 months, but only 2 attending meetings on average
  - Initially Scott Cranfill (core team, CFPB), Thibaud Colas (core team, Torchbox), Andreas Bernacca (Fröjd)
  - Joined by Nick Smith (Torchbox) and Helen Chapman (Torchbox) over the last couple of months for specific tasks
- Met 9 times. We had initially decided on a 3-month membership, but ended up extending to 6 months.
- Focused on 3 areas:
  - Completing the SVG icons conversion to improve accessibility of icons in the CMS admin
  - Documenting [accessibility considerations](https://docs.wagtail.io/en/stable/advanced_topics/accessibility_considerations.html) for Wagtail sites
  - Curating a backlog of accessibility improvements for sites <https://github.com/wagtail/wagtail/projects/10>
- We were also keen to do more automated tests and manual auditing but didn't get around to it.

### Agenda / changes for next 6 months

- Create plan to recruit 5 members
  - Open office hours?
- Create and publish accessibility audits of Wagtail to have a clear record of our current state
- Update Wagtail contribution guidance, and PR template, to make it clear individual pull requests should include accessibility testing. Review issue templates as well
- 45min meetings in the future.
- Thibaud draft RFC for automated accessibility tests

## 2021-01-22 -- Team retrospective

Attendees: Scott, Thibaud

### Actions review

- ✅ Thibaud Report forms issues to Django
  - <https://code.djangoproject.com/ticket/32338>
  - <https://code.djangoproject.com/ticket/32339>
  - <https://code.djangoproject.com/ticket/32340>

### Discussions

- Django forms issues -- need to follow up to provide more specific guidance and devise the fixes
- Retrospective
  - Arrived at the term of our team commitment
  - An occasion to take stock of what we achieved over the last 6 months
  - And what we want to do next?
  - Resuming team activity 5th of March

### Retrospective

- **Start**
  - I would love to get reminders of my TODOs between meetings.
    - Action: Thibaud happy to volunteer to do weekly reminders
  - Recruit more aggressively?
    - Target: 5 members
    - How: posting more
    - Do what we’ve done before but more aggressively?
    - Torchbox internal project helped
    - Outreach / wider audience events to get people interested
    - Action: create plan to recruit 5 members
  - Get people from the #accessibility Slack more involved
  - Create and publish accessibility audits of Wagtail that clearly state how far ahead we are.
    - Action: Create and publish accessibility audits of Wagtail to have a clear record of our current state
  - Reach out to specific people who could be interested in contributing
  - Report back to core team
    - Action: Accessibility team report to core team
- **Stop**
  - Using Zoom? (Can’t access on my work computer.)
    - Action: Switch over to Google Meet.
  - The team’s activity can make it feel like accessibility for Wagtail is solved / handled by us, even though we’re far from it
    - Attitude we want to discourage: “the accessibility team will take care of making this work”
    - Action: Update Wagtail contribution guidance, and PR template. Review issue templates as well
  - Saying yes to other Wagtail activities even though I want to spend time on this
- **Continue**
  - 30 minute meetings every two weeks seems like a good cadence. Could maybe be 45.
    - Action: 45min meetings in the future.
  - Meeting format works well, I think. (Reviewing actions, discussions, adding new actions.)
  - Accessibility-focused sprint was good (January 2020)
  - 6 months felt like a pretty good commitment
  - The “automated accessibility tests when publishing” feels like the most promising way to improve outcomes for users of Wagtail sites
    - Action: Thibaud draft RFC for automated accessibility tests

Actions recap:

- Thibaud happy to volunteer to do weekly reminders
- Create plan to recruit 5 members
- Create and publish accessibility audits of Wagtail to have a clear record of our current state
- Accessibility team report to core team
- Switch over to Google Meet.
- Update Wagtail contribution guidance, and PR template. Review issue templates as well
- 45min meetings in the future.
- Thibaud draft RFC for automated accessibility tests

## 2021-01-08

Attendees: Nick, Thibaud

### Actions

- Thibaud Report forms issues to Django

### Actions review

- No actions last meeting

### Discussions

- Docs sprint
- Django forms markup suggested changes review
  - Remove support for as_table. While deprecated, update all documentation to state that it shouldn't be used, and if used the table should be marked as role="presentation".
  - Remove support for as_ul. While deprecated, update all documentation to state that it shouldn't be used, and if used the ul should be marked as role="presentation".
  - For as_p and the {{ form }} shortcut -- these work as expected for screen reader users. It would be good to document these shouldn't be used for larger forms, where it's important to group fields in fieldset with appropriate legends for accessibility, for all users, but particularly for screen reader users.
  - Django's markup doesn't follow accessibility best practices for RadioSelect ChoiceFields -- it should use a fieldset with legend (and no ul). Change the markup
    - accessible=False for deprecation period (breaks old code at the end of deprecation period, not code that was updated at the end of it)
    - Potentially -- may be able to achieve this once deprecated/removed via a project-level template override (assess how feasible)
  - DateField should always come with the pattern required for the date. Documentation only?
    - Yes
    - Format for display in form: input_formats, <https://docs.djangoproject.com/en/3.1/ref/forms/fields/#datefield>
    - <https://github.com/django/django/blob/master/django/forms/fields.py#L389>
  - DateTimeField should ideally be removed / at least discouraged from being used without / needs a JS widget
    - Messaging / Docs only
  - TimeField needs further consideration
    - Messaging
  - Django's markup doesn't follow accessibility best practices for CheckboxSelectMultiple MultipleChoiceField -- it should use a fieldset with legend (and no ul). Change the markup
  - Deprecation: move to deprecated/legacy config app
  - Suggest as-is replacement as part of request to remove it
  - Template to use to replicate the functionality
  - Removing things is easier than simply changing them

## 2020-12-18

Attendees: Nick, Thibaud

### Actions

No actions this time

### Actions review

- ✅ Thibaud SVG icons for [Settings menu item](https://github.com/wagtail/wagtail/blob/70bb9d934b086d8c2c34f1363c12e9acec970816/wagtail/contrib/settings/registry.py#L12-L19) [@thibaudcolas](https://github.com/thibaudcolas) ([#6649](https://github.com/wagtail/wagtail/pull/6649))
- Scott SearchArea PR review [#6493](https://github.com/wagtail/wagtail/pull/6493) (in progress)
- Scott Comment on [#6535](https://github.com/wagtail/wagtail/issues/6535)
- ✅ Thibaud Explore idea of validating document outline within individual rich text fields ([#6535](https://github.com/wagtail/wagtail/issues/6535))
- ✅ Thibaud Review issues relating to publish success redirection
- Scott Icons PR .url_field .input
- Thibaud Icons PR edit panel title-wrapper
- ✅ Thibaud Fill sprint attendance survey

### Discussions

- Docs sprint (remote)
- Validating document outlines ([#6535](https://github.com/wagtail/wagtail/issues/6535) follow-up)
  - Interested in broader accessibility tests first
  - Preferred approach: rely on page preview to get "end to end" tests
  - Similar to <https://github.com/Aleksi44/wagtailyoast/blob/fa9e64ed758921cdac701c68f0c6002c02522229/wagtailyoast/static/wagtailyoast/src/js/common/Panel.js#L49-L59>
  - Integrate Axe, or Tota11y, or IBM Equal Access checker, or h123
  - For end users -- move preview inline in the admin so end users can see the issues with appropriate context
- Publish success redirection
  - <https://github.com/wagtail/wagtail/blob/master/wagtail/admin/views/pages/edit.py>
  - <https://github.com/thibaudcolas/wagtail/blob/master/wagtail/admin/views/pages/create.py>  
    <https://github.com/wagtail/wagtail/issues/694>

## 2020-12-04 

Attendees: Scott, Thibaud

### Actions

- Thibaud SVG icons for [Settings menu item](https://github.com/wagtail/wagtail/blob/70bb9d934b086d8c2c34f1363c12e9acec970816/wagtail/contrib/settings/registry.py#L12-L19) [@thibaudcolas](https://github.com/thibaudcolas) (in progress)
- Scott SearchArea PR review [#6493](https://github.com/wagtail/wagtail/pull/6493) (in progress)
- Scott Comment on [#6535](https://github.com/wagtail/wagtail/issues/6535)
- Thibaud Explore idea of validating document outline within individual rich text fields (#6535)
- Thibaud Review issues relating to publish success redirection
- Scott Icons PR .url_field .input
- Thibaud Icons PR edit panel title-wrapper
- Thibaud Fill sprint attendance survey

### Actions review

- Thibaud SVG icons for [Settings menu item](https://github.com/wagtail/wagtail/blob/70bb9d934b086d8c2c34f1363c12e9acec970816/wagtail/contrib/settings/registry.py#L12-L19) [@thibaudcolas](https://github.com/thibaudcolas) (in progress)
- Scott SearchArea PR review [#6493](https://github.com/wagtail/wagtail/pull/6493) (in progress)
- ✅ Scott draft PR for paginations icons [#6573](https://github.com/wagtail/wagtail/pull/6573)
- ✅ Thibaud review PR for paginations icons [#6573](https://github.com/wagtail/wagtail/pull/6573)
- ✅ Scott Review [sites accessibility](https://github.com/wagtail/wagtail/projects/10) proposal & highlight top 3
- Andreas Review [sites accessibility](https://github.com/wagtail/wagtail/projects/10) proposal & highlight top 3

### Discussions

- [Review WCAG2.1 AA for sites](https://github.com/wagtail/wagtail/projects/10)
  - Heading levels
    - StreamField charblock or structblock
    - (custom icon prefix for heading text)
    - Scott add comment
    - Option to explore -- validation of heading levels outline
    - Publish next page -- why parent?
      - <https://github.com/wagtail/wagtail/issues/694>
      - <https://github.com/wagtail/wagtail/issues/3348>
    - Draft idea -- accessibility tests on publish / save draft
  - Forms -- review default output
    - Also review extra field types to support #6611
- Icons [#6107](https://github.com/wagtail/wagtail/issues/6107)

## 2020-11-20

Attendees: Andreas, Thibaud, Scott

### Actions

- Thibaud SVG icons for [Settings menu item](https://github.com/wagtail/wagtail/blob/70bb9d934b086d8c2c34f1363c12e9acec970816/wagtail/contrib/settings/registry.py#L12-L19) [@thibaudcolas](https://github.com/thibaudcolas)
- Scott SearchArea PR review <https://github.com/wagtail/wagtail/pull/6493>
- Scott draft PR for paginations icons
- Thibaud review draft PR for paginations icons
- Scott Review sites accessibility proposal & highlight top 3 <https://github.com/wagtail/wagtail/projects/10>
- Andreas Review sites accessibility proposals & highlight top 3 <https://github.com/wagtail/wagtail/projects/10>

### Agenda

- Actions review
  - ✅ Thibaud Finish SearchArea <https://github.com/wagtail/wagtail/pull/6493>
  - Scott  Pagination from 6107
    - ModelAdmin markup generated in Python
  - ✅ Thibaud Finish accessibility considerations doc <https://github.com/wagtail/wagtail/pull/6272>
  - ✅ Thibaud Ask Coen to join next accessibility team meeting
  - Thibaud Propose UI architecture rework to core team -- RFC
    - I haven't done this because I don't think django-pattern-library is ready yet, but close
    - <https://github.com/torchbox/django-pattern-library/releases/tag/v0.3.0>
- Discussions
  - Icons
  - Wagtail sites fixes
  - <https://docs.wagtail.io/en/latest/advanced_topics/accessibility_considerations.html>
  - <https://github.com/wagtail/wagtail/projects/10>
  - Embed titles
    - Torchbox backport
  - Heading levels validation
    - Don't underestimate editors
    - Validation for rich text fields?
    - Highlight empty blocks directly in the field
    - Error message at the end?
    - Potential for automated remediation by stripping all empty heading blocks server-side or client-side
  - Heading levels availability
    - Scott: prefer editors have awareness of the semantics of heading levels
  - Feature request: Support for declaring language on elements in rich text. #4694
    - Everyone supportive
    - CFPB does block-level translations
    - Would be nice to do this at the rich text field (or rich text block?) level

## 2020-10-23

Attendees: Scott, Thibaud

### Actions

- Thibaud Finish SearchArea<https://github.com/wagtail/wagtail/pull/6493>
- Scott Pagination from 6107
- Thibaud Finish accessibility considerations doc<https://github.com/wagtail/wagtail/pull/6272>
- Thibaud Ask Coen to join next accessibility team meeting
- Thibaud Propose UI architecture rework to core team – RFC

### Agenda

- Actions review

  - WIP Thibaud Take on SearchArea from<https://github.com/wagtail/wagtail/issues/6107>
  - Thibaud Take on SettingsMenuItem from<https://github.com/wagtail/wagtail/issues/6107>
  - ✅ Scott Help text from 6107
  - WIP Scott Pagination from 6107
  - ✅ Thibaud Attempt to revive<https://github.com/thibaudcolas/bakerydemo/commits/bakerydemo-thibaudcolas> but with nightly releases
  - Thibaud Ask Coen to join next accessibility team meeting

- Discussions
  - Accessibility compliance dashboard
  - SVG icons
    - <https://github.com/wagtail/wagtail/issues/6107>
    - <https://github.com/wagtail/wagtail/pull/6493>
  - Accessibility considerations
  - bakerydemo nightly
    - Weekly Travis cron builds of<https://github.com/thibaudcolas/bakerydemo/tree/bakerydemo-thibaudcolas-cron>
    - Pushes ready-to-deploy<https://github.com/thibaudcolas/bakerydemo/blob/bakerydemo-thibaudcolas-nightly/requirements/base.txt>
    - Heroku pipeline with review apps & multiple staging apps<https://dashboard.heroku.com/pipelines/4e9fd4e0-0aac-440f-a6cb-2ab13e2e277f>
  - UI architecture rework RFC
    - Waiting for new release of django-pattern-library, ETA early November
  - Team future
    - 3-month commitment ends next week
      - 4 meetings so far
      - Revisit this beginning of the year?
      - Talk to Coen? Find somebody else?
      - 3 people is a good minimum
    - What do the next 3 months hold?
      - Get the icons rework finished
    - Next project ideas
      - Fixes for Wagtail accessibility footguns
        - It’s most important of all for us to encourage the development of accessible websites with Wagtail
        - Raw numbers
      - Automated accessibility tests?
        - Monitoring
        - CI
      - Accessibility audits
        - Chooser modals
        - StreamField
        - More rich text
        - Professional audit?
          - With AT users
- Detecting Wagtail sites
  - Thibaud experiments
  - We 4 authors cluster
  - <https://digital.gov/resources/content-management-systems-used-by-government-agencies/>

## 2020-09-25

Attendees: Thibaud, Scott

### Actions

- Thibaud Take on SearchArea from <https://github.com/wagtail/wagtail/issues/6107>
- Thibaud Take on SettingsMenuItem from <https://github.com/wagtail/wagtail/issues/6107>
- Scott  Help text from 6107
- Scott  Pagination from 6107
- Scott Review accessibility considerations docs WIP PR <https://github.com/wagtail/wagtail/pull/6272>
- Thibaud Propose UI architecture rework to core team -- RFC
- Thibaud Attempt to revive <https://github.com/thibaudcolas/bakerydemo/commits/bakerydemo-thibaudcolas> but with nightly releases
- Thibaud Ask Coen to join next accessibility team meeting

### Agenda

- Actions review
  - ✅ Thibaud to caption Wagtail Space US accessibility & pattern library talks
  - Thibaud Share DjangoCon on Slack
  - ✅ Thibaud Review & merge localstorage icons implementation <https://github.com/wagtail/wagtail/pull/6243>
  - ✅ Scott Look into ModelAdmin SVG icon support <https://github.com/wagtail/wagtail/issues/6379>
  - PR: <https://github.com/wagtail/wagtail/pull/6402>
  - Thibaud Take on a couple items from <https://github.com/wagtail/wagtail/issues/6107>
  - Andreas Take on "Breadcrumb (home icon)" + 1 extra item if time from <https://github.com/wagtail/wagtail/issues/6107>
  - Thibaud Propose UI architecture rework to core team -- RFC
  - Andreas Review accessibility considerations docs WIP PR <https://github.com/wagtail/wagtail/pull/6272>
  - Scott Review accessibility considerations docs WIP PR <https://github.com/wagtail/wagtail/pull/6272>
- Automated accessibility tests
  - <https://github.com/thibaudcolas/wagtail-tooling>
  - <https://github.com/thibaudcolas/django_admin_tests>
  - Bakerydemo running on Wagtail nightly?
    - Needs locking down of content if used for automated tests
- Discussions
  - Icons progress for 2.11
    - Still achievable
    - Contact Coen
    - About 2-3 weeks before the RC

## 2020-09-11

Attendees: Andreas, Scott, Thibaud

### Actions

- Thibaud to caption Wagtail Space US accessibility & pattern library talks
- Thibaud Share DjangoCon on Slack
- Thibaud Review & merge localstorage icons implementation <https://github.com/wagtail/wagtail/pull/6243>
- Scott Look into ModelAdmin SVG icon support <https://github.com/wagtail/wagtail/issues/6379>
- Thibaud Take on a couple items from <https://github.com/wagtail/wagtail/issues/6107>
- Andreas Take on "Breadcrumb (home icon)" + 1 extra item if time from <https://github.com/wagtail/wagtail/issues/6107>
- Thibaud Propose UI architecture rework to core team -- RFC
- Andreas Review accessibility considerations docs WIP PR <https://github.com/wagtail/wagtail/pull/6272>
- Scott Review accessibility considerations docs WIP PR <https://github.com/wagtail/wagtail/pull/6272>

### Agenda

- Actions review
  - ✅ Get in touch with colleagues / potential people interested in helping with accessibility -- Everyone
    - Jane from Torchbox, not participating in this very group, but working on accessibility of Wagtail sites with Thibaud over 3 months
    - Scott one colleague, not for now :)
    - Andreas no luck
  - ✅ Identify Wagtail Space US accessibility good first issues @thibaudcolas
  - ✅ Prepare Wagtail Space US accessibility talk @thibaudcolas
    - WIP: #6090 Document accessibility considerations
  - ✅ [Accessibility issue for dropdowns in Wagtail Admin](https://github.com/wagtail/wagtail/issues/6072) -- Andreas
    - Merged!
  - ✅ SVG Icons -- Scott
- Discussions
  - <https://github.com/fregante/github-issue-link-status>
  - <https://github.com/wagtail/wagtail/issues/3804>
  - [django-pattern-library](https://github.com/torchbox/django-pattern-library) for Wagtail
    - Feedback from Naomi would be great, as well as other people with Wagtail UI architecture experience, Jonny, Janneke
    - Mix of React and non-React code needs clarifying
    - Jinja macros vs template tags?
    - Jinja makes it possible to put more logic in templates
    - Advise for caution
    - Consider switching to Jinja? But not go so far as to fall into the "logic in templates" trap
    - Testing logic in templates is tough (compared to Python)
    - Scott's Wagtail solution: move logic to page models' get_context
    - Refactoring justified for testability
    - Would make it easier for people to understand the codebase (and contribute)
    - <https://github.com/wagtail/wagtail/pull/6272>

## 2020-07-17

Attendees: Scott, Andreas, Thibaud

### Actions

- Thibaud Identify Wagtail Space US accessibility good first issues
  - Either have different labels, or Projects board for “Websites’ accessibility”
- Thibaud Prepare Wagtail Space talk
- Andreas Finish PR for Site settings dropdown icon confusion
- Scott Review icon transition PRs
- Everyone Get in touch with colleagues / potential people interested in helping with accessibility
- Bonus
  - Scott Open a new icon transition PRs
  - Thibaud What’s the most accessible video call software?

### Agenda

Poll:<https://doodle.com/poll/euv4mfh2mhfqnmtp>

- Welcome & introductions
  - Thibaud – happy for Torchbox to make time for this, and focusing on accessibility
  - Andreas – Wagtail dev for 3 years at Fröjd
    - Came up from legal requirements with clients
    - Internal accessibility group for WCAG2.1 AA compliance
  - Scott – CFPB, interested in accessibility for years
    - Aiming for WCAG 2.1 AA too
    - Not just public websites but also tools for employees, equally as liable
- Intro to current accessibility effort
  - [Wagtail admin WCAG2.1 AA](https://github.com/wagtail/wagtail/projects/5),[RFC](https://github.com/wagtail/rfcs/pull/37)– Andreas: 1, Scott: 1B, Thibaud: 2
  - [Issues for Wagtail websites #6090](https://github.com/wagtail/wagtail/issues/6090) – Andreas: 2, Scott: 1A, Thibaud: 1
  - [Accessibility features ideas](https://docs.google.com/document/d/1rFw5S4vJa4As6aH-k1QNnEZTmE1jkLOM8ABh7X8WZOQ/edit) – Andreas: 3, Scott: 3, Thibaud: 3
  - Thibaud’s Wagtail Space talk
    - The above, and
    - Tooling
- What do we all want to achieve with the #accessibility team?
  - Personal accountability :)
  - The bi-weekly nudge
  - Thibaud about 5h per week on Wagtail
  - Priorities are different for people who are very experienced and already aware of Wagtail gotchas
  - Future vision:
    - Wagtail is the best CMS to build accessible websites
    - Great selling point for companies proposing Wagtail
    - Contrast with Episerver for Fjörd
  - WebAim 1 million & Gatsby
  - What’s the most accessible video call software?
    - <https://www.smashingmagazine.com/2020/06/accessible-video-conferencing-tools/>
- How the team works
  - Initial plan: open membership, collaboration via Slack first, 30-min chats to provide feedback and take actions.
  - 3 months membership?
  - MVP
  - 30min every two weeks
  - Friday morning , afternoon to evening Europe/Africa
  - 11h eastern, 4pm Thibaud, 5pm Andreas
- Timezones
  - Scott: EDT (UK-5)
  - Andreas: CET/CEST (UTC+2?)
  - Thibaud: BST
- What do we all want to do next?
  - See actions above
- See you all at the next Wagtail Space :)
  - Timezones work!
