See https://github.com/EloiStree/2025_02_01_GameStateUnityToWsTOML

-----------

# 2025_02_01_GameStateWsTOML

Is a python code that host a UDP package of 65507 bytes, it broadcast the package to all clients when changed.
I am designing some small games to be played by 10-256 players.

The server is compose of two text package and two bytes package.

A TOML is for specific to the game state information
https://toml.io/en/

All positions and rotation are in millimeters mm.

A CSV for player position:
`PLAYER_ID:PLAYER_LOBBY_ID:TEAM_ID:POSITION_X:POSITION_Y:POSITIONZ:ROTATION_X:ROTATION_Y:ROTATION_Z:SCALE:FLAT_XZ_ANGLE`

A Byte array of player position uncompressed:
`PLAYER_ID:PLAYER_LOBBY_ID:TEAM_ID:POSITION_X:POSITION_Y:POSITIONZ:ROTATION_X:ROTATION_Y:ROTATION_Z:SCALE:FLAT_XZ_ANGLE`
`PLAYER_ID` 4 bytes int
`PLAYER_LOBBY_ID` 4 bytes int
`TEAM_ID` 4 bytes int
`POSITION_X` 4 bytes  int
`POSITION_Y` 4 bytes int
`POSITION_Z` 4 bytes int
`ROTATION_X` 4 bytes int
`ROTATION_Y` 4 bytes int
`ROTATION_Z` 4 bytes int
`SCALE` 4 bytes int
`FLAT_XZ_ANGLE` 4 bytes int


