local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("I here tu", "Synapse")

local Tab = Window:NewTab("MAIN")
local Section = Tab:NewSection("MAIN")

Section:NewButton("fast attack", "ButtonInfo", function()
    spawn(function()
   game:GetService("RunService").RenderStepped:Connect(function()
    pcall(function()
        local Combat = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework)
        local Cemara = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker)
        Cemara.CameraShakeInstance.CameraShakeState = {FadingIn = 3, FadingOut = 2, Sustained = 0, Inactive = 1}
        Combat.activeController.timeToNextAttack = 0
    end)
end) 
end)


spawn(function()
   game:GetService("RunService").RenderStepped:Connect(function()
    pcall(function()
        game:GetService'VirtualUser':CaptureController()
        game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
    end)
end) 
end)
end)

local Tab = Window:NewTab("TELEPORT")
local Section = Tab:NewSection("Teleport")

Section:NewButton("Spawn", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1983.00354, 48.2867546, -1536.38525, -0.658254325, -1.42631746e-08, 0.752795577, -3.69414188e-08, 1, -1.33551197e-08, -0.752795577, -3.66004045e-08, -0.658254325)
end)

Section:NewButton("Pirate Island", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(3387.70117, 37.896862, -404.97879, -0.513284504, 6.28909946e-09, 0.858218491, -2.18308731e-08, 1, -2.0384725e-08, -0.858218491, -2.91988229e-08, -0.513284504)
end)

Section:NewButton("Solder Island", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1771.99329, 39.3538818, 65.7369156, 0.927556396, 4.28231228e-10, -0.373683214, 1.27543265e-08, 1, 3.28047598e-08, 0.373683214, -3.51943434e-08, 0.927556396)
end)

Section:NewButton("Chef Ship", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(207.756042, 86.686676, 119.072746, -0.499380946, -3.6314816e-08, -0.866382539, 3.23802212e-08, 1, -6.05793389e-08, 0.866382539, -5.83058259e-08, -0.499380946)
end)

Section:NewButton("Snow Island", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1319.39771, 18.2896729, 1440.82446, 0.269851446, -6.56841763e-08, -0.96290195, 9.22021073e-08, 1, -4.23753441e-08, 0.96290195, -7.73465416e-08, 0.269851446)
end)

Section:NewButton("Desert Island", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1245.12195, 12.8412886, 2100.60132, 0.890699685, -1.02507416e-08, -0.454592228, 3.0618807e-08, 1, 3.74432751e-08, 0.454592228, -4.72697828e-08, 0.890699685)
end)
