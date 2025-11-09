# Tailwind-CSS-Complete-Cheatsheet

## For Structuring and Layout of Components

- w-full → Makes the element span the full width of its parent.
- container, mx-auto, and p-4 → For container sized, centered responsive layout.

```html
<div class="w-full">
  <div class="container mx-auto p-4">
    <content>
  </div>
</div>
```

## Background Stylings
- **Background Color:** bg-{color}-{shade}, bg-[url('image_url')], bg-[custom_value]-[custom_shade_value]
- **Background Image:** bg-none, bg-gradient-to-r/l/t/b
- **Position:** bg-top, bg-center, bg-bottom, bg-left, bg-right
- **Size:** bg-auto, bg-cover, bg-contain
- **Repeat:** bg-repeat, bg-no-repeat, bg-repeat-x, bg-repeat-y
- **Attachment:** bg-fixed, bg-local, bg-scroll
- **Clip:** bg-clip-border, bg-clip-padding, bg-clip-content, bg-clip-text
- **Opacity:** bg-opacity-{0–10}

## Text Styling
- **Font Size:** text-xs ... text-9xl, text-[custom_value]
- **Font Weight:** font-thin ... font-black, font-[custom_value]
- **Font Style:** italic, not-italic
- **Text Alignment:** text-left, text-center, text-right, text-justify, text-start, text-end
- **Text Decoration:** underline, overline, line-through, no-underline, decoration-{color},
 decoration-{style}, decoration-{thickness}
- **Text Transform:** uppercase, lowercase, capitalize, normal-case
- **Line Height:** leading-none ... leading-loose
- **Letter Spacing:** tracking-tighter ... tracking-widest
- **Text Color:** text-{color}-{shade}, text-[custom_color_value]-[custom_shade_value]
- **Text Opacity:** text-opacity-{0–100}
- **Whitespace:** whitespace-normal, whitespace-nowrap, whitespace-pre, whitespace-pre-line,
 whitespace-pre-wrap
- **Word Break:** break-normal, break-words, break-all

## Image Styling
- **Object Fit:** `object-contain`, `object-cover`, `object-fill`, `object-none`, `object-scale-down`
- **Object Position:** `object-center`, `object-top`, `object-bottom`, `object-left`, `object-right`, `object-left-top`, `object-left-bottom`, `object-right-top`, `object-right-bottom`
- **Image Rendering:** `antialiased`, `subpixel-antialiased`

## Size/Dimension (width, height, min/max)
- **Width:** w-1/2, w-1/3, w-full, w-min, w-max, w-fit, w-screen, w-[custom_value]
- **Height:** h-1/2, h-full, h-screen
- **Max/Min:** max-w-lg, min-h-screen, min-h-0,max-h-full

## Spacing (Margin & Padding)
- **Margin:** mx-{n}, my-{n}, mt-{n}, mr-{n}, mb-{n}, ml-{n}, m-{n}, negative: -m-{n}, m(t/b/l/r)-[custom_value]
- **Padding:** px-{n}, py-{n}, pt-{n}, pr-{n}, pb-{n}, pl-{n}, p-{n},  p(t/b/l/r)-[custom_value]
- **Scale values:** 0, 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4, 5, 6, 8, 10, 12, 16, 20, 24, 28, 32, 36, 40, 44, 48, 52, 56, 60, 64, 72, 80, 96

## Border
- **Border Width:** border, border-0, border-2, border-4, border-8
- **Sides:** border-t, border-b, border-l, border-r
- **Color:** border-{color}-{shade}
- **Style:** border-solid, dashed, dotted, double, none

## Border Radius
- rounded-none, sm, md, lg, xl

## Display
- block, inline-block, inline, flex, inline-flex, grid, inline-grid, table, hidden, contents.
- **position:**  static, relative, absolute, fixed, sticky
- **Inset:** top-0, right-0, bottom-0, left-0, inset-0, inset-x-0, inset-y-0
- **Z-Index:** z-0 ... z-50, z-auto

## Flexbox 
- flex, inline-flex
- **direction:** flex-row,flex-col
- **wrap:** flex-wrap, flex-wrap-reverse, flex-nowrap
- **Justify Content:** justify-start, justify-center, justify-between, justify-end, justify-around, justify-evenly
- **Align Items:** items-start, items-center, items-end, items-baseline, items-stretch
- **Align Self:** self-auto, self-start, self-center, self-end, self-stretch
- **Align Content:** content-start, content-center, content-end, content-between, content-around, content-evenly
- **Gap:** gap-1, gap-2, gap-4, gap-[custom_value]
- **Grow & Shrink:** flex-grow, flex-grow-0, flex-shrink, flex-shrink-0
- **Order:** order-1, order-2, order-last, etc.

## Grid
- grid, inline-grid
- **Columns:** grid-cols-1, grid-cols-2, grid-cols-3, ..., grid-cols-12, grid-cols-[custom_value]
- **Rows:** grid-rows-1, grid-rows-2, grid-rows-3, ..., grid-rows-[custom_value]
- **grid-cols-[repeat(auto-fit,_minmax(250px,_1fr))]:**   For Auto-fit responsive card structure
- **Gap:** gap-1, gap-2, gap-4, gap-[custom_value]
- **Column Gap:** gap-x-1, gap-x-2, gap-x-4, gap-x-[custom_value]
- **Row Gap:** gap-y-1, gap-y-2, gap-y-4, gap-y-[custom_value]
- **Span:** col-span-1, col-span-2, ..., row-span-1, row-span-2
- **Start / End:** col-start-1, col-start-2, col-end-3, row-start-1, row-end-3
- **Auto Flow:** grid-flow-row, grid-flow-col, grid-flow-row-dense, grid-flow-col-dense
- **Justify Content:** justify-start, justify-center, justify-end, justify-between, justify-around, justify-evenly
- **Align Items:** items-start, items-center, items-end, items-stretch
- **Justify Items:** justify-items-start, justify-items-center, justify-items-end, justify-items-stretch
- **Place Content:** place-content-center, place-content-start, place-content-end, place-content-between, place-content-around, place-content-evenly
- **Place Items:** place-items-start, place-items-center, place-items-end, place-items-stretch

  #### Example1: Responsive 3-Column Grid
```html
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 p-4">
  <div class="bg-blue-200 p-4 rounded-lg text-center">Grid Item 1</div>
  <div class="bg-blue-300 p-4 rounded-lg text-center">Grid Item 2</div>
  <div class="bg-blue-400 p-4 rounded-lg text-center">Grid Item 3</div>
</div>
```
  #### Example2: Full Responsive Auto Sized Card layout
```html
<div class="grid grid-cols-[repeat(auto-fit,_minmax(250px,_1fr))] gap-6 p-4">
  <div class="bg-blue-200 p-6 rounded-lg text-center">Card 1</div>
  <div class="bg-blue-300 p-6 rounded-lg text-center">Card 2</div>
  <div class="bg-blue-400 p-6 rounded-lg text-center">Card 3</div>
  <div class="bg-blue-500 p-6 rounded-lg text-center">Card 4</div>
</div>

```

## Box Shadow
- shadow-xs, sm, md, lg, xl, 2xl, inner, none. shadow-[custom_value_seprated with underscores]
- shadow-{color}
  #### Example
```html
<div class="shadow-[2px_2px_4px_grey,_-1px_-1px_4px_grey] p-6 rounded-lg">
  Custom shadow example
</div>
```

## Transition
- transition, \ transition-all, transition-colors, transition-opacity, transition-shadow, transition-transform, transition-[properties]
- **Duration:** duration-75 ... duration-1000
- **Timing:** ease-linear, ease-in, ease-out, ease-in-out
- **Delay:** delay-75 ... delay-300

## Transform (2D & 3D)

- transform
- **Scale:** scale-0, scale-50, scale-75, scale-90, scale-95, scale-100, scale-105, scale-110, scale-125, scale-150, scale-[custom_value]
- **Rotate:** rotate-0, rotate-1, rotate-2, ..., rotate-45, rotate-90, rotate-180, rotate-[custom_value]
- **Translate (Move):**
  - **X-axis:** translate-x-0, translate-x-1, translate-x-2, ..., translate-x-full, translate-x-[custom_value]
  - **Y-axis:** translate-y-0, translate-y-1, translate-y-2, ..., translate-y-full, translate-y-[custom_value]
- **Skew (Tilt):**
  - **X-axis:** skew-x-0, skew-x-1, ..., skew-x-12, skew-x-[custom_value]
  - **Y-axis:** skew-y-0, skew-y-1, ..., skew-y-12, skew-y-[custom_value]
- **Origin (Transform Origin):** origin-center, origin-top, origin-top-right, origin-right, origin-bottom-right, origin-bottom, origin-bottom-left, origin-left, origin-top-left
- **Perspective (3D Depth):** perspective-[custom_value]
- **3D Rotate:**
  - rotate-x-[deg], rotate-y-[deg], rotate-z-[deg]
- **Preserve 3D (for nested transforms):** transform-style-preserve-3d
- **Backface Visibility:** backface-visible, backface-hidden


## Hover and Other Pseudo Classes

- **Hover:** hover:
- **Focus:** focus:
- **Active:** active:
- **Visited:** visited:
- **Checked:** checked:
- **Disabled:** disabled:
- **First Child:** first:
- **Last Child:** last:
- **[&:nth-child(number)]:**
- **[&:has(selector)]:**
- **Odd / Even Elements:** odd:, even:
- **Group Hover (Parent Hover):** group-hover:
- **Peer Hover (Sibling Hover):** peer-hover:
- **Focus Within:** focus-within:
- **Focus Visible:** focus-visible:
- **Target:** target:
- **Placeholder Text:** placeholder:
- **Selection:** selection:
- **File Selector Button:** file:
- **First Letter / Line:** first-letter:, first-line:
- **Marker (List):** marker:
- **In Range / Out of Range:** in-range:, out-of-range:
- **Read Only / Read Write:** read-only:, read-write:
- **Required / Optional:** required:, optional:
- **Motion Safe / Reduce:** motion-safe:, motion-reduce:
- **Dark Mode:** dark:
- **RTL / LTR Support:** rtl:, ltr:

## After and Before
- before: , after:
- before/after:content-['value']
- before/after:h-[size_value]
- before/after:w-[size_value]
- before/after:absolute
- before/after:top-{value}
- before/after:left-{value}
- before/after:bottom-{value}
- before/after:right-{value}

## Animations
- animate-none
- animate-spin
- animate-ping
- animate-pulse
- animate-bounce
- animate-[custom_value_seprated_by_underscores]

#### Example of custom animate
```html
<div class="w-20 h-20 bg-purple-500 animate-[keyframe_name_1s_ease-in-out_infinite]"></div>
```
  

  












