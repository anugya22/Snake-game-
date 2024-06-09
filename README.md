The HTML structure consists of the following elements:

<head>: Contains metadata and the title of the document.
<body>: The main content of the document.
Styling
The code includes some CSS styles to customize the appearance of the game:
canvas: Sets a black border around the canvas element.
h1: Styles the heading with red text and a green background.
body: Sets the text alignment to center and the background color to powder pink.
footer: Styles the footer element with a pink background and padding.
button: Styles the buttons with margin, padding, and a cursor pointer.
button:hover: Changes the opacity of the buttons on hover.
JavaScript Logic
The JavaScript code handles the game logic and interaction with the canvas element:
const canvas = document.getElementById("gameCanvas");: Retrieves the canvas element from the HTML document.
const ctx = canvas.getContext("2d");: Retrieves the 2D rendering context of the canvas.
let snake = [...]: Initializes the snake's initial position as an array of objects representing the snake's segments.
let direction = "right";: Sets the initial direction of the snake.
let food = { x: 10, y: 10 };: Sets the initial position of the food.
let snakeColor = "green";: Sets the default color of the snake.
function changeColor(color) { ... }: Updates the snake's color based on the button clicked in the footer.
function generateFood() { ... }: Generates random positions for the food.
function checkCollision() { ... }: Checks if the snake collides with itself or the boundaries of the canvas.
function drawSegment(segment, isHead) { ... }: Draws a segment of the snake on the canvas.
function updateGame() { ... }: Updates the game state, including the snake's movement, food generation, collision detection, and rendering.
document.addEventListener("keydown", (event) => { ... }: Listens for keydown events to change the direction of the snake.
generateFood();: Generates the initial food position.
updateGame();: Starts the game loop to update and render the game.
