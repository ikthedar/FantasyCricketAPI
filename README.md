# FantasyCricketAPI
FantasyCricketAPI is a Django Rest Framework-based backend for creating and managing fantasy cricket teams. It includes features like team creation, player stats integration, game week management, and leaderboards.

## Requirements
**Functional**:
-Users can create fantasy cricket teams.
-Retrieve player stats and details (e.g., recent performances).
-Suggest players for a team based on certain criteria (e.g., form, budget).
-Allow team updates (adding/removing players).
-Score computation for teams after matches.

**Non-Functional**:
-Fast API responses.
-Secure endpoints (authentication/authorization).
-Scalable architecture for handling multiple teams and large datasets.
-Reliable third-party integrations for cricket stats.

## Core Entities
*Models*:
Player: Name, team, role (batter, bowler, all-rounder, wicketkeeper), price, recent stats.
Team: Name, user, budget, list of players, total score.
User: Username, email, password (authentication purposes).
Match: Teams playing, date, stats summary.
