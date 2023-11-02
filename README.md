# Tailwind Dashboard Splash Page

- npm init -y (to create a package.json)
- npm i -D tailwindcss (install tailwind as a dependency)
- create a .gitignore file
- npx tailwindcss init (to create tailwind.config.js file)
    - in "content" point it to where to watch files with tailwind classes
        - ex: content: ['./*.html'],
        - that's for html files in the root directory
- created input.css and added 3 tailwind imports (can add custom CSS to this file, too)
    - @tailwind base;
    - @tailwind components;
    - @tailwind utilities;
- add two scripts to package.json
    - "build": "tailwindcss -i ./input.css -o ./css/main.css",
    - "watch": "tailwindcss -i ./input.css -o ./css/main.css --watch",
        - the -i is the input file
        - the -o is the output file
        - "build" will run once and build the css
        - "watch" will run constantly during development