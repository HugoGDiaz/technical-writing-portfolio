# CSS Flexbox Layout Guide
*Step-by-step guide to building flexible, one-dimensional layouts with CSS Flexbox.*

## Overview
CSS Flexbox is a layout system designed for arranging elements in a single direction—either horizontally or vertically. It excels at distributing space, aligning items, and adapting layouts based on available space.

This guide introduces CSS Flexbox through practical explanations and examples, focusing on how to control alignment, spacing, and flow in modern user interfaces.

---

## When to Use CSS Flexbox
Flexbox is best suited for layouts where content flow and alignment are more important than overall page structure.

Use CSS Flexbox when you need to:
- Align items along a single axis (row or column)
- Distribute space dynamically between elements
- Center content vertically or horizontally
- Build flexible UI components such as navigation bars, cards, and toolbars

---

## Core Concepts

### Flex Container
A Flexbox layout begins by defining a flex container:

```css
display: flex;
```

This enables flex behavior for all direct children of the container.

### Main Axis and Cross Axis
Flexbox layouts are defined by two axes:

- **Main axis**: the primary direction of layout (row or column)  
- **Cross axis**: perpendicular to the main axis  

Understanding these axes is essential for controlling alignment and spacing.

### Flex Items
Each direct child of a flex container becomes a flex item and can be individually aligned or resized.

---

## Creating a Basic Flex Layout
Example: a horizontal navigation bar with evenly spaced items.

- Items are laid out in a row  
- Space is distributed automatically  
- Items remain aligned as the container resizes  

Flexbox adapts naturally to content size and viewport changes.

---

## Controlling Alignment and Spacing
Flexbox provides dedicated properties for alignment:

```css
justify-content: space-between;
align-items: center;
```

- `justify-content` controls alignment along the main axis  
- `align-items` controls alignment along the cross axis  

These properties eliminate the need for manual spacing hacks.

---

## Flexible Item Sizing
Flex items can grow, shrink, or maintain fixed sizes:

```css
flex: 1;
```

This allows layouts to adapt fluidly without explicit width calculations.

---

## Responsive Layouts with Flexbox
Flexbox works well in responsive design scenarios.

Common strategies include:
- Switching `flex-direction` based on screen size  
- Allowing items to wrap using `flex-wrap`  
- Combining Flexbox with media queries for layout adjustments  

This makes Flexbox ideal for component-level responsiveness.

---

## Common Mistakes to Avoid
- Using Flexbox for full page layouts where Grid would be clearer  
- Overusing `flex: 1` without understanding item sizing  
- Mixing axis concepts (main vs cross) incorrectly  

Flexbox works best when used for alignment and flow, not full structural layout.