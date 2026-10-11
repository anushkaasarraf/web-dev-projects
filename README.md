# web-dev-projects

A collection of beginner-friendly frontend projects built with plain **HTML, CSS and vanilla JavaScript**. There are no frameworks and no build step. Each project has its own folder inside this repo and can be opened directly in the browser.

## Projects in this repository

| Folder | Project | Highlights |
| --- | --- | --- |
| [`portfolio/`](./portfolio) | Portfolio Website | Responsive personal site with a contact form |
| [`todoList/`](./todoList) | To-Do List | Add, complete, edit and delete tasks; saved in `localStorage` |
| [`weather app/`](./weather%20app) | Weather App | Live weather by city using the OpenWeatherMap API |


## Repository structure

```
web-dev-projects/
├── README.md
├──portfolio/
|   ├── index.html
|   ├── style.css
|   └── images/
├── todoList/
│   ├── index.html
│   ├── style.css
│   └── script.js
└── weather app/
    ├── index.html
    ├── style.css
    ├── script.js
    └── images/

```

## Project details

### 1. Portfolio Website
- Sections: Home, About, Services, My Work, Contact
- Responsive layout with a hamburger side menu on mobile
- Tabbed Skills / Experience / Education panel
- Contact form that submits to Google Sheets via Google Apps Script
- Icons from Font Awesome and the Poppins font
- Downloadable CV (`images/cv.pdf`)

### 2. To-Do List
- Add tasks with the **Add** button or the **Enter** key
- Tick a checkbox to mark a task complete (strike-through style)
- **Double-click** a task to edit it
- Delete tasks with the **Delete** button
- Tasks persist between visits using `localStorage`

### 3. Weather App
- Search any city by name (button click or Enter)
- Shows temperature (°C), humidity (%) and wind speed
- Icon changes with conditions: clear, clouds, rain, drizzle, mist
- Shows an "Invalid city name" message for unknown cities
- Uses the [OpenWeatherMap Current Weather API](https://openweathermap.org/current)


## Getting started

```bash
git clone https://github.com/<anushkaasarraf>/web-dev-projects.git
cd web-dev-projects
```

No installation is needed. Open the `index.html` file inside any project folder in your browser, or run a local server (for example, the VS Code **Live Server** extension):

```bash
npx serve .
```

### Weather app API key

1. Create a free account at [openweathermap.org](https://openweathermap.org/api) and generate an API key.
2. Open `weather app/script.js` and set your key:
   ```js
   const apiKey = "YOUR_API_KEY";
   ```

> **Note:** never commit a real API key to a public repository.

## Tech stack

- HTML5
- CSS3 (Flexbox, Grid, responsive design)
- JavaScript (ES6+, DOM manipulation, `fetch`, `localStorage`)
- External services: OpenWeatherMap API, Google Apps Script, Font Awesome, Google Fonts (Poppins)

## What I practiced

- DOM manipulation and event handling
- Persisting data with `localStorage`
- Calling REST APIs with `async`/`await`
- Building responsive layouts and mobile navigation
- Handling form submissions with a serverless endpoint

## Future improvements

- Weather app: snow icon support, loading and error states, hide the API key
- To-Do List: filters (all / active / completed)
- Portfolio: replace placeholder text and links with real content

## License

This project is open source and available under the [MIT License](LICENSE).
