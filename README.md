--How to Setup Leaderstats for Roblox 

local Players = game:GetService("Players")

local function setupPlayerData(player: player)
	local leaderstats = Instance.new("Folder", player)
	leaderstats.Name = "leaderstats"
	
	local power = Instance.new("IntValue", leaderstats)
	power.Name = "Test" -- put what you want for your leaderstats here where it says Test 
	power.Value = 0
	
	local coins = Instance.new("IntValue", leaderstats)
	coins.Name = "Test" -- put what you want for your leaderstats here where it says Test 
	coins.Value = 0

end

Players.PlayerAdded:Connect(setupPlayerData)
