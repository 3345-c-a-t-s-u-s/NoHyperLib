# Hello, NoHyper

## Example
```lua
local NoHyper = loadstring(game:HttpGet('https://raw.githubusercontent.com/3345-c-a-t-s-u-s/NoHyperLib/main/source.dll'))()
local Window = NoHyper.new('Hello, NoHyper',nil--[[YOUR LOGO - RBX]],'Welcome back!')

Window:AddYoutube('https://www.youtube.com/your-youtube-channel')
Window:AddWebsite('https://example.com/your-website')
Window:AddDiscord('https://discord.gg/your-discord')

local General = Window:NewTab('General','earth') -- [[Icon: ads list folder earth locked home positon notify close color]]
local Example = General:NewSection('Example','positon','left') -- [left , right]

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
```
