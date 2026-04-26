# Technical Reference

This document contains the full technical specification for SVG-to-PPT compatible diagram generation.

For the original detailed guide, see the skill files:
- [Chinese Version](../skills/svg-ppt-guide-zh.md)
- [English Version](../skills/svg-ppt-guide-en.md)

## Vertical Centering Formula

```
y = box.y + box.height / 2 + font_size / 3
```

## Data-Driven Coordinate Mapping

```
y_coordinate = Base_Y - (Total_Height * Percentage)
```

## Arrow Construction Pattern

```xml
<g id="Arrow_1">
  <!-- Line penetrates 3px into polygon -->
  <line x1="100" y1="200" x2="203" y2="200" stroke="#7a8b7a" stroke-width="2"/>
  <polygon points="200,195 210,200 200,205" fill="#7a8b7a"/>
</g>
```

## Morandi Color Palette Reference

| Name | Hex | Usage |
|------|-----|-------|
| Sage Green | `#7a8b7a` | Primary blocks |
| Dusty Rose | `#c4a6a6` | Accent / highlights |
| Warm Gray | `#a8a0a0` | Borders / lines |
| Slate Blue | `#7b8fa2` | Secondary blocks |
| Sand | `#c8b99a` | Background elements |
| Muted Mauve | `#b09eb0` | Tertiary elements |
