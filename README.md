-- Gui to Lua
-- Version: 3.2

-- Instances:

local CoolNewGui = Instance.new("ScreenGui")
local HackFrame = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local BGFrame = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local FrameFarm = Instance.new("Frame")
local AutoFarmFrame = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local Eei = Instance.new("Frame")
local UICorner_4 = Instance.new("UICorner")
local AutoFarmText = Instance.new("TextLabel")
local UITextSizeConstraint = Instance.new("UITextSizeConstraint")
local Eisc = Instance.new("Frame")
local UICorner_5 = Instance.new("UICorner")
local True = Instance.new("TextButton")
local UICorner_6 = Instance.new("UICorner")
local Stats = Instance.new("TextLabel")
local UITextSizeConstraint_2 = Instance.new("UITextSizeConstraint")
local False = Instance.new("TextButton")
local UICorner_7 = Instance.new("UICorner")
local TextBoxtool = Instance.new("TextBox")
local UICorner_8 = Instance.new("UICorner")
local ToolEquip = Instance.new("Frame")
local UICorner_9 = Instance.new("UICorner")
local Eei_2 = Instance.new("Frame")
local UICorner_10 = Instance.new("UICorner")
local AAAAAAA = Instance.new("TextLabel")
local UITextSizeConstraint_3 = Instance.new("UITextSizeConstraint")
local Eisc_2 = Instance.new("Frame")
local UICorner_11 = Instance.new("UICorner")
local True_2 = Instance.new("TextButton")
local UICorner_12 = Instance.new("UICorner")
local Stats_2 = Instance.new("TextLabel")
local UITextSizeConstraint_4 = Instance.new("UITextSizeConstraint")
local False_2 = Instance.new("TextButton")
local UICorner_13 = Instance.new("UICorner")
local Frame = Instance.new("Frame")
local UICorner_14 = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")
local UITextSizeConstraint_5 = Instance.new("UITextSizeConstraint")
local TextLabel_2 = Instance.new("TextLabel")
local UITextSizeConstraint_6 = Instance.new("UITextSizeConstraint")
local AutoFarm = Instance.new("TextButton")
local UITextSizeConstraint_7 = Instance.new("UITextSizeConstraint")
local TextButton = Instance.new("TextButton")
local UICorner_15 = Instance.new("UICorner")
local UITextSizeConstraint_8 = Instance.new("UITextSizeConstraint")

--Properties:

CoolNewGui.Name = "CoolNewGui"
CoolNewGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
CoolNewGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

HackFrame.Name = "HackFrame"
HackFrame.Parent = CoolNewGui
HackFrame.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
HackFrame.Position = UDim2.new(0.271481305, 0, 0.212972984, 0)
HackFrame.Size = UDim2.new(0.249341071, 0, 0.358918905, 0)

UICorner.Parent = HackFrame

BGFrame.Name = "BGFrame"
BGFrame.Parent = HackFrame
BGFrame.BackgroundColor3 = Color3.fromRGB(33, 33, 33)
BGFrame.BorderColor3 = Color3.fromRGB(255, 0, 4)
BGFrame.Position = UDim2.new(0.0147991544, 0, 0.0150602404, 0)
BGFrame.Size = UDim2.new(0.970401704, 0, 0.966867447, 0)

UICorner_2.Parent = BGFrame

FrameFarm.Name = "FrameFarm"
FrameFarm.Parent = BGFrame
FrameFarm.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
FrameFarm.BackgroundTransparency = 1.000
FrameFarm.Position = UDim2.new(0.387799561, 0, 0.0186915882, 0)
FrameFarm.Size = UDim2.new(0.575163424, 0, 0.940809965, 0)

AutoFarmFrame.Name = "AutoFarmFrame"
AutoFarmFrame.Parent = FrameFarm
AutoFarmFrame.BackgroundColor3 = Color3.fromRGB(81, 81, 81)
AutoFarmFrame.Position = UDim2.new(0.0189393945, 0, 0.029801324, 0)
AutoFarmFrame.Size = UDim2.new(0.962121189, 0, 0.11258278, 0)

UICorner_3.Parent = AutoFarmFrame

Eei.Name = "Eei"
Eei.Parent = AutoFarmFrame
Eei.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Eei.Position = UDim2.new(0.051181104, 0, 0.205882356, 0)
Eei.Size = UDim2.new(0.0787401572, 0, 0.5, 0)

UICorner_4.CornerRadius = UDim.new(8, 8)
UICorner_4.Parent = Eei

AutoFarmText.Name = "AutoFarmText"
AutoFarmText.Parent = AutoFarmFrame
AutoFarmText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
AutoFarmText.BackgroundTransparency = 1.000
AutoFarmText.Position = UDim2.new(0.0905511826, 0, 0.205882356, 0)
AutoFarmText.Size = UDim2.new(0.555118084, 0, 0.558823526, 0)
AutoFarmText.Text = "Auto-Farm"
AutoFarmText.TextColor3 = Color3.fromRGB(255, 255, 255)
AutoFarmText.TextScaled = true
AutoFarmText.TextSize = 14.000
AutoFarmText.TextStrokeTransparency = 0.000
AutoFarmText.TextWrapped = true

UITextSizeConstraint.Parent = AutoFarmText
UITextSizeConstraint.MaxTextSize = 25

Eisc.Name = "Eisc"
Eisc.Parent = AutoFarmFrame
Eisc.BackgroundColor3 = Color3.fromRGB(232, 232, 232)
Eisc.Position = UDim2.new(0.779527545, 0, 0.264705896, 0)
Eisc.Size = UDim2.new(0.145669296, 0, 0.411764711, 0)

UICorner_5.CornerRadius = UDim.new(8, 8)
UICorner_5.Parent = Eisc

True.Name = "True"
True.Parent = AutoFarmFrame
True.BackgroundColor3 = Color3.fromRGB(38, 255, 0)
True.Position = UDim2.new(0.0629921257, 0, 1.08823526, 0)
True.Size = UDim2.new(0.236220479, 0, 1.05882359, 0)
True.Font = Enum.Font.SourceSans
True.Text = "เริ่ม"
True.TextColor3 = Color3.fromRGB(255, 255, 255)
True.TextScaled = true
True.TextSize = 14.000
True.TextStrokeTransparency = 0.000
True.TextWrapped = true

UICorner_6.Parent = True

Stats.Name = "Stats"
Stats.Parent = AutoFarmFrame
Stats.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Stats.BackgroundTransparency = 1.000
Stats.Position = UDim2.new(0.0511811003, 0, 2.14705896, 0)
Stats.Size = UDim2.new(0.905511796, 0, 0.735294104, 0)
Stats.Text = "ออโต้ฟาร์ม สถานะ : ปิด"
Stats.TextColor3 = Color3.fromRGB(255, 255, 255)
Stats.TextScaled = true
Stats.TextSize = 14.000
Stats.TextStrokeTransparency = 0.000
Stats.TextWrapped = true

UITextSizeConstraint_2.Parent = Stats
UITextSizeConstraint_2.MaxTextSize = 25

False.Name = "False"
False.Parent = AutoFarmFrame
False.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
False.Position = UDim2.new(0.688976407, 0, 0.99999994, 0)
False.Size = UDim2.new(0.236220479, 0, 1.05882359, 0)
False.Font = Enum.Font.SourceSans
False.Text = "หยุด"
False.TextColor3 = Color3.fromRGB(255, 255, 255)
False.TextScaled = true
False.TextSize = 14.000
False.TextStrokeTransparency = 0.000
False.TextWrapped = true

UICorner_7.Parent = False

TextBoxtool.Name = "TextBoxtool"
TextBoxtool.Parent = FrameFarm
TextBoxtool.BackgroundColor3 = Color3.fromRGB(90, 90, 90)
TextBoxtool.Position = UDim2.new(0.0749965385, 0, 0.435450464, 0)
TextBoxtool.Size = UDim2.new(0.848398328, 0, 0.151300579, 0)
TextBoxtool.Font = Enum.Font.SourceSans
TextBoxtool.Text = "ชื่อไอเท็ม"
TextBoxtool.TextColor3 = Color3.fromRGB(255, 255, 255)
TextBoxtool.TextScaled = true
TextBoxtool.TextSize = 14.000
TextBoxtool.TextStrokeTransparency = 0.000
TextBoxtool.TextWrapped = true

UICorner_8.Parent = TextBoxtool

ToolEquip.Name = "ToolEquip"
ToolEquip.Parent = FrameFarm
ToolEquip.BackgroundColor3 = Color3.fromRGB(81, 81, 81)
ToolEquip.Position = UDim2.new(0.0189393945, 0, 0.635003626, 0)
ToolEquip.Size = UDim2.new(0.962121189, 0, 0.11258278, 0)

UICorner_9.Parent = ToolEquip

Eei_2.Name = "Eei"
Eei_2.Parent = ToolEquip
Eei_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Eei_2.Position = UDim2.new(0.051181104, 0, 0.205882356, 0)
Eei_2.Size = UDim2.new(0.0787401572, 0, 0.5, 0)

UICorner_10.CornerRadius = UDim.new(8, 8)
UICorner_10.Parent = Eei_2

AAAAAAA.Name = "AAAAAAA"
AAAAAAA.Parent = ToolEquip
AAAAAAA.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
AAAAAAA.BackgroundTransparency = 1.000
AAAAAAA.Position = UDim2.new(0.0905511826, 0, 0.205882356, 0)
AAAAAAA.Size = UDim2.new(0.555118084, 0, 0.558823526, 0)
AAAAAAA.Text = "ถือไอเท็มออโต้"
AAAAAAA.TextColor3 = Color3.fromRGB(255, 255, 255)
AAAAAAA.TextScaled = true
AAAAAAA.TextSize = 14.000
AAAAAAA.TextStrokeTransparency = 0.000
AAAAAAA.TextWrapped = true

UITextSizeConstraint_3.Parent = AAAAAAA
UITextSizeConstraint_3.MaxTextSize = 25

Eisc_2.Name = "Eisc"
Eisc_2.Parent = ToolEquip
Eisc_2.BackgroundColor3 = Color3.fromRGB(232, 232, 232)
Eisc_2.Position = UDim2.new(0.779527545, 0, 0.264705896, 0)
Eisc_2.Size = UDim2.new(0.145669296, 0, 0.411764711, 0)

UICorner_11.CornerRadius = UDim.new(8, 8)
UICorner_11.Parent = Eisc_2

True_2.Name = "True"
True_2.Parent = ToolEquip
True_2.BackgroundColor3 = Color3.fromRGB(38, 255, 0)
True_2.Position = UDim2.new(0.0629921257, 0, 1.08823526, 0)
True_2.Size = UDim2.new(0.236220479, 0, 1.05882359, 0)
True_2.Font = Enum.Font.SourceSans
True_2.Text = "เปิด"
True_2.TextColor3 = Color3.fromRGB(255, 255, 255)
True_2.TextScaled = true
True_2.TextSize = 14.000
True_2.TextStrokeTransparency = 0.000
True_2.TextWrapped = true

UICorner_12.Parent = True_2

Stats_2.Name = "Stats"
Stats_2.Parent = ToolEquip
Stats_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Stats_2.BackgroundTransparency = 1.000
Stats_2.Position = UDim2.new(0.0511811003, 0, 2.14705896, 0)
Stats_2.Size = UDim2.new(0.905511796, 0, 0.735294104, 0)
Stats_2.Text = "ถือไอเท็มออโต้ สถานะ  : None"
Stats_2.TextColor3 = Color3.fromRGB(255, 255, 255)
Stats_2.TextScaled = true
Stats_2.TextSize = 14.000
Stats_2.TextStrokeTransparency = 0.000
Stats_2.TextWrapped = true

UITextSizeConstraint_4.Parent = Stats_2
UITextSizeConstraint_4.MaxTextSize = 25

False_2.Name = "False"
False_2.Parent = ToolEquip
False_2.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
False_2.Position = UDim2.new(0.688976407, 0, 0.99999994, 0)
False_2.Size = UDim2.new(0.236220479, 0, 1.05882359, 0)
False_2.Font = Enum.Font.SourceSans
False_2.Text = "หยุด"
False_2.TextColor3 = Color3.fromRGB(255, 255, 255)
False_2.TextScaled = true
False_2.TextSize = 14.000
False_2.TextStrokeTransparency = 0.000
False_2.TextWrapped = true

UICorner_13.Parent = False_2

Frame.Parent = HackFrame
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.Position = UDim2.new(0.0126849888, 0, 0.0150602404, 0)
Frame.Size = UDim2.new(0.357293874, 0, 0.966867447, 0)

UICorner_14.Parent = Frame

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.Position = UDim2.new(0.035502959, 0, 0.0186915882, 0)
TextLabel.Size = UDim2.new(0.911242604, 0, 0.0841121525, 0)
TextLabel.Text = "Blox Fruit [มือถือ]"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextStrokeTransparency = 0.000
TextLabel.TextWrapped = true

UITextSizeConstraint_5.Parent = TextLabel
UITextSizeConstraint_5.MaxTextSize = 20

TextLabel_2.Parent = Frame
TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.BackgroundTransparency = 1.000
TextLabel_2.Position = UDim2.new(0.035502959, 0, 0.0934579447, 0)
TextLabel_2.Size = UDim2.new(0.804733753, 0, 0.0685358271, 0)
TextLabel_2.Text = "สโม๊คเทส"
TextLabel_2.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.TextScaled = true
TextLabel_2.TextSize = 14.000
TextLabel_2.TextStrokeTransparency = 0.000
TextLabel_2.TextTransparency = 0.210
TextLabel_2.TextWrapped = true

UITextSizeConstraint_6.Parent = TextLabel_2
UITextSizeConstraint_6.MaxTextSize = 18

AutoFarm.Name = "ฟาร์ม"
AutoFarm.Parent = Frame
AutoFarm.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
AutoFarm.BorderColor3 = Color3.fromRGB(0, 0, 0)
AutoFarm.Position = UDim2.new(0.0118343197, 0, 0.196261689, 0)
AutoFarm.Size = UDim2.new(0.988165677, 0, 0.115264796, 0)
AutoFarm.Text = "AutoFarm"
AutoFarm.TextColor3 = Color3.fromRGB(203, 203, 203)
AutoFarm.TextScaled = true
AutoFarm.TextSize = 13.000
AutoFarm.TextStrokeTransparency = 0.000
AutoFarm.TextWrapped = true

UITextSizeConstraint_7.Parent = AutoFarm
UITextSizeConstraint_7.MaxTextSize = 15

TextButton.Parent = CoolNewGui
TextButton.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
TextButton.Position = UDim2.new(0.224565104, 0, 0.0108108111, 0)
TextButton.Size = UDim2.new(0.031101739, 0, 0.0551351346, 0)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = ""
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextScaled = true
TextButton.TextSize = 14.000
TextButton.TextWrapped = true

UICorner_15.Parent = TextButton

UITextSizeConstraint_8.Parent = TextButton
UITextSizeConstraint_8.MaxTextSize = 14

-- Scripts:

local function XMRS_fake_script() -- HackFrame.RGB_Script 
	local script = Instance.new('LocalScript', HackFrame)

	-- Made By Auradomix --
	-- Visit My Channel On YT and Twitch = @Auradomix
	
	-- PUT "RGB_GUI" ON STARTERGUI
	-- PUT THIS ON ANY FRAME OR BUTTON OR BOX OR ...
	-- ONLY ADAPTED FOR GUI, Please Referance To my Other Model For Brick
	
	-- Local Script = Client
	-- Script = Server
	
	-- For more fast Server Put them as a Local Scrpit for Gui
	
	while wait() do
		script.Parent.BackgroundColor3 = Color3.new(255/255,0/255,0/255)
		for i = 0,255,10 do
			wait()
			script.Parent.BackgroundColor3 = Color3.new(255/255,i/255,0/255)
		end
		for i = 255,0,-10 do
			wait()
			script.Parent.BackgroundColor3 = Color3.new(i/255,255/255,0/255)
		end
		for i = 0,255,10 do
			wait()
			script.Parent.BackgroundColor3 = Color3.new(0/255,255/255,i/255)
		end
		for i = 255,0,-10 do
			wait()
			script.Parent.BackgroundColor3 = Color3.new(0/255,i/255,255/255)
		end
		for i = 0,255,10 do
			wait()
			script.Parent.BackgroundColor3 = Color3.new(i/255,0/255,255/255)
		end
		for i = 255,0,-10 do
			wait()
			script.Parent.BackgroundColor3 = Color3.new(255/255,0/255,i/255)
		end
	end
end
coroutine.wrap(XMRS_fake_script)()
local function EBZK_fake_script() -- True.LocalScript 
	local script = Instance.new('LocalScript', True)

	script.Parent.MouseButton1Click:Connect(function()
		_G.autofarmworld3 = true
	
		while _G.autofarmworld3 do wait()
			pcall(function()
				local MyLevel = game.Players.LocalPlayer.Data.Level.Value
				for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
					if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
						if MyLevel == 1500 or MyLevel <= 1524 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-285.56527709961, 43.793357849121, 5566.9194335938)
							wait(1.5)
							Ms = "Pirate Millionaire [Lv. 1500]"
							NaemQuest = "PiratePortQuest"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1525 or MyLevel <= 1574 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-441.63903808594, 118.92677307129, 5972.6767578125)
							wait(1.5)
							Ms = "Pistol Billionaire [Lv. 1525]"
							NaemQuest = "PiratePortQuest"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1575 or MyLevel <= 1599 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(6243.9326171875, 51.522083282471, -1307.4636230469)
							wait(1.5)
							Ms = "Dragon Crew Warrior [Lv. 1575]"
							NaemQuest = "AmazonQuest"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1600 or MyLevel <= 1624 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(6721.1928710938, 432.10375976563, 113.82357788086)
							wait(1.5)
							Ms = "Dragon Crew Archer [Lv. 1600]"
							NaemQuest = "AmazonQuest"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1625 or MyLevel <= 1649 then
						    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5389.7250976563, 670.49377441406, 601.73083496094)
						    wait(1.5)
							Ms = "Female Islander [Lv. 1625]"
							NaemQuest = "AmazonQuest2"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1650 or MyLevel <= 1699 then
						    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4543.9096679688, 656.75701904297, -105.84915924072)
						    wait(1.5)
						    Ms = "Giant Islander [Lv. 1650]"
							NaemQuest = "AmazonQuest2"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1700 or MyLevel <= 1724 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2270.876953125, 73.175827026367, -7107.5649414063)
							wait(1.5)
							Ms = "Marine Commodore [Lv. 1700]"
							NaemQuest = "MarineTreeIsland"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1725 or MyLevel <= 1774 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(3661.6530761719, 160.54985046387, -7030.3237304688)
							wait(1.5)
							Ms = "Marine Rear Admiral [Lv. 1725]"
							NaemQuest = "MarineTreeIsland"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1775 or MyLevel <= 1799 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10590.745117188, 331.78845214844, -8738.7666015625)
							wait(1.5)
							Ms = "Fishman Raider [Lv. 1775]"
							NaemQuest = "DeepForestIsland3"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1800 or MyLevel <= 1824 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10590.745117188, 331.78845214844, -8738.7666015625)
							wait(1.5)
							Ms = "Fishman Captain [Lv. 1800]"
							NaemQuest = "DeepForestIsland3"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1825 or MyLevel <= 1849 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13217.8515625, 332.40396118164, -7647.9262695313)
							wait(1.5)
							Ms = "Forest Pirate [Lv. 1825]"
							NaemQuest = "DeepForestIsland"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1850 or MyLevel <= 1899 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13188.842773438, 622.64276123047, -7008.4184570313)
							wait(1.5)
							Ms = "Mythological Pirate [Lv. 1850]"
							NaemQuest = "DeepForestIsland"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1900 or MyLevel <= 1925 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12111.450195313, 443.05541992188, -10545.873046875)
							wait(1.5)
							Ms = "Jungle Pirate [Lv. 1900]"
							NaemQuest = "DeepForestIsland2"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel > 1925 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13154.280273438, 576.67321777344, -10078.7890625)
							wait(1.5)
							Ms = "Musketeer Pirate [Lv. 1925]"
							NaemQuest = "DeepForestIsland2"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						end
					elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if v.Name == Ms then
							repeat wait()
								game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
								v.HumanoidRootPart.Size = Vector3.new(60,30,60)
								v.HumanoidRootPart.CanCollide = true						
								v.HumanoidRootPart.Transparency = 0.7
							until v.Humanoid.Health <= 0 or not _G.autofarmworld3
						end
					end
				end
			end)
		end
	end)
end
coroutine.wrap(EBZK_fake_script)()
local function SDPSEKQ_fake_script() -- True.LocalScript 
	local script = Instance.new('LocalScript', True)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Stats.Text = "Auto Farm Stats : OPEN"
	end)
end
coroutine.wrap(SDPSEKQ_fake_script)()
local function BBDVA_fake_script() -- False.LocalScript 
	local script = Instance.new('LocalScript', False)

	script.Parent.MouseButton1Click:Connect(function()
		_G.autofarmworld3 = false
	
		while _G.autofarmworld3 do wait()
			pcall(function()
				local MyLevel = game.Players.LocalPlayer.Data.Level.Value
				for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
					if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
						if MyLevel == 1500 or MyLevel <= 1524 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-285.56527709961, 43.793357849121, 5566.9194335938)
							wait(1.5)
							Ms = "Pirate Millionaire [Lv. 1500]"
							NaemQuest = "PiratePortQuest"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1525 or MyLevel <= 1574 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-441.63903808594, 118.92677307129, 5972.6767578125)
							wait(1.5)
							Ms = "Pistol Billionaire [Lv. 1525]"
							NaemQuest = "PiratePortQuest"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1575 or MyLevel <= 1599 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(6243.9326171875, 51.522083282471, -1307.4636230469)
							wait(1.5)
							Ms = "Dragon Crew Warrior [Lv. 1575]"
							NaemQuest = "AmazonQuest"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1600 or MyLevel <= 1624 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(6721.1928710938, 432.10375976563, 113.82357788086)
							wait(1.5)
							Ms = "Dragon Crew Archer [Lv. 1600]"
							NaemQuest = "AmazonQuest"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1625 or MyLevel <= 1649 then
						    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5389.7250976563, 670.49377441406, 601.73083496094)
						    wait(1.5)
							Ms = "Female Islander [Lv. 1625]"
							NaemQuest = "AmazonQuest2"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1650 or MyLevel <= 1699 then
						    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4543.9096679688, 656.75701904297, -105.84915924072)
						    wait(1.5)
						    Ms = "Giant Islander [Lv. 1650]"
							NaemQuest = "AmazonQuest2"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1700 or MyLevel <= 1724 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2270.876953125, 73.175827026367, -7107.5649414063)
							wait(1.5)
							Ms = "Marine Commodore [Lv. 1700]"
							NaemQuest = "MarineTreeIsland"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1725 or MyLevel <= 1774 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(3661.6530761719, 160.54985046387, -7030.3237304688)
							wait(1.5)
							Ms = "Marine Rear Admiral [Lv. 1725]"
							NaemQuest = "MarineTreeIsland"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1775 or MyLevel <= 1799 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10590.745117188, 331.78845214844, -8738.7666015625)
							wait(1.5)
							Ms = "Fishman Raider [Lv. 1775]"
							NaemQuest = "DeepForestIsland3"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1800 or MyLevel <= 1824 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10590.745117188, 331.78845214844, -8738.7666015625)
							wait(1.5)
							Ms = "Fishman Captain [Lv. 1800]"
							NaemQuest = "DeepForestIsland3"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1825 or MyLevel <= 1849 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13217.8515625, 332.40396118164, -7647.9262695313)
							wait(1.5)
							Ms = "Forest Pirate [Lv. 1825]"
							NaemQuest = "DeepForestIsland"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1850 or MyLevel <= 1899 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13188.842773438, 622.64276123047, -7008.4184570313)
							wait(1.5)
							Ms = "Mythological Pirate [Lv. 1850]"
							NaemQuest = "DeepForestIsland"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel == 1900 or MyLevel <= 1925 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12111.450195313, 443.05541992188, -10545.873046875)
							wait(1.5)
							Ms = "Jungle Pirate [Lv. 1900]"
							NaemQuest = "DeepForestIsland2"
							LevelQuest = 1
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						elseif MyLevel > 1925 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13154.280273438, 576.67321777344, -10078.7890625)
							wait(1.5)
							Ms = "Musketeer Pirate [Lv. 1925]"
							NaemQuest = "DeepForestIsland2"
							LevelQuest = 2
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
						end
					elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if v.Name == Ms then
							repeat wait()
								game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
								v.HumanoidRootPart.Size = Vector3.new(60,30,60)
								v.HumanoidRootPart.CanCollide = true						
								v.HumanoidRootPart.Transparency = 0.7
							until v.Humanoid.Health <= 0 or not _G.autofarmworld3
						end
					end
				end
			end)
		end
	end)
end
coroutine.wrap(BBDVA_fake_script)()
local function WGKQQZ_fake_script() -- False.LocalScript 
	local script = Instance.new('LocalScript', False)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Stats.Text = "Auto Farm Stats : Close"
	end)
end
coroutine.wrap(WGKQQZ_fake_script)()
local function KYWXN_fake_script() -- True_2.LocalScript 
	local script = Instance.new('LocalScript', True_2)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Stats.Text = "Auto Equip Tool Stats : OPEN"
	end)
end
coroutine.wrap(KYWXN_fake_script)()
local function JRQFQVJ_fake_script() -- True_2.LocalScript 
	local script = Instance.new('LocalScript', True_2)

	script.Parent.MouseButton1Click:Connect(function()
		_G.equiptoolss = true
		while _G.equiptoolss do wait()
		    pcall(function()
			local ToolName = script.Parent.Parent.Parent.TextBoxtool.Text
			local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolName)
			game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
			end)
		end
	end)
end
coroutine.wrap(JRQFQVJ_fake_script)()
local function PXHVCN_fake_script() -- False_2.LocalScript 
	local script = Instance.new('LocalScript', False_2)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Stats.Text = "Auto Equip Tool Stats : Close"
	end)
end
coroutine.wrap(PXHVCN_fake_script)()
local function CSXEYU_fake_script() -- False_2.LocalScript 
	local script = Instance.new('LocalScript', False_2)

	script.Parent.MouseButton1Click:Connect(function()
		_G.equiptoolss = false
		while _G.equiptoolss do wait()
		    pcall(function()
			local ToolName = script.Parent.Parent.Parent.TextBoxtool.Text
	local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolName)
	game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end)
		end
		end)
end
coroutine.wrap(CSXEYU_fake_script)()
local function UEEN_fake_script() -- AutoFarm.LocalScript 
	local script = Instance.new('LocalScript', AutoFarm)

	script.Parent.MouseButton1Click:Connect(function()
		if script.Parent.Parent.Parent.BGFrame.FrameFarm.Visible == false then
		script.Parent.BackgroundColor3 = Color3.fromRGB(47, 47, 47)
		wait()
			script.Parent.Parent.Parent.BGFrame.FrameFarm.Visible = true
		elseif script.Parent.Parent.Parent.BGFrame.FrameFarm.Visible == true then
		script.Parent.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
		wait()
			script.Parent.Parent.Parent.BGFrame.FrameFarm.Visible = false
		end	
	end)
	
end
coroutine.wrap(UEEN_fake_script)()
local function AUABBJ_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

	script.Parent.MouseButton1Click:Connect(function()
		if script.Parent.Parent.HackFrame.Visible == false then
			script.Parent.Parent.HackFrame.Visible = true
			script.Parent.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
		elseif script.Parent.Parent.HackFrame.Visible == true then
			script.Parent.Parent.HackFrame.Visible = false
			script.Parent.BackgroundColor3 = Color3.fromRGB(0, 255, 0)
		end
	end)
end
coroutine.wrap(AUABBJ_fake_script)()
