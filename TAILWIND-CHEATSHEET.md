# 🎯 TAILWIND CSS QUICK REFERENCE CHEATSHEET

## ⚡ INSTANT SETUP

```html
<!-- Add to <head> -->
<script src="https://cdn.tailwindcss.com"></script>
<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          primary: "#E8422F",
          accent: "#2D9CDB",
        },
      },
    },
  };
</script>
```

---

## 📐 LAYOUT

### Display

```
block           display: block
inline          display: inline
inline-block    display: inline-block
flex            display: flex
inline-flex     display: inline-flex
grid            display: grid
hidden          display: none
```

### Container

```
container       max-width: 100% at each breakpoint
mx-auto         margin: 0 auto (center)
```

---

## 📦 FLEXBOX

### Flex Direction

```
flex-row        flex-direction: row
flex-col        flex-direction: column
flex-row-reverse
flex-col-reverse
```

### Justify Content (Main Axis)

```
justify-start       justify-content: flex-start
justify-center      justify-content: center
justify-end         justify-content: flex-end
justify-between     justify-content: space-between
justify-around      justify-content: space-around
justify-evenly      justify-content: space-evenly
```

### Align Items (Cross Axis)

```
items-start     align-items: flex-start
items-center    align-items: center
items-end       align-items: flex-end
items-stretch   align-items: stretch
items-baseline  align-items: baseline
```

### Gap

```
gap-0   0
gap-1   0.25rem (4px)
gap-2   0.5rem (8px)
gap-3   0.75rem (12px)
gap-4   1rem (16px)
gap-6   1.5rem (24px)
gap-8   2rem (32px)
```

---

## 🎨 GRID

### Grid Columns

```
grid-cols-1     1 column
grid-cols-2     2 columns
grid-cols-3     3 columns
grid-cols-4     4 columns
grid-cols-12    12 columns (for complex layouts)

Custom: grid-cols-[250px_1fr_380px]
```

### Column Span

```
col-span-1      span 1 column
col-span-2      span 2 columns
col-span-full   span all columns
```

---

## 📏 SPACING

### Padding

```
p-0     0
p-1     0.25rem (4px)
p-2     0.5rem (8px)
p-3     0.75rem (12px)
p-4     1rem (16px)
p-5     1.25rem (20px)
p-6     1.5rem (24px)
p-8     2rem (32px)

px-4    horizontal padding
py-4    vertical padding
pt-4    padding-top
pr-4    padding-right
pb-4    padding-bottom
pl-4    padding-left
```

### Margin (Same as Padding)

```
m-4     margin
mx-4    horizontal margin
my-4    vertical margin
mx-auto  center horizontally

-m-4    negative margin
```

---

## 📐 SIZING

### Width

```
w-0         0
w-full      100%
w-screen    100vw
w-auto      auto
w-1/2       50%
w-1/3       33.333%
w-2/3       66.666%
w-1/4       25%
w-3/4       75%

w-4         1rem (16px)
w-8         2rem (32px)
w-16        4rem (64px)
w-64        16rem (256px)
```

### Max Width

```
max-w-xs    20rem (320px)
max-w-sm    24rem (384px)
max-w-md    28rem (448px)
max-w-lg    32rem (512px)
max-w-xl    36rem (576px)
max-w-2xl   42rem (672px)
max-w-7xl   80rem (1280px)
max-w-full  100%
```

### Height

```
h-full      100%
h-screen    100vh
h-4         1rem
h-64        16rem
min-h-screen  min-height: 100vh
```

---

## 🎨 COLORS

### Text Color

```
text-white
text-black
text-gray-500
text-blue-500
text-red-500
text-green-500

text-[#E8422F]  custom hex
```

### Background Color

```
bg-white
bg-black
bg-gray-100
bg-blue-500
bg-red-500

bg-blue-500/50  50% opacity
```

### Gradient

```
bg-gradient-to-r    left to right
bg-gradient-to-b    top to bottom
bg-gradient-to-br   bottom-right diagonal

from-blue-500       start color
via-purple-500      middle color
to-pink-500         end color

Example:
bg-gradient-to-r from-blue-500 to-purple-500
```

---

## ✍️ TYPOGRAPHY

### Font Size

```
text-xs     0.75rem (12px)
text-sm     0.875rem (14px)
text-base   1rem (16px)
text-lg     1.125rem (18px)
text-xl     1.25rem (20px)
text-2xl    1.5rem (24px)
text-3xl    1.875rem (30px)
text-4xl    2.25rem (36px)
```

### Font Weight

```
font-thin       100
font-light      300
font-normal     400
font-medium     500
font-semibold   600
font-bold       700
font-black      900
```

### Text Align

```
text-left
text-center
text-right
text-justify
```

### Text Transform

```
uppercase       UPPERCASE
lowercase       lowercase
capitalize      Capitalize Each Word
```

### Line Height

```
leading-tight   1.25
leading-normal  1.5
leading-relaxed 1.625
leading-loose   2
```

---

## 🎯 BORDERS

### Border Width

```
border          1px
border-2        2px
border-4        4px
border-t        top
border-r        right
border-b        bottom
border-l        left
```

### Border Radius

```
rounded-none    0
rounded         0.25rem
rounded-md      0.375rem
rounded-lg      0.5rem
rounded-xl      0.75rem
rounded-2xl     1rem
rounded-full    9999px (circle)

rounded-t-lg    top corners
rounded-tl-lg   top-left corner
```

### Border Color

```
border-gray-300
border-blue-500
border-[#E8422F]
```

---

## ✨ EFFECTS

### Shadow

```
shadow-sm       small
shadow          default
shadow-md       medium
shadow-lg       large
shadow-xl       extra large
shadow-2xl      2xl
shadow-none     none
```

### Opacity

```
opacity-0       0%
opacity-25      25%
opacity-50      50%
opacity-75      75%
opacity-100     100%
```

### Ring (Outline)

```
ring-2          2px ring
ring-4          4px ring
ring-blue-500   color
ring-offset-2   offset
```

---

## 🎭 POSITIONING

### Position

```
static          default
relative        relative positioning
absolute        absolute positioning
fixed           fixed positioning
sticky          sticky positioning
```

### Top/Right/Bottom/Left

```
top-0
right-0
bottom-0
left-0

top-1/2         50%
left-1/2        50%

-translate-x-1/2  -50% transform (centering)
-translate-y-1/2  -50% transform (centering)
```

### Z-Index

```
z-0
z-10
z-20
z-50
```

---

## 🎬 TRANSITIONS & ANIMATIONS

### Transitions

```
transition              all properties
transition-colors       colors only
transition-transform    transform only
transition-opacity      opacity only

duration-150    150ms
duration-300    300ms
duration-500    500ms

ease-in
ease-out
ease-in-out
```

### Transform

```
scale-0         0%
scale-100       100%
scale-110       110%

rotate-45       45deg
rotate-90       90deg
rotate-180      180deg

hover:scale-110 hover effect
```

### Animations

```
animate-spin
animate-ping
animate-pulse
animate-bounce
```

---

## 📱 RESPONSIVE

### Breakpoints

```
sm:     640px and up
md:     768px and up
lg:     1024px and up
xl:     1280px and up
2xl:    1536px and up
```

### Usage

```html
<!-- Mobile first approach -->
<div class="text-sm md:text-base lg:text-lg">Responsive text</div>

<div class="hidden md:block">Visible on tablet+</div>

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3">
  Responsive grid
</div>
```

---

## 🎯 STATE VARIANTS

### Hover

```
hover:bg-blue-600
hover:text-white
hover:scale-110
hover:shadow-lg
```

### Focus

```
focus:outline-none
focus:ring-2
focus:ring-blue-500
focus:border-blue-500
```

### Active

```
active:bg-blue-700
active:scale-95
```

### Disabled

```
disabled:opacity-50
disabled:cursor-not-allowed
```

### Group Hover

```html
<div class="group">
  <img class="group-hover:scale-110" />
  <p class="group-hover:text-blue-500">Hover parent</p>
</div>
```

---

## 🎨 COMMON PATTERNS

### Center Everything

```html
<div class="flex items-center justify-center min-h-screen">Centered</div>
```

### Card

```html
<div class="bg-white rounded-lg shadow-md p-6 hover:shadow-xl transition">
  Card content
</div>
```

### Button

```html
<button
  class="bg-blue-500 hover:bg-blue-600 active:bg-blue-700 text-white font-bold py-2 px-6 rounded-lg transition focus:outline-none focus:ring-4 focus:ring-blue-300"
>
  Button
</button>
```

### Input

```html
<input
  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent"
  type="text"
/>
```

### Badge

```html
<span
  class="bg-blue-100 text-blue-800 text-xs font-semibold px-2.5 py-0.5 rounded-full"
>
  Badge
</span>
```

### Avatar

```html
<img
  class="w-10 h-10 rounded-full ring-2 ring-blue-500 ring-offset-2"
  src="avatar.jpg"
/>
```

### Overlay

```html
<div class="relative">
  <img src="image.jpg" class="w-full" />
  <div class="absolute inset-0 bg-black/50 flex items-center justify-center">
    <h2 class="text-white text-3xl">Overlay</h2>
  </div>
</div>
```

---

## 💡 PRO TIPS

1. **Spacing Scale**: Remember 4px multiplier (4, 8, 12, 16, 20, 24...)
2. **Mobile First**: Start with mobile, add larger breakpoints
3. **Always Add Transition**: `transition` class for smooth interactions
4. **Use Gap**: Instead of margins between flex/grid items
5. **Group Classes**: Layout → Spacing → Typography → Visual → States
6. **Custom Values**: Use `[value]` for one-offs: `w-[137px]`
7. **Ring > Border**: For focus states, use `ring` instead of `border`
8. **Arbitrary Values**: `bg-[#E8422F]` for custom colors

---

## 🔥 YOUR DASHBOARD SPECIFIC

### Custom Colors

```html
<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          primary: "#E8422F",
          accent: "#2D9CDB",
          bgLight: "#E1F5FE",
        },
      },
    },
  };
</script>

<!-- Usage -->
<header class="bg-primary">
  <i class="text-accent"> <body class="bg-bgLight"></body></i>
</header>
```

### Dashboard Grid

```html
<main
  class="grid grid-cols-1 lg:grid-cols-[280px_1fr_380px] gap-6 max-w-7xl mx-auto p-5"
>
  <aside>Left</aside>
  <section>Center</section>
  <aside>Right</aside>
</main>
```

---

## 🚀 SPEED HACKS

### Class Organization

```html
<div
  class="
    /* Layout */
    flex items-center justify-between
    
    /* Spacing */
    p-4 gap-4
    
    /* Typography */
    text-lg font-bold
    
    /* Visual */
    bg-white rounded-lg shadow-md
    
    /* States */
    hover:shadow-xl transition"
></div>
```

### Common Combos

```
flex items-center justify-between    Navbar
flex flex-col items-center gap-4     Vertical center stack
grid grid-cols-3 gap-6               Three column grid
max-w-7xl mx-auto                    Centered container
hover:scale-105 transition           Hover zoom
focus:ring-2 focus:ring-blue-500     Focus ring
```

---

## ⚡ SHORTCUTS FOR YOUR CLASS

```html
<!-- Header -->
bg-primary flex items-center justify-between p-5 text-white

<!-- Card -->
bg-white rounded-lg shadow-md p-6 hover:shadow-xl transition

<!-- Stat Item -->
flex items-center justify-between hover:bg-gray-50 px-3 py-2 rounded-lg
transition cursor-pointer

<!-- Icon -->
text-accent hover:scale-110 transition

<!-- Badge -->
bg-gray-100 px-2.5 py-1 rounded-full text-xs font-bold

<!-- Grid Layout -->
grid grid-cols-1 lg:grid-cols-[280px_1fr_380px] gap-6 max-w-7xl mx-auto p-5
```

---

**Print this out or keep it handy while coding!** 📌

**Remember**: The more you use Tailwind, the faster you'll memorize these classes. Start with this cheatsheet and soon you won't need it! 💪
