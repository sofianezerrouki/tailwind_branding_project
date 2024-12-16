# Tailwind Branding Project

A simple branding project built using Tailwind CSS. Follow the steps below to set up and run the project.

---

## Installation and Setup

### 1. Install Tailwind CSS
Run the following commands in your terminal to install and initialize Tailwind CSS:

```bash
npm install -D tailwindcss
npx tailwindcss init
```

---

### 2. Configure `tailwind.config.js`

Update the generated `tailwind.config.js` file to specify your content paths:

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

---

### 3. Create the Input CSS File

Inside the `src` directory, create a file named `input.css` and add the following Tailwind CSS directives:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

### 4. Build the Tailwind CSS File

Run the following command to generate your output CSS file and watch for changes:

```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

---

### 5. Create the HTML File

Inside the `src` directory, create an `index.html` file. Open it with **Live Server** to see the changes in real-time as you work.

---

## Development Workflow

1. Start the **Tailwind CSS watcher** with the command:
   ```bash
   npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
   ```
2. Open the `index.html` file in **Live Server** to preview your project.
3. Edit the `index.html` file, and the CSS will be automatically updated as you make changes.

---

## Folder Structure

```plaintext
tailwind_branding_project/
├── src/
│   ├── input.css      # Tailwind CSS input file
│   ├── output.css     # Generated Tailwind CSS file (do not edit manually)
│   ├── index.html     # Your project HTML file
├── tailwind.config.js # Tailwind CSS configuration
├── package.json       # Node.js package file
```

---

## Additional Resources

- [Tailwind CSS Documentation](https://tailwindcss.com/docs)

  
