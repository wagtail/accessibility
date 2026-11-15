# 2021-10-15 -- retrospective

Attendees: Scott, Thibaud, Saptak

## Actions

- Saptak Share research on uppercase / capitalized text
- ✅ Thibaud Trial removing all uppercase
- [Wagtail Slack thread on removing all uppercase](https://wagtailcms.slack.com/archives/CB7L6L5S6/p1634332413035500?thread_ts=1634249236.029900&cid=CB7L6L5S6)
- ✅ Thibaud Share retrospective with core team

## Discussions

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
