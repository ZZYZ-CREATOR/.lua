-- Gui to Lua
-- Version: 3.2

-- Instances:

local DropGUI = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local DropTool = Instance.new("TextButton")
local Equip = Instance.new("TextButton")
local Version = Instance.new("TextButton")
local Cred = Instance.new("TextButton")

--Properties:

DropGUI.Name = "Drop GUI"
DropGUI.Parent = game.CoreGui
DropGUI.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

main.Name = "main"
main.Parent = DropGUI
main.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
main.Position = UDim2.new(0.0809101239, 0, 0.203790441, 0)
main.Size = UDim2.new(0, 150, 0, 128)
main.Active = true
main.Draggable = true

DropTool.Name = "Drop Tool"
DropTool.Parent = main
DropTool.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
DropTool.Position = UDim2.new(0.0597826242, 0, 0.119906127, 0)
DropTool.Size = UDim2.new(0, 55, 0, 50)
DropTool.Font = Enum.Font.SourceSans
DropTool.Text = "Drop"
DropTool.TextColor3 = Color3.fromRGB(0, 0, 0)
DropTool.TextScaled = true
DropTool.TextSize = 14.000
DropTool.TextWrapped = true
DropTool.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Parent = game.Workspace
end)

Equip.Name = "Equip"
Equip.Parent = main
Equip.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Equip.Position = UDim2.new(0.55251956, 0, 0.119906083, 0)
Equip.Size = UDim2.new(0, 58, 0, 50)
Equip.Font = Enum.Font.SourceSans
Equip.Text = "Equip"
Equip.TextColor3 = Color3.fromRGB(0, 0, 0)
Equip.TextScaled = true
Equip.TextSize = 14.000
Equip.TextWrapped = true
Equip.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Backpack:FindFirstChildOfClass("Tool").Parent = game.Players.LocalPlayer.Character
end)

Version.Name = "Version"
Version.Parent = main
Version.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Version.Position = UDim2.new(0, 0, 0.999885917, 0)
Version.Size = UDim2.new(0, 151, 0, 34)
Version.Font = Enum.Font.SourceSans
Version.Text = "Version 1"
Version.TextColor3 = Color3.fromRGB(0, 0, 0)
Version.TextScaled = true
Version.TextSize = 14.000
Version.TextWrapped = true

Cred.Name = "Cred"
Cred.Parent = main
Cred.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Cred.Position = UDim2.new(0, 0, -0.266169071, 0)
Cred.Size = UDim2.new(0, 151, 0, 34)
Cred.Font = Enum.Font.SourceSans
Cred.Text = "Script made by WarriorRoberr"
Cred.TextColor3 = Color3.fromRGB(0, 0, 0)
Cred.TextSize = 14.000
Cred.TextWrapped = true