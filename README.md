# capstone1
capstone 1 fantasy football project. 

Users Table:

User ID (Primary Key)
Username
Email
Password (hashed)
Additional user-related fields (e.g., profile picture, settings)
Leagues Table:

League ID (Primary Key)
League Name
League Type (e.g., Standard, PPR)
Scoring Rules (e.g., points per reception)
Number of Teams
Start Date, End Date
Teams Table:

Team ID (Primary Key)
User ID (Foreign Key referencing Users Table)
League ID (Foreign Key referencing Leagues Table)
Team Name
Draft Date
Current Rank, Points, Wins, Losses, Ties
Total Points Scored, Total Points Against
Players Table:

Player ID (Primary Key)
Player Name
Position (QB, RB, WR, TE, etc.)
Team (NFL Team)
Additional player-related fields (e.g., status, injury info)
Rosters Table:

Roster ID (Primary Key)
Team ID (Foreign Key referencing Teams Table)
Player ID (Foreign Key referencing Players Table)
Start Date, End Date
Lineups Table:

Lineup ID (Primary Key)
Roster ID (Foreign Key referencing Rosters Table)
Player ID (Foreign Key referencing Players Table)
Position (e.g., QB, RB, WR, TE)
Start Date, End Date
Transactions Table:

Transaction ID (Primary Key)
Team ID (Foreign Key referencing Teams Table)
Transaction Type (Add, Drop, Trade, etc.)
Player ID (Foreign Key referencing Players Table)
Transaction Date
