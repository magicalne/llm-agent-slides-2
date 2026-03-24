# LLM Agent Slides - Part 2

A presentation project about LLM Agents - Part 2: Deep Dive.

## Quick Start

1. Open `index.html` in a browser to start the presentation
2. Use arrow keys or click left/right sides to navigate
3. Press `F` for fullscreen mode

## Project Structure

```
llm-agent-slides-2/
├── index.html           # Presentation controller (entry point)
├── CLAUDE.md            # Project documentation
├── styles/
│   ├── theme.css        # Shared theme styles
│   └── fonts.css        # Font face declarations
├── fonts/               # Self-hosted font files
│   ├── urbanist-*.woff2
│   ├── ibm-plex-sans-*.woff2
│   └── jetbrains-mono-*.woff2
├── slides/              # Individual slide files
│   ├── 01-title.html
│   ├── 02-chatbot-vs-agent.html
│   └── 03-context-window.html
└── notes/               # Content notes/drafts
    ├── 01-intro.md
    └── 02-context-window.md
```

## Adding New Slides

1. Create a new HTML file in `slides/` folder (e.g., `04-topic.html`)
2. Use the template below with appropriate slide class
3. Add the slide path to the `SLIDES` array in `index.html`

### Slide Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Slide Title</title>
<link rel="stylesheet" href="../styles/fonts.css">
<link rel="stylesheet" href="../styles/theme.css">
</head>
<body>

<div class="slide slide-[TYPE]">
  <div class="slide-inner">
    <!-- Content here -->
  </div>
</div>

</body>
</html>
```

## Slide Types

Use these classes on the `.slide` element:

| Class | Description |
|-------|-------------|
| `slide-title` | Title slide with centered tag, heading, subtitle, author |
| `slide-content` | Section label, heading, lead text, 3-column cards |
| `slide-highlight` | Big number/stat, quote, centered layout |
| `slide-two-column` | Two-column layout for text + visual |
| `slide-list` | Bulleted list with icons |
| `slide-code` | Code snippet with syntax highlighting |

## Stepped Slides

For slides with multiple steps (animations/reveals), use this format in `index.html`:

```javascript
const SLIDES = [
  'slides/01-title.html',
  { file: 'slides/02-topic.html', steps: 3 },  // 3 steps
];
```

And in the slide HTML:

```html
<div class="step-content active" id="step-0">...</div>
<div class="step-content" id="step-1">...</div>
<div class="step-content" id="step-2">...</div>

<script>
let currentStep = 0;
function goToStep(step) {
  currentStep = step;
  document.querySelectorAll('.step-content').forEach((el, i) => {
    el.classList.toggle('active', i === step);
  });
}
window.addEventListener('message', (e) => {
  if (e.data.type === 'goToStep') goToStep(e.data.step);
});
</script>
```

## Presentation Controls

| Control | Action |
|---------|--------|
| `←` `→` | Previous / Next slide |
| `Space` | Next slide |
| `F` | Toggle fullscreen |
| `Home` / `End` | First / Last slide |
| `Esc` | Exit fullscreen |
| Click left/right | Navigate slides |
| Swipe (mobile) | Navigate slides |

## Theme Specifications

### Colors
- **Background:** `#1A0B2E` (deep purple)
- **Background Primary:** `#110721` (darker purple)
- **Primary Text:** `#FFFFFF` (white)
- **Secondary Text:** `#B8A9CC` (light purple)
- **Muted Text:** `#7B6B8D` (muted purple)
- **Accent:** `#A855F7` (bright purple)
- **Accent Soft:** `#C084FC` (lighter purple)

### Typography
- **Heading Font:** Urbanist (weights: 300-800)
- **Body Font:** IBM Plex Sans (weights: 300-600)

### Design Elements
- Card backgrounds: `rgba(255,255,255,0.04)`
- Borders: `rgba(255,255,255,0.05)`
- Border radius: 10-12px (containers), 100px (tags/pills)
- Subtle glow effects using accent color
- Radial gradient overlays for depth

## Guidelines

1. Follow the established color palette and typography
2. Keep slide content focused - one main idea per slide
3. Use card components for listing features, steps, or comparisons
4. Include visual hierarchy: section labels → headings → body text
5. Maintain consistent padding (64-72px) and spacing
