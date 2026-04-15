# Unified Accessibility Baseline Reference — WCAG 2.2 Level AA

> **All Formats: PDF | Word | Excel | PowerPoint | HTML | CSS**

---

## Purpose and Source

This document is a comprehensive, unified reference combining all 24 baselines from the **ICT Testing Baseline Portfolio**, published by the U.S. Access Board (atbcb). It is designed to serve as a self-contained knowledge base for accessibility testing across multiple document and web formats.

**Sources:**
- [ICT Testing Baseline for Electronic Documents v1.0](https://github.com/atbcb/ICTTestingBaseline/tree/main/_baselines/document-baselines) (published September 30, 2024) — covers PDF, Word, Excel, PowerPoint
- [ICT Testing Baseline for Web v3.1](https://github.com/atbcb/ICTTestingBaseline/tree/main/_baselines/web-baselines) (published April 1, 2024) — covers HTML and CSS

The ICT Testing Baseline Portfolio establishes the minimum requirements for evaluating the conformance of ICT with the Revised Section 508 of the Rehabilitation Act of 1973 (29 U.S.C. 794d). Section 508 incorporates WCAG 2.0 Level A and AA by reference; this document references the WCAG 2.2 Understanding articles for improved clarity.

---

## Key Scoping Rules

### Section 508 Exemptions for Non-Web Documents

Per **Section 508 E205.4**, the following WCAG success criteria do **NOT** apply to non-web documents (PDF, Word, Excel, PowerPoint):

| WCAG SC | Description | Applies to Web? | Applies to Documents? |
|---------|-------------|:--------------:|:--------------------:|
| 2.4.1 | Bypass Blocks | ✅ Yes | ❌ No |
| 2.4.5 | Multiple Ways | ✅ Yes | ❌ No |
| 3.2.3 | Consistent Navigation | ✅ Yes | ❌ No |
| 3.2.4 | Consistent Identification | ✅ Yes | ❌ No |

### Deprecated Success Criterion

**SC 4.1.1 Parsing** is deprecated in WCAG 2.2 and the WCAG 2.0 Errata states it should be considered as always satisfied for HTML or XML content. **Baseline 24 always passes — no testing required.**

### Web-Only Baselines

| Baseline | Description | Documents |
|----------|-------------|:---------:|
| Baseline 4 | Repetitive Content (Bypass Blocks, Consistent Navigation, Consistent Identification) | ❌ N/A |
| Baseline 19 | Frames and iFrames | ❌ N/A |
| Baseline 23 | Multiple Ways | ❌ N/A |

---

## Quick-Reference Table: WCAG 2.2 Level AA → Baseline Mapping

| WCAG SC | Name | Baseline # | PDF | Word | Excel | PPT | HTML/CSS |
|---------|------|:----------:|:---:|:----:|:-----:|:---:|:--------:|
| 1.1.1 | Non-Text Content | 6, 7, 10 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.2.1 | Audio-only and Video-only (Prerecorded) | 16 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.2.2 | Captions (Prerecorded) | 17 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.2.4 | Captions (Live) | 17 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.2.5 | Audio Description (Prerecorded) | 17 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.3.1 | Info and Relationships | 10, 12, 13, 18 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.3.2 | Meaningful Sequence | 18 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.3.3 | Sensory Characteristics | 7 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.4.1 | Use of Color | 7 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.4.2 | Audio Control | 21 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.4.3 | Contrast (Minimum) | 8 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.4.4 | Resize Text | 22 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 1.4.5 | Images of Text | 6 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.1.1 | Keyboard | 1 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.1.2 | No Keyboard Trap | 1, 3 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.2.1 | Timing Adjustable | 21 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.2.2 | Pause, Stop, Hide | 21 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.3.1 | Three Flashes or Below Threshold | 9, 3 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.4.1 | Bypass Blocks | 4 | ❌ N/A | ❌ N/A | ❌ N/A | ❌ N/A | ✅ |
| 2.4.2 | Page Titled | 11 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.4.3 | Focus Order | 2 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.4.4 | Link Purpose (In Context) | 14 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.4.5 | Multiple Ways | 23 | ❌ N/A | ❌ N/A | ❌ N/A | ❌ N/A | ✅ |
| 2.4.6 | Headings and Labels | 10, 13 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 2.4.7 | Focus Visible | 2 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.1.1 | Language of Page | 15 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.1.2 | Language of Parts | 15 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.2.1 | On Focus | 2 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.2.2 | On Input | 10 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.2.3 | Consistent Navigation | 4 | ❌ N/A | ❌ N/A | ❌ N/A | ❌ N/A | ✅ |
| 3.2.4 | Consistent Identification | 4 | ❌ N/A | ❌ N/A | ❌ N/A | ❌ N/A | ✅ |
| 3.3.1 | Error Identification | 10 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.3.2 | Labels or Instructions | 10 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.3.3 | Error Suggestion | 10 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 3.3.4 | Error Prevention (Legal, Financial, Data) | 10 | ✅ | ✅ | ✅ | ✅ | ✅ |
| 4.1.1 | Parsing (deprecated) | 24 | ✅ Auto-pass | ✅ Auto-pass | ✅ Auto-pass | ✅ Auto-pass | ✅ Auto-pass |
| 4.1.2 | Name, Role, Value | 5, 6, 10, 12, 14 | ✅ | ✅ | ✅ | ✅ | ✅ |

---

## Baseline 1: Keyboard Accessible

**WCAG Success Criteria:** 2.1.1 Keyboard, 2.1.2 No Keyboard Trap, Conformance Requirement 5: Non-Interference

### Limitations, Assumptions, or Exceptions

- Tests are performed on a standard physical keyboard for a Windows PC. Keyboard emulators may be used with adapted instructions.
- Mouse Keys (Windows/Mac feature) is not considered a keyboard emulator.
- SC 2.1.1 exception: where the underlying function requires path-dependent input (not just endpoints), keyboard access is not required.
- SC 2.1.2 is a non-interference criterion: failure affects the entire document regardless of where the non-conforming content appears.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 1.A-1 | All functionality accessible by mouse is also accessible by keyboard (Tab, Enter, Space, Arrow keys, Escape, etc.). | 2.1.1 |
| 1.A-2 | If a keyboard-only path to a function is not provided, an alternate keyboard-accessible control with equivalent functionality is available. | 2.1.1 |
| 1.A-3 | Individual keystrokes do not require specific timings for activation. | 2.1.1 |
| 1.B-1 | Keyboard focus can be moved away from every interactive component — no keyboard traps exist. | 2.1.2 |
| 1.B-2 | If non-standard keys are required to escape a component, the user is clearly notified of the method. | 2.1.2 |

### Format-Specific Implementation Techniques

| Format | Techniques and Notes |
|--------|---------------------|
| **PDF** | All form fields, links, and interactive elements must be in the document's tab order (PDF3). Test using Tab/Shift+Tab navigation. Embedded media players must have keyboard-accessible controls. |
| **Word** | All hyperlinks, form content controls, and embedded objects must be reachable via Tab. Use the Tab/Arrow keys to navigate between fields. Check that embedded objects don't trap focus. |
| **Excel** | All cell links, form controls (buttons, dropdowns, checkboxes), and ActiveX controls must be keyboard-accessible. Navigate with Tab, Arrow, Enter, Escape. |
| **PowerPoint** | All hyperlinks, action buttons, and interactive objects must be keyboard-accessible. Use Tab to navigate between objects on a slide; Escape to release selection. |
| **HTML/CSS** | Use native interactive elements (`<a>`, `<button>`, `<input>`, `<select>`, `<textarea>`) which are keyboard-accessible by default. If using custom ARIA widgets, implement full keyboard interaction patterns per [WAI-ARIA Authoring Practices](https://www.w3.org/WAI/ARIA/apg/). |

---

## Baseline 2: Focus

**WCAG Success Criteria:** 2.4.3 Focus Order, 2.4.7 Focus Visible, 3.2.1 On Focus

### Limitations, Assumptions, or Exceptions

- Some non-interactive components (e.g., form instructions) may be in the tab order and must show visible focus.
- Loss of visible focus during manual navigation is a failure; loss when a function moves focus (e.g., internal link) is not automatically a failure.
- Focus may be moved via keyboard (Tab) or mouse click. Moving the mouse over a control does not move focus unless scripting implements this.
- Focus order is not required to move left-to-right, top-to-bottom, but must preserve meaning and operability.
- Focus must shift to modal dialogs and remain within the dialog until closed by the user.
- Testing SC 3.2.1 (On Focus) is performed using the keyboard only to avoid unintentional activation via mouse.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 2.A-1 | A visible focus indicator is provided when keyboard focus is on an interactive component. | 2.4.7 |
| 2.A-2 | The focus indicator persists — it must not disappear while focus remains on the component. | 2.4.7 |
| 2.B-1 | When hidden content (menus, dialogs) is revealed via keyboard, revealed focusable content is included in the focus order. | 2.4.3 |
| 2.B-2 | When hidden content is closed, focus returns to the trigger control. | 2.4.3 |
| 2.B-3 | The overall focus order preserves the meaning and usability of the content. | 2.4.3 |
| 2.C-1 | When a component receives keyboard focus, it does NOT initiate an unexpected change of context (no auto-submit, no new window launch, no unexpected focus move). | 3.2.1 |

### Format-Specific Implementation Techniques

| Format | Techniques and Notes |
|--------|---------------------|
| **PDF** | Correct tab and reading order must be set (PDF3). Use Acrobat's Order panel to verify and repair tab order. All interactive elements must display a visible focus rectangle. |
| **Word** | Built-in focus indicators are provided by the OS/application. Ensure custom controls (content controls, ActiveX) show visible focus. Form fields must appear in logical tab order. |
| **Excel** | Tab key moves focus between unlocked cells and controls. Ensure locked/protected sheets retain logical focus order for interactive elements. |
| **PowerPoint** | Tab order through objects on each slide is set via the Selection Pane (Home → Arrange → Selection Pane). Reading order corresponds to the visual tab order. |
| **HTML/CSS** | Use `:focus` and `:focus-visible` CSS pseudo-classes to provide visible focus styles. Do not use `outline: none` without providing a custom focus indicator. Use `tabindex="0"` to add non-native elements to the tab order; `tabindex="-1"` to allow programmatic focus only. Avoid `tabindex` values greater than 0. |

---

## Baseline 3: Non-Interference

**WCAG Requirements:** Conformance Requirement 5 (Non-Interference) — SCs 1.4.2, 2.1.2, 2.3.1, 2.2.2 apply to ALL content including non-relied-upon content

### Limitations, Assumptions, or Exceptions

- This baseline is a logical AND of results from Baseline Tests 21.D (Audio Control), 1.B (No Keyboard Trap), 9.A (Flashes), 21.B (Moving Information), and 21.C (Auto-Update). All must pass.
- Any failure of these SCs can interfere with a user's ability to use the entire document/page.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 3.A-1 | All Non-Interference SCs pass: 1.4.2-AudioControl, 2.1.2-NoKeyboardTrap, 2.3.1-Flashes, 2.2.2-PauseStopHide. | CR5 |

### Format-Specific Notes

| Format | Notes |
|--------|-------|
| **All Formats** | This is a composite test. Results are derived from Baselines 1, 9, and 21. Report as pass only when all four SCs pass throughout the entire document/page. |
| **HTML/CSS** | Particularly relevant for scripted animations, auto-playing media, and embedded widgets. |

---

## Baseline 4: Repetitive Content

**WCAG Success Criteria:** 2.4.1 Bypass Blocks, 3.2.3 Consistent Navigation, 3.2.4 Consistent Identification

### ⚠️ Applicability

| Format | Applies? | Notes |
|--------|:--------:|-------|
| PDF | ❌ No | Per Section 508 E205.4, non-web documents are exempt from 2.4.1, 3.2.3, and 3.2.4 |
| Word | ❌ No | Same exemption |
| Excel | ❌ No | Same exemption |
| PowerPoint | ❌ No | Same exemption |
| HTML/CSS | ✅ Yes | All three SCs apply to web content |

### Limitations, Assumptions, or Exceptions (Web Only)

- Small repeated sections (individual words, phrases, single links) are not "blocks" for bypass purposes.
- Bypass methods must work with the keyboard alone — ARIA landmarks and headings as skip mechanisms are not included in this baseline test (they require assistive technology to function).
- Same relative order means the same position relative to other items; items may be inserted or removed.
- Consistent text alternatives that follow a consistent format (e.g., "Go to page 4", "Go to page 5") are acceptable even if not identical.

### Universal Test Checks (HTML/CSS Only)

| Test ID | Check | SC |
|---------|-------|----|
| 4.A-1 | A keyboard-accessible mechanism is provided to bypass blocks of repeated content. | 2.4.1 |
| 4.A-2 | The bypass mechanism works as intended (focus moves past or hides the repetitive block). | 2.4.1 |
| 4.B-1 | Navigational mechanisms repeated across pages appear in the same relative order each time. | 3.2.3 |
| 4.C-1 | Components with the same functionality are identified consistently across pages. | 3.2.4 |

### Format-Specific Implementation (HTML/CSS)

| Technique | Description |
|-----------|-------------|
| Skip links | `<a href="#main-content">Skip to main content</a>` placed before navigation blocks |
| Internal anchor links | `<a href="#section2">Skip to section</a>` pointing to `<div id="section2">` |
| Expandable menus | SCR28: Collapsible menu that can be closed via keyboard |
| Consistent layout | Navigation menus, headers, footers appear in the same relative order across all pages |
| Consistent labeling | Same-function buttons (e.g., "Search") use identical or consistently formatted labels |

---

## Baseline 5: User Controls

**WCAG Success Criteria:** 4.1.2 Name, Role, Value

### Limitations, Assumptions, or Exceptions

- A user interface component is perceived by users as a single control for a distinct function.
- The accessibility properties (name, role, state, value) must remain correct when the control changes.
- Visited/unvisited state of links is excluded from this test (authors cannot set it programmatically).
- Form elements (Baseline 10) and links (Baseline 14) have dedicated tests; map to those for accessible name testing.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 5.A-1 | The combination of accessible name and accessible description is not empty. | 4.1.2 |
| 5.A-2 | The non-empty accessible name/description describes the control's purpose. | 4.1.2 |
| 5.A-3 | If the control's name changes on user interaction, the accessible name is correct after the change. | 4.1.2 |
| 5.B-1 | The role of the control is valid and appropriate for its function. | 4.1.2 |
| 5.C-1 | The state of the control (checked, expanded, hidden, pressed, disabled, etc.) is correct. | 4.1.2 |
| 5.C-2 | After the user changes the control's state, the state is correctly reflected. | 4.1.2 |
| 5.D-1 | The value of the control is correct. | 4.1.2 |
| 5.D-2 | After the user changes the control's value, the value is correctly reflected. | 4.1.2 |

### Format-Specific Implementation Techniques

| Format | Techniques and Notes |
|--------|---------------------|
| **PDF** | Interactive elements must have correct tags and roles (e.g., buttons tagged as `<Form>` with `/T` tooltip entry). Use PDF12 for form field name/role/value. PDF Tags panel in Acrobat verifies roles. |
| **Word** | Content controls (Developer tab) must have descriptive titles and tags. ActiveX controls must have accessible names via the Name property. |
| **Excel** | Form controls and ActiveX controls need accessible names. Set via the control's Format → Object → Alt Text or Name Box. |
| **PowerPoint** | Action buttons and interactive objects must have accessible names set via Alt Text pane. |
| **HTML/CSS** | Use native HTML elements when possible. For custom widgets: `aria-label` or `aria-labelledby` for name, valid WAI-ARIA `role` values for role, `aria-checked`/`aria-expanded`/`aria-pressed`/`aria-disabled` for state, `aria-valuenow`/`aria-valuetext` for value. |

---

## Baseline 6: Images

**WCAG Success Criteria:** 1.1.1 Non-Text Content, 1.4.5 Images of Text, 4.1.2 Name, Role, Value

### Limitations, Assumptions, or Exceptions

- An image with a non-empty text alternative has been determined to be meaningful by the author.
- An image with an empty text alternative has been determined to be decorative by the author.
- Common image formats: .jpg, .png, .svg, .gif, .tiff, .bmp.
- Images of text essential to information being conveyed (including logotypes) are exempt from SC 1.4.5.
- Images that are part of a picture with significant other visual content (e.g., graphs, screenshots, diagrams) are not considered "images of text."
- Captchas: Not applicable to non-web documents; for HTML, test that alternatives identify the CAPTCHA purpose and that alternative CAPTCHA forms are provided.
- Web: `role="presentation"` or `role="none"` on images must not conflict with other attributes or roles.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 6.A-1 | Meaningful images have a non-empty text alternative that is not used for design/formatting only and is not invisible. | 1.1.1 |
| 6.A-2 | The non-empty text alternative provides an equivalent description of the image's purpose. | 1.1.1 |
| 6.B-1 | Decorative images are programmatically hidden from assistive technology. | 1.1.1 |
| 6.B-2 | Decorative images are not in the tab order, do not convey meaningful information, and do not initiate actions. | 1.1.1 |
| 6.D-1 | Images of text are not used when the same visual presentation can be achieved using text. | 1.4.5 |
| 6.D-2 | If images of text are used, they can be visually customized to user requirements (font, size, color, background). | 1.4.5 |

### Format-Specific Implementation Techniques

| Format | Meaningful Images (Alt Text) | Decorative Images | Images of Text |
|--------|------------------------------|-------------------|----------------|
| **PDF** | `/Alt` entry on the image structure element (PDF1). OCR for scanned PDFs (PDF7). | Mark as Artifact using `/Artifact` tag (PDF4). | Avoid; use actual text elements instead. |
| **Word** | Right-click image → Edit Alt Text → enter description. | Right-click image → Edit Alt Text → check "Mark as decorative." | Avoid SmartArt/WordArt that conveys essential information as images. |
| **Excel** | Right-click image → Edit Alt Text → enter description. | Right-click image → Edit Alt Text → check "Mark as decorative." | Avoid chart text that cannot be customized. |
| **PowerPoint** | Select image → Alt Text pane (Picture Format tab) → enter description. | Select image → Alt Text pane → check "Mark as decorative." | Avoid text-in-image slides; use actual text placeholders. |
| **HTML/CSS** | `<img alt="descriptive text">` or `aria-label`. `role="img"` with `aria-label` for SVG. | `<img alt="">`, CSS `background-image`, or `aria-hidden="true"`. Do NOT combine `role="none"` with non-empty `alt`. | Use real text with CSS styling. If unavoidable, provide `alt` text that matches image text. |

---

## Baseline 7: Sensory Characteristics

**WCAG Success Criteria:** 1.1.1 Non-Text Content, 1.3.3 Sensory Characteristics, 1.4.1 Use of Color

### Limitations, Assumptions, or Exceptions

- SC 1.4.1 does not prohibit the use of color; it can be met by adding another visual cue (e.g., color AND shape).
- Color alone distinguishing visited vs. unvisited links is an exception — this does not fail SC 1.4.1.
- Colors that differ in both hue and lightness with a contrast ratio of 3:1 or greater meet SC 1.4.1 for distinguishing elements, provided the user doesn't need to perceive the specific color.
- SC 1.3.3 instructions cannot be met by providing multiple sensory characteristics together; a non-sensory cue is required.
- Short sounds (notification beeps, error chimes) are covered here; audio in time-based media is covered in Baseline 16.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 7.A-1 | Content using color to convey meaning also provides: (a) on-screen text describing the color/meaning, OR (b) another visual differentiator (shape, position, size, underline), OR (c) colors with ≥3:1 contrast ratio where precise color identification is not required. | 1.4.1 |
| 7.B-1 | Instructions do not rely solely on shape, size, visual location, orientation, or sound — additional non-sensory identification is provided. | 1.3.3 |
| 7.C-1 | Audible notification cues are accompanied by a visible text alternative. | 1.1.1 |

### Format-Specific Implementation Techniques

| Format | Use of Color | Sensory Instructions | Audible Cues |
|--------|-------------|---------------------|--------------|
| **PDF** | Add visible text labels or patterns alongside color coding (e.g., status indicators). | Avoid instructions like "see the red box on the right" — add text labels. | Embed text alongside any audio notification elements. |
| **Word** | Use icon + color (not color alone) for status indicators. | Add non-positional text identifiers in instructions. | Use text captions alongside audio notifications. |
| **Excel** | Use cell text, icons, or patterns alongside conditional formatting colors. Data bars with text values preferred. | Reference cell content, not cell color, in formulas and instructions. | Pair notification sounds with visible cell indicators. |
| **PowerPoint** | Supplement color-coded charts and diagrams with text labels or distinct patterns/shapes. | Provide non-sensory references in speaker notes and slide text. | Include caption text for any notification sounds in presentations. |
| **HTML/CSS** | Use CSS `border`, `::before`/`::after` content, `background-image` with patterns, or icon fonts in addition to color. `F73`, `F81` are common failures. | Provide text labels for position-based instructions; avoid relying solely on left/right/above/below. | Provide `<span>` or `aria-live` regions alongside audio alerts. |

---

## Baseline 8: Contrast

**WCAG Success Criteria:** 1.4.3 Contrast (Minimum)

### Limitations, Assumptions, or Exceptions

**Exceptions — the following are NOT required to meet contrast requirements:**
- Logotypes and brand name text
- Inactive (disabled) user interface components (note: read-only ≠ disabled; read-only elements must meet contrast)
- Pure decorative text with no functionality or meaning
- Text contained within a picture that contains significant other visual content

- Large text is defined as ≥18pt (24px) regular, or ≥14pt (18.5px) bold.
- Disabled elements do not receive keyboard focus and are not included in this test.
- Contrast testing includes changes due to mouse hover and selection status.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 8.A-1 | Normal text has a contrast ratio of at least **4.5:1** against its background. | 1.4.3 |
| 8.A-2 | Large text (≥18pt regular or ≥14pt bold) has a contrast ratio of at least **3:1** against its background. | 1.4.3 |
| 8.A-3 | Images of text meet the same contrast thresholds as regular text. | 1.4.3 |

### Format-Specific Implementation Techniques

| Format | How to Check and Fix |
|--------|---------------------|
| **PDF** | Use Acrobat's accessibility checker; supplement with external contrast analyzer tools. Adjust text and background colors in the source application before PDF export. |
| **Word** | Use external color contrast analyzer (e.g., APCA, WebAIM Contrast Checker) on text/background combinations. Avoid light gray text on white, yellow on white, etc. |
| **Excel** | Check cell text color vs. cell fill color. Conditional formatting colors must also meet contrast. Use Accessibility Checker as a starting point, then verify with contrast tool. |
| **PowerPoint** | Check all text against slide backgrounds, including text on images. Theme colors must meet contrast. Use Format Background to check background colors. |
| **HTML/CSS** | Use CSS to set foreground/background colors with sufficient contrast. Tools: axe, WAVE, WebAIM Contrast Checker, browser DevTools accessibility panel. Use `color-contrast()` CSS function (future support). |

---

## Baseline 9: Flashing

**WCAG Success Criteria:** 2.3.1 Three Flashes or Below Threshold; Conformance Requirement 5: Non-Interference

### Limitations, Assumptions, or Exceptions

- Flicker and blink may be used synonymously with flash for this test.
- Flashing from user display settings or connectivity is beyond the author's control and not included.
- Blinking content that passes this test may still need to comply with SC 2.2.2 (Baseline 21) if it lasts more than 5 seconds.
- SC 2.3.1 is a non-interference criterion — applies to all content.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 9.A-1 | Content does not flash more than 3 times per second (3 Hz). | 2.3.1 |
| 9.A-2 | If flashing exceeds 3 Hz or frequency is unknown: the combined flashing area is ≤341×256 pixels at 1024×768 resolution (small area), OR the flash does not include "general flashes" (≥10% luminance change where darker image luminance <0.80), OR the flash does not include "saturated red flashes." | 2.3.1 |

### Format-Specific Implementation Techniques

| Format | Notes |
|--------|-------|
| **PDF** | Avoid animated GIFs and embedded video with high-frequency flashing. Test any embedded animations for flash rate. |
| **Word** | Animated images and embedded media must not contain high-frequency flashing. |
| **Excel** | Avoid blinking or flashing cell content (e.g., animated conditional formatting). |
| **PowerPoint** | Slide transitions and animations must not create high-frequency flashing. Avoid strobe-like animation effects. |
| **HTML/CSS** | Avoid CSS animations with high flash frequency. Use `animation-duration` values that stay below 3 Hz. Test with Photosensitive Epilepsy Analysis Tool (PEAT) for complex animations. |

---

## Baseline 10: Forms

**WCAG Success Criteria:** 1.1.1 Non-Text Content (Controls), 1.3.1 Info and Relationships, 2.4.6 Headings and Labels, 3.2.2 On Input, 3.3.1 Error Identification, 3.3.2 Labels or Instructions, 3.3.3 Error Suggestion, 3.3.4 Error Prevention (Legal, Financial, Data), 4.1.2 Name, Role, Value

### Limitations, Assumptions, or Exceptions

- Read-only fields (pre-filled) receive focus and are selectable but not modifiable; they must be labeled and programmatically determinable.
- Disabled input elements do not receive focus and are not included in this test.
- Clicking/selecting an option selects it but should not initiate a change of context.
- Changes of context include: new window/user agent, viewport change, focus move, content change that changes document meaning.
- SC 3.3.2 applies only to data entry controls, not to links or expand/collapse widgets.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 10.A-1 | Each form field has a non-empty combination of accessible name and accessible description. | 4.1.2 |
| 10.A-2 | The accessible name/description describes the form field's purpose. | 4.1.2, 1.1.1 |
| 10.A-3 | All related instructions/cues are programmatically associated with their form controls. | 1.3.1 |
| 10.B-1 | Labels for form fields describe purpose, expected input, and required format (e.g., date format MM/DD/YYYY). | 2.4.6 |
| 10.C-1 | Changing a form field value or navigating away does NOT cause an unexpected change of context. | 3.2.2 |
| 10.D-1 | When an input error is automatically detected: the user is alerted, the error is described in text, and the field in error is identified in text. | 3.3.1 |
| 10.E-1 | Each form field has a visible label while it has keyboard focus. | 3.3.2 |
| 10.F-1 | When errors are detected and correction suggestions are known, suggestions are provided (unless this would jeopardize security). | 3.3.3 |
| 10.G-1 | For legal/financial/data submissions: at least one of these is true — (1) reversible, (2) errors are checked with opportunity to correct, (3) review/confirm before finalizing. | 3.3.4 |

### Format-Specific Implementation Techniques

| Format | Implementation |
|--------|---------------|
| **PDF** | PDF5 (required fields), PDF10 (labels for form fields), PDF12 (name/role/value for form fields), PDF15 (submit button), PDF22 (error notification). Use Acrobat's Form Editing tools to set field properties. |
| **Word** | Use Developer tab content controls (Rich Text, Plain Text, Date Picker, Dropdown). Set Title property for accessible name. Use error validation macros for error prevention. |
| **Excel** | Use Data Validation (Data → Data Validation) for input constraints. Provide descriptive cell labels adjacent to input cells. Use input messages for instructions and error alerts for error notification. |
| **PowerPoint** | PowerPoint has limited native form support. Forms embedded as OLE objects must have accessible labels. Recommend linking to a web-based or Word form for complex data entry. |
| **HTML/CSS** | `<label for="fieldId">`, `aria-labelledby`, `aria-describedby` for names. `<fieldset>`/`<legend>` for grouping. `required` attribute for required fields. `aria-invalid="true"` and error messages for error identification. `autocomplete` attributes for user input. |

---

## Baseline 11: Document Titles (Page Titles)

**WCAG Success Criteria:** 2.4.2 Page Titled

### Limitations, Assumptions, or Exceptions

- Every document must have a descriptive title — this test always applies.
- For collections of documents (e.g., PDF portfolios), each document must have its own title.
- The title must describe the document's content or purpose.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 11.A-1 | The document/page has a title property defined. | 2.4.2 |
| 11.A-2 | The title describes the contents or purpose of the document/page. | 2.4.2 |

### Format-Specific Implementation Techniques

| Format | How to Set the Title |
|--------|---------------------|
| **PDF** | Set via File → Properties → Description → Title (Document Properties). Must appear in the document information dictionary (PDF18). Ensure "Display document title" is selected in Initial View settings. |
| **Word** | File → Info → Properties → Title field. Or right-click file → Properties → Details → Title. |
| **Excel** | File → Info → Properties → Title field. |
| **PowerPoint** | File → Info → Properties → Title field. |
| **HTML/CSS** | `<title>Descriptive Page Title</title>` in `<head>`. Should be unique across the site and describe the page content. Format: `[Page Content] - [Site Name]` is a common pattern. |

---

## Baseline 12: Tables

**WCAG Success Criteria:** 1.3.1 Info and Relationships, 4.1.2 Name, Role, Value

### Limitations, Assumptions, or Exceptions

- **Data tables:** Tables where cells require row/column header context to be understood.
- **Layout tables:** Tables used for visual placement only; content is meaningful when linearized (read top-to-bottom, left-to-right). Layout tables must NOT use data table structure attributes.
- Rows of related data must have row headers for AT users to understand relationships.
- Complex data tables (merged/split cells, multiple header rows/columns) must have explicit programmatic associations.
- Linearization: presenting table content in one-dimensional source order (row 1 left-to-right, then row 2, etc.).

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 12.A-1 | Each data table has a programmatically assigned table role. | 4.1.2 |
| 12.A-2 | Each data cell has a data cell role; each header cell has a header role. | 4.1.2 |
| 12.B-1 | All data cells are programmatically associated with their row and/or column headers. | 1.3.1 |
| 12.C-1 | Layout tables do NOT use data table markup (no row/column headers, no captions, no summary/scope). | 4.1.2 |

### Format-Specific Implementation Techniques

| Format | Data Tables | Layout Tables |
|--------|-------------|---------------|
| **PDF** | Use table structure elements with `<Table>`, `<TR>`, `<TH>`, `<TD>` tags (PDF6). Use Table Editor in Acrobat to repair mistagged tables (PDF20). Header cells must have scope attribute set. | Mark layout-only tables as artifacts; do not tag as data tables. |
| **Word** | Use Insert → Table and apply header row/column styling. Right-click header row → Table Properties → Check "Repeat as header row." Use Alt Text (Table Properties → Alt Text) to provide table summary. | Keep layout tables simple; avoid setting header styles on layout cells. |
| **Excel** | Use Insert → Table (Ctrl+T) to create structured tables with header rows. Column headers auto-generate accessible names for data cells in the table. | Keep layout-only cell arrangements without Table formatting. |
| **PowerPoint** | Insert → Table. Set first row as header row via Table Design tab. Add Alt Text for the table (Right-click → Edit Alt Text). | Avoid using tables for slide layout; use text boxes and placeholders instead. |
| **HTML/CSS** | `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th scope="col/row">`, `<td>`. Use `id`/`headers` attributes for complex tables. Add `<caption>` for table title. | If using `<table>` for layout (avoid this), set `role="presentation"` and omit `<th>`, `<caption>`, `scope`, `headers`. Better: use CSS Grid/Flexbox for layout. |

---

## Baseline 13: Content Structure

**WCAG Success Criteria:** 2.4.6 Headings and Labels, 1.3.1 Info and Relationships

### Limitations, Assumptions, or Exceptions

- A document with only one heading does not have a heading structure to evaluate for hierarchy.
- Multiple H1s or no H1 is acceptable.
- H1 is not required to match the document title.
- Heading levels may skip downward (H1→H3) but should reflect visual hierarchy.
- Not all lists require markup (e.g., comma-separated inline lists in sentences).
- Navigation menus are excluded from the visually apparent lists test.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 13.A-1 | Each heading describes the topic or purpose of its content. | 2.4.6 |
| 13.B-1 | Visual headings are programmatically tagged as headings with heading levels that logically match the visual hierarchy. | 1.3.1 |
| 13.C-1 | Programmatic headings (H1–H6 tags) correspond to actual visual headings — heading markup is not used for emphasis on non-heading content. | 1.3.1 |
| 13.D-1 | Visually apparent unordered lists are marked as bulleted lists. | 1.3.1 |
| 13.D-2 | Visually apparent ordered/numbered lists are marked as numbered or multilevel lists. | 1.3.1 |

### Format-Specific Implementation Techniques

| Format | Headings | Lists |
|--------|----------|-------|
| **PDF** | Apply heading tags H1–H6 via Acrobat Tags panel (PDF9). Export from authoring tools (Word, InDesign) with heading styles to produce correct tags automatically. | Apply List tags (L, LI, Lbl, LBody) via Acrobat Tags panel (PDF21). Export from Word with list styles. |
| **Word** | Apply Heading 1, Heading 2, Heading 3, etc. from the Styles pane. Do not use bold/large text without applying a heading style. Check with Navigation Pane (View → Navigation Pane). | Use List Bullet, List Number styles. Do not manually indent and add characters. |
| **Excel** | Headings in Excel are typically column/row headers in tables. Use bold formatting + merged cells for visual section headers, but note programmatic heading tags are limited. For complex documents, consider using named ranges and table headers. | Excel has limited native list markup. Represent lists as separate rows in a structured range. |
| **PowerPoint** | Use built-in slide layouts with title/content placeholders (not text boxes). Outline View shows heading hierarchy. Title placeholder = primary heading. | Use the built-in bullet list formatting in content placeholders. Do not use manual bullet characters (asterisks, dashes). |
| **HTML/CSS** | `<h1>` through `<h6>` for headings. Do not use `<h>` tags for styling — use CSS. `<ul>` for unordered lists, `<ol>` for ordered lists, `<dl>`/`<dt>`/`<dd>` for description lists. |

---

## Baseline 14: Links

**WCAG Success Criteria:** 2.4.4 Link Purpose (In Context), 4.1.2 Name, Role, Value

### Limitations, Assumptions, or Exceptions

- A link's purpose may be intentionally obscured (e.g., "Door #1, Door #2" in a game) — this is acceptable if ambiguity is intentional for all users.
- Programmatically determined link context includes: text in the same paragraph, list, or table cell as the link, or text in an associated table header cell.
- The combination of accessible name and accessible description is the text alternative.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 14.A-1 | Each link has a non-empty combination of accessible name and accessible description. | 4.1.2 |
| 14.A-2 | The purpose of each link can be determined from: (a) the link text alone, or (b) the link text plus its programmatically determined context. | 2.4.4 |

### Format-Specific Implementation Techniques

| Format | Techniques |
|--------|-----------|
| **PDF** | Use PDF11 (Link annotation with `/Link` structure element) for tagged links. Use PDF13 (/Alt entry in the link structure element for alternative text when link text alone is insufficient). Avoid "click here" or "read more" as link text. |
| **Word** | Insert hyperlinks with descriptive display text (Insert → Link). Right-click hyperlink → Edit Hyperlink → Text to display. Use ScreenTip for additional context when needed. |
| **Excel** | Insert → Link. Provide descriptive Cell Text. For email links, use HYPERLINK formula with descriptive friendly_name parameter. |
| **PowerPoint** | Insert → Link. Enter descriptive text. For image links, provide Alt Text that describes the link destination. |
| **HTML/CSS** | Use meaningful text within `<a>` elements. For icon-only links: `aria-label` on `<a>`, or visually hidden `<span>` text. For images as links: `alt` attribute on `<img>`. Use `aria-describedby` to point to nearby context. |

---

## Baseline 15: Language

**WCAG Success Criteria:** 3.1.1 Language of Page, 3.1.2 Language of Parts

### Limitations, Assumptions, or Exceptions

- The primary document language is based on the application's language preference settings.
- Exception: proper names, technical terms, words of indeterminate language, and words/phrases absorbed into the surrounding language's vernacular are not required to have language attributes.
- Dialects specified after the primary language tag are not part of this test (e.g., testing for `en` vs. `en-US`).

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 15.A-1 | The document's default human language property is set and matches the primary language of the content. | 3.1.1 |
| 15.B-1 | Text passages in a language different from the document's default language have the appropriate language programmatically specified. | 3.1.2 |

### Format-Specific Implementation Techniques

| Format | Default Language | Language of Parts |
|--------|-----------------|-------------------|
| **PDF** | Set `/Lang` entry in the document catalog (PDF16). In Acrobat: File → Properties → Advanced → Language. | Set `/Lang` attribute on individual tagged elements containing non-default-language content (PDF19). |
| **Word** | Review → Language → Set Proofing Language (applies to entire document as default). | Select text → Review → Language → Set Proofing Language → choose language for that passage. |
| **Excel** | File → Options → Language → Office display language. Spreadsheet language set via Review → Language. | Select cells → Review → Language → Set Proofing Language for specific ranges. |
| **PowerPoint** | Review → Language → Set Proofing Language for default. | Select specific text → Review → Language → Set Proofing Language for that text. |
| **HTML/CSS** | `<html lang="en">` (or appropriate BCP 47 language tag) on the root element (H57). | `lang="fr"` attribute on any element containing non-default-language content: `<span lang="fr">Bonjour</span>` (H58). |

---

## Baseline 16: Audio-Only and Video-Only

**WCAG Success Criteria:** 1.2.1 Audio-only and Video-only (Prerecorded)

### Limitations, Assumptions, or Exceptions

- **Audio-only:** Time-based presentation containing only audio (no video, no interaction). Short notification sounds (beeps, chimes) are excluded — covered in Baseline 7.
- **Video-only:** Time-based presentation containing only video (no audio, no interaction).
- Media labeled as a "media alternative for text" is exempt if it is genuinely equivalent to the accompanying text.
- Audio synchronized with video/slides/animations is NOT audio-only — test under Baseline 17.
- Video accompanied by meaningful audio/dialogue is NOT video-only — test under Baseline 17.
- Video-only moving/blinking content must also comply with Baseline 21 (Timed Events).

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 16.A-1 | Prerecorded audio-only content has a text transcript. | 1.2.1 |
| 16.A-2 | The transcript is in actual text format (not an image of text). | 1.2.1 |
| 16.A-3 | The transcript is accurate and complete, including all dialogue, speaker identification, and relevant non-speech sounds (doors, sirens, music, etc.). | 1.2.1 |
| 16.B-1 | Prerecorded video-only content has either a text alternative or a descriptive audio track. | 1.2.1 |
| 16.B-2 | The alternative describes all meaningful visual content including actions, characters, scene changes, and on-screen text. | 1.2.1 |

### Format-Specific Notes

| Format | Notes |
|--------|-------|
| **PDF** | Audio/video embedded in PDFs (via multimedia annotations) must include transcripts/descriptions linked within or adjacent to the media. |
| **Word** | Embedded audio/video objects must have transcripts as accompanying text in the document. |
| **Excel** | Audio/video embedded in cells or as objects must have transcript text in adjacent cells or linked documents. |
| **PowerPoint** | Embedded audio/video on slides must have transcript text on the slide or in speaker notes. |
| **HTML/CSS** | Provide transcript text adjacent to, or linked from, the audio/video element. `<audio>` and `<video>` elements with the `controls` attribute. Link to transcript: `<a href="transcript.html">Transcript</a>`. |

---

## Baseline 17: Synchronized Media

**WCAG Success Criteria:** 1.2.2 Captions (Prerecorded), 1.2.3 Audio Description or Media Alternative (Prerecorded) [Level A — not tested at AA], 1.2.4 Captions (Live), 1.2.5 Audio Description (Prerecorded); Section 508: 503.4, 503.4.1, 503.4.2

### Limitations, Assumptions, or Exceptions

- **Synchronized media:** Audio or video synchronized with another format for presenting information and/or with time-based interactive components.
- Media labeled as a "media alternative for text" is exempt if genuinely equivalent to the text.
- Captions must convey speech AND non-dialogue audio (sound effects, music, speaker identification, laughter).
- Captions and audio descriptions need to be available but not necessarily enabled by default.
- They may be in separate media files (captioned version, audio-described version).
- If all video track information is available in the audio track, audio description is not required.
- SC 1.2.5 (Level AA) is tested for this Section 508 baseline. SC 1.2.3 (Level A) is marked Not Applicable at the AA level.
- Live captions exception: Two-way multimedia calls between individuals through web apps are excluded.
- Section 508 503.4.x requirements apply when ICT displays video with synchronized audio and has volume/program selection controls.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 17.A-1 | Media player provides user controls for captions. | 508 503.4 |
| 17.A-2 | Media player provides user controls for audio descriptions. | 508 503.4 |
| 17.B-1 | Caption controls are at the same menu level as volume adjustment controls. | 508 503.4.1 |
| 17.C-1 | Audio description controls are at the same menu level as volume/program selection controls. | 508 503.4.2 |
| 17.D-1 | Prerecorded synchronized media has captions. | 1.2.2 |
| 17.D-2 | Captions are accurate, time-synchronized, and include all dialogue plus non-dialogue audio information. | 1.2.2 |
| 17.D-3 | Captions do not obscure relevant video content. | 1.2.2 |
| 17.E-1 | Prerecorded synchronized media has audio descriptions of important visual content not conveyed in the audio track. | 1.2.5 |
| 17.F-1 | Live synchronized media has captions. | 1.2.4 |
| 17.F-2 | Live captions include dialogue and important sounds. | 1.2.4 |

### Format-Specific Notes

| Format | Notes |
|--------|-------|
| **PDF** | Embedded media players must expose caption and audio description controls. Use media player controls that support captions (e.g., `.srt` or WebVTT tracks). |
| **Word** | Embedded video must include captions. Use media players with built-in caption support. |
| **Excel** | Embedded video must include captions. Rarely applicable; link to external captioned media when needed. |
| **PowerPoint** | Embedded video supports captions via PowerPoint's Video Caption feature (Insert → Captions). Alternatively, use Microsoft Stream which supports captioned video embedding. |
| **HTML/CSS** | `<video>` element with `<track kind="captions" src="captions.vtt" srclang="en" label="English">`. Audio descriptions via `<track kind="descriptions">` or separate audio-described video file. ARIA: `aria-label` on media player controls. |

---

## Baseline 18: Meaningful Content and Sequence (Stylesheet Non-Dependence)

**WCAG Success Criteria:** 1.3.1 Info and Relationships, 1.3.2 Meaningful Sequence

### Limitations, Assumptions, or Exceptions

- Meaningful content includes content in headers, footers, watermarks, master page items, artifacts, and floating elements.
- Inline styling is included in this test.
- Invisible content (same-color text/background used for accessibility) is covered in 18.B.
- Programmatically identified content is what is exposed to assistive technology.
- For web: removing or disabling CSS must not cause loss of information or scrambled reading order.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 18.A-1 | All meaningful content is available in the document body or is programmatically identified (not lost in headers/footers/artifacts). | 1.3.1 |
| 18.B-1 | The reading order (tag order / source order) of all meaningful content is logical and preserves meaning. | 1.3.2 |

### Format-Specific Implementation Techniques

| Format | Techniques |
|--------|-----------|
| **PDF** | Use PDF3 to ensure correct tab and reading order. Use PDF4 to mark decorative/background elements as artifacts. Use Acrobat's Reading Order tool and Tags panel to verify tag order. Use PDF17 for consistent page numbering. Remove content from headers/footers if it needs to be in the reading sequence. |
| **Word** | Use the Navigation Pane and Outline View to review document structure. Ensure text boxes and floating elements are either in-line or have correct reading position. Use "Wrap Text → In Line with Text" for objects that carry meaning. |
| **Excel** | Reading order follows cell order (left to right, top to bottom). For merged cells and visual arrangements, verify that content makes sense when read in cell order. |
| **PowerPoint** | Reading order per slide is set in the Selection Pane (Home → Arrange → Selection Pane). Objects at the bottom of the list are read first. Title placeholders should be at the bottom (read first). |
| **HTML/CSS** | Ensure DOM order matches visual/logical reading order. Do not use CSS `position: absolute/fixed`, `float`, or `order` (Flexbox/Grid) in ways that create visual order that diverges from DOM order. Verify by disabling CSS (browser Dev Tools → uncheck stylesheets). |

---

## Baseline 19: Frames and iFrames

**WCAG Success Criteria:** 4.1.2 Name, Role, Value

### ⚠️ Applicability

| Format | Applies? | Notes |
|--------|:--------:|-------|
| PDF | ❌ No | Frames/iframes are not implemented in non-web documents |
| Word | ❌ No | Same |
| Excel | ❌ No | Same |
| PowerPoint | ❌ No | Same |
| HTML/CSS | ✅ Yes | `<frame>` (deprecated but may exist) and `<iframe>` must be titled |

### Limitations, Assumptions, or Exceptions (HTML/CSS Only)

- `<frame>` is obsolete in HTML5 but may still be encountered.
- The combination of accessible name and accessible description of an `<iframe>` is its text alternative.
- Do not use `role="presentation"` or `aria-hidden="true"` on a focusable element (ARIA 4th Rule).
- All interactive elements must have an accessible name (ARIA 5th Rule).

### Universal Test Checks (HTML/CSS Only)

| Test ID | Check | SC |
|---------|-------|----|
| 19.A-1 | Each `<frame>` has a non-empty `title` attribute. | 4.1.2 |
| 19.A-2 | The `title` attribute describes the frame's content. | 4.1.2 |
| 19.B-1 | Each focusable `<iframe>` has a non-empty combination of accessible name and description. | 4.1.2 |
| 19.B-2 | The accessible name/description for each `<iframe>` describes its content. | 4.1.2 |
| 19.B-3 | `<iframe>` does not have `role="presentation"`, `role="none"`, or `aria-hidden="true"`. | 4.1.2 |

### Format-Specific Implementation (HTML/CSS)

```html
<!-- Correct iFrame -->
<iframe src="navigation.html" title="Site Navigation Menu" width="200" height="400"></iframe>

<!-- Correct frame (legacy) -->
<frame src="content.html" title="Main Content Area">

<!-- Incorrect: no title -->
<iframe src="widget.html"></iframe>
```

---

## Baseline 20: Conforming Alternate Version

**WCAG Conformance Requirement 1:** Conforming Alternate Version

### Limitations, Assumptions, or Exceptions

- It is NOT a WCAG requirement to provide a conforming alternate version. This test applies only when such a version exists.
- If no conforming alternate version exists, the result is "Does Not Apply" (not a failure).
- The alternate version does not need to be page-for-page matched with the original.
- For multi-language content, conforming alternate versions are required for each offered language.
- The conforming version does not need to reside within the same site, as long as it is as freely available.
- Supplementary content (which supports the original) is not an alternate version.
- To meet Level AA, the document must satisfy all Level A and AA SCs, OR a Level AA conforming alternate version must be provided.

### Universal Test Checks (All Formats)

| Test ID | Check | Requirement |
|---------|-------|-------------|
| 20.A-1 | The alternate version provides all the same information and functionality in the same human language. | CAV |
| 20.A-2 | The alternate version is as up to date as the non-conforming content. | CAV |
| 20.A-3 | The alternate version passes all applicable baseline tests. | CAV |
| 20.A-4 | At least one of: (a) the conforming version is reachable from the non-conforming version via an accessibility-supported mechanism, OR (b) the non-conforming version can only be reached from the conforming version, OR (c) the non-conforming version can only be reached from a conforming page that also provides access to the conforming version. | CAV |
| 20.A-5 | The content indicates that a conforming alternate version is available. | CAV |

---

## Baseline 21: Timed Events

**WCAG Success Criteria:** 1.4.2 Audio Control, 2.2.1 Timing Adjustable, 2.2.2 Pause, Stop, Hide; Conformance Requirement 5: Non-Interference (for 1.4.2 and 2.2.2)

### Limitations, Assumptions, or Exceptions

**Exceptions to SC 2.2.1 (Timing Adjustable) — time limits that are NOT included:**
- Real-time event exception: time limit is required for real-time events (e.g., auctions)
- Essential exception: extending the time limit would invalidate the activity
- 20-hour exception: time limit is longer than 20 hours
- Content that repeats and is under user control (scrolling text with controls, captioning, carousels)

**SC 2.2.2 (Pause, Stop, Hide):**
- "In parallel" means the content appears alongside other content simultaneously.
- "Essential" means removing the moving/blinking/scrolling content would fundamentally change its information or functionality.

**SC 1.4.2 (Audio Control):** Control of volume includes being able to reduce to zero. System mute is not sufficient — the control must be independent of system volume.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 21.A-1 | For each time limit, at least one of: (1) user can turn it off, (2) user can adjust to ≥10× default, OR (3) user is warned before expiry AND given ≥20 seconds to extend AND can extend ≥10 times. | 2.2.1 |
| 21.B-1 | Moving/blinking/scrolling content that starts automatically, lasts >5 seconds, and is presented in parallel has a pause, stop, or hide mechanism. | 2.2.2 |
| 21.C-1 | Auto-updating content that starts automatically and is presented in parallel has a pause, stop, hide, or frequency control mechanism. | 2.2.2 |
| 21.D-1 | Auto-playing audio (>3 seconds) has a mechanism at the beginning of content to pause/stop OR to control volume independently of system volume. | 1.4.2 |

### Format-Specific Implementation Techniques

| Format | Notes |
|--------|-------|
| **PDF** | Multimedia players embedded in PDFs must include play/pause controls accessible to keyboard users. Autoplay audio must have a visible, keyboard-accessible stop/volume control. |
| **Word** | Auto-playing audio in documents must have accessible controls. Timed form sessions must provide timeout warnings with extension options. |
| **Excel** | Auto-refreshing data connections with visible indicators must have user controls. Auto-playing sounds must have accessible controls. |
| **PowerPoint** | Slide transitions and animations set to auto-advance must provide user controls or not be the only way to access content. Auto-playing audio on slides must have start/stop controls. |
| **HTML/CSS** | `<video autoplay>` must have player controls. Use `<button>` to pause animations. CSS animations can be paused: use `animation-play-state: paused` via JavaScript. Respect `prefers-reduced-motion` media query. |

---

## Baseline 22: Resize Text

**WCAG Success Criteria:** 1.4.4 Resize Text

### Limitations, Assumptions, or Exceptions

- Exception: captions and images of text are not included.
- Resize mechanisms include: browser/application zoom, text-sizing features, OS accessibility features, or on-page controls.
- Text in form controls must also resize.

### Universal Test Checks (All Formats)

| Test ID | Check | SC |
|---------|-------|----|
| 22.A-1 | A mechanism exists to resize/scale content to at least 200% of original size. | 1.4.4 |
| 22.A-2 | At 200%, text is NOT clipped, truncated, or obscured. | 1.4.4 |
| 22.A-3 | At 200%, text in form controls resizes fully. | 1.4.4 |
| 22.A-4 | At 200%, all content remains available. | 1.4.4 |
| 22.A-5 | At 200%, all functionality remains available. | 1.4.4 |

### Format-Specific Implementation Techniques

| Format | Resize Mechanism | Common Failures |
|--------|-----------------|-----------------|
| **PDF** | Acrobat/Reader zoom (Ctrl/Cmd+= or View → Zoom). Ensure reflowable/tagged PDF allows text reflow at zoom. | Fixed-position text boxes that overflow; images of text that don't scale; untagged PDFs that don't reflow. |
| **Word** | View → Zoom. Word documents should reflow when zoomed. | Text boxes with fixed dimensions that clip content at high zoom. |
| **Excel** | View → Zoom. Cell content should be readable at 200%. | Fixed row heights that clip tall text at high zoom. |
| **PowerPoint** | View → Zoom. Presentation slides should scale. | Fixed-size text boxes that clip content. |
| **HTML/CSS** | Browser zoom (Ctrl/Cmd++). Use relative units (`em`, `rem`, `%`) for font sizes and container dimensions. Avoid `px`-only font sizes in critical contexts, `vw` for font sizes (F94), and fixed-width containers that don't accommodate text expansion. |

---

## Baseline 23: Multiple Ways

**WCAG Success Criteria:** 2.4.5 Multiple Ways

### ⚠️ Applicability

| Format | Applies? | Notes |
|--------|:--------:|-------|
| PDF | ❌ No | Per Section 508 E205.4, non-web documents are exempt from SC 2.4.5 |
| Word | ❌ No | Same exemption |
| Excel | ❌ No | Same exemption |
| PowerPoint | ❌ No | Same exemption |
| HTML/CSS | ✅ Yes | SC 2.4.5 applies to web content |

### Limitations, Assumptions, or Exceptions (HTML/CSS Only)

- Exception: web pages that are the result of, or a step in, a process are excluded.

### Universal Test Checks (HTML/CSS Only)

| Test ID | Check | SC |
|---------|-------|----|
| 23.A-1 | The web page provides at least two ways to locate it within the set of related web pages. | 2.4.5 |

### Acceptable Techniques (HTML/CSS)

- Site maps
- Site search functionality
- Tables of contents
- Navigation menus or dropdowns
- Navigation trees
- Links between related pages (e.g., previous/next)
- Breadcrumb navigation

---

## Baseline 24: Parsing (Auto-Pass)

**WCAG Success Criteria:** 4.1.1 Parsing

### ⚠️ Automatic Pass — No Testing Required

**Rationale:** WCAG 2.2 has deprecated SC 4.1.1 Parsing because accessibility issues previously addressed by this criterion are now handled by browsers/user agents. The WCAG 2.0 Errata states: "This criterion should be considered as always satisfied for any content using HTML or XML."

Section 508 incorporates WCAG 2.0 by reference (where 4.1.1 is not deprecated), but the WCAG 2.0 Errata applies.

| Test ID | Check | SC |
|---------|-------|----|
| 24.A | No testing necessary — this baseline automatically passes for all formats. | 4.1.1 |

---

## Format-Specific Exceptions Summary

The following table summarizes which baselines apply (✅), do not apply (❌), or auto-pass (✅*) for each format:

| Baseline | PDF | Word | Excel | PPT | HTML/CSS | Notes |
|----------|:---:|:----:|:-----:|:---:|:--------:|-------|
| 1. Keyboard | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 2. Focus | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 3. Non-Interference | ✅ | ✅ | ✅ | ✅ | ✅ | Composite of 1.B, 9.A, 21.B/C/D |
| 4. Repetitive Content | ❌ | ❌ | ❌ | ❌ | ✅ | Section 508 E205.4 exemption |
| 5. User Controls | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 6. Images | ✅ | ✅ | ✅ | ✅ | ✅ | CAPTCHAs: N/A for docs, test for web |
| 7. Sensory | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 8. Contrast | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 9. Flashing | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 10. Forms | ✅ | ✅ | ✅ | ✅* | ✅ | PPT has limited native form support |
| 11. Document Titles | ✅ | ✅ | ✅ | ✅ | ✅ | HTML: `<title>` element |
| 12. Tables | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 13. Structure | ✅ | ✅ | ✅* | ✅ | ✅ | Excel has limited heading support |
| 14. Links | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 15. Language | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 16. Audio/Video-Only | ✅ | ✅ | ✅ | ✅ | ✅ | Only if media is present |
| 17. Sync Media | ✅ | ✅ | ✅ | ✅ | ✅ | Only if synchronized media present |
| 18. Meaningful Sequence | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 19. Frames/iFrames | ❌ | ❌ | ❌ | ❌ | ✅ | Not implemented in non-web documents |
| 20. Alt Versions | ✅ | ✅ | ✅ | ✅ | ✅ | Only if alternate version exists |
| 21. Timed Events | ✅ | ✅ | ✅ | ✅ | ✅ | Only if timed content present |
| 22. Resize Text | ✅ | ✅ | ✅ | ✅ | ✅ | |
| 23. Multiple Ways | ❌ | ❌ | ❌ | ❌ | ✅ | Section 508 E205.4 exemption |
| 24. Parsing | ✅* | ✅* | ✅* | ✅* | ✅* | Auto-pass for all formats |

---

## PDF-Specific WCAG Techniques Reference

| Technique | Description | Baseline |
|-----------|-------------|:--------:|
| PDF1 | Applying text alternatives to images with the Alt entry | 6 |
| PDF3 | Ensuring correct tab and reading order | 1, 2, 18 |
| PDF4 | Hiding decorative images with the Artifact tag | 6, 18 |
| PDF5 | Indicating required form controls | 10 |
| PDF6 | Using table elements for table markup | 12 |
| PDF7 | Performing OCR on scanned PDFs | 6 |
| PDF9 | Providing headings by marking content with heading tags | 13 |
| PDF10 | Providing labels for interactive form controls | 10 |
| PDF11 | Providing links using the Link annotation and /Link structure element | 14 |
| PDF12 | Providing name, role, value for form fields | 10 |
| PDF13 | Providing replacement text for links using /Alt entry | 14 |
| PDF15 | Providing submit buttons with submit-form action | 10 |
| PDF16 | Setting the default language using /Lang in document catalog | 15 |
| PDF17 | Specifying consistent page numbering | 18 |
| PDF18 | Specifying document title using Title entry in document information dictionary | 11 |
| PDF19 | Specifying language for passages using Lang entry | 15 |
| PDF20 | Using Acrobat Table Editor to repair mistagged tables | 12 |
| PDF21 | Using List tags for lists | 13 |
| PDF22 | Indicating when user input falls outside required format in PDF forms | 10 |

---

## Accessibility Checker Tools Reference

| Format | Built-in Tool | Third-Party Tools |
|--------|--------------|-------------------|
| **PDF** | Acrobat → All tools → Prepare for accessibility → Accessibility Check | PAC 2024, CommonLook PDF, NVDA + Adobe Acrobat |
| **Word** | Review → Check Accessibility | NVDA/JAWS + Word, AMP (Accessibility Management Platform) |
| **Excel** | Review → Check Accessibility | NVDA/JAWS + Excel |
| **PowerPoint** | Review → Check Accessibility | NVDA/JAWS + PowerPoint |
| **HTML/CSS** | Browser DevTools Accessibility panel | axe, WAVE, NVDA, JAWS, VoiceOver, Lighthouse |

---

*Document generated from the [ICT Testing Baseline Portfolio](https://github.com/atbcb/ICTTestingBaseline) — U.S. Access Board (atbcb)*  
*Baseline for Electronic Documents v1.0 (September 30, 2024) and Baseline for Web v3.1 (April 1, 2024)*  
*This unified reference is designed for ingestion into AI/LLM knowledge bases and accessibility testing workflows.*
