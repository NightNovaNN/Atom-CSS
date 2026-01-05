# Commands

This file lists **every utility class, component class, and special modifier** available in ATOM.css.  
Classes are grouped by category for easy reference.

## Layout & Flexbox Utilities

| Class                | Description                                                                          |
| -------------------- | ------------------------------------------------------------------------------------ |
| `.flex`              | `display: flex`                                                                      |
| `.row`               | `flex-direction: row` (default)                                                      |
| `.col`               | `flex-direction: column`                                                             |
| `.wrap`              | `flex-wrap: wrap`                                                                    |
| `.items-start`       | `align-items: flex-start`                                                            |
| `.items-center`      | `align-items: center`                                                                |
| `.items-end`         | `align-items: flex-end`                                                              |
| `.justify-start`     | `justify-content: flex-start`                                                        |
| `.justify-center`    | `justify-content: center`                                                            |
| `.justify-end`       | `justify-content: flex-end`                                                          |
| `.justify-between`   | `justify-content: space-between`                                                     |
| `.justify-around`    | `justify-content: space-around`                                                      |
| `.center`            | Centers both horizontally and vertically (`align-items` + `justify-content: center`) |
| `.gap-1` to `.gap-5` | `gap: 4px → 24px` (uses `--space-1` to `--space-5`)                                  |

## Spacing Utilities

| Class              | Description                        |
| ------------------ | ---------------------------------- |
| `.p-1` to `.p-5`   | Padding all sides (`4px` → `24px`) |
| `.px-1` to `.px-5` | Horizontal padding                 |
| `.py-1` to `.py-5` | Vertical padding                   |
| `.m-1` to `.m-5`   | Margin all sides                   |

## Background & Text Color Utilities

| Class          | Description                |
| -------------- | -------------------------- |
| `.bg-0`        | Main background (`--bg-0`) |
| `.bg-1`        | Secondary background       |
| `.bg-2`        | Tertiary background        |
| `.bg-code`     | Code block background      |
| `.bg-accent`   | Accent / hover background  |
| `.text-main`   | Primary text color         |
| `.text-muted`  | Muted / secondary text     |
| `.text-blue`   | Accent blue                |
| `.text-purple` | Accent purple              |
| `.text-green`  | Accent green               |
| `.text-orange` | Accent orange              |
| `.text-red`    | Accent red                 |
| `.text-yellow` | Accent yellow              |

## Typography & Font Utilities

| Class          | Description                    |
| -------------- | ------------------------------ |
| `.text-sm`     | Smaller font (`0.85rem`)       |
| `.text-md`     | Medium font (`1rem`) – default |
| `.text-lg`     | Larger font (`1.2rem`)         |
| `.font-bold`   | `font-weight: 700`             |
| `.font-italic` | `font-style: italic`           |

## Border Radius & Shadow

| Class         | Description                         |
| ------------- | ----------------------------------- |
| `.round-sm`   | Small radius (`6px`)                |
| `.round-md`   | Medium radius (`10px`)              |
| `.round-lg`   | Large radius (`16px`)               |
| `.round-full` | Full pill shape (`999px`)           |
| `.shadow-sm`  | Small shadow                        |
| `.shadow-md`  | Medium shadow (used on hover often) |

## Buttons

| Class        | Description         |
| ------------ | ------------------- |
| `.btn`       | Base button style   |
| `.btn-blue`  | Blue filled button  |
| `.btn-green` | Green filled button |
| `.btn-red`   | Red filled button   |

## Labels & Tags

| Class            | Description                   |
| ---------------- | ----------------------------- |
| `.label`         | Base label style              |
| `.keyword-label` | Purple keyword style          |
| `.label-blue`    | Blue translucent background   |
| `.label-green`   | Green translucent background  |
| `.label-orange`  | Orange translucent background |

## Code & Syntax Highlighting

| Class                                    | Usage                                                  |
| ---------------------------------------- | ------------------------------------------------------ |
| `.inline-code`                           | Inline code styling                                    |
| `pre > code`                             | Block code – automatically highlighted by Highlight.js |
| `.language-python`, `.language-js`, etc. | Add to `<code>` for specific language highlighting     |
| `.code-wrap`                             | Wrapper for code block + copy button                   |
| `.copy-btn`                              | Copy button (JS-enhanced)                              |
| `.copy-btn.copied`                       | Applied automatically on successful copy               |

## Tabs / Pages (Pure CSS)

**HTML Structure Example:**

```html
<div class="tabs">
  <input type="radio" id="tab1" name="tab-group" checked />
  <label for="tab1" class="tab-label">Tab 1</label>
  <div class="tab-content">Content 1</div>

  <input type="radio" id="tab2" name="tab-group" />
  <label for="tab2" class="tab-label">Tab 2</label>
  <div class="tab-content">Content 2</div>
</div>
```

| Class          | Description                               |
| -------------- | ----------------------------------------- |
| `.tabs`        | Container for tabs                        |
| `.tab-labels`  | Optional wrapper for labels (visual only) |
| `.tab-label`   | Styling for each tab label                |
| `.tab-content` | Hidden/shown content panel                |

## Accordion (Pure CSS)

**HTML Structure:**

```html
<div class="accordion">
  <input type="checkbox" id="acc1" />
  <label for="acc1" class="acc-label">Header</label>
  <div class="acc-content">Content</div>
</div>
```

| Class          | Description                      |
| -------------- | -------------------------------- |
| `.accordion`   | Container (optional flex column) |
| `.acc-label`   | Clickable header                 |
| `.acc-content` | Collapsible content              |

## Tooltip

**Usage:**

```html
<span class="tooltip" data-tooltip="Your text here">Hover me</span>
```

| Class      | Description                                     |
| ---------- | ----------------------------------------------- |
| `.tooltip` | Enables hover tooltip using `data-tooltip` attr |

## Modal (JS Required)

**Usage:**

```html
<button data-modal-target="myModal">Open</button>
<div class="modal" id="myModal">
  ...<button class="close-modal">Close</button>
</div>
```

| Class            | Description                       |
| ---------------- | --------------------------------- |
| `.modal`         | Overlay container                 |
| `.modal.active`  | Shown state (added/removed by JS) |
| `.modal-content` | Inner centered content box        |
| `.close-modal`   | Button class for closing          |

## Sidebar

| Class             | Description                             |
| ----------------- | --------------------------------------- |
| `.sidebar`        | Fixed left sidebar                      |
| `.sidebar.closed` | Hidden on mobile (toggle with JS)       |
| `.sidebar-toggle` | Mobile menu button (☰)                  |
| `.main-content`   | Push content right when sidebar is open |

## Lists & Bullets

| Class          | Description               |
| -------------- | ------------------------- |
| `.list-circle` | `list-style-type: circle` |
| `.list-square` | `list-style-type: square` |
| `.list-none`   | Remove bullets/numbers    |

## Cards, Alerts & Progress

| Class            | Description                                 |
| ---------------- | ------------------------------------------- |
| `.card`          | Elevated card with padding and hover shadow |
| `.alert`         | Base alert style                            |
| `.alert-info`    | Blue info alert                             |
| `.alert-success` | Green success alert                         |
| `.alert-warning` | Orange warning alert                        |
| `.alert-danger`  | Red danger alert                            |
| `.progress`      | Progress container                          |
| `.progress-bar`  | Inner bar (set width inline or via JS)      |

## Form Elements

| Element / Class | Description                                   |
| --------------- | --------------------------------------------- |
| `textarea`      | Enhanced styling, focus ring, resize vertical |

## Theme & Config

| Attribute / File                 | Purpose                                                          |
| -------------------------------- | ---------------------------------------------------------------- |
| `data-theme="light"` on `<html>` | Switches to built-in light theme                                 |
| `atcss.config.json`              | Optional config for theme, fonts, custom CSS, variable overrides |

## Animations (Add to any element)

| Class       | Description                 |
| ----------- | --------------------------- |
| `.fade-in`  | Fade in on load             |
| `.slide-up` | Slide up from below on load |

---

This reference covers **all classes** currently available in ATOM.css v0.1.
Use them freely — most are utility-first and can be combined.
