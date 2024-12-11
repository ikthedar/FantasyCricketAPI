# FantasyCricketAPI
FantasyCricketAPI is a Django Rest Framework-based backend for creating and managing fantasy cricket teams. It includes features like team creation, player stats integration, game week management, and leaderboards.

## Requirements
**Functional**:
* Users can create fantasy cricket teams.
* Retrieve player stats and details (e.g., recent performances).
* Suggest players for a team based on certain criteria (e.g., form, budget).
* Allow team updates (adding/removing players).
* Score computation for teams after matches.

**Non-Functional**:
* Fast API responses.
* Secure endpoints (authentication/authorization).
* Scalable architecture for handling multiple teams and large datasets.
* Reliable third-party integrations for cricket stats.

## Core Entities
*Models*:
* Player: Name, team, role (batter, bowler, all-rounder, wicketkeeper), price, recent stats.
* Team: Name, user, budget, list of players, total score.
* User: Username, email, password (authentication purposes).
* Match: Teams playing, date, stats summary.

## API Endpoints
*User Authentication*:

* POST /register: Register a user.
* POST /login: Login a user and return a token.

*Player Management*:

* GET /players: List all players.
* GET /players/<id>: Get details of a specific player.

*Team Management*:

* POST /teams: Create a new fantasy team.
* GET /teams/<id>: View details of a team.
* PUT /teams/<id>: Update team (add/remove players).
* DELETE /teams/<id>: Delete a team.

*Match Stats*:

* GET /matches: Get details of recent matches.
* GET /matches/<id>: Get stats for a specific match.

*Score Computation*:

* GET /teams/<id>/score: Compute and return the total score of a fantasy team.
