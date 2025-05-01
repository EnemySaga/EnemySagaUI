## 🧩 UI Library
```
local UILib = loadstring(game:HttpGet("https://github.com/EnemySaga/EnemySagaUI"))()
local Window = UILib:Create("My Script Hub")
```
## 🧩 Notification
```
game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = "Script Loaded",
    Text = "Welcome to EnemySaga Hub!",
    Duration = 5
})
```
## 🧩 Create Tabs
```
local MainTab = Window:AddTab("Main")
```
## 🧩 Button
```
MainTab:AddButton("Kill All", function()
    -- Your kill all function here
    print("Kill All activated")
end)
```
## 🧩 Toggle
```
MainTab:AddToggle("God Mode", false, function(state)
    -- Your god mode function here
    print("God Mode:", state)
end)
```
## 🧩 Slider
```
MainTab:AddSlider("WalkSpeed", 16, 500, 16, function(value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)
```
## 🧩 Dropdown
```
MainTab:AddDropdown("ESP Color", {"Red", "Green", "Blue", "White"}, function(selected)
    -- Your ESP color function here
    print("Selected color:", selected)
end)
```
