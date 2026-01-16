# VEAF Foothold Afghanistan v0.0.995

## Presentation

This is a modification of the original Foothold Afghanistan mission by Leka, that I adapted to make it load all the script files and config directly from the server.

**Done using the latest version updated on 2026.01.11.**

## Update

### Triggers

#### For Foothold

Add this triggers on MissionStart:

**Modern:**
name: `Foothold loading`
do_script:
```lua
FOOTHOLD_DYNAMIC_PATH = [[C:\Users\veaf\Saved Games\DCS.missions\_TEMPLATES\Missions\foothold\Afghanistan\Modern\]]
env.info("FOOTHOLD LOADING")
assert(loadfile(FOOTHOLD_DYNAMIC_PATH .. "VEAF_loader.lua")) ()
```

**Cold War:**
name: `Foothold loading`
do_script:
```lua
FOOTHOLD_DYNAMIC_PATH = [[C:\Users\veaf\Saved Games\DCS.missions\_TEMPLATES\Missions\foothold\Afghanistan\Coldwar\]]
env.info("FOOTHOLD LOADING")
assert(loadfile(FOOTHOLD_DYNAMIC_PATH .. "VEAF_loader.lua")) ()
```

### Code

## Things to do

[ ] activer les rapports BDA (surement dans le mission editor)
