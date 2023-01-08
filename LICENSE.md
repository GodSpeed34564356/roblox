local Library = loadstring(game:HttpGet("https://pastebin.com/raw/mBL7gfbv"))()
local Window = Library.CreateLib("ZOMBIE MENU", "BloodTheme")
    

local Main = Window:NewTab("Main")
local MainSection = Main:NewSection("credits")
local MainSection = Main:NewSection("made by ZOMBIE#5978")
local MainSection = Main:NewSection("helper ZooM#2133")
local MainSection = Main:NewSection("https://discord.gg/bZ2X2ZXdN9")

local Main2 = Window:NewTab("AimBot")
local Main2Section = Main2:NewSection("Aimlock")

Main2Section:NewButton("Aimlock", "AIMBOT", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/DStKGupb'))()
end)

Main2Section:NewButton("Silent Aim", "", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/jzbR4Ch9'))()
end)

local ESP = Window:NewTab("Player")
local ESPSection = ESP:NewSection("ESP")

ESPSection:NewToggle("ESP-V1", "you can see enemies through the wall", function(state)
    if state then
        loadstring(game:HttpGet('https://pastebin.com/raw/5iXiLGHY'))()
    else
        loadstring(game:HttpGet('https://pastebin.com/raw/6D68zn2V'))()
    end
end)

ESPSection:NewToggle("ESP-V2", "you can see enemies through the wall", function(state)
    if state then
        loadstring(game:HttpGet('https://pastebin.com/raw/VLEDsi96'))()
    else
        loadstring(game:HttpGet('https://pastebin.com/raw/bBKFyZ4u'))()
    end
end)


local Misc = Window:NewTab("Misc")
local MiscSection = Misc:NewSection("Misc")

MiscSection:NewSlider("WalkSpeed", "Changes The WalkSpeed", 500, 16, function(v) -- 500 (MaxValue) | 0 (MinValue)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
end)
MiscSection:NewSlider("JumpPower", "Changes the JumpPower", 350, 50, function(v) -- 500 (MaxValue) | 0 (MinValue)
game.Players.LocalPlayer.Character.Humanoid.JumpPower = v
end)

MiscSection:NewButton("Fly (E)", "Fly Makes U Fly Press E TO Turn On/Off", function()
    print("Clicked")
    loadstring(game:HttpGet(('https://pastebin.com/raw/vhGSLy7Y'),true))()
end)
MiscSection:NewButton("invisibility (F)", "F TO Turn On/Off", function()
    loadstring(game:HttpGet(('https://pastebin.com/raw/KBsibJ74'),true))()
end)


MiscSection:NewToggle("infinite jump", "", function(state)
    if state then
        loadstring(game:HttpGet('https://pastebin.com/raw/eBeNp5Ra'))()
    else
        loadstring(game:HttpGet('https://pastebin.com/raw/PKrPMsft'))()
    end
end)

MiscSection:NewButton("Auto Clicker (V)", "", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/6tzk26wD'))()
end)

local settings = Window:NewTab("settings")
local settingsSection = settings:NewSection("settings")

settingsSection:NewKeybind("minimize (P)", "", Enum.KeyCode.P, function()
	Library:ToggleUI()
end)
