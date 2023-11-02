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
- run "npm run build" and it will create the css file in a css folder
- create index.html and add link to stylesheet
    - <link rel="stylesheet" href="css/main.css">
    - add content to the page (<h1 class="text-3xl">Hello World!</h1>)
- run "npm run watch" to let tailwind monitor the project
- run live server and view the page (it will refresh the browser when changes are made now)
- add screen sizes to "theme" in tailwind.config.js
```js
    screens: {
      sm: '480px',
      md: '768px',
      lg: '976px',
      xl: '1440px'
    },
```