# Echoes of the Vault

A first-person puzzle rapid prototype built in Unreal Engine 5.7 (Blueprint-only) for SNHU GAM-303, based on the First Person Puzzle game design scenario.

The player explores an abandoned underground testing vault — learning to move, look, jump, and interact — then solves a timed relay puzzle and a physics-based environmental puzzle before facing the Vault Warden, a boss defeated only through environmental mechanics learned earlier in the level. That describes the complete design; see **Current state** below for what is implemented in this build.

## Opening the project

**Git LFS is required.** All Blueprints and maps are stored in LFS. Cloning without it produces 131-byte placeholder files and the project will not open.

```bash
git lfs install
git clone https://github.com/kptmail-game/SNHU_GAM303_FPSPuzzle.git
```

If you already cloned without LFS, run `git lfs install` followed by `git lfs pull` inside the repository.

Open `GAM303_FPSPuzzle/GAM303_FPSPuzzle.uproject` in **Unreal Engine 5.7**. The playable map is `Content/maps/TestEnvironment`, set as both the default and editor startup map, so pressing Play works immediately. No Starter Content or asset packs are used.

## Current state — Alpha (Milestone Two)

**Implemented:** first-person movement, look, jump and interact; colored-button environmental puzzle; physics grab, carry and drop; collectibles; turret enemy with player tracking and projectile damage; health and defeat with automatic level restart; HUD with health bar, MM:SS game timer and mission objective; complete level blockout.

**Scheduled for the Final phase:** timed puzzle, boss actor and its environment-based defeat mechanic, boss health bar, win/lose screen widgets, and the contextual interact prompt.

Scheduling and test results are in [`docs/GAM303_Traceability_and_Test_Plan.xlsx`](docs/GAM303_Traceability_and_Test_Plan.xlsx) — sheet one is the traceability matrix, sheet two the test plan.

## Repository workflow

Each feature is developed on a `feature/*` branch and merged to `main` via pull request. See the closed pull requests and commit history for the development log.

## AI usage acknowledgment

I used Anthropic's Claude (via Claude Code) as a support tool on this project: it handled version control and repository management (branching, commits, pull requests, .gitignore and Git LFS setup) and assisted with formatting and updating project documentation. All game design, Blueprint scripting, and level construction in Unreal Engine are my own work. Claude's contributions are also credited directly in the commit history via Co-Authored-By tags.
