# Roblox Minutes Tracker

This is a Lua script for Roblox designed to track player game time in minutes. It uses the `DataStoreService` to save and load each player's game time data.

## How It Works:

-   **Player Join:** When a player joins the game, the script creates an `IntValue` called "Minutos" within a `leaderstats` folder, making it visible on the leaderboards.
-   **Data Loading:** It checks if the player already has saved data. If so, it loads the value. Otherwise, the counter starts at 0.
-   **Time Counting:** A routine is started to update the "Minutos" value every 60 seconds (1 minute).
-   **Player Leaving:** When the player leaves the game, the script saves the current "Minutos" value to the `DataStore` using the player's `UserId` as the key.
