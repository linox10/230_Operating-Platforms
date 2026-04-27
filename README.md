# 230_Operating-Platforms

The Gaming Room wanted to expand their Android game Draw It or Lose It into a web-based application that could run across multiple operating systems and devices.
I did particularly well at connecting each design constraint directly to a technical decision, such as using the Singleton pattern to enforce the requirement that only one game instance can exist in memory at a time.
Working through the design document before writing any code helped me think through how the Game, Team, and Player classes related to each other through the GameService before getting into implementation details.
If I could revise one part it would be the Evaluation section, since the platform comparisons could be more specific to the game's actual requirements rather than staying at a general level.
The client's need for cross-platform access, unique identifiers, and single-instance game management were each translated into specific decisions like the Singleton pattern, unique ID generation in GameService, and a Linux cloud environment with WebSocket support, because addressing those needs in the design phase is far easier than correcting them during development.
I approached the design by starting with the client's constraints and working outward toward architecture decisions like cloud hosting, PostgreSQL storage, and load balancing, and in the future I would continue that same requirements-first approach while prototyping earlier to test assumptions before committing them to documentation.
