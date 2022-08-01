local h = game.Players.LocalPlayer.Character.Humanoid
local c = game.Players.LocalPlayer.Character
local p = game.Players.LocalPlayer

local Mercury = loadstring(game:HttpGet("https://raw.githubusercontent.com/deeeity/mercury-lib/master/src.lua"))()

local GUI = Mercury:Create{
    Name = "zsr",
    Size = UDim2.fromOffset(600, 400),
    Theme = Mercury.Themes.Dark,
    Link = "https://github.com/z4xi/z4sscripts"
}

-- PLAYER
local PlayerTab = GUI:Tab{
    Name = "Player",
    Icon = "http://www.roblox.com/asset/?id=10162222820"
}

PlayerTab:Slider{
    Name = "Speed",
    Description = "Changes the player's speed.",
    Min = 16,
    Max = 500,
    Default = 16,
    Callback = function(v)
        h.WalkSpeed = v
    end
}

PlayerTab:Slider{
    Name = "Jump Power",
    Description = "Changes the player's jump power.",
    Min = 50,
    Max = 500,
    Default = 50,
    Callback = function(v)
        h.JumpPower = v
    end
}

PlayerTab:Button{
    Name = "Respawn",
    Description = "Respawns the character.",
    Callback = function()
        GUI:Prompt{
            Followup = false,
            Title = "Respawn",
            Text = "Would you like to respawn?",
            Buttons = {
                yes = function()
                    game.Players.LocalPlayer.Character.Head:Destroy()
                    if game.Players.LocalPlayer.Character.Humanoid.Health < 5 then 
                        local currentPos = game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").position
                        wait(1.5)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(currentPos)
                    end
                end,
                no = function()
                    return
                end
            }
        }
    end
}

-- SCRIPTS
local ScriptsTab = GUI:Tab{
    Name = "Scripts",
    Icon = "http://www.roblox.com/asset/?id=10382901926"
}

ScriptsTab:Button{
    Name = "Orca",
    Description = "A beautiful universal script."
}

ScriptsTab:Button{
    Name = "Sharkswap",
    Description = "A boombox script.",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/specowos/lua-projects/main/small%20projects/sharkswap/src.lua"))()
    end
}

ScriptsTab:Button{
    Name = "ToolSpin",
    Description = "Spins equipped tools around your character.",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/specowos/scriptsforvideos1/f93ecb5ed61c6fd380d57a799b40f22a36d05624/simple%20hatspin%20mod%20for%20tools"))()
    end
}

ScriptsTab:Button{
    Name = "Project: 2016",
    Description = "Makes Roblox look like it did in 2016.",
    Callback = function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/specowos/lua-projects/main/small%20projects/project%3A2016/2016raw.lua',true))()
    end
}

ScriptsTab:Button{
    Name = "Universal FE Hub",
    Description = "An FE hub with tons of scripts.",
    Callback = function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/Dvrknvss/UniversalFEScriptHub/main/Script'))()
    end
}
-- COLA MAN
local ColaMan = GUI:Tab{
    Name = "Cola Man",
    Icon = "http://www.roblox.com/asset/?id=10162555280"    
}

ColaMan:Button{
    Name = "Dupe Cola",
    Description = "Dupes cola",
    Callback = function(s)
        local fart = game:GetService("Players").LocalPlayer.Character
        local fart2 = game:GetService("Players").LocalPlayer
        game.Players:Chat("-cola")
        wait(1)
        fart.BloxyCola.Parent = workspace
    end
}

ColaMan:Button{
    Name = "Equip all",
    Description = "Equips all colas",
    Callback = function()
        for i, v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetDescendants()) do
        if v:IsA("Tool") and v.Name == "BloxyCola" then
            v.Parent = game:GetService("Players").LocalPlayer.Character
        end
    end    
    end
}

ColaMan:Button{
    Name = "Spin selected",
    Description = "Spins selected colas",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/specowos/scriptsforvideos1/f93ecb5ed61c6fd380d57a799b40f22a36d05624/simple%20hatspin%20mod%20for%20tools"))()    
    end
}

-- BOOMBOX STUFF
local BoomboxTab = GUI:Tab{
    Name = "Boombox",
    Icon = "https://www.roblox.com/asset/?id=10384298553"
}

BoomboxTab:Button{
    Name = "Dupe boombox",
    Description = "Dupes boomboxes",
    Callback = function()
        --// run this like 15 times
        local fart = game.Players.LocalPlayer.Character
        game.Players.LocalPlayer.Backpack.BoomBox.Parent = fart
        fart.BoomBox.Parent = workspace
        wait()
        game.Players:Chat("-re")
    end
}

BoomboxTab:Button {
    Name = "Equip all",
    Description = "Equips all boomboxes",
    Callback = function()
        for i, v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetDescendants()) do
        if v:IsA("Tool") and v.Name == "BoomBox" then
            v.Parent = game:GetService("Players").LocalPlayer.Character
        end
        end
    end
}

BoomboxTab:Button {
    Name = "Spin tools",
    Description = "Spin all boomboxes",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/specowos/scriptsforvideos1/f93ecb5ed61c6fd380d57a799b40f22a36d05624/simple%20hatspin%20mod%20for%20tools"))() 
    end
}
