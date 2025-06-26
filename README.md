# CurrentAngleV2
*ATTENTION TO READERS: I DID NOT LEAK THE REANIMATE INITIALLY. THEY HAVE RELEASED MULTIPLE VERSIONS, THIS IS JUST MY NEW VERSION. THERE IS NO SENSE IN GATEKEEPING SOMETHING LEAKED IN PUBLIC SERVERS WITH HUNDREDS OF PEOPLE*
Since it was leaked, i shouldnt have shared if it wasnt leaked, here it is skids. (friendly fire?)

Credits to geecee for the original method. I re found the method, and mixed with my old reanimate, they leaked it (not geecee), after i made it private. Now it is spreading, lol, so ill just get the job done. (they literally released their full file version.)

not placeholder anymore: it is open now due to the oxide server release, no blaming on them.

also this was made like a week ago (as the time of writing, check commits)

# It would be nice to have credits.. just leaving this here..
![Interesing](https://github.com/somethingsimade/CurrentAngleV2/blob/main/justleavingthishere.png)
???
![what](https://github.com/somethingsimade/CurrentAngleV2/blob/main/image.png)

![copied](https://github.com/somethingsimade/CurrentAngleV2/blob/main/imgrun.png)

https://www.diffchecker.com/NnfMruqk/

^^^^
# also would appreciate you guys comparing both oxide and MY v1 (read commits, it was released over a week ago. basically less than 3 people had the version; it is not from kampachi) (DO NOT USE THE SIDE BAR TO COMPARE, USE YOUR EYES)

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
settings["Hide HumanoidRootPart"] = false --[[ Enabled by default. when enabled, your chat bubble or name tag
will not appear above your character, but you will have your character immortal in the Fencing arena.
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
