# 2021-12 – Page editor feedback & design considerations

Designs (for editing): [Wagtail editor 4 (Accessibility team copy)](https://www.figma.com/file/UTuPx9UV1vzBEXzcaeEqVH/Wagtail-Editor-4-(Accessibility-team-copy)?node-id=2201%3A29434)

Prototype (with hotspots): [Wagtail Editor 4 prototype](https://www.figma.com/proto/7l3IqiyVZqHT5wrzEAivCe/Wagtail-Editor-4?page-id=225%3A3&node-id=1702%3A21256&starting-point-node-id=1702%3A21256)

[Accessibility bluelines](https://dribbble.com/shots/6269661-Accessibility-Bluelines)

## 2021-12 Saptak feedback

## 2021-12 Thibaud feedback

- Top bar – is it ok to have two tablists? Or do we want tablist + something more bespoke
- Heading navigation
  - Does the title field get preceded with a SR-only <h1>? Or no h1?
  - Do field panels make fieldsets and legends, or sections and headings, or both

## 2021-11-16 Thibaud feedback

This has all been shared with Ben already and taken into account – copying here for reference.

- Title
  - I think it’d be worth trying to have some affordance that the title is editable without relying on hover – when I create a page, can I tell there is a field here?
  - - Potentially having a small "Title" label above this
  - - Or perhaps a character count? That’s something we’ve been keen to have more of anyway
  - - Or something more visually prominent but perhaps only there when the field is empty, say a Material UI - style underline
- Help text
  - With the help text inline, we should provide a recommended "maximum help text length" so it fits in a single line – and perhaps have it truncated above? (expandable on demand)
- Date picker
  - Could we try placing the icon on the right, and having it appear as a focusable button, similar to [Duet Date Picker](https://duetds.github.io/date-picker/?)
  - This would be important for keyboard and screen reader users, so there is a separate UI element dedicated to triggering the appearance of the date picker.
  - It doesn’t need to be fully recognisable as a button, but it needs to be distinguishable from the decorative icons we have next to labels. And needs to be focusable separately from the field.
- Textarea
  - Could we make it so those text boxes are resizeable by end users? Could also be worthwhile adding a character count on here so we make sure there is space somewhere.
- Asterisk / error message
  - I like the subdued asterisk but wonder if that will work with error message styling – what would they look like?
  - See [Fixes #7241 and improves error visibility in high-contrast](https://github.com/wagtail/wagtail/pull/7663), which also introduces an icon so error messages are distinguishable with something else than color. I don’t think the icon is necessary to meet any particular accessibility requirement, but it’s an interesting consideration.
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
  - Something we might lose a bit with this inline preview is the ability to add content checks within the preview like [wagtail-accessibility](https://github.com/neon-jungle/wagtail-accessibility) (since there won’t be enough space). Would be nice if there was a place within this inline preview UI to trigger those checks?
- Page history
  - Couple of points here – I think this looks great but I doubt we’d want to build the page history listing this way considering the complexity (unless we used a similar virtualised / fading listing pattern in more valuable places)
  - - The fading-out list pattern is pretty hard to do well in browsers
  - - We’d likely need pagination or "scroll to load" for pages that have lots of entry
- Field groups font size
  - It’d be nice to increase the font size throughout also so we can give Wagtail implementers more heading levels to play with?
  - We have those h2-level styles for top-level field groups, then I can easily see at least one h3-level "group within group", and then h4-type styles for field labels
- Dark mode
  - Have we considered a dark mode version? As well as the cool factor, I understand it’d help with accessibility for people with low vision.
