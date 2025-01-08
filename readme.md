npm install -D tailwindcss postcss autoprefixer vite
npx tailwindcss init -p



/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}


@tailwind base;
@tailwind components;
@tailwind utilities;


"scripts": {
    "dev": "vite",
    "build": "tailwindcss -i ./src/main.css -o ./css/style.css",
    "watch": "tailwindcss -i ./src/main.css -o ./css/style.css --watch",
    "preview": "vite preview"
  }

npm run dev


npm run watch