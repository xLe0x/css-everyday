# `resize` Property in CSS

Ever wanted to let users control an element's size with minimal effort? The `resize` property makes it incredibly simple!

## 🖥️ Resize both width and height
```css
.element {
    resize: both;
    overflow: auto;
}
```
This allows the user to adjust both dimensions freely.

## ↔️ Resize width only
```css
.element {
    resize: horizontal;
    overflow: auto;
}
```
This restricts resizing to horizontal adjustments.

## ↕️ Resize height only
```css
.element {
    resize: vertical;
    overflow: auto;
}
```
This restricts resizing to vertical adjustments.

## ⚠️ Important Note:
The `resize` property **does not work** on:
- ❌ **Inline elements**
- ❌ Block elements with `overflow: visible`

To make it work, set `overflow` to `auto`, `scroll`, or `hidden`.

🔥 **Use this to enhance user interaction and make elements dynamically adjustable!** 🚀

