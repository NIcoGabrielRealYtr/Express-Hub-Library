
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/NIcoGabrielRealYtr/Express-Hub-Library/refs/heads/main/Source"))()

local Window = Library:MakeWindow({
    Name = "Title",
    HomeTab = false,
    DiscordLink = "discord.gg/example"
})
local MainTab = Window:MakeTab({
    Name = "Tab",
    Icon = "rbxassetid://10723407389"
})

local CombatSubTab = MainTab:AddSubTab({
    Name = "SubTab 1",
    Columns = 1
})

local CombatSubTab = MainTab:AddSubTab({
    Name = "Subtab 2",
    Columns = 1
})

local CombatSection = MainTab:AddSection({
    Name = "Section",
    Side = 1
})

local AimbotToggle = CombatSection:AddToggle({
    Name = "Toggle",
    Flag = "AimbotEnabled",
    Default = false,
    Tooltip = "Automatically aims at enemies",
    Callback = function(Value)
        print("Aimbot enabled:", Value)
        if Value then
            -- Start aimbot logic
        else
            -- Stop aimbot logic
        end
    end
})

local AimbotSensitivity = CombatSection:AddSlider({
    Name = "Slider",
    Flag = "AimbotSmoothness",
    Default = 5,
    Min = 1,
    Max = 20,
    Increment = 1,
    ValueName = "smooth",
    Callback = function(Value)
        print("Smoothness set to:", Value)
    end
})

local AimPartDropdown = CombatSection:AddDropdown({
    Name = "Aim Part",
    Flag = "AimPart",
    Options = {"Head", "Torso", "HumanoidRootPart"},
    Default = "Head",
    Multi = false,
    Callback = function(Value)
        print("Aiming for:", Value)
    end
})

local AimbotKeybind = CombatSection:AddLabel("Aimbot Keybind"):AddKeybind({
    Flag = "keybind label",
    Default = Enum.KeyCode.Q,
    Mode = "Hold",
    Callback = function()
        print("Keybind pressed")
    end
})

local VisualSection = MainTab:AddSection({
    Name = "Section",
    Side = 2
})

local ESPColor = VisualSection:AddColorpicker({
    Name = "Colorpicker",
    Flag = "ESPColor",
    Default = Color3.fromRGB(255, 0, 0),
    Callback = function(Color)
        print("ESP color changed to:", Color)
    end
})

local ESPToggle, ESPColorPicker = VisualSection:AddToggleColorPicker({
    Name = "Colorpicker",
    Flag = "ESP",
    Default = false,
    ColorPickerDefault = Color3.fromRGB(0, 255, 0),
    Callback = function(Color, Enabled)
        print("ESP:", Enabled, "Color:", Color)
    end
})
