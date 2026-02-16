# 🎯 TAILWIND CSS PRACTICE EXERCISES

Complete these exercises to master Tailwind CSS! Each exercise builds on the previous one.

---

## 📚 EXERCISE 1: Basic Layout (10 minutes)

### Task

Create a simple centered card with:

- White background
- Rounded corners
- Shadow
- Padding
- Centered text

### Expected Result

```html
<!-- Write your code here -->
<div class="flex items-center justify-center min-h-screen bg-gray-100">
  <!-- Your card here -->
</div>
```

### Solution (Don't peek until you try!)

<details>
<summary>Click to reveal</summary>

```html
<div class="flex items-center justify-center min-h-screen bg-gray-100">
  <div class="bg-white rounded-lg shadow-md p-8 text-center">
    <h2 class="text-2xl font-bold mb-4">My Card</h2>
    <p class="text-gray-600">This is a simple card</p>
  </div>
</div>
```

</details>

---

## 🎨 EXERCISE 2: Button Styles (15 minutes)

### Task

Create 4 different button styles:

1. Primary button (blue background, white text, hover effect)
2. Secondary button (gray background)
3. Outline button (transparent with border)
4. Danger button (red, with active state)

### Starter Code

```html
<div class="flex gap-4 p-8">
  <!-- Button 1: Primary -->
  <button class="">Primary</button>

  <!-- Button 2: Secondary -->
  <button class="">Secondary</button>

  <!-- Button 3: Outline -->
  <button class="">Outline</button>

  <!-- Button 4: Danger -->
  <button class="">Danger</button>
</div>
```

### Solution

<details>
<summary>Click to reveal</summary>

```html
<div class="flex gap-4 p-8">
  <!-- Primary -->
  <button
    class="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 px-6 rounded-lg transition"
  >
    Primary
  </button>

  <!-- Secondary -->
  <button
    class="bg-gray-200 hover:bg-gray-300 text-gray-800 font-semibold py-2 px-6 rounded-lg transition"
  >
    Secondary
  </button>

  <!-- Outline -->
  <button
    class="border-2 border-blue-500 text-blue-500 hover:bg-blue-500 hover:text-white font-semibold py-2 px-6 rounded-lg transition"
  >
    Outline
  </button>

  <!-- Danger -->
  <button
    class="bg-red-500 hover:bg-red-600 active:bg-red-700 text-white font-semibold py-2 px-6 rounded-lg transition"
  >
    Danger
  </button>
</div>
```

</details>

---

## 📱 EXERCISE 3: Responsive Navbar (20 minutes)

### Task

Create a responsive navbar that:

- Has logo on left, links in center, button on right (desktop)
- Stacks vertically on mobile
- Has hover effects
- Sticky to top

### Starter Code

```html
<nav class="">
  <h1>Logo</h1>
  <div>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </div>
  <button>Sign In</button>
</nav>
```

### Solution

<details>
<summary>Click to reveal</summary>

```html
<nav
  class="sticky top-0 bg-white shadow-md px-6 py-4 flex flex-col md:flex-row items-center justify-between gap-4 z-50"
>
  <h1 class="text-2xl font-bold text-blue-600">Logo</h1>

  <div class="flex flex-col md:flex-row gap-4 md:gap-6">
    <a href="#" class="text-gray-700 hover:text-blue-600 transition font-medium"
      >Home</a
    >
    <a href="#" class="text-gray-700 hover:text-blue-600 transition font-medium"
      >About</a
    >
    <a href="#" class="text-gray-700 hover:text-blue-600 transition font-medium"
      >Contact</a
    >
  </div>

  <button
    class="bg-blue-500 hover:bg-blue-600 text-white font-semibold px-6 py-2 rounded-lg transition"
  >
    Sign In
  </button>
</nav>
```

</details>

---

## 🎴 EXERCISE 4: Card Grid (25 minutes)

### Task

Create a responsive card grid that shows:

- 1 column on mobile
- 2 columns on tablet
- 3 columns on desktop
- Each card has image, title, description, and button
- Hover effect on cards

### Starter Code

```html
<div class="">
  <!-- Card 1 -->
  <div class="">
    <img src="https://via.placeholder.com/400x300" alt="Card 1" />
    <h3>Card Title 1</h3>
    <p>Description here</p>
    <button>Learn More</button>
  </div>

  <!-- Card 2 -->
  <!-- Card 3 -->
  <!-- Add more cards -->
</div>
```

### Solution

<details>
<summary>Click to reveal</summary>

```html
<div
  class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 p-6 bg-gray-100"
>
  <!-- Card 1 -->
  <div
    class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-xl hover:scale-105 transition duration-300"
  >
    <img
      src="https://via.placeholder.com/400x300"
      alt="Card 1"
      class="w-full h-48 object-cover"
    />
    <div class="p-6">
      <h3 class="text-xl font-bold text-gray-800 mb-2">Card Title 1</h3>
      <p class="text-gray-600 mb-4">
        This is a description of the card content.
      </p>
      <button
        class="bg-blue-500 hover:bg-blue-600 text-white font-semibold px-4 py-2 rounded transition"
      >
        Learn More
      </button>
    </div>
  </div>

  <!-- Card 2 -->
  <div
    class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-xl hover:scale-105 transition duration-300"
  >
    <img
      src="https://via.placeholder.com/400x300"
      alt="Card 2"
      class="w-full h-48 object-cover"
    />
    <div class="p-6">
      <h3 class="text-xl font-bold text-gray-800 mb-2">Card Title 2</h3>
      <p class="text-gray-600 mb-4">
        This is a description of the card content.
      </p>
      <button
        class="bg-blue-500 hover:bg-blue-600 text-white font-semibold px-4 py-2 rounded transition"
      >
        Learn More
      </button>
    </div>
  </div>

  <!-- Card 3 -->
  <div
    class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-xl hover:scale-105 transition duration-300"
  >
    <img
      src="https://via.placeholder.com/400x300"
      alt="Card 3"
      class="w-full h-48 object-cover"
    />
    <div class="p-6">
      <h3 class="text-xl font-bold text-gray-800 mb-2">Card Title 3</h3>
      <p class="text-gray-600 mb-4">
        This is a description of the card content.
      </p>
      <button
        class="bg-blue-500 hover:bg-blue-600 text-white font-semibold px-4 py-2 rounded transition"
      >
        Learn More
      </button>
    </div>
  </div>
</div>
```

</details>

---

## 🖼️ EXERCISE 5: Profile Card (30 minutes)

### Task

Recreate a LinkedIn-style profile card with:

- Banner image at top
- Profile picture overlapping banner (centered)
- Name and bio
- Stats (connections, views, etc.)
- Hover effects

### Solution

<details>
<summary>Click to reveal</summary>

```html
<div
  class="max-w-sm mx-auto bg-white rounded-xl shadow-md overflow-hidden hover:shadow-2xl transition"
>
  <!-- Banner & Profile Picture -->
  <div class="relative">
    <img
      src="https://via.placeholder.com/400x150"
      alt="Banner"
      class="w-full h-24 object-cover"
    />
    <img
      src="https://via.placeholder.com/100"
      alt="Profile"
      class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-20 h-20 rounded-full border-4 border-white"
    />
  </div>

  <!-- Info Section -->
  <div class="pt-12 px-6 pb-6 text-center">
    <h2 class="text-xl font-bold text-gray-800">John Doe</h2>
    <p class="text-gray-600 text-sm mb-4">Software Engineer | Web Developer</p>
    <p class="text-gray-500 text-xs mb-6">Building amazing web experiences</p>

    <!-- Stats -->
    <div class="flex justify-around border-t border-gray-200 pt-4">
      <div class="text-center">
        <p class="text-2xl font-bold text-blue-600">500+</p>
        <p class="text-xs text-gray-500">Connections</p>
      </div>
      <div class="text-center">
        <p class="text-2xl font-bold text-blue-600">1.2K</p>
        <p class="text-xs text-gray-500">Views</p>
      </div>
      <div class="text-center">
        <p class="text-2xl font-bold text-blue-600">42</p>
        <p class="text-xs text-gray-500">Posts</p>
      </div>
    </div>

    <!-- Button -->
    <button
      class="mt-6 w-full bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 rounded-lg transition"
    >
      Connect
    </button>
  </div>
</div>
```

</details>

---

## 🎨 EXERCISE 6: Image Overlay (20 minutes)

### Task

Create an image with text overlay that appears on hover:

- Image takes full container
- Dark overlay appears on hover
- Text fades in from bottom
- Smooth transitions

### Solution

<details>
<summary>Click to reveal</summary>

```html
<div
  class="relative max-w-md mx-auto overflow-hidden rounded-lg group cursor-pointer"
>
  <!-- Image -->
  <img
    src="https://via.placeholder.com/600x400"
    alt="Image"
    class="w-full h-64 object-cover transition duration-300 group-hover:scale-110"
  />

  <!-- Overlay (hidden by default, appears on hover) -->
  <div
    class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end"
  >
    <div
      class="p-6 transform translate-y-4 group-hover:translate-y-0 transition duration-300"
    >
      <h3 class="text-white text-2xl font-bold mb-2">Image Title</h3>
      <p class="text-gray-200 text-sm">
        Beautiful image description that appears on hover
      </p>
    </div>
  </div>
</div>
```

</details>

---

## 📋 EXERCISE 7: Form Styling (35 minutes)

### Task

Create a beautiful signup form with:

- Input fields with labels
- Focus states (ring effect)
- Validation states (error styling)
- Submit button
- Responsive design

### Solution

<details>
<summary>Click to reveal</summary>

```html
<div
  class="min-h-screen flex items-center justify-center bg-gradient-to-br from-blue-500 to-purple-600 p-6"
>
  <div class="bg-white rounded-2xl shadow-2xl p-8 max-w-md w-full">
    <h2 class="text-3xl font-bold text-gray-800 mb-2 text-center">
      Create Account
    </h2>
    <p class="text-gray-600 text-center mb-8">Sign up to get started</p>

    <form class="space-y-6">
      <!-- Full Name -->
      <div>
        <label class="block text-gray-700 font-semibold mb-2 text-sm"
          >Full Name</label
        >
        <input
          type="text"
          class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition"
          placeholder="John Doe"
        />
      </div>

      <!-- Email -->
      <div>
        <label class="block text-gray-700 font-semibold mb-2 text-sm"
          >Email</label
        >
        <input
          type="email"
          class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition"
          placeholder="you@example.com"
        />
      </div>

      <!-- Password -->
      <div>
        <label class="block text-gray-700 font-semibold mb-2 text-sm"
          >Password</label
        >
        <input
          type="password"
          class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition"
          placeholder="••••••••"
        />
        <p class="text-xs text-gray-500 mt-1">Must be at least 8 characters</p>
      </div>

      <!-- Error Example -->
      <div>
        <label class="block text-gray-700 font-semibold mb-2 text-sm"
          >Confirm Password</label
        >
        <input
          type="password"
          class="w-full px-4 py-3 border-2 border-red-500 rounded-lg focus:outline-none focus:ring-2 focus:ring-red-500 bg-red-50"
          placeholder="••••••••"
        />
        <p class="text-xs text-red-500 mt-1 flex items-center gap-1">
          <i class="fas fa-exclamation-circle"></i>
          Passwords do not match
        </p>
      </div>

      <!-- Checkbox -->
      <div class="flex items-center gap-2">
        <input
          type="checkbox"
          id="terms"
          class="w-4 h-4 text-blue-500 rounded focus:ring-2 focus:ring-blue-500"
        />
        <label for="terms" class="text-sm text-gray-700">
          I agree to the
          <a href="#" class="text-blue-500 hover:underline"
            >Terms & Conditions</a
          >
        </label>
      </div>

      <!-- Submit Button -->
      <button
        type="submit"
        class="w-full bg-gradient-to-r from-blue-500 to-purple-600 hover:from-blue-600 hover:to-purple-700 text-white font-bold py-3 rounded-lg transition transform hover:scale-105 active:scale-95 shadow-lg"
      >
        Sign Up
      </button>

      <!-- Divider -->
      <div class="relative">
        <div class="absolute inset-0 flex items-center">
          <div class="w-full border-t border-gray-300"></div>
        </div>
        <div class="relative flex justify-center text-sm">
          <span class="px-2 bg-white text-gray-500">Or continue with</span>
        </div>
      </div>

      <!-- Social Buttons -->
      <div class="grid grid-cols-2 gap-4">
        <button
          class="flex items-center justify-center gap-2 border border-gray-300 hover:border-gray-400 rounded-lg py-2.5 transition hover:bg-gray-50"
        >
          <i class="fab fa-google text-red-500"></i>
          <span class="text-sm font-semibold text-gray-700">Google</span>
        </button>
        <button
          class="flex items-center justify-center gap-2 border border-gray-300 hover:border-gray-400 rounded-lg py-2.5 transition hover:bg-gray-50"
        >
          <i class="fab fa-github text-gray-800"></i>
          <span class="text-sm font-semibold text-gray-700">GitHub</span>
        </button>
      </div>

      <!-- Footer -->
      <p class="text-center text-sm text-gray-600">
        Already have an account?
        <a href="#" class="text-blue-500 hover:underline font-semibold"
          >Sign In</a
        >
      </p>
    </form>
  </div>
</div>
```

</details>

---

## 🏆 EXERCISE 8: Dashboard Sidebar (40 minutes)

### Task

Create your dashboard's left sidebar with:

- Banner and profile picture overlap
- Profile info section
- Stats with hover effects
- Multiple sections with icons
- Responsive design

This is similar to YOUR actual dashboard project!

### Solution

<details>
<summary>Click to reveal</summary>

```html
<aside class="w-full max-w-xs bg-white rounded-xl shadow-lg overflow-hidden">
  <!-- Banner & Profile -->
  <div class="relative">
    <div class="h-24 bg-gradient-to-r from-blue-500 to-purple-500"></div>
    <img
      src="https://via.placeholder.com/100"
      alt="Profile"
      class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-20 h-20 rounded-full border-4 border-white shadow-lg"
    />
  </div>

  <!-- Profile Info -->
  <div class="pt-12 px-6 pb-4 text-center space-y-3">
    <h2 class="text-xl font-bold text-gray-800">Kalisa Felix</h2>
    <div class="flex items-center justify-center gap-2 text-sm text-gray-600">
      <i class="fa-solid fa-message text-blue-500"></i>
      <span>Frontend Developer</span>
    </div>
    <a href="#" class="text-blue-500 text-sm hover:underline inline-block">
      add headline
    </a>
  </div>

  <!-- Stats -->
  <div class="px-4 py-4 border-t border-gray-200 space-y-2">
    <div
      class="flex items-center justify-between hover:bg-gray-50 px-3 py-2.5 rounded-lg transition cursor-pointer group"
    >
      <div class="flex items-center gap-3">
        <i
          class="fa-solid fa-eye text-blue-500 group-hover:scale-110 transition"
        ></i>
        <span class="text-sm text-gray-700">Profile Viewers</span>
      </div>
      <span
        class="text-sm font-bold text-gray-900 bg-gray-100 px-2.5 py-1 rounded-full group-hover:bg-blue-500 group-hover:text-white transition"
        >68</span
      >
    </div>

    <div
      class="flex items-center justify-between hover:bg-gray-50 px-3 py-2.5 rounded-lg transition cursor-pointer group"
    >
      <div class="flex items-center gap-3">
        <i
          class="fa-solid fa-briefcase text-blue-500 group-hover:scale-110 transition"
        ></i>
        <span class="text-sm text-gray-700">Job Applications</span>
      </div>
      <span
        class="text-sm font-bold text-gray-900 bg-gray-100 px-2.5 py-1 rounded-full group-hover:bg-blue-500 group-hover:text-white transition"
        >13</span
      >
    </div>
  </div>

  <!-- Company Section -->
  <div class="px-4 py-4 border-t border-gray-200 space-y-3">
    <h3 class="text-base font-bold text-gray-800 text-left">Company Page</h3>

    <div
      class="flex items-center gap-3 text-sm hover:bg-gray-50 px-3 py-2 rounded-lg transition cursor-pointer group"
    >
      <i
        class="fa-solid fa-building text-blue-500 group-hover:scale-110 transition"
      ></i>
      <span class="text-gray-700">Create Page</span>
    </div>
  </div>
</aside>
```

</details>

---

## 🎯 CHALLENGE EXERCISE: Complete Dashboard (2+ hours)

### Final Challenge

Combine everything you've learned to recreate YOUR ENTIRE dashboard:

1. Sticky header with navigation
2. Three-column grid layout (responsive)
3. Left sidebar (profile section)
4. Main feed area with posts
5. Right sidebar (news/updates)
6. All with hover effects and transitions

**Hint**: Use `index-tailwind.html` as reference, but try to build it yourself first!

---

## 📊 PROGRESS TRACKER

Track your completion:

- [ ] Exercise 1: Basic Layout
- [ ] Exercise 2: Button Styles
- [ ] Exercise 3: Responsive Navbar
- [ ] Exercise 4: Card Grid
- [ ] Exercise 5: Profile Card
- [ ] Exercise 6: Image Overlay
- [ ] Exercise 7: Form Styling
- [ ] Exercise 8: Dashboard Sidebar
- [ ] Challenge: Complete Dashboard

---

## 💡 TIPS FOR PRACTICE

1. **Don't Peek Too Early**: Try for at least 10 minutes before looking at solution
2. **Experiment**: Change colors, sizes, add your own twist
3. **Break It Down**: If stuck, break the design into smaller pieces
4. **Use DevTools**: Inspect the solutions to understand structure
5. **Rebuild from Memory**: After seeing solution, rebuild without looking
6. **Customize**: Make it your own with different styles

---

## 🎓 LEARNING STRATEGY

### For Each Exercise:

1. ✅ Read the requirements carefully
2. ✅ Plan your approach (which classes you'll need)
3. ✅ Build incrementally (layout → spacing → colors → effects)
4. ✅ Test responsiveness
5. ✅ Compare with solution
6. ✅ Rebuild from scratch for practice

---

## 🚀 NEXT STEPS

After completing these exercises:

1. Convert your original `index.html` to Tailwind
2. Add new features to your dashboard
3. Build a completely new project from scratch
4. Explore Tailwind plugins and advanced features

**You've got this!** 💪 Each exercise makes you stronger!
