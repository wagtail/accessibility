# 2023-01-20 – Accessibility checker demo

Attendees: Saptak, Jesse, Albina, Scott, Thibaud, Storm, Sage,

## **Demo**

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

## **Discussion**

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
