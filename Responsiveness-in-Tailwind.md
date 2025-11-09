## Responsiveness

- **Mobile-first approach:** Styles apply to all screens by default, and larger breakpoints override them.
- **Syntax:** `{breakpoint}:{utility}`

- **Default Breakpoints:**
  - `sm:` → 640px (Small devices)
  - `md:` → 768px (Tablets)
  - `lg:` → 1024px (Laptops)
  - `xl:` → 1280px (Desktops)
  - `2xl:` → 1536px (Large screens)

**Example:**
```html
<div class="p-2 md:p-6 lg:p-10">
  Responsive Padding
</div>
```
