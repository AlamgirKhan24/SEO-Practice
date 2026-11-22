# Checklist: Accessibility

Accessibility checks support an inclusive user experience and often reveal issues in semantics, navigation, and page structure. Automated scanners help find defects, but do not replace keyboard, assistive-technology, or human review.

- [ ] Text and interface colors provide sufficient contrast (WCAG AA: 4.5:1 for normal text and 3:1 for large text and applicable UI components)
- [ ] Meaningful images have useful alternative text; decorative images use empty alt text (`alt=""`)
- [ ] Video and audio have appropriate captions, transcripts, or descriptions where needed
- [ ] Embedded content has a descriptive title or accessible name
- [ ] Headings describe the content and follow a logical hierarchy
- [ ] Forms expose clear labels, instructions, and errors to assistive technology
- [ ] Links and buttons have clear accessible names and do not rely on visual context alone
- [ ] Interactive controls work with a keyboard and show a visible focus indicator
- [ ] Content remains usable with zoom and reflow at narrow viewport widths
- [ ] Automated scans are run on representative templates; serious results are manually reviewed

Treat accessibility findings on their own evidence and applicable standards. Do not infer overall conformance from a clean automated scan.

**Related fix guides:** `fixes/accessibility/`
