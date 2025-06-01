<h1>Aman Kumar: Building the Classic Pac-Man Game Using JavaScript</h1>

<p>Aman Kumar, a dedicated software developer, successfully built a Pac-Man game using javscript, demonstrating his expertise in programming and game development. Inspired by the iconic arcade game, he leveraged the guidance of Harshith YT Coding Channel to bring his project to life, implementing game mechanics with precision and creativity.</p>

<h1>Project Inspiration and Vision</h1>

<p>Pac-Man, originally released in 1980, remains one of the most beloved video games worldwide. Aman set out to recreate this classic, maintaining its nostalgic appeal while integrating modern programming techniques. His goal was to develop a seamless and engaging experience where players navigate Pac-Man through a maze, collect pellets, and evade ghosts.</p>

<img src ="https://github.com/Amansinha110/Pac-Man/blob/master/Screenshot%202025-06-01%20050509.png">
<a href="https://amansinha110.github.io/Pac-Man/"><img src="https://github.com/Amansinha110/Pac-Man/blob/master/OIP.jpeg"></a>

<h1>Click Blue Button For Play</h1>

<h3>Development Process and Technologies Used</h3>

<p>I am chose Javascript as the primary language for development due to its versatility and ease of use. The Pygame library played a crucial role in handling graphics, animations, and user interactions.</p>

<h4>Key Features Implemented:</h4>

<p>Pac-Man Movement: Smooth player control and responsiveness using keyboard input.

Maze Generation: A structured grid-based maze where Pac-Man navigates and collects points.

Ghost AI: Implementing enemy movement patterns to challenge the player.

Collision Detection: Ensuring Pac-Man interacts correctly with walls, pellets, and enemies.

Score System: Keeping track of points earned by consuming pellets and power-ups.</p>

<h2> Challenges and Learning Experience</h2>

<p> During development, I am faced challenges such as optimizing ghost AI behavior, handling smooth player movement, and maintaining performance efficiency. By referring to Harshith YT Coding Channel, he overcame debugging issues and refined his coding approach.

This project significantly enhanced Aman’s knowledge of Python programming, logic-based game mechanics, and creative problem-solving. His ability to design interactive experiences became a highlight of his journey.</p>

<h3>Sample Code: Basic Pac-Man Game in Javascript using Pygame</h3>

```javascript
// Set up the canvas
const canvas = document.getElementById("gameCanvas");
const ctx = canvas.getContext("2d");

// Pac-Man properties
let pacman = {
    x: 50,
    y: 50,
    radius: 20,
    speed: 5,
    direction: "right"
};

// Draw Pac-Man
function drawPacman() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    
    ctx.beginPath();
    ctx.arc(pacman.x, pacman.y, pacman.radius, 0.2 * Math.PI, 1.8 * Math.PI); // Open mouth
    ctx.lineTo(pacman.x, pacman.y);
    ctx.fillStyle = "yellow";
    ctx.fill();
}

// Move Pac-Man based on keyboard input
document.addEventListener("keydown", (event) => {
    if (event.key === "ArrowRight") pacman.x += pacman.speed;
    if (event.key === "ArrowLeft") pacman.x -= pacman.speed;
    if (event.key === "ArrowUp") pacman.y -= pacman.speed;
    if (event.key === "ArrowDown") pacman.y += pacman.speed;

    drawPacman();
});

// Initialize game
drawPacman();
```

<h1>Homework:</h1>

<p>You can continue working on this project if you like. You can design your own map by modifying the tileMap if you want. You can add power pellets to allow pacman to eat the ghosts. In addition, there is an opening on left and right, where if pacman goes through, it would appear on the other side of the map. Currently pacman just moves off screen out of the map so a fix would be needed to make pacman appear the other side. For more of a challenge, you can modify the ghosts movement to cover areas unreachable since the ghosts only change directions when they collide against a wall, and not when theres another path available to go through.</p>
