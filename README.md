# Hello, NoHyper
![Real](https://github.com/3345-c-a-t-s-u-s/NoHyperLib/assets/117000269/acb192b2-b8c5-4b32-9ad8-e8932faa32aa)
![reala](https://github.com/3345-c-a-t-s-u-s/NoHyperLib/assets/117000269/b1c5eb95-33e7-4493-9cef-ffada36c04c1)

## Example
```lua
local NoHyper = require(script:WaitForChild('ModuleScript'))

NoHyper.set_theme('nohyper') -- [[nohyper , bedol , neverlose, green]]

local Window = NoHyper.new('Hello, '..game.Players.LocalPlayer.DisplayName,"rbxassetid://16763260622",'Welcome back!') -- My Logo you can replace it
Window:NewSize(UDim2.new(0.1,430,0.1,300))

Window:AddYoutube('https://www.youtube.com/your-youtube-channel')
Window:AddWebsite('https://example.com/your-website')
Window:AddDiscord('https://discord.gg/your-discord')

local General = Window:NewTab('General','earth') -- [[Icon: ads list folder earth locked home positon notify close color]]
local Setting = Window:NewTab('Setting','list')
local Example = General:NewSection('Example','positon','left') -- [left , right]
local RightSection = General:NewSection('Section','ads','right')
local SettingSection = Setting:NewSection('Settings','crown','left')

SettingSection:AddToggle('Auto Save',false,function(v)
	print('auto save: ',v)
end)

Example:AddButton('Example',function()
	print('click!')
end)

Example:AddToggle('Toggle',false,function(value)
	print('click!',value)
end)

Example:AddKeybind('Keybind',Enum.KeyCode.E,function(value)
	print('bind!',value)
end)

Example:AddSlider('Keybind',{Min = 0,Max = 100,Default = 50,ValueT = '%'},function(value)
	print('number is ',value)
end)

Example:AddDropdown('Dropdown',{1,2,3,4,5,6,7,8,9,10},5,function(value)
	print('select ',value)
end)

RightSection:AddToggle('Aimbot',false,function(...)
	print('Boolen: ',...)
end)

RightSection:AddToggle('Esp',false,function(...)
	print('Boolen: ',...)
end)

RightSection:AddToggle('XRay',false,function(...)
	print('Boolen: ',...)
end)
```
