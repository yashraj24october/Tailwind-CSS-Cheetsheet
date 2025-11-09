# Tailwind-CSS-Installation-using-CLI

### Install tailwind css cli
```html
npm install tailwindcss @tailwindcss/cli
```

### Import Tailwind css in input.css for accessing classes of tailwind
```html
@import "tailwindcss";
```

## Compile input.css into output.css
```html
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```
