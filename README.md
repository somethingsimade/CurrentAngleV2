# CurrentAngleV2
Since it was leaked, i shouldnt have shared, here it is skids. (friendly fire?)

Credits to geecee for the original method. I re found the method, and mixed with my old reanimate, they leaked it (not geecee), after i made it private. Now it is spreading, lol, so ill just get the job done. (they literally released their full file version.)

IT DOESNT RUN ON ITS OWN, please put the script in "-- u paste the script here for now, theres no loadstring httpget for now." (replace it)
not placeholder anymore: it is open now due to the oxide server release, no blaming on them.
# httpget
```lua
-- SETTINGS --
local settings = _G

settings["Use default animations"] = true
settings["Fake character transparency level"] = 1 -- 0 to disable
settings["Disable character scripts"] = true
settings["Fake character should collide"] = true
settings["Parent real character to fake character"] = false
settings["Respawn character"] = true --[[ only should be disabled if
your character havent played ANY animations, otherwise it breaks the reanimate ]]
settings["Instant respawn"] = false --[[ Instant respawns the
character, it will still wait the respawn time, but your character wont be dead.
Requires: replicatesignal function
Enable if you want the feature
]]

settings["Names to exclude from transparency"] = {
    --[[ example:
    ["HumanoidRootPart"] = true,
    ["Left Arm"] = true
    ]]
}
(function() if getgenv then return getgenv() else return _G end end)().fling = nil
local finished = false

task.spawn(function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/somethingsimade/CurrentAngleV2/refs/heads/main/v2"))()
end)

repeat task.wait() until finished

-- USAGE: getgenv().fling(character, time, yield) if you dont have getgenv: _G.fling(character, time, yield)
-- or just fling(character, time, yield)

-- time is for how much time in seconds it will fling
-- the character

-- yield is if the fling function will yield

-- you can put your converted script under here
```
