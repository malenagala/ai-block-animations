# AI Animations

Animated HTML blocks for embedding in a CMS. Each animation runs as a self-contained iframe inside a responsive wrapper block.

## Structure

```
AI ANIMATIONS/
├── block-*.html                  # CMS embed blocks (5 total)
│   ├── block-typing-small.html
│   ├── block-process-small.html
│   ├── block-refinement-small.html
│   ├── block-report-small.html
│   └── block-result-small.html
│
├── standalone-animations/        # Animation source files (loaded by blocks via iframe)
│   ├── typing-animation.html
│   ├── process-animation.html
│   ├── refinement-animation.html
│   ├── report-animation.html
│   └── result-animation.html
│
├── src/
│   └── assets/                   # Images used by the animations
│       ├── chart_1.png
│       ├── chart_2.png
│       ├── content.png
│       ├── cursor.png
│       ├── refinement-animation-image.png
│       ├── report_base.png
│       ├── report_tag.png
│       ├── result-content.png
│       └── sparkle.png
│
├── guidelines/                   # Design guidelines
└── ATTRIBUTIONS.md
```

## Usage

Drop any `block-*.html` file into your CMS as an HTML embed. Each block file references its animation via a relative path — keep the folder structure intact when uploading.

The `block-*.html` files include responsive scaling logic with configurable zoom and pan per breakpoint (desktop / tablet / mobile).
