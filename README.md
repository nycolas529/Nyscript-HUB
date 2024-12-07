local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "Script Hub",
   LoadingTitle = "Loading Script Hub",
   LoadingSubtitle = "By RAZER#6027",
   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Player Changer"
   },
   Discord = {
      Enabled = true,
      Invite = "5tBNqX3Ngp", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },
   KeySystem = false, -- Set this to true to use our key system
   KeySettings = {
      Title = "Untitled",
      Subtitle = "Key System",
      Note = "No method of obtaining the key is provided",
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"Hello"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local MainTab = Window:CreateTab("Main", nil) -- Title, Image
local MainSection = MainTab:CreateSection("Main")

Rayfield:Notify({
   Title = "Executed The Script Successfully",
   Content = "A Good Script Hub",
   Duration = 5,
   Image = nil,
   Actions = { -- Notification Buttons
      Ignore = {
         Name = "Okay!",
         Callback = function()
         print("The user tapped Okay!")
      end
   },
},
})

local Button = MainTab:CreateButton({
   Name = "Infinite Yield",
   Callback = function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
   end,
})



local Button = MainTab:CreateButton({
   Name = "game hub x",
   Callback = function()
        --[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "Blox fruit (redz)",
   Callback = function()
        --[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/BloxFruits/main/redz9999"))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "Blox fruit (relz)",
   Callback = function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/farghii/relzhub/main/execute.hack", true))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "game hub v3",
   Callback = function()
        --[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
loadstring(game:HttpGet("https://raw.githubusercontent.com/GamerScripter/Game-Hub/main/loader"))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "telecinesse",
   Callback = function()
        --[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
loadstring(game:HttpGet(('https://raw.githubusercontent.com/SAZXHUB/Control-update/main/README.md'),true))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "fe gui nyscript",
   Callback = function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/nycolas529/Fe-gui-nyscript/refs/heads/main/README.md"))()
   end,
})

local Tab = Window:CreateTab("Info", nil) -- Title, Image

local Paragraph = Tab:CreateParagraph({Title = "Info", Content = "By Nyscript"})

local Paragraph = Tab:CreateParagraph({Title = "Info", Content = "Discord Server : https://discord.gg/T6asu9Wd})
