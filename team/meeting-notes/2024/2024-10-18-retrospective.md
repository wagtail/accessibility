# 2024-10-18 – retrospective

Attendees: Chiemezuo, Scott, Thibaud, Saptak, Storm, Victoria

## Retrospective

### Start – things we’re not doing currently, which we should start doing

* Change meeting time / day to work better for more people🍎🍈🍋 🍓🍌
  * Giving shifting timezone meetings a chance? 🍈🍌
    * So we have something that works for more people
    * Make room for people in Asia / Oceania
    * Previously: meetings on Thursday & Friday
* If we find we’re “running out” of high impact tasks for Wagtail, perhaps we take our collected knowledge and experience up the ecosystem and help Django out? 🍒🍌🍋🍋
  * And Python too?
* Emphasise the importance of accessibility with site developers (outreach) 🍈🍋🍒
* Regular external accessibility audits and user testing with assistive tech users and publishing finding🍈🍎🍒🍌
* Comparing Wagtail with other projects / researching other projects that are great at specific aspects of accessibility🍓🍎🍌
* Restart publishing meeting notes 🍈🍎🍌
* Invest more in automated tests (monitoring for sites? Continuous integration?) 🍒🍌
* Packages accessibility review? 🍈🍎
* Encouraging people to speak about Wagtail at accessibility events🍈🍋
* Doing accessibility training together? Like a book club type of thing?🍓🍌
* Advocacy for Wagtail CMS- Event Partnerships🍓🍎
  * Workshop for people who either haven’t used, or already use Wagtail
  * Feedback mechanism. Survey or form?
    * Workshop experience and feedback about Wagtail
  * Example from Scott & Meagen: [djangoconwagtail2024](https://github.com/vossisboss/djangoconwagtail2024), [pyconwagtail2024](https://github.com/vossisboss/pyconwagtail2024)
  * Good target event: [OSCA 2025](https://festival.oscafrica.org/)
* Find better ways to engage with the #accessibility channel members 🍓
* Curate all accessibility talks we’re all working on in a dedicated page / listing 🍈
* Better crediting people who heavily contribute to accessibility improvements 🍋
  * Suggestion: Create a repo where people list their names and contributions
* Find a better format to collaborate on accessibility R&D and publish our findings

### Stop – things we should stop doing (or do less of)

* Stop giving “everyone with the link” edit access to this doc 🍈🍋🍎🍌
* Leaving accessibility bugs open for so long / un-triaged 🍈🍎🍌
* Ignoring (maybe that's too strong of a word) certain assistive tech like voice control 🍋🍒
* Leaving accessibility documentation to the standalone “accessibility considerations”, “accessibility features” pages🍒
* Relying almost entirely on Torchbox staff or interns for the majority of code contributions

### Continue – things we should keep doing

* Work together in a small group on a specific task, like the GSoC image description project 🍋🍈🍓🍎🍌🍒
* Gathering data about accessibility on Wagtail websites in the wild, like done with the image alt text research 🍋🍈🍓🍎🍌
  * Thibaud has been hoarding statistics (and spreadsheets)
  * Quantifies our impact / how sites out there are doing
* Encouraging people to talk about accessibility at Wagtail/Django/Python/tech events🍈🍓🍎🍌
* Being transparent about our efforts in accessibility 🍋🍌🍎🍒
* Supporting GSoC/Outreachy/other internship projects to improve accessibility 🍋🍈🍌
* Building upon existing work done.🍌
* Adding more items to the accessibility checker’s default rules
* Idea: give developers a good baseline for how to do accessibility testing on Wagtail website projects
  * Guide for devs to follow, on existing or new projects

Votes: 🥭 Jesse, 🍎 Saptak, 🍐 Jane, 🍒 Scott, 🍋 Thibaud, 🍇 Sage, 🍊Albina, 🍈 Storm 🍍Ben M, 🍓 Victoria, 🍉Sherry, Ahmed 🥕, 🍌 Chiemezuo

## Retrospective actions

* Run 2x meetings, on 2 different days, at 2 different times – based on a poll for good times
* Prepare a Wagtail accessibility workshop for [OSCA 2025](https://festival.oscafrica.org/) and [DjangoCon Africa 2025](https://djangocon.africa/)
* Document accessibility data gathering setup
* Plan Wagtail websites analysis for 2025
* Think of accessibility project plans for 2025 (GSoC 2025?)
* Stop giving “everyone with the link” edit access to this doc

## Discussions

* Great work Victoria and Albina on [“prefers contrast” improvements](https://github.com/wagtail/wagtail/pull/12348)!
* Congratulations Chiemezuo 🌈 (and Saptak and Storm) [AbstractImage description](https://github.com/wagtail/wagtail/pull/11792), [ImageBlock blocks](https://github.com/wagtail/wagtail/pull/12416)
  * I’m really excited to never have to define a Wagtail image block when setting up a site ever again
    * Scott Cranfill
* Next: voice control?
  * “Put a question mark”
* [2024 team plans review](https://docs.google.com/document/d/1YUxOs5jYZMd8rX291mDE123xIK7tbD63PzSR9ooFa4c/edit?tab=t.0#heading=h.tcmzl3f9xss1)
* Other things we did
  * New alt text accessibility rule
  * [Readability metrics research](https://docs.google.com/document/d/1YUxOs5jYZMd8rX291mDE123xIK7tbD63PzSR9ooFa4c/edit?tab=t.0#bookmark=id.syixulscx7lt)
  * [Wagtail accessibility](https://wagtail.github.io/accessibility/)
  * GSoC project: Low-carbon accessible project template
  * Alt text with AI research
* Retrospective
  * Went way past the set term of our team commitment
  * An occasion to take stock of what we achieved over the last 12 months
  * And what we want to do next?
  * Resuming team activities in a few weeks

## 2024 team plans review

* ✅ Triage “design needed” accessibility contributions 🍒🍋🍍🍊🍓🍎
  * [Design-needed task ideas to review](https://docs.google.com/document/d/1YUxOs5jYZMd8rX291mDE123xIK7tbD63PzSR9ooFa4c/edit?tab=t.0#heading=h.xk52ne9lzjjc)
* ✅ Outreachy: wagtail.org website accessibility 🍎🍊🍈🍋🍇🍓🍉
  * [Blog: Making wagtail.org more accessible](https://wagtail.org/blog/making-wagtailorg-more-accessible/)
* ✅ High-contrast light and dark themes for Wagtail🍋🍊🍓🍍🍉
  * [Prefers-contrast admin theming](https://github.com/wagtail/wagtail/issues/12176)
* ⌛️ Work with people using assistive technology to discover areas of improvement 🍎🍋 🍒🍇🍓🍉
  * Or maybe testimonials for Wagtail.org? Wagtail is an accessible CMS!
  * +1 to user testing with assistive tech users
  * A lot of issues opened (and fixed) thanks to their feedback
* ✅ Accessible image model by default (current implementation uses filename as title / alt text ) 🍎🍈 🍒🍍🍓
  * [RFC 51: Contextual Alt Text](https://github.com/wagtail/rfcs/pull/51)
  * [Addition of new "description" property to AbstractImage class #11792](https://github.com/wagtail/wagtail/pull/11792)
  * [New ImageBlock for StreamField #11791](https://github.com/wagtail/wagtail/pull/11791)
* 🔴Improve how we automatically test Wagtail’s accessibility (add more tests, add better tooling, etc.) to prevent accessibility regressions 🍋🍈🍇 🍒
* ✅ Meetup/conference talks related to accessibility work across wagtail 🍎 🍒🍇🍓
  * Scott and Meagen’s workshop at PyCon US, May 2024
  * Vince and Thibaud’s PyCon US poster, May 2024
  * Saptak’s DjangoCon Europe workshop, June 2024
  * Scott and Meagen’s workshop at DjangoCon US, September 2024
* ✅ Support Django’s accessibility team with their direction 🍒🍇🍎🍈
* ⌛️ Audit Wagtail design system for accessible contrast as measured by [the new APCA contrast model](https://www.myndex.com/APCA/) (Possibly too early if we’re concerned about it not being an official part of the standard yet?) 🍈🍊🍇🍓
* 🔴 Update Rich Text link modal to include aria-label field 🍋 🍒🍎
* 🔴 Accessibility audits for docs.wagtail.org and guide.wagtail.org 🍎🍈🍓
* ✅ Outreachy: accessibility features documentation 🍋 🍒🍓
  * [Accessibility features](https://guide.wagtail.org/en-latest/concepts/accessibility-features/)
* ⌛️ATAG audit review 🍎🍍🍋
* ⌛️Updated Wagtail CMS audit for new WCAG 2.2 rules (also updating the accessibility statement maybe to include that?) 🍊🍎
* 🔴Triage “community management & marketing” accessibility contributions🍋🍓
* 🔴Propose adding a stock Heading Block to Wagtail core, which can implement validation for not skipping levels 🍒
* ✅ VPAT (Voluntary Product Accessibility Template, primarily a Section 508 thing) for Wagtail🍋
  * [Wagtail 5.2 VPAT](https://wagtail.github.io/accessibility/audits/vpat/)
* ✅ Wagtail websites’ accessibility benchmarking (statistics for GAAD 2024)
* ⌛️ Help us look for sponsorships to fund more accessibility checker improvements

## Retrospective: examples from the past

* I would love to get reminders of my TODOs between meetings.
* Get people from the #accessibility Slack more involved
