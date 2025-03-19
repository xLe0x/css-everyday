Do you still write CSS like this?

```css
.container p {
  color: white;
}

.container span {
  color: white;
}
```

Or maybe like this?

```css
.container p,
.container span {
  color: white;
}
```

Well, it's time to level up your CSS! 🚀
Instead of repeating yourself, you can use `:is()` to make your code cleaner and shorter:

```css
.container :is(p, span) {
  color: white;
}
```

This way, you write less code while keeping it more readable and maintainable!
