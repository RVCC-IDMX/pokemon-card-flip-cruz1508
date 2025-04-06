# Pokémon Card Flip App

# How to Run Locally

To run the project locally, clone the repository and open the folder in your code editor. Then run npx serve in the terminal to start a local server and preview the app in your browser. Make sure you have Node.js installed.

# Challenges Faced

Some sprites were way too big and broke the layout. I fixed this by adding a .pokemon-img class and styling it with max-width, object-fit, and auto height.

When I first started, card flipping didn’t always work. I used event.target tracing and made sure the event listener was using delegation properly.



## Features

- Responsive 4x3 grid of cards showing Pokéball images initially
- Cards flip to reveal random Pokémon when clicked
- Each card displays:
  - Pokémon name (capitalized)
  - Pokémon type(s) with color coding
  - Pokémon sprite image from the PokéAPI
  - Additional stats (height, weight, abilities)
- Fetches 12 random Pokémon from the PokéAPI when the page loads
- Cards maintain their Pokémon until the page is refreshed
- Simple card flip animations
- Loading spinner during API requests

## Technologies Used

- HTML5
- CSS3 with transitions and animations
- JavaScript (ES6+)
- Fetch API
- [PokéAPI](https://pokeapi.co/)

## Project Structure

```
pokemon-card-flip/
├── index.html           # Main HTML structure
├── css/
│   └── styles.css       # CSS styling
├── js/
│   ├── app.js           # Main application logic
│   └── pokemon.js       # Pokémon data fetching functions
├── assets/
│   ├── pokeball.png     # Pokéball image for card fronts
├── docs/                # Documentation resources
│   ├── index.html       # Documentation home
│   ├── assignment.html  # Instruction
│   ├── js-tutorial.html # DOM manipulation tutorial
│   ├── global.html      # Window object guide
│   └── testing.html     # Testing strategy
├── eslint.config.mjs    # ESLint configuration
└── README.md            # Project documentation
└── LICENSE.md           # Project license information
```

## How to Use

### Local Development

1. Clone this repository:

2. Open `index.html` in your browser or use a local server:
   ```
   npm install
   npx serve
   ```

3. Click on cards to reveal Pokémon
4. Refresh the page to get a new set of random Pokémon

### Deploy to Netlify

This project is ready to deploy to Netlify for free hosting:

1. **Create a Netlify account** if you don't have one at [netlify.com](https://www.netlify.com/)

2. **Deploy directly from GitHub**:
   - Log in to Netlify
   - Click "New site from Git"
   - Select GitHub and authorize Netlify
   - Choose your pokemon-card-flip repository
   - Use these build settings:
     - Build command: leave blank (no build required)
     - Publish directory: `.` (root directory)
   - Click "Deploy site"


Your site will be live at a URL like `https://your-site-name.netlify.app`

### Continuous Deployment

After setting up with GitHub, any changes you push to your repository will automatically trigger a new deployment on Netlify. This gives you a seamless workflow:

1. Make changes to your code
2. Commit and push to GitHub
3. Netlify automatically deploys the updated version

## Extensions and Improvements

Here are some ways you could extend this project:

- Add filter buttons to show Pokémon by type
- Implement a "Catch Pokémon" feature using localStorage
- Create a detailed view modal for each Pokémon
- Add search functionality to find specific Pokémon
- Implement sound effects for card flips and Pokémon cries

## Documentation

The `docs/` folder contains helpful guides and resources:

- **Home Page** (`index.html`): Central hub with links to all documentation
- **Pokémon Assignment Instructions** (`assignment.html`): Details on the assignment requirements and objectives
- **DOM Manipulation Tutorial** (`js-tutorial.html`): Learn how to create and manipulate DOM elements
- **Global Scope Guide** (`global.html`): Understand how we use the window object
- **Testing Approach** (`testing.html`): Learn about the project's testing strategy


## ESLint Integration

This project uses ESLint for code quality. Run:

```
npm install
npm run lint
```

## Credits

- Pokémon data provided by [PokéAPI](https://pokeapi.co/)
- Pokéball image is used for educational purposes
- Pokémon is a trademark of Nintendo, Game Freak, and Creatures Inc.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.