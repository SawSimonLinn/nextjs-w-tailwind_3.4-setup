# Next.js with Tailwindss--version.3.4-setup

<hr/>

## 🔧 Step 1: Create a New Next.js App

```bash
npx create-next-app@latest ./
```

## 💅 Step 2: Install Tailwind CSS v3.4

```bash
npm install -D tailwindcss@3.4 postcss autoprefixer
npx tailwindcss init -p
```

## 📦 Step 3: Configure Tailwind

In **tailwind.config.js**, update like this:

```bash
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./pages/**/*.{js,ts,jsx,tsx}",
    "./components/**/*.{js,ts,jsx,tsx}",
    "./app/**/*.{js,ts,jsx,tsx}", // If you're using the App Router
  ],
  theme: {
    extend: {
      colors: {
        background: "var(---background)",
        foreground: "var(--foreground)",
      },
    },
  },
  plugins: [],
}
```

## 💖 Step 4: Add Tailwind to Your CSS

In **./styles/globals.css**, replace everything with:

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## 🚀 Step 5: Run the App

```bash
npm run dev
```

## It's me SIMON.
