# Fantasy Premier League API endpoint guide:

## General Information

The ‘bootstrap-static’ is the general call for basic info. Will provide ID fields for fixtures and players (see next endpoints)

Full URL: https://fantasy.premierleague.com/api/bootstrap-static/

Data included:

    A summary of all 38 gameweeks
    The game’s settings
    Basic information on all 20 PL teams
    Total number of FPL Users and overall chip usage
    Basic information on all Premier League players
    List of stats that FPL keeps track of
    The different FPL positions

Bootstrap-static will provide essential analysis data and keys such as: Basic player info, player positions, all 38 gameweeks

## Individual Premier League Players

Grab the player’s ID from the bootstrap-static call. Detailed player stats

Full URL: https://fantasy.premierleague.com/api/element-summary/{player-id}/

There’s also an additional URL that allows you to view the performance of all players for a specified gameweek.

Full URL: https://fantasy.premierleague.com/api/event/{GW}/live/

Data included: Shows below stats, but for the gameweek for every player, rather than a single player for every gameweek.

Data included:

    Remaining fixtures for the player, including:
        Kickoff time
        Gameweek number
        Home or Away
        Difficulty

    Previous fixtures and performance, including:
        Minutes played
        Goals
        Assists
        Conceded
        Cards
        Bonus
        Influence
        Creativity
        xG
        xA
        Value
        Transfer delta for that gameweek
