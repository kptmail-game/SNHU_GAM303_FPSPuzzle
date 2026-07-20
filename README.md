# Echoes of the Vault

A first-person puzzle rapid prototype built in Unreal Engine 5.7 (Blueprint-only) for SNHU GAM-303, based on the First Person Puzzle game design scenario.

The player explores an abandoned underground testing vault — learning to move, look, jump, and interact — then solves a timed relay puzzle and a physics-based environmental puzzle before facing the Vault Warden, a boss defeated only through environmental mechanics learned earlier in the level.

## Opening the project

Clone the repository (Git LFS required for binary assets) and open `GAM303_FPSPuzzle/GAM303_FPSPuzzle.uproject` in Unreal Engine 5.7. The playable map is `Content/maps/TestEnvironment`. No Starter Content or asset packs are used.

## Repository workflow

Each feature is developed on a `feature/*` branch and merged to `main` via pull request. See the closed pull requests and commit history for the development log.

## AI usage acknowledgment

I used Anthropic's Claude (via Claude Code) as a support tool on this project: it handled version control and repository management (branching, commits, pull requests, .gitignore and Git LFS setup) and assisted with formatting and updating project documentation. All game design, Blueprint scripting, and level construction in Unreal Engine are my own work. Claude's contributions are also credited directly in the commit history via Co-Authored-By tags.
