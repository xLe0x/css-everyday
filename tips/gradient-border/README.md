Tired of using `::before` and `::after` just to create a gradient border? There's a much easier way! 😍

### ✨ The magic code:

```css
button {
  border: 5px solid; /* A border is required for it to work */
  border-image: linear-gradient(to right, purple, red) 1;
  border-radius: 8px; /* Optional for a smoother look */
}
```

![](../_images/gradient-border.png)

🔥 **The result?** A beautiful gradient border with zero extra elements!
