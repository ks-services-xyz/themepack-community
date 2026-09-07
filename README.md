# CSS Theme Utilities

A lightweight CSS utility file that provides simple, semantic classes for using **theme-based CSS variables**.

Instead of using color values directly, these utilities use your design-system theme tokens such as `--color-ks-bg-primary`, `--color-ks-text-primary`, etc.

## Usage

Include the CSS file in your project:

```html
<link rel="stylesheet" href="theme.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@kraft.stitch/themepack/theme-pack.min.css">
```

Then use the utility classes directly:

```html
<div class="bg-primary text-primary border-primary">
  Hello World
</div>
```

## Controls

Theme utilities can also be used with common UI controls such as:

Example:

```html
<button class="bg-brand text-primary border-brand">
  Save
</button>

<input class="bg-primary text-primary border-secondary text-placeholder"
       placeholder="Enter your name">
```

## Theme Variables

These classes do not define colors themselves. They use CSS variables provided by your theme.

Example:

```css
:root {
  --color-ks-bg-primary: #ffffff;
  --color-ks-text-primary: #111111;
  --color-ks-border-primary: #dddddd;
}
```

This makes it easy to switch themes without changing your HTML.

```css
.dark {
  --color-ks-bg-primary: #111111;
  --color-ks-text-primary: #ffffff;
  --color-ks-border-primary: #333333;
}
```

The same HTML can then work with different themes:

```html
<div class="bg-primary text-primary border-primary">
  Theme-aware component
</div>
```

## Available Utilities

| Category   | Examples                                         |
| ---------- | ------------------------------------------------ |
| Background | `bg-primary`, `bg-secondary`, `bg-brand`         |
| Foreground | `fg-primary`, `fg-secondary`, `fg-brand`         |
| Text       | `text-primary`, `text-error`, `text-success`     |
| Border     | `border-primary`, `border-error`, `border-brand` |
| Controls   | Buttons, inputs, selects, switches, etc.         |

## Design

The utilities are intentionally **small, semantic, and theme-aware**.

You use:

```html
text-primary
```

instead of:

```css
color: #111827;
```

This keeps components independent from specific colors and allows the theme to control the actual appearance.

## 📚 Documentation

For detailed documentation, utility references, examples, and usage guidelines, visit the KSPack community repository:

👉 **[KSPack Documentation](https://github.com/ks-services-xyz/csspack-community)**

---

## 🐛 Issues & Feature Requests

Found a bug, have a feature idea, or want to suggest an improvement?

Please open an issue in the KSPack community repository.

👉 **[Report an Issue or Request a Feature](https://github.com/ks-services-xyz/themepack-community/issues)**

You can use GitHub Issues for:

* 🐛 Bug reports
* 💡 Feature requests
* 🎨 Utility suggestions
* 📚 Documentation improvements
* ⚡ Performance improvements
* 💬 General feedback

---

## 🤝 Contributing

Contributions and suggestions are welcome.

If you would like to contribute to KSPack:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Test your changes.
5. Create a pull request.

Please check the community repository for contribution guidelines.

👉 **[Contribute to KSPack](https://github.com/ks-services-xyz/themepack-community)**

---

## 📄 License

KSPack is released under the **MIT License**.

See the [LICENSE](LICENSE) file for the complete license text.

---

## ⭐ Support the Project

If you find KSPack useful, consider giving the project a ⭐ on GitHub.

Your feedback, suggestions, and contributions help improve KSPack.

**Made with ❤️ by @kraft.stitch**

