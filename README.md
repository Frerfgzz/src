if game:GetService("StarterGui"):SetCore("SendNotification",
    {
        Title = "SMZ HUB Blox Fruit",
        Text = "Loading.....",
        Icon = "http://www.roblox.com/asset/?id=8873625488",
        Duration = 4
    }
   ) then
    wait(20)
end

repeat wait(5) until game:IsLoaded()

if game.CoreGui:FindFirstChild("LLL") then
    game.CoreGui:FindFirstChild("LLL"):Destroy()
end

local LLL = Instance.new("ScreenGui")
local LLLL = Instance.new("TextButton")
local LLLLL = Instance.new("UICorner")
local LLLLLL = Instance.new("ImageLabel")

LLL.Name = "LLL"
        LLL.Parent = game.CoreGui
        LLL.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

        LLLL.Name = "LLLL"
        LLLL.Parent = LLL
        LLLL.BackgroundColor3 = Color3.fromRGB(30,20,20)
        LLLL.BorderSizePixel = 0
        LLLL.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
        LLLL.Size = UDim2.new(0, 50, 0, 50)
        LLLL.Font = Enum.Font.SourceSans
        LLLL.Text = ""
        LLLL.TextColor3 = Color3.fromRGB(0, 0, 0)
        LLLL.TextSize = 14.000
        LLLL.Draggable = true
        LLLL.MouseButton1Click:Connect(function()
        game.CoreGui:FindFirstChild("NBTxTP Lib").Enabled = not game.CoreGui:FindFirstChild("NBTxTP Lib").Enabled
        end)
        do
        if game:GetService("CoreGui"):FindFirstChild("NBTxTP Lib") then
        end
        end

        LLLLL.Name = "LLLLL"
        LLLLL.Parent = LLLL

        LLLLLL.Name = "LLLLLL"
        LLLLLL.Parent = LLLL
        LLLLLL.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        LLLLLL.BackgroundTransparency = 1.000
        LLLLLL.BorderSizePixel = 0
        LLLLLL.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
        LLLLLL.Size = UDim2.new(0, 39, 0, 39)
        LLLLLL.Image = "http://www.roblox.com/asset/?id=8873625488"


if game:GetService("StarterGui"):SetCore("SendNotification",
    {
        Title = "SMZHUB",
        Text = "Blox Fruit Free Script",
        Icon = "http://roblox.com/asset/?id=8873625488",
        Duration = 4
    }
   ) then
    wait(20)
end

OldWorld = false
NewWorld = false
ThreeWorld = false
local placeId = game.PlaceId
if placeId == 2753915549 then
    OldWorld = true
elseif placeId == 4442272183 then
    NewWorld = true
elseif placeId == 7449423635 then
	ThreeWorld = true
end

FM = false
sky = false

function CheckQuestSMZHUB()
    if OldWorld then
        local MyLevel = game.Players.LocalPlayer.Data.Level.Value
        Dis = 300
        if MyLevel == 1 or MyLevel <= 9 then -- Bandit
            magbring = 400
            Ms = "Bandit [Lv. 5]"
            NaemQuest = "BanditQuest1"
            LevelQuest = 1
            NameMon = "Bandit"
            CFrameQuest = CFrame.new(1061.66699, 16.5166187, 1544.52905, -0.942978859, -3.33851502e-09, 0.332852632, 7.04340497e-09, 1, 2.99841325e-08, -0.332852632, 3.06188177e-08, -0.942978859)
            CFrameMon = CFrame.new(1199.31287, 52.2717781, 1536.91516, -0.929782331, 6.60215846e-08, -0.368109822, 3.9077392e-08, 1, 8.06501603e-08, 0.368109822, 6.06023249e-08, -0.929782331)
        elseif MyLevel == 10 or MyLevel <= 14 then -- Monkey
            magbring = 400
            Ms = "Monkey [Lv. 14]"
            NaemQuest = "JungleQuest"
            LevelQuest = 1
            NameMon = "Monkey"
            CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
            CFrameMon = CFrame.new(-1502.74609, 98.5633316, 90.6417007, 0.836947978, 0, 0.547282517, -0, 1, -0, -0.547282517, 0, 0.836947978)
        elseif MyLevel == 15 or MyLevel <= 29 then -- Gorilla
            magbring = 240
            Ms = "Gorilla [Lv. 20]"
            NaemQuest = "JungleQuest"
            LevelQuest = 2
            NameMon = "Gorilla"
            CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
            CFrameMon = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
        elseif MyLevel == 30 or MyLevel <= 39 then -- Pirate
            Dis = 150
            Ms = "Pirate [Lv. 35]"
            NaemQuest = "BuggyQuest1"
            LevelQuest = 1
            NameMon = "Pirate"
            CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
            CFrameMon = CFrame.new(-1219.32324, 4.75205183, 3915.63452, -0.966492832, -6.91238853e-08, 0.25669381, -5.21195496e-08, 1, 7.3047012e-08, -0.25669381, 5.72206496e-08, -0.966492832)
        elseif MyLevel == 40 or MyLevel <= 59 then -- Brute
            Dis = 150
            Ms = "Brute [Lv. 45]"
            NaemQuest = "BuggyQuest1"
            LevelQuest = 2
            NameMon = "Brute"
            CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
            CFrameMon = CFrame.new(-1146.49646, 96.0936813, 4312.1333, -0.978175163, -1.53222057e-08, 0.207781896, -3.33316912e-08, 1, -8.31738873e-08, -0.207781896, -8.82843523e-08, -0.978175163)
        elseif MyLevel == 60 or MyLevel <= 74 then -- Desert Bandit
            Ms = "Desert Bandit [Lv. 60]"
            NaemQuest = "DesertQuest"
            LevelQuest = 1
            NameMon = "Desert Bandit"
            CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
            CFrameMon = CFrame.new(932.788818, 6.4503746, 4488.24609, -0.998625934, 3.08948351e-08, 0.0524050146, 2.79967303e-08, 1, -5.60361286e-08, -0.0524050146, -5.44919629e-08, -0.998625934)
        elseif MyLevel == 75 or MyLevel <= 89 then -- Desert Officre
            Ms = "Desert Officer [Lv. 70]"
            NaemQuest = "DesertQuest"
            LevelQuest = 2
            NameMon = "Desert Officer"
            CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
            CFrameMon = CFrame.new(1580.03198, 4.61375761, 4366.86426, 0.135744005, -6.44280718e-08, -0.990743816, 4.35738308e-08, 1, -5.90598574e-08, 0.990743816, -3.51534837e-08, 0.135744005)
        elseif MyLevel == 90 or MyLevel <= 99 then -- Snow Bandits
            Ms = "Snow Bandit [Lv. 90]"
            NaemQuest = "SnowQuest"
            LevelQuest = 1
            NameMon = "Snow Bandits"
            CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
            CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
        elseif MyLevel == 100 or MyLevel <= 119 then -- Snowman
            Ms = "Snowman [Lv. 100]"
            NaemQuest = "SnowQuest"
            LevelQuest = 2
            NameMon = "Snowman"
            CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
            CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
        elseif MyLevel == 120 or MyLevel <= 149 then -- Chief Petty Officer
            Ms = "Chief Petty Officer [Lv. 120]"
            NaemQuest = "MarineQuest2"
            LevelQuest = 1
            NameMon = "Chief Petty Officer"
            CFrameQuest = CFrame.new(-5035.0835, 28.6520386, 4325.29443, 0.0243340395, -7.08064647e-08, 0.999703884, -6.36926814e-08, 1, 7.23777944e-08, -0.999703884, -6.54350671e-08, 0.0243340395)
            CFrameMon = CFrame.new(-4882.8623, 22.6520386, 4255.53516, 0.273695946, -5.40380647e-08, -0.96181643, 4.37720793e-08, 1, -4.37274998e-08, 0.96181643, -3.01326679e-08, 0.273695946)
        elseif MyLevel == 150 or MyLevel <= 174 then -- Sky Bandit
            Ms = "Sky Bandit [Lv. 150]"
            NaemQuest = "SkyQuest"
            LevelQuest = 1
            NameMon = "Sky Bandit"
            CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
            CFrameMon = CFrame.new(-4970.74219, 294.544342, -2890.11353, -0.994874597, -8.61311236e-08, -0.101116329, -9.10836206e-08, 1, 4.43614923e-08, 0.101116329, 5.33441664e-08, -0.994874597)
        elseif MyLevel == 175 or MyLevel <= 189 then -- Dark Master
            Ms = "Dark Master [Lv. 175]"
            NaemQuest = "SkyQuest"
            LevelQuest = 2
            NameMon = "Dark Master"
            CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
            CFrameMon = CFrame.new(-5220.58594, 430.693298, -2278.17456, -0.925375521, 1.12086873e-08, 0.379051805, -1.05115507e-08, 1, -5.52320891e-08, -0.379051805, -5.50948407e-08, -0.925375521)
        elseif MyLevel == 190 or MyLevel <= 209 then
            Ms = "Prisoner [Lv. 190]"
            LevelQuest = 1
            NaemQuest = "PrisonerQuest"
            NameMon = "Prisoner"
            CFrameMon = CFrame.new(4937.40674, 15.6515369, 565.219666, -0.483960688, 1.04728592e-07, -0.875089705, 2.53960444e-08, 1, 1.05632488e-07, 0.875089705, 2.88981568e-08, -0.483960688)
            CFrameQuest = CFrame.new(5308.72119, 1.65511298, 474.088745, 0.391072512, 5.46925989e-08, -0.92035985, -1.40744483e-08, 1, 5.34448219e-08, 0.92035985, -7.94724375e-09, 0.391072512)
    
        elseif MyLevel == 210 or MyLevel <= 249 then
            Ms = "Dangerous Prisoner [Lv. 210]"
            LevelQuest = 2
            NaemQuest = "PrisonerQuest"
            NameMon = "Dangerous Prisoner"
            CFrameMon = CFrame.new(4937.40674, 15.6515369, 565.219666, -0.483960688, 1.04728592e-07, -0.875089705, 2.53960444e-08, 1, 1.05632488e-07, 0.875089705, 2.88981568e-08, -0.483960688)
            CFrameQuest = CFrame.new(5463.104, 15.6328878, 973.506042, -0.682176471, 4.0302389e-08, -0.731187582, 6.34130473e-08, 1, -4.04342249e-09, 0.731187582, -4.91251591e-08, -0.682176471)
        elseif MyLevel == 250 or MyLevel <= 274 then -- Toga Warrior
            Ms = "Toga Warrior [Lv. 250]"
            NaemQuest = "ColosseumQuest"
            LevelQuest = 1
            NameMon = "Toga Warrior"
            CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
            CFrameMon = CFrame.new(-1779.97583, 44.6077499, -2736.35474, 0.984437346, 4.10396339e-08, 0.175734788, -3.62286876e-08, 1, -3.05844168e-08, -0.175734788, 2.3741821e-08, 0.984437346)
        elseif MyLevel == 275 or MyLevel <= 299 then -- Gladiato
            Ms = "Gladiator [Lv. 275]"
            NaemQuest = "ColosseumQuest"
            LevelQuest = 2
            NameMon = "Gladiato"
            CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
            CFrameMon = CFrame.new(-1274.75903, 58.1895943, -3188.16309, 0.464524001, 6.21005611e-08, 0.885560572, -4.80449414e-09, 1, -6.76054768e-08, -0.885560572, 2.71497012e-08, 0.464524001)
        elseif MyLevel == 300 or MyLevel <= 324 then -- Military Soldier
            Ms = "Military Soldier [Lv. 300]"
            NaemQuest = "MagmaQuest"
            LevelQuest = 1
            NameMon = "Military Soldier"
            CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
            CFrameMon = CFrame.new(-5363.01123, 41.5056877, 8548.47266, -0.578253984, -3.29503091e-10, 0.815856814, 9.11209668e-08, 1, 6.498761e-08, -0.815856814, 1.11920997e-07, -0.578253984)
        elseif MyLevel == 325 or MyLevel <= 374 then -- Military Spy
            FM = false
            Ms = "Military Spy [Lv. 325]"
            NaemQuest = "MagmaQuest"
            LevelQuest = 2
            NameMon = "Military Spy"
            CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
            CFrameMon = CFrame.new(-5787.99023, 120.864456, 8762.25293, -0.188358366, -1.84706277e-08, 0.982100308, -1.23782129e-07, 1, -4.93306951e-09, -0.982100308, -1.22495649e-07, -0.188358366)
        elseif MyLevel == 375 or MyLevel <= 399 then -- Fishman Warrior
            FM = true
            Ms = "Fishman Warrior [Lv. 375]"
            NaemQuest = "FishmanQuest"
            LevelQuest = 1
            NameMon = "Fishman Warrior"
            CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
            CFrameMon = CFrame.new(60946.6094, 48.6735229, 1525.91687, -0.0817126185, 8.90751153e-08, 0.996655822, 2.00889794e-08, 1, -8.77269599e-08, -0.996655822, 1.28533992e-08, -0.0817126185)
        elseif MyLevel == 400 or MyLevel <= 449 then -- Fishman Commando
            FM = true
            Ms = "Fishman Commando [Lv. 400]"
            NaemQuest = "FishmanQuest"
            LevelQuest = 2
            NameMon = "Fishman Commando"
            CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
            CFrameMon = CFrame.new(61885.5039, 18.4828243, 1504.17896, 0.577502489, 0, -0.816389024, -0, 1.00000012, -0, 0.816389024, 0, 0.577502489)
        elseif MyLevel == 450 or MyLevel <= 474 then -- God's Guards
            FM = false
            Ms = "God's Guard [Lv. 450]"
            NaemQuest = "SkyExp1Quest"
            LevelQuest = 1
            NameMon = "God's Guards"
            CFrameQuest = CFrame.new(-4721.71436, 845.277161, -1954.20105, -0.999277651, -5.56969759e-09, 0.0380011722, -4.14751478e-09, 1, 3.75035256e-08, -0.0380011722, 3.73188307e-08, -0.999277651)
            CFrameMon = CFrame.new(-4716.95703, 853.089722, -1933.92542, -0.93441087, -6.77488776e-09, -0.356197298, 1.12145182e-08, 1, -4.84390199e-08, 0.356197298, -4.92565206e-08, -0.93441087)
        elseif MyLevel == 475 or MyLevel <= 524 then -- Shandas
            sky = false
            Ms = "Shanda [Lv. 475]"
            NaemQuest = "SkyExp1Quest"
            LevelQuest = 2
            NameMon = "Shandas"
            CFrameQuest = CFrame.new(-7863.63672, 5545.49316, -379.826324, 0.362120807, -1.98046344e-08, -0.93213129, 4.05822291e-08, 1, -5.48095125e-09, 0.93213129, -3.58431969e-08, 0.362120807)
            CFrameMon = CFrame.new(-7685.12354, 5601.05127, -443.171509, 0.150056243, 1.79768236e-08, -0.988677442, 6.67798661e-09, 1, 1.91962481e-08, 0.988677442, -9.48289181e-09, 0.150056243)
        elseif MyLevel == 525 or MyLevel <= 549 then -- Royal Squad
            sky = true
            Ms = "Royal Squad [Lv. 525]"
            NaemQuest = "SkyExp2Quest"
            LevelQuest = 1
            NameMon = "Royal Squad"
            CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
            CFrameMon = CFrame.new(-7685.02051, 5606.87842, -1442.729, 0.561947823, 7.69527464e-09, -0.827172697, -4.24974544e-09, 1, 6.41599973e-09, 0.827172697, -9.01838604e-11, 0.561947823)
        elseif MyLevel == 550 or MyLevel <= 624 then -- Royal Soldier
            Dis = 240
            sky = true
            Ms = "Royal Soldier [Lv. 550]"
            NaemQuest = "SkyExp2Quest"
            LevelQuest = 2
            NameMon = "Royal Soldier"
            CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
            CFrameMon = CFrame.new(-7864.44775, 5661.94092, -1708.22351, 0.998389959, 2.28686137e-09, -0.0567218624, 1.99431383e-09, 1, 7.54200258e-08, 0.0567218624, -7.54117195e-08, 0.998389959)
        elseif MyLevel == 625 or MyLevel <= 649 then -- Galley Pirate
            Dis = 240
            sky = false
            Ms = "Galley Pirate [Lv. 625]"
            NaemQuest = "FountainQuest"
            LevelQuest = 1
            NameMon = "Galley Pirate"
            CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
            CFrameMon = CFrame.new(5595.06982, 41.5013695, 3961.47095, -0.992138803, -2.11610267e-08, -0.125142589, -1.34249509e-08, 1, -6.26613996e-08, 0.125142589, -6.04887518e-08, -0.992138803)
        elseif MyLevel >= 650 then -- Galley Captain
            Dis = 240
            Ms = "Galley Captain [Lv. 650]"
            NaemQuest = "FountainQuest"
            LevelQuest = 2
            NameMon = "Galley Captain"
            CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
            CFrameMon = CFrame.new(5658.5752, 38.5361786, 4928.93506, -0.996873081, 2.12391046e-06, -0.0790185928, 2.16989656e-06, 1, -4.96097414e-07, 0.0790185928, -6.66008248e-07, -0.996873081)
        end
    elseif NewWorld then
        local MyLevel = game.Players.LocalPlayer.Data.Level.Value
        Dis = 240
        if MyLevel == 700 or MyLevel <= 724 then -- Raider [Lv. 700]
            Ms = "Raider [Lv. 700]"
            NaemQuest = "Area1Quest"
            LevelQuest = 1
            NameMon = "Raider"
            CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
            CFrameMon = CFrame.new(-737.026123, 39.1748352, 2392.57959, 0.272128761, 0, -0.962260842, -0, 1, -0, 0.962260842, 0, 0.272128761)
        elseif MyLevel == 725 or MyLevel <= 774 then -- Mercenary [Lv. 725]
            Ms = "Mercenary [Lv. 725]"
            NaemQuest = "Area1Quest"
            LevelQuest = 2
            NameMon = "Mercenary"
            CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
            CFrameMon = CFrame.new(-973.731995, 95.8733215, 1836.46936, 0.999135971, 2.02326991e-08, -0.0415605344, -1.90767793e-08, 1, 2.82094952e-08, 0.0415605344, -2.73922804e-08, 0.999135971)
        elseif MyLevel == 775 or MyLevel <= 799 then -- Swan Pirate [Lv. 775]
            Ms = "Swan Pirate [Lv. 775]"
            NaemQuest = "Area2Quest"
            LevelQuest = 1
            NameMon = "Swan Pirate"
            CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
            CFrameMon = CFrame.new(970.369446, 142.653198, 1217.3667, 0.162079468, -4.85452638e-08, -0.986777723, 1.03357589e-08, 1, -4.74980872e-08, 0.986777723, -2.50063148e-09, 0.162079468)
        elseif MyLevel == 800 or MyLevel <= 874 then -- Factory Staff [Lv. 800]
            Ms = "Factory Staff [Lv. 800]"
            NaemQuest = "Area2Quest"
            LevelQuest = 2
            NameMon = "Factory Staff"
            CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
            CFrameMon = CFrame.new(296.786499, 72.9948196, -57.1298141, -0.876037002, -5.32364979e-08, 0.482243896, -3.87658332e-08, 1, 3.99718729e-08, -0.482243896, 1.63222538e-08, -0.876037002)
        elseif MyLevel == 875 or MyLevel <= 899 then -- Marine Lieutenant [Lv. 875]
            Ms = "Marine Lieutenant [Lv. 875]"
            NaemQuest = "MarineQuest3"
            LevelQuest = 1
            NameMon = "Marine Lieutenant"
            CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
            CFrameMon = CFrame.new(-2913.26367, 73.0011826, -2971.64282, 0.910507619, 0, 0.413492233, 0, 1.00000012, 0, -0.413492233, 0, 0.910507619)
        elseif MyLevel == 900 or MyLevel <= 949 then -- Marine Captain [Lv. 900]
            Ms = "Marine Captain [Lv. 900]"
            NaemQuest = "MarineQuest3"
            LevelQuest = 2
            NameMon = "Marine Captain"
            CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
            CFrameMon = CFrame.new(-1868.67688, 73.0011826, -3321.66333, -0.971402287, 1.06502087e-08, 0.237439692, 3.68856199e-08, 1, 1.06050372e-07, -0.237439692, 1.11775684e-07, -0.971402287)
        elseif MyLevel == 950 or MyLevel <= 974 then -- Zombie [Lv. 950]
            Ms = "Zombie [Lv. 950]"
            NaemQuest = "ZombieQuest"
            LevelQuest = 1
            NameMon = "Zombie"
            CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
            CFrameMon = CFrame.new(-5634.83838, 126.067039, -697.665039, -0.992770672, 6.77618939e-09, 0.120025545, 1.65461245e-08, 1, 8.04023372e-08, -0.120025545, 8.18070234e-08, -0.992770672)
        elseif MyLevel == 975 or MyLevel <= 999 then -- Vampire [Lv. 975]
            Ms = "Vampire [Lv. 975]"
            NaemQuest = "ZombieQuest"
            LevelQuest = 2
            NameMon = "Vampire"
            CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
            CFrameMon = CFrame.new(-6030.32031, 6.4377408, -1313.5564, -0.856965423, 3.9138893e-08, -0.515373945, -1.12178942e-08, 1, 9.45958547e-08, 0.515373945, 8.68467822e-08, -0.856965423)
        elseif MyLevel == 1000 or MyLevel <= 1049 then -- Snow Trooper [Lv. 1000] **
            Ms = "Snow Trooper [Lv. 1000]"
            NaemQuest = "SnowMountainQuest"
            LevelQuest = 1
            NameMon = "Snow Trooper"
            CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
            CFrameMon = CFrame.new(535.893433, 401.457062, -5329.6958, -0.999524176, 0, 0.0308452044, 0, 1, -0, -0.0308452044, 0, -0.999524176)
        elseif MyLevel == 1050 or MyLevel <= 1099 then -- Winter Warrior [Lv. 1050]
            Ms = "Winter Warrior [Lv. 1050]"
            NaemQuest = "SnowMountainQuest"
            LevelQuest = 2
            NameMon = "Winter Warrior"
            CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
            CFrameMon = CFrame.new(1223.7417, 454.575226, -5170.02148, 0.473996818, 2.56845354e-08, 0.880526543, -5.62456428e-08, 1, 1.10811016e-09, -0.880526543, -5.00510211e-08, 0.473996818)
        elseif MyLevel == 1100 or MyLevel <= 1124 then -- Lab Subordinate [Lv. 1100]
            Ms = "Lab Subordinate [Lv. 1100]"
            NaemQuest = "IceSideQuest"
            LevelQuest = 1
            NameMon = "Lab Subordinate"
            CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
            CFrameMon = CFrame.new(-5769.2041, 37.9288292, -4468.38721, -0.569419742, -2.49055017e-08, 0.822046936, -6.96206541e-08, 1, -1.79282633e-08, -0.822046936, -6.74401548e-08, -0.569419742)
        elseif MyLevel == 1125 or MyLevel <= 1174 then -- Horned Warrior [Lv. 1125]
            Ms = "Horned Warrior [Lv. 1125]"
            NaemQuest = "IceSideQuest"
            LevelQuest = 2
            NameMon = "Horned Warrior"
            CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
            CFrameMon = CFrame.new(-6400.85889, 24.7645149, -5818.63574, -0.964845479, 8.65926566e-08, -0.262817472, 3.98261392e-07, 1, -1.13260398e-06, 0.262817472, -1.19745812e-06, -0.964845479)
        elseif MyLevel == 1175 or MyLevel <= 1199 then -- Magma Ninja [Lv. 1175]
            Ms = "Magma Ninja [Lv. 1175]"
            NaemQuest = "FireSideQuest"
            LevelQuest = 1
            NameMon = "Magma Ninja"
            CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
            CFrameMon = CFrame.new(-5496.65576, 58.6890411, -5929.76855, -0.885073781, 0, -0.465450764, 0, 1.00000012, -0, 0.465450764, 0, -0.885073781)
        elseif MyLevel == 1200 or MyLevel <= 1249 then -- Lava Pirate [Lv. 1200]
            Ms = "Lava Pirate [Lv. 1200]"
            NaemQuest = "FireSideQuest"
            LevelQuest = 2
            NameMon = "Lava Pirate"
            CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
            CFrameMon = CFrame.new(-5169.71729, 34.1234779, -4669.73633, -0.196780294, 0, 0.98044765, 0, 1.00000012, -0, -0.98044765, 0, -0.196780294)
        elseif MyLevel == 1250 or MyLevel <= 1274 then -- Ship Deckhand [Lv. 1250]
            Ms = "Ship Deckhand [Lv. 1250]"
            NaemQuest = "ShipQuest1"
            LevelQuest = 1
            NameMon = "Ship Deckhand"
            CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
            CFrameMon = CFrame.new(1163.80872, 138.288452, 33058.4258, -0.998580813, 5.49076979e-08, -0.0532564968, 5.57436763e-08, 1, -1.42118655e-08, 0.0532564968, -1.71604082e-08, -0.998580813)
        elseif MyLevel == 1275 or MyLevel <= 1299 then -- Ship Engineer [Lv. 1275]
            Ms = "Ship Engineer [Lv. 1275]"
            NaemQuest = "ShipQuest1"
            LevelQuest = 2
            NameMon = "Ship Engineer"
            CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
            CFrameMon = CFrame.new(916.666504, 44.0920448, 32917.207, -0.99746871, -4.85034697e-08, -0.0711069331, -4.8925461e-08, 1, 4.19294288e-09, 0.0711069331, 7.66126895e-09, -0.99746871)
        elseif MyLevel == 1300 or MyLevel <= 1324 then -- Ship Steward [Lv. 1300]
            Ms = "Ship Steward [Lv. 1300]"
            NaemQuest = "ShipQuest2"
            LevelQuest = 1
            NameMon = "Ship Steward"
            CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
            CFrameMon = CFrame.new(918.743286, 129.591064, 33443.4609, -0.999792814, -1.7070947e-07, -0.020350717, -1.72559169e-07, 1, 8.91351277e-08, 0.020350717, 9.2628369e-08, -0.999792814)
        elseif MyLevel == 1325 or MyLevel <= 1349 then -- Ship Officer [Lv. 1325]
            Ms = "Ship Officer [Lv. 1325]"
            NaemQuest = "ShipQuest2"
            LevelQuest = 2
            NameMon = "Ship Officer"
            CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
            CFrameMon = CFrame.new(786.051941, 181.474106, 33303.2969, 0.999285698, -5.32193063e-08, 0.0377905183, 5.68968588e-08, 1, -9.62386864e-08, -0.0377905183, 9.83201005e-08, 0.999285698)
        elseif MyLevel == 1350 or MyLevel <= 1374 then -- Arctic Warrior [Lv. 1350]
            Ms = "Arctic Warrior [Lv. 1350]"
            NaemQuest = "FrostQuest"
            LevelQuest = 1
            NameMon = "Arctic Warrior"
            CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
            CFrameMon = CFrame.new(5995.07471, 57.3188477, -6183.47314, 0.702747107, -1.53454167e-07, -0.711440146, -1.08168464e-07, 1, -3.22542007e-07, 0.711440146, 3.03620908e-07, 0.702747107)
        elseif MyLevel == 1375 or MyLevel <= 1424 then -- Snow Lurker [Lv. 1375]
            Ms = "Snow Lurker [Lv. 1375]"
            NaemQuest = "FrostQuest"
            LevelQuest = 2
            NameMon = "Snow Lurker"
            CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
            CFrameMon = CFrame.new(5518.00684, 60.5559731, -6828.80518, -0.650781393, -3.64292951e-08, 0.759265184, -4.07668654e-09, 1, 4.44854642e-08, -0.759265184, 2.58550248e-08, -0.650781393)
        elseif MyLevel == 1425 or MyLevel <= 1449 then -- Sea Soldier [Lv. 1425]
            Ms = "Sea Soldier [Lv. 1425]"
            NaemQuest = "ForgottenQuest"
            LevelQuest = 1
            NameMon = "Sea Soldier"
            CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
            CFrameMon = CFrame.new(-3029.78467, 66.944252, -9777.38184, -0.998552859, 1.09555076e-08, 0.0537791774, 7.79564235e-09, 1, -5.89660658e-08, -0.0537791774, -5.84614881e-08, -0.998552859)
        elseif MyLevel >= 1450 then -- Water Fighter [Lv. 1450]
            Ms = "Water Fighter [Lv. 1450]"
            NaemQuest = "ForgottenQuest"
            LevelQuest = 2
            NameMon = "Water Fighter"
            CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
            CFrameMon = CFrame.new(-3262.00098, 298.699615, -10553.6943, -0.233570755, -4.57538185e-08, 0.972339869, -5.80986068e-08, 1, 3.30992194e-08, -0.972339869, -4.87605725e-08, -0.233570755)
        end
    elseif ThreeWorld then
        local MyLevel =  game.Players.LocalPlayer.Data.Level.Value
        Dis = 240
        if MyLevel == 1500 or MyLevel <= 1524 then
            Ms = "Pirate Millionaire [Lv. 1500]"
            NaemQuest = "PiratePortQuest"
            LevelQuest = 1
            NameMon = "Pirate Millionaire"
            CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
        elseif MyLevel == 1525 or MyLevel <= 1574 then
            Ms = "Pistol Billionaire [Lv. 1525]"
            NaemQuest = "PiratePortQuest"
            LevelQuest = 2
            NameMon = "Pistol Billionaire"
            CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
        elseif MyLevel == 1575 or MyLevel <= 1599 then
            Ms = "Dragon Crew Warrior [Lv. 1575]"
            NaemQuest = "AmazonQuest"
            LevelQuest = 1
            NameMon = "Dragon Crew Warrior"
            CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
            CFrameMon = CFrame.new(6241.9951171875, 51.522083282471, -1243.9771728516)
        elseif MyLevel == 1600 or MyLevel <= 1624 then
            Ms = "Dragon Crew Archer [Lv. 1600]"
            NaemQuest = "AmazonQuest"
            LevelQuest = 2
            NameMon = "Dragon Crew Archer"
            CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
            CFrameMon = CFrame.new(6488.9155273438, 383.38375854492, -110.66246032715)
        elseif MyLevel == 1625 or MyLevel <= 1649 then
            Ms = "Female Islander [Lv. 1625]"
            NaemQuest = "AmazonQuest2"
            LevelQuest = 1
            NameMon = "Female Islander"
            CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            CFrameMon = CFrame.new(4770.4990234375, 758.95520019531, 1069.8680419922)
        elseif MyLevel == 1650 or MyLevel <= 1699 then
            Ms = "Giant Islander [Lv. 1650]"
            NaemQuest = "AmazonQuest2"
            LevelQuest = 2
            NameMon = "Giant Islander"
            CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            CFrameMon = CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789)
        elseif MyLevel == 1700 or MyLevel <= 1724 then
            Ms = "Marine Commodore [Lv. 1700]"
            NaemQuest = "MarineTreeIsland"
            LevelQuest = 1
            NameMon = "Marine Commodore"
            CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
            CFrameMon = CFrame.new(2490.0844726563, 190.4232635498, -7160.0502929688)
        elseif MyLevel == 1725 or MyLevel <= 1774 then
            Ms = "Marine Rear Admiral [Lv. 1725]"
            NaemQuest = "MarineTreeIsland"
            LevelQuest = 2
            NameMon = "Marine Rear Admiral"
            CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
            CFrameMon = CFrame.new(3951.3903808594, 229.11549377441, -6912.81640625)
        elseif MyLevel == 1775 or MyLevel <= 1799 then
            Ms = "Fishman Raider [Lv. 1775]"
            NaemQuest = "DeepForestIsland3"
            LevelQuest = 1
            NameMon = "Fishman Raider"
            CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            CFrameMon = CFrame.new(-10322.400390625, 390.94473266602, -8580.0908203125)
        elseif MyLevel == 1800 or MyLevel <= 1824 then
            Ms = "Fishman Captain [Lv. 1800]"
            NaemQuest = "DeepForestIsland3"
            LevelQuest = 2
            NameMon = "Fishman Captain"
            CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            CFrameMon = CFrame.new(-11194.541992188, 442.02795410156, -8608.806640625)
        elseif MyLevel == 1825 or MyLevel <= 1849 then
            Ms = "Forest Pirate [Lv. 1825]"
            NaemQuest = "DeepForestIsland"
            LevelQuest = 1
            NameMon = "Forest Pirate"
            CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
            CFrameMon = CFrame.new(-13225.809570313, 428.19387817383, -7753.1245117188)
        elseif MyLevel == 1850 or MyLevel <= 1899 then
            Ms = "Mythological Pirate [Lv. 1850]"
            NaemQuest = "DeepForestIsland"
            LevelQuest = 2
            NameMon = "Mythological Pirate"
            CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
            CFrameMon = CFrame.new(-13869.172851563, 564.95251464844, -7084.4135742188)
        elseif MyLevel == 1900 or MyLevel <= 1924 then
            Ms = "Jungle Pirate [Lv. 1900]"
            NaemQuest = "DeepForestIsland2"
            LevelQuest = 1
            NameMon = "Jungle Pirate"
            CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
            CFrameMon = CFrame.new(-11982.221679688, 376.32522583008, -10451.415039063)
        elseif MyLevel == 1925 or MyLevel <= 1974 then
            Ms = "Musketeer Pirate [Lv. 1925]"
            NaemQuest = "DeepForestIsland2"
            LevelQuest = 2
            NameMon = "Musketeer Pirate"
            CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
            CFrameMon = CFrame.new(-13282.3046875, 496.23684692383, -9565.150390625)
        elseif MyLevel == 1975 or MyLevel <= 1999 then
            Ms = "Reborn Skeleton [Lv. 1975]"
            NaemQuest = "HauntedQuest1"
            LevelQuest = 1
            NameMon = "Reborn Skeleton"
            CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            CFrameMon = CFrame.new(-8761.3154296875, 164.85829162598, 6161.1567382813)
        elseif MyLevel == 2000 or MyLevel <= 2024 then
            Ms = "Living Zombie [Lv. 2000]"
            NaemQuest = "HauntedQuest1"
            LevelQuest = 2
            NameMon = "Living Zombie"
            CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            CFrameMon = CFrame.new(-10093.930664063, 237.38233947754, 6180.5654296875)
        elseif MyLevel == 2025 or MyLevel <= 2049 then
            Ms = "Demonic Soul [Lv. 2025]"
            NaemQuest = "HauntedQuest2"
            LevelQuest = 1
            NameMon = "Demonic Soul"
            CFrameQuest = CFrame.new(-9514.78027, 171.162918, 6078.82373, 0.301918149, 7.4535027e-09, 0.953333855, -3.22802141e-09, 1, -6.79604995e-09, -0.953333855, -1.02553133e-09, 0.301918149)
            CFrameMon = CFrame.new(-9466.72949, 171.162918, 6132.01514)
        elseif MyLevel == 2050 or MyLevel <= 2074 then
            Ms = "Posessed Mummy [Lv. 2050]" 
            NaemQuest = "HauntedQuest2"
            LevelQuest = 2
            NameMon = "Posessed Mummy"
            CFrameQuest = CFrame.new(-9514.78027, 171.162918, 6078.82373, 0.301918149, 7.4535027e-09, 0.953333855, -3.22802141e-09, 1, -6.79604995e-09, -0.953333855, -1.02553133e-09, 0.301918149)
            CFrameMon = CFrame.new(-9589.93848, 4.85058546, 6190.27197)
        elseif MyLevel == 2075 or MyLevel <= 2099 then
            Ms = "Peanut Scout [Lv. 2075]"
            NaemQuest = "NutsIslandQuest"
            LevelQuest = 1
            NameMon = "Peanut Scout"
            CFrameQuest = CFrame.new(-2075.9643554688, 38.129207611084, -10172.815429688)
            CFrameMon = CFrame.new(-2150.587890625, 122.49767303467, -10358.994140625)
        elseif MyLevel == 2100 or MyLevel <= 2124 then
            Ms = "Peanut President [Lv. 2100]"
            NaemQuest = "NutsIslandQuest"
            LevelQuest = 2
            NameMon = "Peanut President"
            CFrameQuest = CFrame.new(-2075.9643554688, 38.129207611084, -10172.815429688)
            CFrameMon = CFrame.new(-2150.587890625, 122.49767303467, -10358.994140625)
        elseif MyLevel == 2125 or MyLevel <= 2149 then
            Ms = "Ice Cream Chef [Lv. 2125]"
            NaemQuest = "IceCreamIslandQuest"
            LevelQuest = 1
            NameMon = "Ice Cream Chef"
            CFrameQuest = CFrame.new(-819.84533691406, 65.845329284668, -10965.487304688)
            CFrameMon = CFrame.new(-890.55895996094, 186.34135437012, -11127.306640625)
        elseif MyLevel == 2150 or MyLevel <= 2199 then
            Ms = "Ice Cream Commander [Lv. 2150]"
            NaemQuest = "IceCreamIslandQuest"
            LevelQuest = 2
            NameMon = "Ice Cream Commander"
            CFrameQuest = CFrame.new(-819.84533691406, 65.845329284668, -10965.487304688)
            CFrameMon = CFrame.new(-890.55895996094, 186.34135437012, -11127.306640625)
           elseif MyLevel == 2200 or MyLevel <= 2225 then
              Ms = "Cookie Crafter [Lv. 2200]"
              LevelQuest = 1
              NaemQuest = "CakeQuest1"
              NameMon = "Cookie Crafter"
              CFrameMon = CFrame.new(-2269.18994, 90.5692139, -12157.415, -0.241292745, -4.28479332e-08, 0.970452368, -3.0098203e-08, 1, 3.66689363e-08, -0.970452368, -2.03609218e-08, -0.241292745)
              CFrameQuest = CFrame.new(-2018.80884, 38.1414719, -12023.8447, 0.926204681, -9.25598265e-09, 0.377021134, 1.17539365e-08, 1, -4.32487202e-09, -0.377021134, 8.43719938e-09, 0.926204681)
          elseif MyLevel == 2225 or MyLevel <= 2250 then
              Ms = "Cake Guard [Lv. 2225]"
              LevelQuest = 2
              NaemQuest = "CakeQuest1"
              NameMon = "Cake Guard"
              CFrameMon = CFrame.new(-1558.61768, 90.5694199, -12583.4219, -0.790530264, -4.29809255e-08, 0.612422943, -3.70810653e-08, 1, 2.23166392e-08, -0.612422943, -5.0673159e-09, -0.790530264)
              CFrameQuest = CFrame.new(-2018.80884, 38.1414719, -12023.8447, 0.926204681, -9.25598265e-09, 0.377021134, 1.17539365e-08, 1, -4.32487202e-09, -0.377021134, 8.43719938e-09, 0.926204681)
          elseif MyLevel == 2250 or MyLevel <= 2275 then
              Ms = "Baking Staff [Lv. 2250]"
              LevelQuest = 1
              NaemQuest = "CakeQuest2"
              NameMon = "Baking Staff"
              CFrameMon = CFrame.new(-1769.45056, 90.5691681, -13038.4648, -0.847998321, -2.02224353e-08, 0.529998958, -2.03078834e-08, 1, 5.66300029e-09, -0.529998958, -5.96094241e-09, -0.847998321)
              CFrameQuest = CFrame.new(-1914.99646, 38.1413841, -12835.5117, 0.545026958, 0, 0.838418543, -0, 1, -0, -0.838418543, 0, 0.545026958)
          elseif MyLevel == 2275 or MyLevel <= 2300 then
              Ms = "Head Baker [Lv. 2275]"
              LevelQuest = 2
              NaemQuest = "CakeQuest2"
              NameMon = "Head Baker"
              CFrameMon = CFrame.new(-2068.16577, 84.8175354, -13017.8848, -0.527114272, 4.41528734e-08, 0.849794447, 4.18282369e-08, 1, -2.6011719e-08, -0.849794447, 2.18342535e-08, -0.527114272)
              CFrameQuest = CFrame.new(-1914.99646, 38.1413841, -12835.5117, 0.545026958, 0, 0.838418543, -0, 1, -0, -0.838418543, 0, 0.545026958)
          elseif MyLevel == 2300 or MyLevel <= 2324 then
              Ms = "CoCoa Warriors [Lv. 2300]"
              LevelQuest = 1
              NaemQuest = "ChocQuest1"
              NameMon = "CoCoa Warriors"
              CFrameMon = CFrame.new(88.7954102, 73.6419296, -12313.6445, -0.957159817, -1.11052387e-07, -0.289560139, -9.50311545e-08, 1, -6.9389344e-08, 0.289560139, -3.88994614e-08, -0.957159817)
              CFrameQuest = CFrame.new(229.584381, 24.7342587, -12189.1475, 0.999511659, 7.65095436e-08, -0.0312486049, -7.62648966e-08, 1, 9.02106656e-09, 0.0312486049, -6.63348976e-09, 0.999511659)
          elseif MyLevel == 2325 or MyLevel <= 2349 then
              Ms = "Chocolate Bar Battler [Lv. 2325]"
              LevelQuest = 2
              NaemQuest = "ChocQuest1"
              NameMon = "Chocolate Bar Battler"
              CFrameMon = CFrame.new(715.158508, 69.274086, -12589.7568, 0.848450363, -6.87506514e-08, -0.52927494, 1.04103712e-07, 1, 3.69867976e-08, 0.52927494, -8.64809522e-08, 0.848450363)
              CFrameQuest = CFrame.new(229.584381, 24.7342587, -12189.1475, 0.999511659, 7.65095436e-08, -0.0312486049, -7.62648966e-08, 1, 9.02106656e-09, 0.0312486049, -6.63348976e-09, 0.999511659)
          elseif MyLevel == 2350 or MyLevel <= 2374 then
              Ms = "Sweet Thief [Lv. 2350]"
              LevelQuest = 1
              NaemQuest = "ChocQuest2"
              NameMon = "Sweet Thief"
              CFrameMon = CFrame.new(-18.7927246, 69.5068817, -12697.5566, -0.56289655, 3.78088458e-08, 0.826527357, 7.12002945e-09, 1, -4.08952019e-08, -0.826527357, -1.71348695e-08, -0.56289655)
              CFrameQuest = CFrame.new(142.522064, 24.7938404, -12772.083, 0.31704393, -2.01267625e-08, -0.948410869, -2.25982149e-08, 1, -2.8775915e-08, 0.948410869, 3.0555622e-08, 0.31704393)
          elseif MyLevel >= 2350 then
              Ms = "Candy Rebel [Lv. 2375]"
              LevelQuest = 2
              NaemQuest = "ChocQuest2"
              NameMon = "Candy Rebel"
              CFrameMon = CFrame.new(135.289688, 77.2218857, -12879.4258, 0.961599529, -1.10834684e-08, -0.274456471, 1.99045331e-08, 1, 2.93551867e-08, 0.274456471, -3.36908599e-08, 0.961599529)
              CFrameQuest = CFrame.new(142.522064, 24.7938404, -12772.083, 0.31704393, -2.01267625e-08, -0.948410869, -2.25982149e-08, 1, -2.8775915e-08, 0.948410869, 3.0555622e-08, 0.31704393)
        end
    end
end
CheckQuestSMZHUB()

library = loadstring(game:HttpGet("https://pastebin.com/raw/aUBdarn7"))()
local window = library:Win()
local tap1 = window:addtap("Main")
local tap2 = window:addtap("Stats")
local tap3 = window:addtap("Players")
local tap4 = window:addtap("Dungeon")
local tap5 = window:addtap("Island")
local tap6 = window:addtap("Misc")
local tap7 = window:addtap("Esp - Fruits")
local tap8 = window:addtap("Shop")
local page1 = tap1:addpage()
local page2 = tap1:addpage()
local page11 = tap2:addpage()
local Players = tap3:addpage()
local Players1 = tap3:addpage()
local Raid = tap4:addpage()
local Raid1 = tap4:addpage()
local Teleport = tap5:addpage()
local Misc = tap6:addpage()
local espfruit = tap7:addpage()
local espfruit1 = tap7:addpage()
local BuyItem = tap8:addpage()

page1:Toggle("Auto SetSpawnPoint", _G.AutoSetSpawn, function(a)
    _G.AutoSetSpawn = a
end)

page1:Button("Redeem All Code", function()
   	function UseCode(Text)
        game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Text)
    end
    UseCode("UPD16")
    UseCode("2BILLION")
    UseCode("UPD17")
    UseCode("UPD15")
    UseCode("FUDD10")
    UseCode("BIGNEWS")
    UseCode("THEGREATACE")
    UseCode("SUB2GAMERROBOT_EXP1")
    UseCode("StrawHatMaine")
    UseCode("Sub2OfficialNoobie")
    UseCode("SUB2NOOBMASTER123")
    UseCode("Sub2Daigrock")
    UseCode("Axiore")
    UseCode("TantaiGaming")
    UseCode("STRAWHATMAINE")
    UseCode("Bluxxy")
end)

spawn(function()
    pcall(function()
        while wait() do
            if _G.AutoSetSpawn then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
            end
        end
    end)
end)

page1:Ti("Farm")

page1:Toggle("Auto Farm Level", _G.AutoFarmLv, function(vu)
    _G.AutoFarmLv = vu
    StopTween(_G.AutoFarmLv)
end)


   spawn(function()
      while wait() do
         if _G.AutoFarmLv then
            if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
               MagnetActive = false
               CheckQuestSMZHUB()
                topos(CFrameQuest)
               if (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
                  CheckQuestSMZHUB()
                  if (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 20 then
                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
                     wait(2)
                  else
                     
                    topos(CFrameQuest)
                  end
               end
            elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
               pcall(function()
                  CheckQuestSMZHUB()
                  if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                     for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == Ms and v:FindFirstChild("Humanoid") then
                           if v.Humanoid.Health > 0 then
                              repeat game:GetService("RunService").Heartbeat:wait()
                                 if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                                    if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
                                       EquipWeapon(_G.SelectToolWeapon)
                                        if OldWorld then
                                            TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
                                        elseif NewWorld then
                                            TP(v.HumanoidRootPart.CFrame * CFrame.new(0,10,15))
                                        elseif ThreeWorld then
                                            TP(v.HumanoidRootPart.CFrame * CFrame.new(0,10,15))
                                        end
                                       v.HumanoidRootPart.CanCollide = false
                                       v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                       game:GetService("VirtualUser"):CaptureController()
                                       game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
                                       PosMon = v.HumanoidRootPart.CFrame
                                       MagnetActive = true
                                    else
                                       MagnetActive = false    
                                       game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                                    end
                                 else
                                    MagnetActive = false
                                    CheckQuestSMZHUB()
                                 end
                              until not v.Parent or v.Humanoid.Health <= 0 or _G.AutoFarmLv == false or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not game:GetService("Workspace").Enemies:FindFirstChild(v.Name)
                           end
                        end
                     end
                  else
                     MagnetActive = false
                     CheckQuestSMZHUB()
                  end
               end)
            end
         end
      end
   end)

    spawn(function()
        while wait() do
            if _G.AutoFarmLv then
                Attack()
            end
        end
    end)

page1:Ti("Auto")

page1:Toggle("Auto  Superhuman", _G.AutoSuperhuman, function(vu)
    _G.AutoSuperhuman = vu
    Superhuman = vu
end)

spawn(function()
    pcall(function()
        while wait() do 
            if _G.AutoSuperhuman then
                if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 150000 then
                    UnEquipWeapon("Combat")
                    wait(.1)
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyBlackLeg")
                end   
                if game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") or game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") then
                    _G.SelectToolWeapon = "Superhuman"
                end  
                if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") then
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 299 then
                        _G.SelectToolWeapon = "Black Leg"
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 299 then
                        _G.SelectToolWeapon = "Electro"
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value <= 299 then
                        _G.SelectToolWeapon = "Fishman Karate"
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value <= 299 then
                        _G.SelectToolWeapon = "Dragon Claw"
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300 and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 300000 then
                        UnEquipWeapon("Black Leg")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
                    end
                    if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300 and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 300000 then
                        UnEquipWeapon("Black Leg")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 300 and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 750000 then
                        UnEquipWeapon("Electro")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
                    end
                    if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300 and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 750000 then
                        UnEquipWeapon("Electro")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300 and game:GetService("Players")["Localplayer"].Data.Fragments.Value >= 1500 then
                        UnEquipWeapon("Fishman Karate")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","1")
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2") 
                    end
                    if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300 and game:GetService("Players")["Localplayer"].Data.Fragments.Value >= 1500 then
                        UnEquipWeapon("Fishman Karate")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","1")
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2") 
                    end
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300 and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 3000000 then
                        UnEquipWeapon("Dragon Claw")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
                    end
                    if game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 300 and game:GetService("Players")["LocalPlayer"].Data.Beli.Value >= 3000000 then
                        UnEquipWeapon("Dragon Claw")
                        wait(.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
                    end 
                end
            end
        end
    end)
end)

if not OldWorld then    
page1:Toggle("Auto Buy Legendary Sword",_G.BuySwordLegendary,function(value)
_G.BuySwordLegendary = value
end)
page1:Toggle("Auto Buy Buso Color",_G.AutoBusoColor,function(value)

_G.BuyHakiColorsDealer = value
end)
end

spawn(function()
    while wait() do
        if _G.BuySwordLegendary then
            while _G.BuySwordLegendary do wait()
    local args = {
       [1] = "LegendarySwordDealer",
       [2] = "2"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
 end
end
end
end)

spawn(function()
while wait() do
if _G.BuyHakiColorsDealer then
while _G.BuyHakiColorsDealer do wait()
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ColorsDealer","2")
end
end
end
end)


function UnEquipWeapon(Weapon)
    if game.Players.LocalPlayer.Character:FindFirstChild(Weapon) then
        _G.NotAutoEquip = true
        wait(.5)
        game.Players.LocalPlayer.Character:FindFirstChild(Weapon).Parent = game.Players.LocalPlayer.Backpack
        wait(.1)
        _G.NotAutoEquip = false
    end
end

function topos(Pos)
    Distance = (Pos.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
    if game.Players.LocalPlayer.Character.Humanoid.Sit == true then game.Players.LocalPlayer.Character.Humanoid.Sit = false end
    pcall(function() tween = game:GetService("TweenService"):Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(Distance/210, Enum.EasingStyle.Linear),{CFrame = Pos}) end)
    tween:Play()
    if Distance <= 250 then
        tween:Cancel()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Pos
    end
    if _G.StopTween == true then
        tween:Cancel()
        _G.Clip = false
    end
end

function StopTween(target)
    if not target then
        _G.StopTween = true
        wait()
        topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
        wait()
        if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
            game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
        end
        _G.StopTween = false
        _G.Clip = false
    end
end

if not ThreeWorld then
page1:Ti("Auto World")
end
if OldWorld then
page1:Toggle("Auto Second Sea",_G.AutoSecondSea,function(vu)
    _G.AutoSecondSea = vu
    StopTween(_G.AutoSecondSea)
  end)
end
  spawn(function()
    while wait() do
        if _G.AutoThirdSea then
            pcall(function()
                if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1500 and World2 then
                    _G.AutoFarmLv = false
                    if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Check") == 0 then
                        topos(CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016))
                        if (CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
                            wait(1.5)
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Begin")
                        end
                        wait(1.8)
                        if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v.Name == "rip_indra [Lv. 1500] [Boss]" then
                                    OldCFrameThird = v.HumanoidRootPart.CFrame
                                    repeat task.wait()
                                        AutoHaki()
                                        EquipWeapon(_G.SelectToolWeapon)
                                        topos(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
                                        v.HumanoidRootPart.CFrame = OldCFrameThird
                                        v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                        v.HumanoidRootPart.CanCollide = false
                                        v.Humanoid.WalkSpeed = 0
                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
                                        sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                        game:GetService("VirtualUser"):CaptureController()
                                        game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
                                    until _G.AutoThirdSea == false or v.Humanoid.Health <= 0 or not v.Parent
                                end
                            end
                        elseif not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") and (CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1000 then
                            topos(CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016))
                        end
                    end
                end
            end)
        end
    end
end)
  if NewWorld then
  page1:Toggle("Auto Third Sea",_G.AutoThirdSea,function(th)
    _G.AutoThirdSea = th
    StopTween(_G.AutoThirdSea)
  end)
end
  spawn(function()
    while wait() do 
        if _G.AutoSecondSea then
            pcall(function()
                local MyLevel = game:GetService("Players").LocalPlayer.Data.Level.Value
                if MyLevel >= 700 and World1 then
                    if game:GetService("Workspace").Map.Ice.Door.CanCollide == false and game:GetService("Workspace").Map.Ice.Door.Transparency == 1 then
                        local CFrame1 = CFrame.new(4849.29883, 5.65138149, 719.611877)
                        repeat topos(CFrame1) wait() until (CFrame1.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or _G.AutoSecondSea == false
                        wait(1.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("DressrosaQuestProgress","Detective")
                        wait(0.5)
                        EquipWeapon("Key")
                        repeat topos(CFrame.new(1347.7124, 37.3751602, -1325.6488)) wait() until (Vector3.new(1347.7124, 37.3751602, -1325.6488)-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or _G.AutoSecondSea == false
                        wait(0.5)
                    else
                        if game:GetService("Workspace").Map.Ice.Door.CanCollide == false and game:GetService("Workspace").Map.Ice.Door.Transparency == 1 then
                            if game:GetService("Workspace").Enemies:FindFirstChild("Ice Admiral [Lv. 700] [Boss]") then
                                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                    if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
                                        if not v.Humanoid.Health <= 0 then
                                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                                OldCFrameSecond = v.HumanoidRootPart.CFrame
                                                repeat task.wait()
                                                    AutoHaki()
                                                    EquipWeapon(_G.SelectToolWeapon)
                                                    v.HumanoidRootPart.CanCollide = false
                                                    v.Humanoid.WalkSpeed = 0
                                                    v.Head.CanCollide = false
                                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                    v.HumanoidRootPart.CFrame = OldCFrameSecond
                                                    topos(v.HumanoidRootPart.CFrame * CFrame.new(0,10,15))
                                                    sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                                    game:GetService("VirtualUser"):CaptureController()
                                                    game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
                                                until not _G.AutoSecondSea or not v.Parent or v.Humanoid.Health <= 0
                                            end
                                        else 
                                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
                                        end
                                    end
                                end
                            else
                                if game:GetService("ReplicatedStorage"):FindFirstChild("Ice Admiral [Lv. 700] [Boss]") then
                                    topos(game:GetService("ReplicatedStorage"):FindFirstChild("Ice Admiral [Lv. 700] [Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
                                end
                            end
                        end
                    end
                end
            end)
        end
    end
end)

page2:Ti("Setting")

Wapon = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
    if v:IsA("Tool") then
        table.insert(Wapon ,v.Name)
    end
end


local SelectWeapona = page2:DropDown("Select Weapon","Select",Wapon,function(Value)
    _G.SelectToolWeapon = Value
    SelectToolWeapon = Value
    SelectToolWeaponOld = Value
    _G.SelectWeaponOld = Value
    _G.SelectWeapon = Value
    _G.SelectToolWeaponOld = Value
    SelectWeapon = Value
end)


page2:Button("Refresh Weapon",function()
    SelectWeapona:Clear()
    for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
        if v:IsA("Tool") then
            SelectWeapona:Add(v.Name)
        end
    end
end)   

_G.BringMob = true
page2:Toggle("Bring Mob",_G.BringMob,function(spawn)
    _G.BringMob = spawn
    Magnet = spawn
end)

_G.FastAttack = true
page2:Toggle("Fast Attack", _G.FastAttack,function(vu)
    _G.FastAttack = vu
    Usefastattack = vu
    SuperFastAttack = vu
    _G.Usefastattack = vu
    _G.SuperFastAttack = vu
    fastattect = vu
end)

_G.AutoHakiBuso = true
page2:Toggle("Auto Buso", _G.AutoHakiBuso,function(vu)
    _G.AutoHakiBuso = vu
end)

page11:Toggle("Melee", _G.Melee, function(Value)
	Melee = Value
    _G.Melee = Value
end)
 
page11:Toggle("Defense", _G.Defense, function(Value)
	Defense = Value
    _G.Defense = Value
end)
 
page11:Toggle("Sword", _G.Sword, function(Value)
	Sword = Value
    _G.Sword = Value
end)
 
page11:Toggle("Gun", _G.Gun, function(Value)
	Gun = Value
    _G.Gun = Value
end)
 
page11:Toggle("Devil Fruit", _G.DevilFruit, function(Value)
	DevilFruit = Value
    _G.DevilFruit = value
end)
 
page11:Toggle("Kaitan Stat", _G.KaitanStat, function(value)
	Kaitan = value
    _G.KaitanStat = value
end)
 
SelectPoint = 1
page11:Slder("Point", 1,50,1, function(Point)
	SelectPoint = Point
end)


 
 spawn(function()
	while wait(.1) do
		if Kaitan then
			pcall(function()
				PointStats = game:GetService("Players").LocalPlayer.Data.Points.Value
				if OldWorld then
					Melee = true
				else
					Defense = true
				end
			end)
		end
	end
 end)
 
 spawn(function()
	while wait(.1) do
		if _G.AutoHakiBuso then
			if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
			end
		end
	end
 end)
 
 spawn(function()
	while wait(.1) do
		if Melee then
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Melee", SelectPoint)
		end
	end
 end)
 
 spawn(function()
	while wait(.1) do
		if Defense then
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Defense", SelectPoint)
		end
	end
 end)
 
 spawn(function()
	while wait(.1) do
		if Sword then
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Sword", SelectPoint)
		end
	end
 end)
 
 spawn(function()
	while wait(.1) do
		if Gun then
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Gun", SelectPoint)
		end
	end
 end)
 
 spawn(function()
	while wait(.1) do
		if DevilFruit then
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Demon Fruit", SelectPoint)
		end
	end
 end)


spawn(function()
pcall(function()
 while wait() do
    for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
       if v:IsA("Tool") then
          if v:FindFirstChild("RemoteFunctionShoot") then 
             SelectToolWeaponGun = v.Name
          end
       end
    end
 end
end)
end)


PlayerName = {}
for i,v in pairs(game.Players:GetChildren()) do  
table.insert(PlayerName ,v.Name)
end

Players:Ti("Players")

local Player = Players:DropDown("Select Player","Select",PlayerName,function(plys)
_G.SelectP = plys
end)
Players:Button("Refresh Player",function()
    PlayerName = {}
    Player:Clear()
    for i,v in pairs(game.Players:GetChildren()) do  
     Player:Add(v.Name)
    end
    end)


WaponP = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
if v:IsA("Tool") then
   table.insert(WaponP, v.Name)
end
end


local SelectWeaponaP = Players1:DropDown("Select Weapon","Select",WaponP,function(tool)
_G.SelectToolWeaponP = tool
end)
Players1:Button("Refresh Weapon",function()
WaponP = {}
SelectWeaponaP:Clear()
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
   if v:IsA("Tool") then
      SelectWeaponaP:Add(v.Name)
   end
end
end)



Players:Toggle("Teleport",false, function(value)
_G.TeleportPly = value
   pcall(function()
      if _G.TeleportPly then
         repeat totarget(game.Players[_G.SelectP].Character.HumanoidRootPart.CFrame) wait() until _G.TeleportPly == false
      else
      tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(.1, Enum.EasingStyle.Linear)
      tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame})
      tween:Play()
      end
   end)
end)

Players:Toggle("Spectate Player",false,function(bool)
Sp = bool
local plr1 = game.Players.LocalPlayer.Character.Humanoid
local plr2 = game.Players:FindFirstChild(_G.SelectP)
repeat wait(.1)
 game.Workspace.Camera.CameraSubject = plr2.Character.Humanoid
until Sp == false 
game.Workspace.Camera.CameraSubject = game.Players.LocalPlayer.Character.Humanoid
end)


Players:Ti("Aimbot")

spawn(function()
 while wait() do
     pcall(function()
         local MaxDistance = math.huge
         for i,v in pairs(game:GetService("Players"):GetPlayers()) do
             if v.Name ~= game.Players.LocalPlayer.Name then
                 local Distance = v:DistanceFromCharacter(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
                 if Distance < MaxDistance then
                     MaxDistance = Distance
                     TargetPlayerAim = v.Name
                 end
             end
         end
     end)
 end
end)

Players:Toggle("Aimbot Gun", false, function(vu)
_G.Aimbot = vu
end)

local lp = game:GetService('Players').LocalPlayer
local mouse = lp:GetMouse()
mouse.Button1Down:Connect(function()
if _G.Aimbot and game.Players.LocalPlayer.Character:FindFirstChild(SelectToolWeaponGun) then
    local args = {
        [1] = game.Players:FindFirstChild(TargetPlayerAim).Character.HumanoidRootPart.Position,
        [2] = game.Players:FindFirstChild(TargetPlayerAim).Character.HumanoidRootPart
    }
    game:GetService("Players").LocalPlayer.Character[SelectToolWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
end
end)

spawn(function()
pcall(function()
  while wait() do
     if _G.Aimbot then
     Click()
     end
  end
end)
end)

Players:Toggle("Aimbot Skill", false, function(vu)
_G.AimbotSkill = vu
end)

spawn(function()
pcall(function()
game:GetService("RunService").RenderStepped:connect(function()
   if _G.AimbotSkill then
      pcall(function()
         if game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool") and game.Players.LocalPlayer.Character[game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name]:FindFirstChild("MousePos") then
             local args = {
                 [1] = game:GetService("Players"):FindFirstChild(TargetPlayerAim).Character.HumanoidRootPart.Position
             }
             game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
         end
     end)
 end
end)
end)
end)

if OldWorld then
    Raid:Label("Can't Use In Frist World")
    Raid1:Label("Can't Use In Frist World")
end

if not OldWorld then

Raid:Ti("Dungeon")

Raid:DropDown("Select Dungeon","Select",{"Flame","Ice","Quake","Light","Dark","String","Rumble","Magma","Human: Buddha","Sand","Bird: Phoenix","Dough"}, function(vu)
   _G.SelectRaid = vu
end)

Raid:Toggle("Auto Start Dungeon", false, function(vu)
   _G.AutoRaid = vu
end)

Raid:Toggle("Auto Farm Dungeon",_G.AutoDungeonFarm,function(vu)
   _G.AutoDungeonFarm = vu
   StopTween(_G.AutoDungeonFarm)
end)

spawn(function()
   while wait(.1) do
       if _G.AutoRaid or RaidSuperhuman then
           pcall(function()
               if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
                   if AutoSuperhuman then
                       if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") or not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
                           for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
                               if not string.find(v.Name, "Fruit") then
                                   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
                               end
                           end
                       end
                   end
                   if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                       game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", _G.SelectRaid)
                   end
                   if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                       game:GetService("StarterGui"):SetCore("SendNotification",
                           {
                               Title = "Dungeon",
                               Text = ".....",
                               Icon = "",
                               Duration = 4
                           }
                       )
                       wait(4)
                   end
                   if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or  game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip")  then
                       if NewWorld then
                           fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
                       elseif ThreeWorld then
                           fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
                       end
                   end
               end
           end)
       end
   end
end)

Raid1:Ti("TeleportDungeon")

if NewWorld then
  Raid1:Button("Teleport to Lab",function()
      TP(Vector3.new(-6438.73535, 250.645355, -4501.50684),CFrame.new(-6438.73535, 250.645355, -4501.50684))
  end)
end
if ThreeWorld then
  Raid1:Button("Teleport to Lab",function()
  TP(Vector3.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818),CFrame.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818))
  end)
end

Raid1:Button("Awakening Room",function()
  TP(Vector3.new(266.227783, 1.39509034, 1857.00732),CFrame.new(266.227783, 1.39509034, 1857.00732))
end)
end

    spawn(function()
      pcall(function() 
      while wait() do
           if _G.AutoDungeonFarm then
               for i,v in pairs(game.Workspace.Enemies:GetDescendants()) do
                   if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                       pcall(function()
                           repeat wait()
                               sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                               v.Humanoid.Health = 0
                               v.HumanoidRootPart.CanCollide = false
                               v.Humanoid.JumpPower = 0
                               v.Humanoid.WalkSpeed = 0
                               v.HumanoidRootPart.Size = Vector3.new(80,80,80)
                                if v.Humanoid:FindFirstChild("Animator") then
                                    v.Humanoid.Animator:Destroy()
                                end
                               v.HumanoidRootPart.Transparency = 1
                           until not _G.AutoDungeonFarm or not v.Parent or v.Humanoid.Health <= 0
                       end)
                   end
               end
           end
       end
      end)
    end)

spawn(function()
   while wait(.1) do
       if _G.AutoDungeonFarm then
           if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
               Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,20,0)})
               tween:Play()
           elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
               Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,20,0)})
               tween:Play()
           elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
               Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,20,0)})
               tween:Play()
           elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
               Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,20,0)})
               tween:Play()
           elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
               Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0,20,0)})
               tween:Play()
           else
              if NewWorld then                        
               Lab2 = Vector3.new(-6438.73535, 250.645355, -4501.50684)
               local Distance = (Lab2 - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               local Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-6438.73535, 250.645355, -4501.50684)})
               tween:Play()             
       end
       if ThreeWorld then                        
               Lab3 = Vector3.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818)
               local Distance = (Lab3 - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- Ã Â¸Ë†Ã Â¸Â¸Ã Â¸â€Ã Â¸â€”Ã Â¸ÂµÃ Â¹Ë†Ã Â¸Ë†Ã Â¸Â°Ã Â¹â€žÃ Â¸â€º Position Only
               local Speed = 150 -- nextisland
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
               tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818)})
               tween:Play() 
       end
              end
       end
   end
end)

   spawn(function()
        while wait(.1) do
            if _G.AutoDungeonFarm then
                local args = {
                    [1] = "Awakener",
                    [2] = "Check"
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                local args = {
                    [1] = "Awakener",
                    [2] = "Awaken"
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end)

                  function toislandfunc(POS1,POS2)
                  local Distance = (POS1 - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
                  local Speed = 200 
                  tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
                  tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = POS2})
                  tween:Play()
                  _G.Clip = true
                  wait(Distance/Speed)
                  _G.Clip = false
               end 
                     Teleport:Button("Teleport To First Sea",function()
                           local args = {
                              [1] = "TravelMain" -- OLD WORLD to NEW WORLD
                           }
                           game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                     end)
                     Teleport:Button("Teleport To Second Sea",function()
                           local args = {
                              [1] = "TravelDressrosa" -- NEW WORLD to OLD WORLD
                           }
                           game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                     end)
                     Teleport:Button("Teleport To Third Sea",function()
                           game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
                     end)
                     Teleport:Button("Teleport to SeaBeast",function()
                        for i,v in pairs(game.Workspace.SeaBeasts:GetChildren()) do
                           if v:FindFirstChild("HumanoidRootPart") then
                              TP(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame*CFrame.new(0,100,0))
                           end
                        end
                        end)
               if OldWorld then
                  local TP = Teleport:DropDown("Select Island","Select", {
                     "Start Island",
                     "Marine Start",
                     "Middle Town",
                     "Jungle",
                     "Pirate Village",
                     "Desert",
                     "Frozen Village",
                     "MarineFord",
                     "Colosseum",
                     "Sky 1st Floor",
                     "Sky 2nd Floor",
                     "Sky 3rd Floor",
                     "Prison",
                     "Magma Village",
                     "Underwater City",
                     "Fountain City",
                     "House Cyborg's",
                     "Shank's Room",
                     "Mob Island"
                  }, function(list)
                  ISLAND = list
                  end)
               end
               if NewWorld then
                  local TP = Teleport:DropDown("Select Island","Select", {
                     "Dock",
                     "Kingdom of Rose",
                     "Mansion",
                     "Flamingo Room",
                     "Green Zone",
                                    "Cafe",
                                    "Factory",
                                    "Colosseum",
                                    "GraveIsland",
                                    "Snow Mountain",
                                    "Cold Island",
                                    "Hot Island",
                                    "Cursed Ship",
                                    "Ice Castle",
                                    "Forgotten Island",
                                    "Usoapp Island",
                                    "Minisky Island"
                                 }, function(list)
                                 ISLAND = list
                                 end)
                              end
                              if ThreeWorld then
                                 local TP = Teleport:DropDown("Select Island","Select", {
                                    "Port Town",
                                    "Hydra Island" ,
                     "Great Tree",
                     "Castle on the Sea",
                     "Floating Turtle",
                     "Mansion",
                     "Secret Temple",
                     "Friendly Arena",
                     "Beautiful Pirate Domain",
                     "Haunted Castle",
                     "Ice Cream Island",
                     "Peanut Island",
                     "Cake Island",
                     "Sea of Treats"
                  }, function(list)
   ISLAND = list
   end)
end

Teleport:Toggle("Teleport",false, function(State)
_G.Teleport = State
               pcall(function()
               if _G.Teleport then
                  if OldWorld then
                     if ISLAND =="Start Island" then
                        toislandfunc(Vector3.new(1071.2832, 16.3085976, 1426.86792),CFrame.new(1071.2832, 16.3085976, 1426.86792))
                     elseif ISLAND =="Marine Start" then
                        toislandfunc(Vector3.new(-2573.3374, 6.88881969, 2046.99817),CFrame.new(-2573.3374, 6.88881969, 2046.99817))
                     elseif ISLAND =="Middle Town" then
                        toislandfunc(Vector3.new(-655.824158, 7.88708115, 1436.67908),CFrame.new(-655.824158, 7.88708115, 1436.67908))
                     elseif ISLAND == "Jungle" then
                        toislandfunc(Vector3.new(-1249.77222, 11.8870859, 341.356476),CFrame.new(-1249.77222, 11.8870859, 341.356476))
                     elseif ISLAND =="Pirate Village" then
                        toislandfunc(Vector3.new(-1122.34998, 4.78708982, 3855.91992),CFrame.new(-1122.34998, 4.78708982, 3855.91992))
               
                     elseif ISLAND =="Desert" then
                        toislandfunc(Vector3.new(1094.14587, 6.47350502, 4192.88721),CFrame.new(1094.14587, 6.47350502, 4192.88721))
               
                     elseif ISLAND =="Frozen Village" then
                        toislandfunc(Vector3.new(1198.00928, 27.0074959, -1211.73376),CFrame.new(1198.00928, 27.0074959, -1211.73376))
               
                     elseif ISLAND =="MarineFord" then
                        toislandfunc(Vector3.new(-4505.375, 20.687294, 4260.55908),CFrame.new(-4505.375, 20.687294, 4260.55908))
               
                     elseif ISLAND =="Colosseum" then
                                    toislandfunc(Vector3.new(-1428.35474, 7.38933945, -3014.37305),CFrame.new(-1428.35474, 7.38933945, -3014.37305))
                           
                                 elseif ISLAND =="Sky 1st Floor" then
                                    toislandfunc(Vector3.new(-4970.21875, 717.707275, -2622.35449),CFrame.new(-4970.21875, 717.707275, -2622.35449))
                           
                                 elseif ISLAND =="Sky 2nd Floor" then
                                    toislandfunc(Vector3.new(-4813.0249, 903.708557, -1912.69055),CFrame.new(-4813.0249, 903.708557, -1912.69055))
                           
                                 elseif ISLAND =="Sky 3rd Floor" then
                                    toislandfunc(Vector3.new(-7952.31006, 5545.52832, -320.704956),CFrame.new(-7952.31006, 5545.52832, -320.704956))
                           
                                 elseif ISLAND =="Prison" then
                                    toislandfunc(Vector3.new(4854.16455, 5.68742752, 740.194641),CFrame.new(4854.16455, 5.68742752, 740.194641))
                           
                                 elseif ISLAND =="Magma Village" then
                                    toislandfunc(Vector3.new(-5231.75879, 8.61593437, 8467.87695),CFrame.new(-5231.75879, 8.61593437, 8467.87695))
                           
                     elseif ISLAND =="Underwater City" then
                        toislandfunc(Vector3.new(61163.8516, 11.7796879, 1819.78418),CFrame.new(61163.8516, 11.7796879, 1819.78418))
               
                     elseif ISLAND =="Fountain City" then
                        toislandfunc(Vector3.new(5132.7124, 4.53632832, 4037.8562),CFrame.new(5132.7124, 4.53632832, 4037.8562))
               
                     elseif ISLAND =="House Cyborg's" then
                        toislandfunc(Vector3.new(6262.72559, 71.3003616, 3998.23047),CFrame.new(6262.72559, 71.3003616, 3998.23047))

      elseif ISLAND =="Shank's Room" then
         toislandfunc(Vector3.new(-1442.16553, 29.8788261, -28.3547478),CFrame.new(-1442.16553, 29.8788261, -28.3547478))

      elseif ISLAND =="Mob Island" then
         toislandfunc(Vector3.new(-2850.20068, 7.39224768, 5354.99268),CFrame.new(-2850.20068, 7.39224768, 5354.99268))
      end
   end

   if NewWorld then
      if ISLAND =="Dock" then
         toislandfunc(Vector3.new(82.9490662, 18.0710983, 2834.98779),CFrame.new(82.9490662, 18.0710983, 2834.98779))

      elseif ISLAND =="Kingdom of Rose" then
         toislandfunc(Vector3.new(-394.983521, 118.503128, 1245.8446),CFrame.new(-394.983521, 118.503128, 1245.8446))

      elseif ISLAND =="Mansion" then
         toislandfunc(Vector3.new(-390.096313, 331.886475, 673.464966),CFrame.new(-390.096313, 331.886475, 673.464966))

      elseif ISLAND =="Flamingo Room" then
         toislandfunc(Vector3.new(2302.19019, 15.1778421, 663.811035),CFrame.new(2302.19019, 15.1778421, 663.811035))

      elseif ISLAND =="Green Zone" then
         toislandfunc(Vector3.new(-2372.14697, 72.9919434, -3166.51416),CFrame.new(-2372.14697, 72.9919434, -3166.51416))

      elseif ISLAND =="Cafe" then
         toislandfunc(Vector3.new(-385.250916, 73.0458984, 297.388397),CFrame.new(-385.250916, 73.0458984, 297.388397))

      elseif ISLAND =="Factroy" then
         toislandfunc(Vector3.new(430.42569, 210.019623, -432.504791),CFrame.new(430.42569, 210.019623, -432.504791))

      elseif ISLAND =="Colosseum" then
         toislandfunc(Vector3.new(-1836.58191, 44.5890656, 1360.30652),CFrame.new(-1836.58191, 44.5890656, 1360.30652))

      elseif ISLAND =="GraveIsland" then
         toislandfunc(Vector3.new(-5411.47607, 48.8234024, -721.272522),CFrame.new(-5411.47607, 48.8234024, -721.272522))

      elseif ISLAND =="Snow Mountain" then
         toislandfunc(Vector3.new(511.825226, 401.765198, -5380.396),CFrame.new(511.825226, 401.765198, -5380.396))

      elseif ISLAND =="Cold Island" then
         toislandfunc(Vector3.new(-6026.96484, 14.7461271, -5071.96338),CFrame.new(-6026.96484, 14.7461271, -5071.96338))

      elseif ISLAND =="Hot Island" then
         toislandfunc(Vector3.new(-5478.39209, 15.9775667, -5246.9126),CFrame.new(-5478.39209, 15.9775667, -5246.9126))

      elseif ISLAND =="Cursed Ship" then
         toislandfunc(Vector3.new(902.059143, 124.752518, 33071.8125),CFrame.new(902.059143, 124.752518, 33071.8125))

      elseif ISLAND =="Ice Castle" then
         toislandfunc(Vector3.new(5400.40381, 28.21698, -6236.99219),CFrame.new(5400.40381, 28.21698, -6236.99219))

      elseif ISLAND =="Forgotten Island" then
         toislandfunc(Vector3.new(-3043.31543, 238.881271, -10191.5791),CFrame.new(-3043.31543, 238.881271, -10191.5791))

      elseif ISLAND =="Usoapp Island" then
         toislandfunc(Vector3.new(4748.78857, 8.35370827, 2849.57959),CFrame.new(4748.78857, 8.35370827, 2849.57959))

      elseif ISLAND =="Minisky Island" then
         toislandfunc(Vector3.new(-260.358917, 49325.7031, -35259.3008),CFrame.new(-260.358917, 49325.7031, -35259.3008))
      end
   end

   if ThreeWorld then
      if ISLAND =="Port Town" then
         toislandfunc(Vector3.new(-236.423828, 6.72993994, 5362.34961, 0.985803843, 7.44091579e-08, 0.167901203, -6.67679885e-08, 1, -5.11552045e-08, -0.167901203, 3.92185697e-08, 0.985803843),CFrame.new(-236.423828, 6.72993994, 5362.34961, 0.985803843, 7.44091579e-08, 0.167901203, -6.67679885e-08, 1, -5.11552045e-08, -0.167901203, 3.92185697e-08, 0.985803843))

      elseif ISLAND =="Hydra Island" then
         toislandfunc(Vector3.new(5229.99561, 603.916565, 345.154022, -0.137452736, 6.26227887e-08, -0.990508318, 5.81512971e-08, 1, 5.51532295e-08, 0.990508318, -5.00183823e-08, -0.137452736),CFrame.new(5229.99561, 603.916565, 345.154022, -0.137452736, 6.26227887e-08, -0.990508318, 5.81512971e-08, 1, 5.51532295e-08, 0.990508318, -5.00183823e-08, -0.137452736))

      elseif ISLAND =="Great Tree" then
         toislandfunc(Vector3.new(2174.94873, 28.7312393, -6728.83154),CFrame.new(2174.94873, 28.7312393, -6728.83154))

      elseif ISLAND =="Castle on the Sea" then
         toislandfunc(Vector3.new(-5477.62842, 313.794739, -2808.4585),CFrame.new(-5477.62842, 313.794739, -2808.4585))

      elseif ISLAND =="Floating Turtle" then
         toislandfunc(Vector3.new(-10919.2998, 331.788452, -8637.57227),CFrame.new(-10919.2998, 331.788452, -8637.57227))

      elseif ISLAND =="Mansion" then
         toislandfunc(Vector3.new(-12553.8125, 332.403961, -7621.91748),CFrame.new(-12553.8125, 332.403961, -7621.91748))

      elseif ISLAND =="Secret Temple" then
         toislandfunc(Vector3.new(5217.35693, 6.56511116, 1100.88159, 0.00408430398),CFrame.new(5217.35693, 6.56511116, 1100.88159, 0.00408430398))

      elseif ISLAND =="Friendly Arena" then
         toislandfunc(Vector3.new(5220.28955, 72.8193436, -1450.86304),CFrame.new(5220.28955, 72.8193436, -1450.86304))

      elseif ISLAND =="Beautiful Pirate Domain" then
         toislandfunc(Vector3.new(5310.8095703125, 21.594484329224, 129.39053344727),CFrame.new(5310.8095703125, 21.594484329224, 129.39053344727))

      elseif ISLAND =="Haunted Castle" then
         toislandfunc(Vector3.new(-9506.1064453125, 142.13989257813, 5526.0405273438),CFrame.new(-9506.1064453125, 142.13989257813, 5526.0405273438))
      elseif ISLAND == "Ice Cream Island" then
         toislandfunc(Vector3.new(-871.98492431641, 65.819549560547, -10919.76953125),CFrame.new(-871.98492431641, 65.819549560547, -10919.76953125))
      elseif ISLAND == "Peanut Island" then
         toislandfunc(Vector3.new(-2018.2635498047, 38.103397369385, -10333.181640625),CFrame.new(-2018.2635498047, 38.103397369385, -10333.181640625))
      elseif ISLAND == "Cake Island" then
         toislandfunc(Vector3.new(-1866.54, 14.1332, -11615.2),CFrame.new(-1866.54, 14.1332, -11615.2))
      elseif ISLAND == "Sea of Treats" then
         toislandfunc(Vector3.new(229.584381, 24.7342587, -12189.1475, 0.999511659, 7.65095436e-08, -0.0312486049, -7.62648966e-08, 1, 9.02106656e-09, 0.0312486049, -6.63348976e-09, 0.999511659))
      end
   end
else
   tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(.1, Enum.EasingStyle.Linear)
   tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame})
   tween:Play()
   _G.Clip = false
end
end)
end)

Misc:Button("RTX Mode", function()
        if game:GetService("StarterGui"):SetCore("SendNotification",
            {
                Title = "SMZHUB",
                Text = "RTX Mode On",
                Icon = "http://roblox.com/asset/?id=8873625488",
                Duration = 4
            }
           ) then
            wait(10)
        end
	_G.LightMode = true
	if game:GetService("Lighting"):FindFirstChild("BloomEffect") then
		game:GetService("Lighting"):FindFirstChild("BloomEffect"):Destroy()
	end
	if game:GetService("Lighting"):FindFirstChild("ColorCorrectionEffect") then
		game:GetService("Lighting"):FindFirstChild("ColorCorrectionEffect"):Destroy()
	end
	if game:GetService("Lighting"):FindFirstChild("DepthOfFieldEffect") then
		game:GetService("Lighting"):FindFirstChild("DepthOfFieldEffect"):Destroy()
	end
	if game:GetService("Lighting"):FindFirstChild("ColorCorrectionEffect") then
		game:GetService("Lighting"):FindFirstChild("ColorCorrectionEffect"):Destroy()
	end
	if game:GetService("Lighting"):FindFirstChild("ColorCorrectionEffect2") then
		game:GetService("Lighting"):FindFirstChild("ColorCorrectionEffect2"):Destroy()
	end
	if game:GetService("Lighting"):FindFirstChild("SunRaysEffect") then
		game:GetService("Lighting"):FindFirstChild("SunRaysEffect"):Destroy()
	end
	local a = game.Lighting
	a.Ambient = Color3.fromRGB(31, 31, 31)
	a.Brightness = 0.7
	a.ColorShift_Bottom = Color3.fromRGB(255, 255, 255)
	a.ColorShift_Top = Color3.fromRGB(255, 102, 31)
	a.EnvironmentDiffuseScale = 0.205
	a.EnvironmentSpecularScale = 0.522
	a.GlobalShadows = true
	a.OutdoorAmbient = Color3.fromRGB(67, 67, 67)
	a.ShadowSoftness = 0.5
	a.GeographicLatitude = -15.525
	a.ExposureCompensation = 0.75
	local b = Instance.new("BloomEffect", a)
	b.Name = "BloomEffect"
	b.Enabled = true
	b.Intensity = 0.04
	b.Size = 1900
	b.Threshold = 0.915
	local c = Instance.new("ColorCorrectionEffect", a)
	c.Name = "ColorCorrectionEffect"
	c.Brightness = 0.176
	c.Contrast = 0.39
	c.Enabled = true
	c.Saturation = 0.2
	c.TintColor = Color3.fromRGB(255, 227, 128)
	local d = Instance.new("DepthOfFieldEffect", a)
	d.Name = "DepthOfFieldEffect"
	d.Enabled = true
	d.FarIntensity = 0.077
	d.FocusDistance = 21.54
	d.InFocusRadius = 20.77
	d.NearIntensity = 0.277
	local e = Instance.new("ColorCorrectionEffect", a)
	e.Name = "ColorCorrectionEffect"
	e.Brightness = 0.3
	e.Contrast = -0.07
	e.Saturation = 0
	e.Enabled = true
	e.TintColor = Color3.fromRGB(255, 247, 239)
	local e2 = Instance.new("ColorCorrectionEffect", a)
	e2.Name = "ColorCorrectionEffect2"
	e2.Brightness = 0.1
	e2.Contrast = 0.45
	e2.Saturation = -0.1
	e2.Enabled = true
	e2.TintColor = Color3.fromRGB(167, 167, 167)
	local s = Instance.new("SunRaysEffect", a)
	s.Name = "SunRaysEffect"
	s.Enabled = true
	s.Intensity = 0.01
	s.Spread = 0.146
end)

Misc:Button("Server Hop", function()
   DiscordLib:Notification("Hop Server", "Wait For Teleport", "Ok")
   Teleport()
end)

Misc:Button("FPS Boost", function()
    local decalsyeeted = true
    local g = game
    local w = g.Workspace
    local l = g.Lighting
    local t = w.Terrain
    t.WaterWaveSize = 0
    t.WaterWaveSpeed = 0
    t.WaterReflectance = 0
    t.WaterTransparency = 0
    l.GlobalShadows = false
    l.FogEnd = 9e9
    l.Brightness = 0
    settings().Rendering.QualityLevel = "Level01"
    for i, v in pairs(g:GetDescendants()) do
        if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then 
            v.Material = "Plastic"
            v.Reflectance = 0
        elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
            v.Transparency = 1
        elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
            v.Lifetime = NumberRange.new(0)
        elseif v:IsA("Explosion") then
            v.BlastPressure = 1
            v.BlastRadius = 1
        elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
            v.Enabled = false
        elseif v:IsA("MeshPart") then
            v.Material = "Plastic"
            v.Reflectance = 0
            v.TextureID = 10385902758728957
        end
    end
    for i, e in pairs(l:GetChildren()) do
        if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
            e.Enabled = false
        end
    end
end)

Misc:Button("Rejoin Server", function()
   game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").localPlayer)
end)

Misc:Button("Join Pirates", function()
   local args = {
       [1] = "SetTeam",
       [2] = "Pirates"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
   local args = {
       [1] = "BartiloQuestProgress"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

Misc:Button("Join Marines",function()
   local args = {
       [1] = "SetTeam",
       [2] = "Marines"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "BartiloQuestProgress"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

Misc:Button("Fruit Inventory", function()
   local args = {
       [1] = "getInventoryFruits"
   }
   
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventoryFruits")
   game:GetService("Players").LocalPlayer.PlayerGui.Main.FruitInventory.Visible = true
end)

Misc:Button("Inventory", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventoryWeapons")
   game.Players.localPlayer.PlayerGui.Main.Inventory.Visible = true
end)

Misc:Button("Fruit Shop", function()
   local args = {
       [1] = "GetFruits"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   game.Players.localPlayer.PlayerGui.Main.FruitShop.Visible = true
end)

Misc:Button("Title Name", function()
   local args = {
       [1] = "getTitles"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
end)

Misc:Button("Color Haki", function()
   game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
end)

PlayerName = {}
for i,v in pairs(game.Players:GetChildren()) do  
   table.insert(PlayerName ,v.Name)
end
function isnil(thing)
   return (thing == nil)
end
local function round(n)
   return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)
function UpdatePlayerChams()
   for i,v in pairs(game:GetService'Players':GetChildren()) do
       pcall(function()
           if not isnil(v.Character) then
               if ESPPlayer then
                   if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
                       local bill = Instance.new('BillboardGui',v.Character.Head)
                       bill.Name = 'NameEsp'..Number
                       bill.ExtentsOffset = Vector3.new(0, 1, 0)
                       bill.Size = UDim2.new(1,200,1,30)
                       bill.Adornee = v.Character.Head
                       bill.AlwaysOnTop = true
                       local name = Instance.new('TextLabel',bill)
                       name.Font = "GothamBold"
                       name.FontSize = "Size14"
                       name.TextWrapped = true
                       name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
                       name.Size = UDim2.new(1,0,1,0)
                       name.TextYAlignment = 'Top'
                       name.BackgroundTransparency = 1
                       name.TextStrokeTransparency = 0.5
                       if v.Team == game.Players.LocalPlayer.Team then
                           name.TextColor3 = Color3.new(0,255,0)
                       else
                           name.TextColor3 = Color3.new(255,0,0)
                       end
                   else
                       v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
                   end
               else
                   if v.Character.Head:FindFirstChild('NameEsp'..Number) then
                       v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
                   end
               end
           end
       end)
   end
end
function UpdateChestChams() 
   for i,v in pairs(game.Workspace:GetChildren()) do
       pcall(function()
           if string.find(v.Name,"Chest") then
               if ChestESP then
                   if string.find(v.Name,"Chest") then
                       if not v:FindFirstChild('NameEsp'..Number) then
                           local bill = Instance.new('BillboardGui',v)
                           bill.Name = 'NameEsp'..Number
                           bill.ExtentsOffset = Vector3.new(0, 1, 0)
                           bill.Size = UDim2.new(1,200,1,30)
                           bill.Adornee = v
                           bill.AlwaysOnTop = true
                           local name = Instance.new('TextLabel',bill)
                           name.Font = "GothamBold"
                           name.FontSize = "Size14"
                           name.TextWrapped = true
                           name.Size = UDim2.new(1,0,1,0)
                           name.TextYAlignment = 'Top'
                           name.BackgroundTransparency = 1
                           name.TextStrokeTransparency = 0.5
                           if v.Name == "Chest1" then
                               name.TextColor3 = Color3.fromRGB(109, 109, 109)
                               name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           end
                           if v.Name == "Chest2" then
                               name.TextColor3 = Color3.fromRGB(173, 158, 21)
                               name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           end
                           if v.Name == "Chest3" then
                               name.TextColor3 = Color3.fromRGB(85, 255, 255)
                               name.Text = ("Chest 3" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           end
                       else
                           v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                       end
                   end
               else
                   if v:FindFirstChild('NameEsp'..Number) then
                       v:FindFirstChild('NameEsp'..Number):Destroy()
                   end
               end
           end
       end)
   end
end
function UpdateDevilChams() 
   for i,v in pairs(game.Workspace:GetChildren()) do
       pcall(function()
           if DevilFruitESP then
               if string.find(v.Name, "Fruit") then   
                   if not v.Handle:FindFirstChild('NameEsp'..Number) then
                       local bill = Instance.new('BillboardGui',v.Handle)
                       bill.Name = 'NameEsp'..Number
                       bill.ExtentsOffset = Vector3.new(0, 1, 0)
                       bill.Size = UDim2.new(1,200,1,30)
                       bill.Adornee = v.Handle
                       bill.AlwaysOnTop = true
                       local name = Instance.new('TextLabel',bill)
                       name.Font = "GothamBold"
                       name.FontSize = "Size14"
                       name.TextWrapped = true
                       name.Size = UDim2.new(1,0,1,0)
                       name.TextYAlignment = 'Top'
                       name.BackgroundTransparency = 1
                       name.TextStrokeTransparency = 0.5
                       name.TextColor3 = Color3.fromRGB(255, 0, 0)
                       name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
                   else
                       v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
                   end
               end
           else
               if v.Handle:FindFirstChild('NameEsp'..Number) then
                   v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
               end
           end
       end)
   end
end
function UpdateFlowerChams() 
   for i,v in pairs(game.Workspace:GetChildren()) do
       pcall(function()
           if v.Name == "Flower2" or v.Name == "Flower1" then
               if FlowerESP then 
                   if not v:FindFirstChild('NameEsp'..Number) then
                       local bill = Instance.new('BillboardGui',v)
                       bill.Name = 'NameEsp'..Number
                       bill.ExtentsOffset = Vector3.new(0, 1, 0)
                       bill.Size = UDim2.new(1,200,1,30)
                       bill.Adornee = v
                       bill.AlwaysOnTop = true
                       local name = Instance.new('TextLabel',bill)
                       name.Font = "GothamBold"
                       name.FontSize = "Size14"
                       name.TextWrapped = true
                       name.Size = UDim2.new(1,0,1,0)
                       name.TextYAlignment = 'Top'
                       name.BackgroundTransparency = 1
                       name.TextStrokeTransparency = 0.5
                       name.TextColor3 = Color3.fromRGB(255, 0, 0)
                       if v.Name == "Flower1" then 
                           name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           name.TextColor3 = Color3.fromRGB(0, 0, 255)
                       end
                       if v.Name == "Flower2" then
                           name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           name.TextColor3 = Color3.fromRGB(255, 0, 0)
                       end
                   else
                       v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                   end
               else
                   if v:FindFirstChild('NameEsp'..Number) then
                       v:FindFirstChild('NameEsp'..Number):Destroy()
                   end
               end
           end   
       end)
   end
end
espfruit:Ti("ESP")

espfruit:Toggle("ESP Player",false,function(a)
   ESPPlayer = a
   while ESPPlayer do wait()
       UpdatePlayerChams()
   end
end)
espfruit:Toggle("ESP Chest",false,function(a)
   ChestESP = a
   while ChestESP do wait()
       UpdateChestChams() 
   end
end)
espfruit:Toggle("ESP Devil Fruit",false,function(a)
   DevilFruitESP = a
   while DevilFruitESP do wait()
       UpdateDevilChams() 
   end
end)
espfruit:Toggle("ESP Flower",false,function(a)
   FlowerESP = a
   while FlowerESP do wait()
       UpdateFlowerChams() 
   end
end)

espfruit1:Ti("Fruit")

espfruit1:Toggle("Auto Random Fruit",false,function(v)
   DevilAutoBuy = v
end)

spawn(function()
   while wait(1) do
       if DevilAutoBuy then wait()
           game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
       end
   end
end)

espfruit1:Toggle("Auto Drop Fruit", false, function(vu)
   Drop = vu
end)

spawn(function()
   while wait() do
       if Drop then
           pcall(function()
               for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
                   if string.find(v.Name, "Fruit") then
                       EquipWeapon(v.Name)
                       SelectFruit = v.Name
                       wait(.1)
                       if game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible == true then
                           game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible = false
                       end
                       EquipWeapon(v.Name)
                       game:GetService("Players").LocalPlayer.Character:FindFirstChild(SelectFruit).EatRemote:InvokeServer("Drop")
                   end
               end
               for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
                   if string.find(v.Name, "Fruit") then
                       EquipWeapon(v.Name)
                       SelectFruit = v.Name
                       wait(.1)
                       if game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible == true then
                           game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible = false
                       end
                       EquipWeapon(v.Name)
                       game:GetService("Players").LocalPlayer.Character:FindFirstChild(SelectFruit).EatRemote:InvokeServer("Drop")
                   end
               end
           end)
       end
   end
end)

espfruit1:Toggle("Bring Fruit [Droped]",false,function(t)
   _G.BringFruit = t
end)

spawn(function()
   while wait() do
       if _G.BringFruit then
           pcall(function()
               if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
                   for i,v in pairs(game.Workspace:GetChildren()) do
                       if v:IsA("Tool") then
                           if (v.Handle.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 20000 then
                               v.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
                           else 
                               TP(v.Handle.CFrame)
                           end
                       end
                   end
               end
           end)
       end
   end
end)

espfruit1:Toggle("Auto Store Fruit",false,function(value)
   _G.KeepFruit = value
end)

spawn(function()
   while wait() do
       if _G.KeepFruit then
           wait(0.5)
           local a =     {
               "Bomb-Bomb",
               "Spike-Spike",
               "Chop-Chop",
               "Spring-Spring",
               "Kilo-Kilo",
               "Smoke-Smoke",
               "Spin-Spin",
               "Flame-Flame",
               "Brid:Falcon",
               "Ice-Ice",
               "Sand-Sand",
               "Dark-Dark",
               "Diamond-Diamond",
               "Light-Light",
               "Love-Love",
               "Rubber-Rubber",
               "Barrier-Barrier",
               "Magma-Magma",
               "Door-Door",
               "Quake-Quake",
               "Human-Human: Buddha",
               "String-String",
               "Bird-Bird: Phoenix",
               "Rumble-Rumble",
               "Paw-Paw",
               "Gravity-Gravity",
               "Dough-Dough",
               "Venom-Venom",
               "Control-Control",
               "Soul-Soul",
               "Dragon-Dragon"
           }
           pcall(function()  
               for i,v in pairs(a) do
                   if _G.KeepFruit then
                       game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit",v)
                   end
               end
           end)
       end
   end
end)

espfruit1:Ti("Auto Buy Fruit")

espfruit1:Toggle("Buy Devil Fruit Sinper",false,function(value)
   BuyFruitSinper = vu
end)
local l__Remotes__11 = game.ReplicatedStorage:WaitForChild("Remotes");
u45 = l__Remotes__11.CommF_:InvokeServer("GetFruits");
Table_DevilFruitSniper = {}
for i,v in next,u45 do
   table.insert(Table_DevilFruitSniper,v.Name)
end
espfruit1:DropDown("DevilFruit Sniper","Select",Table_DevilFruitSniper,function(ply)
   SelectDevil = ply
end)

spawn(function()
   while wait(.1) do
       if BuyFruitSinper then
           game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("GetFruits")
           game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PurchaseRawFruit",SelectDevil)
       end 
   end
end)

BuyItem:Ti("F")

BuyItem:Button("Refund Stat", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","1")
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","2")
end)

BuyItem:Button("Reroll Race", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Reroll","1")
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Reroll","2")
end)

BuyItem:Ti("Other")

BuyItem:Button("Haki", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Buso")
end)
BuyItem:Button("Geppo", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Geppo")
end)
BuyItem:Button("Soru", function()
  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Soru")
end)
BuyItem:Button("KenHaki", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk","Buy")
end)

BuyItem:Ti("Fighting Style")

BuyItem:Button("Black Leg", function()
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyBlackLeg")
end)

BuyItem:Button("Electro", function()
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
end)

BuyItem:Button("Fishman Karate", function()
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
end)

BuyItem:Button("Dragon Claw", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","1")
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2")
end)

BuyItem:Button("Superhuman", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
end)
BuyItem:Button("Death Step", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
end)
BuyItem:Button("Sharkman Karate", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true)
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
end)
BuyItem:Button("Electric Claw", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw",true)
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
end)

BuyItem:Button("Dragon Talon", function()
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon",true)
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
end)

BuyItem:Ti("Sword")

BuyItem:Button("Katana ($1,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Katana"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Cutlass ($1,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Cutlass"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)  
BuyItem:Button("Dual Katana ($12,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Dual Katana"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Iron Mace ($25,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Iron Mace"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Triple Katana ($60,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Triple Katana"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Pipe ($100,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Pipe"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Soul Cane ($750,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Soul Cane"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Dual-Headed Blade ($400,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Dual-Headed Blade"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Bisento ($1,200,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Bisento"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Ti("Gun")

BuyItem:Button("Slingshot ($5,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Slingshot"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Musket ($8,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Musket"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Flintlock ($10,500 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Flintlock"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Refined Slingshot ($30,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Refined Slingshot"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Refined Flintlock ($65,000 Beli)",function()
   local args = {
       [1] = "BuyItem",
       [2] = "Refined Flintlock"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Kabucha (1,500 Fragments)",function()
   game.ReplicatedStorage.Remotes.CommF_:InvokeServer("BlackbeardReward", "Slingshot", "2")
end)

spawn(function()
while wait() do
    if _G.AutoFarm or _G.AutoFarmMasteryFruit or _G.AutoFarmMasteryGun or _G.AutoFarmBone or Auto_Rengoku or Auto_Ectoplasm then
        if _G.BringMob then
            pcall(function()
                CheckLv()
                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                    for i,x in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == Mon then
                            if x.Name == Mon then
                                if v:FindFirstChild("HumanoidRootPart") and x:FindFirstChild("HumanoidRootPart") then
                                    v.HumanoidRootPart.CFrame = x.HumanoidRootPart.CFrame
                                    v.HumanoidRootPart.CanCollide = false
                                    x.HumanoidRootPart.CanCollide = false
                                    v.Head.CanCollide = false
                                    x.Head.CanCollide = false
                                    v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                                    x.HumanoidRootPart.Size = Vector3.new(60,60,60)
                                    v.Humanoid.WalkSpeed = 0
                                    x.Humanoid.WalkSpeed = 0
                                    sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                                end --SmZSsSSSSSSSSSSSSSSSSSSSS
                            end
                        end
                    end
                end
            end)
        end
    end
end
end)

pcall(function()
	for i,v in pairs(game:GetService("Workspace").Map.Dressrosa.Tavern:GetDescendants()) do
		if v.ClassName == "Seat" then
			v:Destroy()
		end
	end
end)


local placeId = game.PlaceId
Magnet = true
if placeId == 2753915549 then
	OldWorld = true
elseif placeId == 4442272183 then
	NewWorld = true
elseif placeId == 7449423635 then
	ThreeWorld = true
end
function CheckLv()
 
   MyLevel = game:GetService("Players").LocalPlayer.Data.Level.Value
       if OldWorld then
   if MyLevel == 1 or MyLevel <= 9 then
       Mon = "Bandit [Lv. 5]"
       LevelQuest = 1
       NameQuest = "BanditQuest1"
       NameMon = "Bandit"
       PQUEST = Vector3.new(1059.37195, 15.4495068, 1550.4231, 0.939700544, -0, -0.341998369, 0, 1, -0, 0.341998369, 0, 0.939700544)
       CMON = CFrame.new(1184.6668701172, 66.851402282715, 1513.2677001953)
       CQUEST = CFrame.new(1059.37195, 15.4495068, 1550.4231, 0.939700544, -0, -0.341998369, 0, 1, -0, 0.341998369, 0, 0.939700544)
       PMON = Vector3.new(1184.6668701172, 66.851402282715, 1513.2677001953)

   elseif MyLevel == 10 or MyLevel <= 14 then
       Mon = "Monkey [Lv. 14]"
       LevelQuest = 1
       NameQuest = "JungleQuest"
       NameMon = "Monkey"
       PQUEST = Vector3.new(-1598.08911, 35.5501175, 153.377838, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       CMON = CFrame.new(-1606.4381103516, 35.292171478271, 171.13681030273)
       CQUEST = CFrame.new(-1598.08911, 35.5501175, 153.377838, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       PMON = Vector3.new(-1606.4381103516, 35.292171478271, 171.13681030273)

   elseif MyLevel == 15 or MyLevel <= 29 then
       Mon = "Gorilla [Lv. 20]"
       LevelQuest = 2
       NameQuest = "JungleQuest"
       NameMon = "Gorilla"
       PQUEST = Vector3.new(-1598.08911, 35.5501175, 153.377838, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       CMON = CFrame.new(-1289.9700927734, 18.621431350708, -343.4475402832)
       CQUEST = CFrame.new(-1598.08911, 35.5501175, 153.377838, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       PMON = Vector3.new(-1289.9700927734, 18.621431350708, -343.4475402832)

   elseif MyLevel == 30 or MyLevel <= 39 then
       Mon = "Pirate [Lv. 35]"
       LevelQuest = 1
       NameQuest = "BuggyQuest1"
       NameMon = "Pirate"
       PQUEST = Vector3.new(-1141.07483, 4.10001802, 3831.5498, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       CMON = CFrame.new(-1210.4885253906, 4.7520518302917, 3901.2900390625)
       CQUEST = CFrame.new(-1141.07483, 4.10001802, 3831.5498, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       PMON = Vector3.new(-1210.4885253906, 4.7520518302917, 3901.2900390625)

   elseif MyLevel == 40 or MyLevel <= 59 then
       Mon = "Brute [Lv. 45]"
       LevelQuest = 2
       NameQuest = "BuggyQuest1"
       NameMon = "Brute"
       PQUEST = Vector3.new(-1141.07483, 4.10001802, 3831.5498, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       CMON = CFrame.new(-1123.4816894531, 14.809873580933, 4300.3334960938)
       CQUEST = CFrame.new(-1141.07483, 4.10001802, 3831.5498, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       PMON = Vector3.new(-1123.4816894531, 14.809873580933, 4300.3334960938)

   elseif MyLevel == 60 or MyLevel <= 74 then
       Mon = "Desert Bandit [Lv. 60]"
       LevelQuest = 1
       NameQuest = "DesertQuest"
       NameMon = "Desert Bandit"
       PQUEST = Vector3.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
       CMON = CFrame.new(898.62774658203, 6.4384622573853, 4407.58203125)
       CQUEST = CFrame.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
       PMON = Vector3.new(898.62774658203, 6.4384622573853, 4407.58203125)

   elseif MyLevel == 75 or MyLevel <= 89 then
       Mon = "Desert Officer [Lv. 70]"
       LevelQuest = 2
       NameQuest = "DesertQuest"
       NameMon = "Desert Officer"
       PQUEST = Vector3.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
       CMON = CFrame.new(1537.9205322266, 14.452037811279, 4386.3881835938)
       CQUEST = CFrame.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
       PMON = Vector3.new(1537.9205322266, 14.452037811279, 4386.3881835938)

   elseif MyLevel == 90 or MyLevel <= 99 then
       Mon = "Snow Bandit [Lv. 90]"
       LevelQuest = 1
       NameQuest = "SnowQuest"
       NameMon = "Snow Bandit"
       PQUEST = Vector3.new(1389.74451, 88.1519318, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
       CMON = CFrame.new(1379.6555175781, 87.272789001465, -1354.8793945313)
       CQUEST = CFrame.new(1389.74451, 88.1519318, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
       PMON = Vector3.new(1379.6555175781, 87.272789001465, -1354.8793945313)

   elseif MyLevel == 100 or MyLevel <= 119 then
       Mon = "Snowman [Lv. 100]"
       LevelQuest = 2
       NameQuest = "SnowQuest"
       NameMon = "Snowman"
       PQUEST = Vector3.new(1389.74451, 88.1519318, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
       CMON = CFrame.new(1296.3176269531, 105.77800750732, -1586.8228759766)
       CQUEST = CFrame.new(1389.74451, 88.1519318, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
       PMON = Vector3.new(1296.3176269531, 105.77800750732, -1586.8228759766)

   elseif MyLevel == 120 or MyLevel <= 149 then
       Mon = "Chief Petty Officer [Lv. 120]"
       LevelQuest = 1
       NameQuest = "MarineQuest2"
       NameMon = "Chief Petty Officer"
       PQUEST = Vector3.new(-5039.58643, 27.3500385, 4324.68018, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       CMON = CFrame.new(-4926.9541015625, 20.652038574219, 4254.30859375)
       CQUEST = CFrame.new(-5039.58643, 27.3500385, 4324.68018, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       PMON = Vector3.new(-4926.9541015625, 20.652038574219, 4254.30859375)

   elseif MyLevel == 150 or MyLevel <= 174 then
       Mon = "Sky Bandit [Lv. 150]"
       LevelQuest = 1
       NameQuest = "SkyQuest"
       NameMon = "Sky Bandit"
       PQUEST = Vector3.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       CMON = CFrame.new(-5035.4375, 278.06744384766, -2845.1437988281)
       CQUEST = CFrame.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       PMON = Vector3.new(-5035.4375, 278.06744384766, -2845.1437988281)

   elseif MyLevel == 175 or MyLevel <= 189 then
       Mon = "Dark Master [Lv. 175]"
       LevelQuest = 2
       NameQuest = "SkyQuest"
       NameMon = "Dark Master"
       PQUEST = Vector3.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       CMON = CFrame.new(-5252.2421875, 388.65203857422, -2273.1125488281)
       CQUEST = CFrame.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       PMON = Vector3.new(-5252.2421875, 388.65203857422, -2273.1125488281)

    elseif MyLevel == 190 or MyLevel <= 209 then
        Mon = "Prisoner [Lv. 190]"
        LevelQuest = 1
        NameQuest = "PrisonerQuest"
        NameMon = "Prisoner"
        PQUEST = Vector3.new(5308.72119, 1.65511298, 474.088745, 0.391072512, 5.46925989e-08, -0.92035985, -1.40744483e-08, 1, 5.34448219e-08, 0.92035985, -7.94724375e-09, 0.391072512)
        CMON = CFrame.new(4937.40674, 15.6515369, 565.219666, -0.483960688, 1.04728592e-07, -0.875089705, 2.53960444e-08, 1, 1.05632488e-07, 0.875089705, 2.88981568e-08, -0.483960688)
        CQUEST = CFrame.new(5308.72119, 1.65511298, 474.088745, 0.391072512, 5.46925989e-08, -0.92035985, -1.40744483e-08, 1, 5.34448219e-08, 0.92035985, -7.94724375e-09, 0.391072512)
        PMON = Vector3.new(4937.40674, 15.6515369, 565.219666, -0.483960688, 1.04728592e-07, -0.875089705, 2.53960444e-08, 1, 1.05632488e-07, 0.875089705, 2.88981568e-08, -0.483960688)

    elseif MyLevel == 210 or MyLevel <= 249 then
        Mon = "Dangerous Prisoner [Lv. 210]"
        LevelQuest = 2
        NameQuest = "PrisonerQuest"
        NameMon = "Dangerous Prisoner"
        PQUEST = Vector3.new(5463.104, 15.6328878, 973.506042, -0.682176471, 4.0302389e-08, -0.731187582, 6.34130473e-08, 1, -4.04342249e-09, 0.731187582, -4.91251591e-08, -0.682176471)
        CMON = CFrame.new(4937.40674, 15.6515369, 565.219666, -0.483960688, 1.04728592e-07, -0.875089705, 2.53960444e-08, 1, 1.05632488e-07, 0.875089705, 2.88981568e-08, -0.483960688)
        CQUEST = CFrame.new(5463.104, 15.6328878, 973.506042, -0.682176471, 4.0302389e-08, -0.731187582, 6.34130473e-08, 1, -4.04342249e-09, 0.731187582, -4.91251591e-08, -0.682176471)
        PMON = Vector3.new(4937.40674, 15.6515369, 565.219666, -0.483960688, 1.04728592e-07, -0.875089705, 2.53960444e-08, 1, 1.05632488e-07, 0.875089705, 2.88981568e-08, -0.483960688)

   elseif MyLevel == 250 or MyLevel <= 274 then
       Mon = "Toga Warrior [Lv. 250]"
       LevelQuest = 1
       NameQuest = "ColosseumQuest"
       NameMon = "Toga Warrior"
       PQUEST = Vector3.new(-1580.04663, 6.35000277, -2986.47534, -0.515037298, 0, -0.857167721, 0, 1, 0, 0.857167721, 0, -0.515037298)
       CMON = CFrame.new(-1951.6307373047, 7.2890739440918, -2795.9350585938)
       CQUEST = CFrame.new(-1580.04663, 6.35000277, -2986.47534, -0.515037298, 0, -0.857167721, 0, 1, 0, 0.857167721, 0, -0.515037298)
       PMON = Vector3.new(-1951.6307373047, 7.2890739440918, -2795.9350585938)

   elseif MyLevel == 275 or MyLevel <= 299 then
       Mon = "Gladiator [Lv. 275]"
       LevelQuest = 2
       NameQuest = "ColosseumQuest"
       NameMon = "Gladiator"
       PQUEST = Vector3.new(-1580.04663, 6.35000277, -2986.47534, -0.515037298, 0, -0.857167721, 0, 1, 0, 0.857167721, 0, -0.515037298)
       CMON = CFrame.new(-1361.2359619141, 7.4425468444824, -3206.2006835938)
       CQUEST = CFrame.new(-1580.04663, 6.35000277, -2986.47534, -0.515037298, 0, -0.857167721, 0, 1, 0, 0.857167721, 0, -0.515037298)
       PMON = Vector3.new(-1361.2359619141, 7.4425468444824, -3206.2006835938)

   elseif MyLevel == 300 or MyLevel <= 324 then
       Mon = "Military Soldier [Lv. 300]"
       LevelQuest = 1
       NameQuest = "MagmaQuest"
       NameMon = "Military Soldier"
       PQUEST = Vector3.new(-5313.37012, 10.9500084, 8515.29395, -0.499959469, 0, 0.866048813, 0, 1, 0, -0.866048813, 0, -0.499959469)
       CMON = CFrame.new(-5425.244140625, 10.298267364502, 8442.607421875)
       CQUEST = CFrame.new(-5313.37012, 10.9500084, 8515.29395, -0.499959469, 0, 0.866048813, 0, 1, 0, -0.866048813, 0, -0.499959469)
       PMON = Vector3.new(-5425.244140625, 10.298267364502, 8442.607421875)

   elseif MyLevel == 325 or MyLevel <= 449 then
       Mon = "Military Spy [Lv. 325]"
       LevelQuest = 2
       NameQuest = "MagmaQuest"
       NameMon = "Military Spy"
       PQUEST = Vector3.new(-5313.37012, 10.9500084, 8515.29395, -0.499959469, 0, 0.866048813, 0, 1, 0, -0.866048813, 0, -0.499959469)
       CMON = CFrame.new(-5808.0297851563, 82.834617614746, 8825.5166015625)
       CQUEST = CFrame.new(-5313.37012, 10.9500084, 8515.29395, -0.499959469, 0, 0.866048813, 0, 1, 0, -0.866048813, 0, -0.499959469)
       PMON = Vector3.new(-5808.0297851563, 82.834617614746, 8825.5166015625)
  
   elseif MyLevel == 450 or MyLevel <= 474 then
       Mon = "God's Guard [Lv. 450]"
       LevelQuest = 1
       NameQuest = "SkyExp1Quest"
       NameMon = "God's Guard"
       PQUEST = Vector3.new(-4721.88867, 843.874695, -1949.96643, 0.996191859, -0, -0.0871884301, 0, 1, -0, 0.0871884301, 0, 0.996191859)
       CMON = CFrame.new(-4681.8432617188, 845.27716064453, -1955.4534912109)
       CQUEST = CFrame.new(-4721.88867, 843.874695, -1949.96643, 0.996191859, -0, -0.0871884301, 0, 1, -0, 0.0871884301, 0, 0.996191859)
       PMON = Vector3.new(-4681.8432617188, 845.27716064453, -1955.4534912109)

   elseif MyLevel == 475 or MyLevel <= 524 then
       Mon = "Shanda [Lv. 475]"
       LevelQuest = 2
       NameQuest = "SkyExp1Quest"
       NameMon = "Shanda"
       PQUEST = Vector3.new(-7859.09814, 5544.19043, -381.476196, -0.422592998, 0, 0.906319618, 0, 1, 0, -0.906319618, 0, -0.422592998)
       CMON = CFrame.new(-7656.3056640625, 5545.4931640625, -531.23907470703)
       CQUEST = CFrame.new(-7859.09814, 5544.19043, -381.476196, -0.422592998, 0, 0.906319618, 0, 1, 0, -0.906319618, 0, -0.422592998)
       PMON = Vector3.new(-7656.3056640625, 5545.4931640625, -531.23907470703)

   elseif MyLevel == 525 or MyLevel <= 549 then
       Mon = "Royal Squad [Lv. 525]"
       LevelQuest = 1
       NameQuest = "SkyExp2Quest"
       NameMon = "Royal Squad"
       PQUEST = Vector3.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       CMON = CFrame.new(-7722.328125, 5610.9272460938, -1441.6092529297)
       CQUEST = CFrame.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       PMON = Vector3.new(-7722.328125, 5610.9272460938, -1441.6092529297)

   elseif MyLevel == 550 or MyLevel <= 624 then
       Mon = "Royal Soldier [Lv. 550]"
       LevelQuest = 2
       NameQuest = "SkyExp2Quest"
       NameMon = "Royal Soldier"
       PQUEST = Vector3.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       CMON = CFrame.new(-7825.0087890625, 5606.8784179688, -1731.4152832031)
       CQUEST = CFrame.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       PMON = Vector3.new(-7825.0087890625, 5606.8784179688, -1731.4152832031)

   elseif MyLevel == 625 or MyLevel <= 649 then
       Mon = "Galley Pirate [Lv. 625]"
       LevelQuest = 1
       NameQuest = "FountainQuest"
       NameMon = "Galley Pirate"
       PQUEST = Vector3.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
       CMON = CFrame.new(5379.8198242188, 38.501140594482, 4033.5905761719)
       CQUEST = CFrame.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
       PMON = Vector3.new(5379.8198242188, 38.501140594482, 4033.5905761719)

   elseif MyLevel >= 650 then
       Mon = "Galley Captain [Lv. 650]"
       LevelQuest = 2
       NameQuest = "FountainQuest"
       NameMon = "Galley Captain"
       PQUEST = Vector3.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
       CMON = CFrame.new(5556.1420898438, 113.47412109375, 4819.0576171875)
       CQUEST = CFrame.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
       PMON = Vector3.new(5556.1420898438, 113.47412109375, 4819.0576171875)
   end
elseif NewWorld then

   if MyLevel == 700 or MyLevel <= 724 then
       Mon = "Raider [Lv. 700]"
       LevelQuest = 1
       NameQuest = "Area1Quest"
       NameMon = "Raider"
       PQUEST = Vector3.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
       CMON = CFrame.new(-122.82179260254, 39.079746246338, 2362.2602539063)
       CQUEST = CFrame.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
       PMON = Vector3.new(-122.82179260254, 39.079746246338, 2362.2602539063)

   elseif MyLevel == 725 or MyLevel <= 774 then
       Mon = "Mercenary [Lv. 725]"
       LevelQuest = 2
       NameQuest = "Area1Quest"
       NameMon = "Mercenary"
       PQUEST = Vector3.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
       CMON = CFrame.new(-942.66076660156, 72.959716796875, 1720.8294677734)
       CQUEST = CFrame.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
       PMON = Vector3.new(-942.66076660156, 72.959716796875, 1720.8294677734)
       
   elseif MyLevel == 775 or MyLevel <= 799 then
       Mon = "Swan Pirate [Lv. 775]"
       LevelQuest = 1
       NameQuest = "Area2Quest"
       NameMon = "Swan Pirate"
       PQUEST = Vector3.new(638.43811, 71.769989, 918.282898, 0.139203906, 0, 0.99026376, 0, 1, 0, -0.99026376, 0, 0.139203906)
       CMON = CFrame.new(1024.1345214844, 73.029739379883, 1262.7456054688)
       CQUEST = CFrame.new(638.43811, 71.769989, 918.282898, 0.139203906, 0, 0.99026376, 0, 1, 0, -0.99026376, 0, 0.139203906)
       PMON = Vector3.new(1024.1345214844, 73.029739379883, 1262.7456054688)

   elseif MyLevel == 800 or MyLevel <= 874 then
       Mon = "Factory Staff [Lv. 800]"
       NameQuest = "Area2Quest"
       LevelQuest = 2
       NameMon = "Factory Staff"
       CQUEST = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
       PQUEST = Vector3.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
       CMON = CFrame.new(296.786499, 72.9948196, -57.1298141, -0.876037002, -5.32364979e-08, 0.482243896, -3.87658332e-08, 1, 3.99718729e-08, -0.482243896, 1.63222538e-08, -0.876037002)
       PMON = Vector3.new(296.786499, 72.9948196, -57.1298141, -0.876037002, -5.32364979e-08, 0.482243896, -3.87658332e-08, 1, 3.99718729e-08, -0.482243896, 1.63222538e-08, -0.876037002)

   elseif MyLevel == 875 or MyLevel <= 899 then
       Mon = "Marine Lieutenant [Lv. 875]"
       LevelQuest = 1
       NameQuest = "MarineQuest3"
       NameMon = "Marine Lieutenant"
       PQUEST = Vector3.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       CMON = CFrame.new(-2842.595703125, 72.96614074707, -3012.0222167969)
       CQUEST = CFrame.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       PMON = Vector3.new(-2842.595703125, 72.96614074707, -3012.0222167969)

   elseif MyLevel == 900 or MyLevel <= 949 then
       Mon = "Marine Captain [Lv. 900]"
       LevelQuest = 2
       NameQuest = "MarineQuest3"
       NameMon = "Marine Captain"
       PQUEST = Vector3.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       CMON = CFrame.new(-1927.8619384766, 72.96614074707, -3385.0322265625)
       CQUEST = CFrame.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
       PMON = Vector3.new(-1927.8619384766, 72.96614074707, -3385.0322265625)

   elseif MyLevel == 950 or MyLevel <= 974 then
       Mon = "Zombie [Lv. 950]"
       LevelQuest = 1
       NameQuest = "ZombieQuest"
       NameMon = "Zombie"
       PQUEST = Vector3.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
       CMON = CFrame.new(-5685.9233398438, 48.480125427246, -853.23724365234)
       CQUEST = CFrame.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
       PMON = Vector3.new(-5685.9233398438, 48.480125427246, -853.23724365234)

   elseif MyLevel == 975 or MyLevel <= 999 then
       Mon = "Vampire [Lv. 975]"
       LevelQuest = 2
       NameQuest = "ZombieQuest"
       NameMon = "Vampire"
       PQUEST = Vector3.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
       CMON = CFrame.new(-6018.3452148438, 6.4027013778687, -1267.6065673828)
       CQUEST = CFrame.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
       PMON = Vector3.new(-6018.3452148438, 6.4027013778687, -1267.6065673828)

   elseif MyLevel == 1000 or MyLevel <= 1049 then
       Mon = "Snow Trooper [Lv. 1000]"
       LevelQuest = 1
       NameQuest = "SnowMountainQuest"
       NameMon = "Snow Trooper"
       PQUEST = Vector3.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
       CMON = CFrame.new(481.48031616211, 401.42202758789, -5361.2138671875)
       CQUEST = CFrame.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
       PMON = Vector3.new(481.48031616211, 401.42202758789, -5361.2138671875)

   elseif MyLevel == 1050 or MyLevel <= 1099 then
       Mon = "Winter Warrior [Lv. 1050]"
       LevelQuest = 2
       NameQuest = "SnowMountainQuest"
       NameMon = "Winter Warrior"
       PQUEST = Vector3.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
       CMON = CFrame.new(1148.3015136719, 429.38235473633, -5262.1708984375)
       CQUEST = CFrame.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
       PMON = Vector3.new(1148.3015136719, 429.38235473633, -5262.1708984375)

   elseif MyLevel == 1100 or MyLevel <= 1124 then
       Mon = "Lab Subordinate [Lv. 1100]"
       LevelQuest = 1
       NameQuest = "IceSideQuest"
       NameMon = "Lab Subordinate"
       PQUEST = Vector3.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
       CMON = CFrame.new(-5775.5200195313, 42.301044464111, -4483.5092773438)
       CQUEST = CFrame.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
       PMON = Vector3.new(-5775.5200195313, 42.301044464111, -4483.5092773438)

   elseif MyLevel == 1125 or MyLevel <= 1174 then
       Mon = "Horned Warrior [Lv. 1125]"
       LevelQuest = 2
       NameQuest = "IceSideQuest"
       NameMon = "Horned Warrior"
       PQUEST = Vector3.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
       CMON = CFrame.new(-6283.5942382813, 18.321973800659, -5606.4282226563)
       CQUEST = CFrame.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
       PMON = Vector3.new(-6283.5942382813, 18.321973800659, -5606.4282226563)

   elseif MyLevel == 1175 or MyLevel <= 1199 then
       Mon = "Magma Ninja [Lv. 1175]"
       LevelQuest = 1
       NameQuest = "FireSideQuest"
       NameMon = "Magma Ninja"
       PQUEST = Vector3.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       CMON = CFrame.new(-5686.64453125, 15.951762199402, -5713.7026367188)
       CQUEST = CFrame.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       PMON = Vector3.new(-5686.64453125, 15.951762199402, -5713.7026367188)

   elseif MyLevel == 1200 or MyLevel <= 1349 then
       Mon = "Lava Pirate [Lv. 1200]"
       LevelQuest = 2
       NameQuest = "FireSideQuest"
       NameMon = "Lava Pirate"
       PQUEST = Vector3.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       CMON = CFrame.new(-5363.17578125, 15.951762199402, -4754.68359375)
       CQUEST = CFrame.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       PMON = Vector3.new(-5363.17578125, 15.951762199402, -4754.68359375)

   elseif MyLevel == 1350 or MyLevel <= 1374 then
       Mon = "Arctic Warrior [Lv. 1350]"
       LevelQuest = 1
       NameQuest = "FrostQuest"
       NameMon = "Arctic Warrior"
       PQUEST = Vector3.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
       CMON = CFrame.new(6009.58203125, 28.367122650146, -6247.9741210938)
       CQUEST = CFrame.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
       PMON = Vector3.new(6009.58203125, 28.367122650146, -6247.9741210938)

   elseif MyLevel == 1375 or MyLevel <= 1424 then
       Mon = "Snow Lurker [Lv. 1375]"
       LevelQuest = 2
       NameQuest = "FrostQuest"
       NameMon = "Snow Lurker"
       PQUEST = Vector3.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
       CMON = CFrame.new(5476.5615234375, 28.82799911499, -6847.412109375)
       CQUEST = CFrame.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
       PMON = Vector3.new(5476.5615234375, 28.82799911499, -6847.412109375)

   elseif MyLevel == 1425 or MyLevel <= 1449 then
       Mon = "Sea Soldier [Lv. 1425]"
       LevelQuest = 1
       NameQuest = "ForgottenQuest"
       NameMon = "Sea Soldier"
       PQUEST = Vector3.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
       CMON = CFrame.new(-3032.2255859375, 70.041687011719, -9779.5869140625)
       CQUEST = CFrame.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
       PMON = Vector3.new(-3032.2255859375, 70.041687011719, -9779.5869140625)

   elseif MyLevel >= 1450 then
       Mon = "Water Fighter [Lv. 1450]"
       LevelQuest = 2
       NameQuest = "ForgottenQuest"
       NameMon = "Water Fighter"
       PQUEST = Vector3.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
       CMON = CFrame.new(-3261.4780273438, 291.33917236328, -10596.365234375)
       CQUEST = CFrame.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
       PMON = Vector3.new(-3261.4780273438, 291.33917236328, -10596.365234375)
   end
elseif ThreeWorld then

   if MyLevel == 1500 or MyLevel <= 1524 then
       Mon = "Pirate Millionaire [Lv. 1500]"
       LevelQuest = 1
       NameQuest = "PiratePortQuest"
       NameMon = "Pirate Millionaire"
       PQUEST = Vector3.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       CMON = CFrame.new(-366.55215454102, 68.321365356445, 5561.5541992188)
       CQUEST = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       PMON = Vector3.new(-366.55215454102, 68.321365356445, 5561.5541992188)
       
   elseif MyLevel == 1525 or MyLevel <= 1574 then
       Mon = "Pistol Billionaire [Lv. 1525]"
       LevelQuest = 2
       NameQuest = "PiratePortQuest"
       NameMon = "Pistol Billionaire"
       PQUEST = Vector3.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       CMON = CFrame.new(-413.86712646484, 123.34642028809, 5857.123046875)
       CQUEST = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
       PMON = Vector3.new(-413.86712646484, 123.34642028809, 5857.123046875)
       
   elseif MyLevel == 1575 or MyLevel <= 1599 then
       Mon = "Dragon Crew Warrior [Lv. 1575]"
       LevelQuest = 1
       NameQuest = "AmazonQuest"
       NameMon = "Dragon Crew Warrior"
       PQUEST = Vector3.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
       CMON = CFrame.new(6297.5546875, 108.10154724121, -1078.3551025391)
       CQUEST = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
       PMON = Vector3.new(6297.5546875, 108.10154724121, -1078.3551025391)
    elseif MyLevel == 1600 or MyLevel <= 1624 then 
       Mon = "Dragon Crew Archer [Lv. 1600]"
       NameQuest = "AmazonQuest"
       LevelQuest = 2
       NameMon = "Dragon Crew Archer"
       CQUEST = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
       PQUEST = Vector3.new(5833.1147460938, 51.60498046875, -1103.0693359375)
       CMON = CFrame.new(6831.1171875, 441.76708984375, 446.58615112305)
       PMON = Vector3.new(6831.1171875, 441.76708984375, 446.58615112305)
    elseif MyLevel == 1625 or MyLevel <= 1649 then
       Mon = "Female Islander [Lv. 1625]"
       NameQuest = "AmazonQuest2"
       LevelQuest = 1
       NameMon = "Female Islander"
       CQUEST = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
       CMON = CFrame.new(5792.5166015625, 848.14392089844, 1084.1818847656)
       PQUEST = Vector3.new(5446.8793945313, 601.62945556641, 749.45672607422)
       PMON = Vector3.new(5792.5166015625, 848.14392089844, 1084.1818847656)
    elseif MyLevel == 1650 or MyLevel <= 1699 then 
       Mon = "Giant Islander [Lv. 1650]"
       NameQuest = "AmazonQuest2"
       LevelQuest = 2
       NameMon = "Giant Islander"
       CQUEST = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
       CMON = CFrame.new(5009.5068359375, 664.11071777344, -40.960144042969)
       PQUEST = Vector3.new(5446.8793945313, 601.62945556641, 749.45672607422)
       PMON = Vector3.new(5446.8793945313, 601.62945556641, 749.45672607422)    

   elseif MyLevel == 1700 or MyLevel <= 1724 then
       Mon = "Marine Commodore [Lv. 1700]"
       LevelQuest = 1
       NameQuest = "MarineTreeIsland"
       NameMon = "Marine Commodore"
       PQUEST = Vector3.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
       CMON = CFrame.new(2335.4865722656, 190.39758300781, -7183.552734375)
       CQUEST = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
       PMON = Vector3.new(2335.4865722656, 190.39758300781, -7183.552734375)
    elseif MyLevel == 1725 or MyLevel <= 1774 then
       Mon = "Marine Rear Admiral [Lv. 1725]"
       NameMon = "Marine Rear Admiral"
       NameQuest = "MarineTreeIsland"
       LevelQuest = 2
       CQUEST = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
       CMON = CFrame.new(3294.3142089844, 385.41125488281, -7048.6342773438)
       PQUEST = Vector3.new(2179.98828125, 28.731239318848, -6740.0551757813)
       PMON = Vector3.new(3294.3142089844, 385.41125488281, -7048.6342773438)
    
   elseif MyLevel == 1775 or MyLevel <= 1799 then
       Mon = "Fishman Raider [Lv. 1775]"
       LevelQuest = 1
       NameQuest = "DeepForestIsland3"
       NameMon = "Fishman Raider"
       PQUEST = Vector3.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       CMON = CFrame.new(-10310.296875, 426.3200378418, -8592.0048828125)
       CQUEST = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       PMON = Vector3.new(-10310.296875, 426.3200378418, -8592.0048828125)
       
   elseif MyLevel == 1800 or MyLevel <= 1824 then
       Mon = "Fishman Captain [Lv. 1800]"
       LevelQuest = 2
       NameQuest = "DeepForestIsland3"
       NameMon = "Fishman Captain"
       PQUEST = Vector3.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       CMON = CFrame.new(-10728.3046875, 397.76626586914, -9079.86328125)
       CQUEST = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
       PMON = Vector3.new(-10728.3046875, 397.76626586914, -9079.86328125)
       
   elseif MyLevel == 1825 or MyLevel <= 1849 then
       Mon = "Forest Pirate [Lv. 1825]"
       LevelQuest = 1
       NameQuest = "DeepForestIsland"
       NameMon = "Forest Pirate"
       PQUEST = Vector3.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
       CMON = CFrame.new(-13265.977539063, 428.16796875, -7758.57421875)
       CQUEST = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
       PMON = Vector3.new(-13265.977539063, 428.16796875, -7758.57421875)
       
   elseif MyLevel == 1850 or MyLevel <= 1899 then
       Mon = "Mythological Pirate [Lv. 1850]"
       LevelQuest = 2
       NameQuest = "DeepForestIsland"
       NameMon = "Mythological Pirate"
       PQUEST = Vector3.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
       CMON = CFrame.new(-13392.751953125, 622.6171875, -7082.2348632813)
       CQUEST = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
       PMON = Vector3.new(13392.751953125, 622.6171875, -7082.2348632813)
       
   elseif MyLevel == 1900 or MyLevel <= 1924 then
       Mon = "Jungle Pirate [Lv. 1900]"
       LevelQuest = 1
       NameQuest = "DeepForestIsland2"
       NameMon = "Jungle Pirate"
       PQUEST = Vector3.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
       CMON = CFrame.new(-11997.963867188, 431.92016601563, -10300.259765625)
       CQUEST = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
       PMON = Vector3.new(-11997.963867188, 431.92016601563, -10300.259765625)
       
   elseif MyLevel == 1925 or MyLevel <= 1974 then
       Mon = "Musketeer Pirate [Lv. 1925]"
       LevelQuest = 2
       NameQuest = "DeepForestIsland2"
       NameMon = "Musketeer Pirate"
       PQUEST = Vector3.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
       CMON = CFrame.new(-13293.668945313, 496.21118164063, -9573.9326171875)
       CQUEST = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
       PMON = Vector3.new(-13293.668945313, 496.21118164063, -9573.9326171875)

   elseif MyLevel == 1975 or MyLevel <= 1999 then
       Mon = "Reborn Skeleton [Lv. 1975]"
       LevelQuest = 1
       NameQuest = "HauntedQuest1"
       NameMon = "Reborn Skeleton"
       PQUEST = Vector3.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       CMON = CFrame.new(-8767.4658203125, 184.68771362305, 6228.1762695313)
       CQUEST = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       PMON = Vector3.new(-8767.4658203125, 184.68771362305, 6228.1762695313)

   elseif MyLevel == 2000 or MyLevel <= 2024 then
       Mon = "Living Zombie [Lv. 2000]"
       LevelQuest = 2
       NameQuest = "HauntedQuest1"
       NameMon = "Living Zombie"
       PQUEST = Vector3.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       CMON = CFrame.new(-10146.403320313, 139.62678527832, 5987.4208984375)
       CQUEST = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
       PMON = Vector3.new(-10146.403320313, 139.62678527832, 5987.4208984375)

   elseif MyLevel == 2025 or MyLevel <= 2049 then
       Mon = "Demonic Soul [Lv. 2025]"
       LevelQuest = 1
       NameQuest = "HauntedQuest2"
       NameMon = "Demonic Soul"
       PQUEST = Vector3.new(-9516.99316, 172.017181, 6078.46533, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       CMON = CFrame.new(-9365.5595703125, 222.10494995117, 6231.1879882813)
       CQUEST = CFrame.new(-9516.99316, 172.017181, 6078.46533, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       PMON = Vector3.new(-9365.5595703125, 222.10494995117, 6231.1879882813)
       
   elseif MyLevel == 2050 or MyLevel <= 2074 then
       Mon = "Posessed Mummy [Lv. 2050]"
       LevelQuest = 2
       NameQuest = "HauntedQuest2"
       NameMon = "Posessed Mummy"
       PQUEST = Vector3.new(-9516.99316, 172.017181, 6078.46533, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       CMON = CFrame.new(-9556.00488, 66.3880768, 6370.78076, 0.999951124, 3.36073747e-08, -0.00988800824, -3.39445911e-08, 1, -3.39356419e-08, 0.00988800824, 3.42696289e-08, 0.999951124)
       CQUEST = CFrame.new(-9516.99316, 172.017181, 6078.46533, 0, 0, -1, 0, 1, 0, 1, 0, 0)
       PMON = Vector3.new(-9556.00488, 66.3880768, 6370.78076, 0.999951124, 3.36073747e-08, -0.00988800824, -3.39445911e-08, 1, -3.39356419e-08, 0.00988800824, 3.42696289e-08, 0.999951124)
      elseif MyLevel == 2075 or MyLevel <= 2099 then
         Mon = "Peanut Scout [Lv. 2075]"
         LevelQuest = 1
         NameQuest = "NutsIslandQuest"
         NameMon = "Peanut Scout"
         CMON = CFrame.new(-2192.3247070312, 94.319366455078, -10092.274414062)
         PMON = Vector3.new(-2192.3247070312, 94.319366455078, -10092.274414062)
         CQUEST = CFrame.new(-2104.3908691406, 38.104167938232, -10194.21875)
         PQUEST = Vector3.new(-2104.3908691406, 38.104167938232, -10194.21875)
     elseif MyLevel == 2100 or MyLevel <= 2124 then
         Mon = "Peanut President [Lv. 2100]"
         LevelQuest = 2
         NameQuest = "NutsIslandQuest"
         NameMon = "Peanut President"
         CMON = CFrame.new(-2120.5974121094, 124.56230163574, -10441.361328125)
         PMON = Vector3.new(-2192.3247070312, 94.319366455078, -10092.274414062)
         CQUEST = CFrame.new(-2104.3908691406, 38.104167938232, -10194.21875)
         PQUEST = Vector3.new(-2104.3908691406, 38.104167938232, -10194.21875)
     elseif MyLevel == 2125 or MyLevel <= 2149 then
         Mon = "Ice Cream Chef [Lv. 2125]"
         LevelQuest = 1
         NameQuest = "IceCreamIslandQuest"
         NameMon = "Ice Cream Chef"
         CMON = CFrame.new(-898.00366210938, 119.35078430176, -10943.458984375)
         PMON = Vector3.new(-898.00366210938, 119.35078430176, -10943.458984375)
         CQUEST = CFrame.new(-820.64825439453, 65.819526672363, -10965.795898438)
         PQUEST = Vector3.new(-820.64825439453, 65.819526672363, -10965.795898438)
     elseif MyLevel == 2150 or MyLevel <= 2199 then
         Mon = "Ice Cream Commander [Lv. 2150]"
         LevelQuest = 2
         NameQuest = "IceCreamIslandQuest"
         NameMon = "Ice Cream Commander"
         CMON = CFrame.new(-514.06311035156, 172.69267272949, -11215.62890625)
         PMON = Vector3.new(-898.00366210938, 119.35078430176, -10943.458984375)
         CQUEST = CFrame.new(-820.64825439453, 65.819526672363, -10965.795898438)
         PQUEST = Vector3.new(-820.64825439453, 65.819526672363, -10965.795898438)
     elseif MyLevel == 2200 or MyLevel <= 2225 then
         Mon = "Cookie Crafter [Lv. 2200]"
         LevelQuest = 1
         NameQuest = "CakeQuest1"
         NameMon = "Cookie Crafter"
         CMON = CFrame.new(-2269.18994, 90.5692139, -12157.415, -0.241292745, -4.28479332e-08, 0.970452368, -3.0098203e-08, 1, 3.66689363e-08, -0.970452368, -2.03609218e-08, -0.241292745)
         PMON = Vector3.new(-2269.18994, 90.5692139, -12157.415, -0.241292745, -4.28479332e-08, 0.970452368, -3.0098203e-08, 1, 3.66689363e-08, -0.970452368, -2.03609218e-08, -0.241292745)
         CQUEST = CFrame.new(-2018.80884, 38.1414719, -12023.8447, 0.926204681, -9.25598265e-09, 0.377021134, 1.17539365e-08, 1, -4.32487202e-09, -0.377021134, 8.43719938e-09, 0.926204681)
         PQUEST = Vector3.new(-2018.80884, 38.1414719, -12023.8447, 0.926204681, -9.25598265e-09, 0.377021134, 1.17539365e-08, 1, -4.32487202e-09, -0.377021134, 8.43719938e-09, 0.926204681)
     elseif MyLevel == 2225 or MyLevel <= 2250 then
         Mon = "Cake Guard [Lv. 2225]"
         LevelQuest = 2
         NameQuest = "CakeQuest1"
         NameMon = "Cake Guard"
         CMON = CFrame.new(-1558.61768, 90.5694199, -12583.4219, -0.790530264, -4.29809255e-08, 0.612422943, -3.70810653e-08, 1, 2.23166392e-08, -0.612422943, -5.0673159e-09, -0.790530264)
         PMON = Vector3.new(-1558.61768, 90.5694199, -12583.4219, -0.790530264, -4.29809255e-08, 0.612422943, -3.70810653e-08, 1, 2.23166392e-08, -0.612422943, -5.0673159e-09, -0.790530264)
         CQUEST = CFrame.new(-2018.80884, 38.1414719, -12023.8447, 0.926204681, -9.25598265e-09, 0.377021134, 1.17539365e-08, 1, -4.32487202e-09, -0.377021134, 8.43719938e-09, 0.926204681)
         PQUEST = Vector3.new(-2018.80884, 38.1414719, -12023.8447, 0.926204681, -9.25598265e-09, 0.377021134, 1.17539365e-08, 1, -4.32487202e-09, -0.377021134, 8.43719938e-09, 0.926204681)
     elseif MyLevel == 2250 or MyLevel <= 2275 then
         Mon = "Baking Staff [Lv. 2250]"
         LevelQuest = 1
         NameQuest = "CakeQuest2"
         NameMon = "Baking Staff"
         CMON = CFrame.new(-1769.45056, 90.5691681, -13038.4648, -0.847998321, -2.02224353e-08, 0.529998958, -2.03078834e-08, 1, 5.66300029e-09, -0.529998958, -5.96094241e-09, -0.847998321)
         PMON = Vector3.new(-1769.45056, 90.5691681, -13038.4648, -0.847998321, -2.02224353e-08, 0.529998958, -2.03078834e-08, 1, 5.66300029e-09, -0.529998958, -5.96094241e-09, -0.847998321)
         CQUEST = CFrame.new(-1914.99646, 38.1413841, -12835.5117, 0.545026958, 0, 0.838418543, -0, 1, -0, -0.838418543, 0, 0.545026958)
         PQUEST = Vector3.new(-1914.99646, 38.1413841, -12835.5117, 0.545026958, 0, 0.838418543, -0, 1, -0, -0.838418543, 0, 0.545026958)
     elseif MyLevel >= 2275 then
         Mon = "Head Baker [Lv. 2275]"
         LevelQuest = 2
         NameQuest = "CakeQuest2"
         NameMon = "Head Baker"
         CMON = CFrame.new(-2068.16577, 84.8175354, -13017.8848, -0.527114272, 4.41528734e-08, 0.849794447, 4.18282369e-08, 1, -2.6011719e-08, -0.849794447, 2.18342535e-08, -0.527114272)
         PMON = Vector3.new(-2068.16577, 84.8175354, -13017.8848, -0.527114272, 4.41528734e-08, 0.849794447, 4.18282369e-08, 1, -2.6011719e-08, -0.849794447, 2.18342535e-08, -0.527114272)
         CQUEST = CFrame.new(-1914.99646, 38.1413841, -12835.5117, 0.545026958, 0, 0.838418543, -0, 1, -0, -0.838418543, 0, 0.545026958)
         PQUEST = Vector3.new(-1914.99646, 38.1413841, -12835.5117, 0.545026958, 0, 0.838418543, -0, 1, -0, -0.838418543, 0, 0.545026958)
      end
end
end


local TweenSpeed= 300
local TweenSpeedF = 205
function TeleportTween(dist, Speed)
   local char = game.Players.LocalPlayer.Character
   local hm = char:WaitForChild("HumanoidRootPart")
    local info = TweenInfo.new((hm.Position - dist.Position).magnitude / Speed,Enum.EasingStyle.Linear)
    local tween =  game:service"TweenService":Create(hm, info, {CFrame = dist})
    tween:Play()
    tween.Completed:Wait()
end

function TP(P1)
    Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
    if Distance < 250 then
        Speed = 600
    elseif Distance < 500 then
        Speed = 400
    elseif Distance < 1000 then
        Speed = 350
    elseif Distance >= 1000 then
        Speed = 200
    end
    game:GetService("TweenService"):Create(
        game.Players.LocalPlayer.Character.HumanoidRootPart,
        TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
        {CFrame = P1}
    ):Play()
end

function Click()
    game:GetService'VirtualUser':CaptureController()
    game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
    game:GetService'VirtualUser':CaptureController()
    game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
end

function AutoHaki()
    if game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
    else
    local args = {
        [1] = "Buso"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end
end

_G.SelectToolWeapon = nil
function EquipWeapon(ToolSe)
   pcall(function()
   if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
       getgenv().tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
       wait(.1)
       game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
   end
end)
end

spawn(function()
    pcall(function()
        while wait() do
            if _G.AutoFarmLv or _G.AutoDungeonFarm or _G.AutoThirdSea or _G.AutoSecondSea or _G.Auto_Bone then
                if not game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
                    local Noclip = Instance.new("BodyVelocity")
                    Noclip.Name = "BodyClip"
                    Noclip.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
                    Noclip.MaxForce = Vector3.new(100000,100000,100000)
                    Noclip.Velocity = Vector3.new(0,0,0)
                end
            end
        end
    end)
end)

spawn(function()
    pcall(function()
        game:GetService("RunService").Stepped:Connect(function()
            if _G.AutoFarmLv or _G.AutoDungeonFarm or _G.AutoThirdSea or _G.AutoSecondSea or _G.Auto_Bone then
                for _, v in pairs(game:GetService("Players").LocalPlayer.Character:GetDescendants()) do
                    if v:IsA("BasePart") then
                        v.CanCollide = false    
                    end
                end
            end
        end)
    end)
end)

spawn(function()
    while wait() do
        if _G.AutoFarmLv or _G.AutoDungeonFarm or _G.AutoThirdSea or _G.AutoSecondSea or _G.Auto_Bone then
            pcall(function()
                game:GetService("ReplicatedStorage").Remotes.CommE:FireServer("Ken",true)
            end)
        end    
    end
end)

  function totarget(CFgo)
   local tween_s = game:service"TweenService"
   local info = TweenInfo.new((game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart.Position - CFgo.Position).Magnitude/300, Enum.EasingStyle.Linear)
   local tween, err = pcall(function()
       tween = tween_s:Create(game.Players.LocalPlayer.Character["HumanoidRootPart"], info, {CFrame = CFgo})
       tween:Play()
   end)
   if not tween then return err end
end

function CheckLvBoss()
   if SelectBoss == "Diamond [Lv. 750] [Boss]" then
      MsBoss = "Diamond [Lv. 750] [Boss]"
      NaemQuestBoss = "Area1Quest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
      CFrameBoss = CFrame.new(-1736.26587, 198.627731, -236.412857, -0.997808516, 0, -0.0661673471, 0, 1, 0, 0.0661673471, 0, -0.997808516)
   elseif SelectBoss == "Jeremy [Lv. 850] [Boss]" then
      MsBoss = "Jeremy [Lv. 850] [Boss]"
      NaemQuestBoss = "Area2Quest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
      CFrameBoss = CFrame.new(2203.76953, 448.966034, 752.731079, -0.0217453763, 0, -0.999763548, 0, 1, 0, 0.999763548, 0, -0.0217453763)
   elseif SelectBoss == "Fajita [Lv. 925] [Boss]" then
      MsBoss = "Fajita [Lv. 925] [Boss]"
      NaemQuestBoss = "MarineQuest3"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
      CFrameBoss = CFrame.new(-2297.40332, 115.449463, -3946.53833, 0.961227536, -1.46645796e-09, -0.275756449, -2.3212845e-09, 1, -1.34094433e-08, 0.275756449, 1.35296352e-08, 0.961227536)
   elseif SelectBoss == "Don Swan [Lv. 1000] [Boss]" then
      MsBoss = "Don Swan [Lv. 1000] [Boss]"
      CFrameBoss = CFrame.new(2288.802, 15.1870775, 863.034607, 0.99974072, -8.41247214e-08, -0.0227668174, 8.4774733e-08, 1, 2.75850098e-08, 0.0227668174, -2.95079072e-08, 0.99974072)
   elseif SelectBoss == "Smoke Admiral [Lv. 1150] [Boss]" then
      MsBoss = "Smoke Admiral [Lv. 1150] [Boss]"
      NaemQuestBoss = "IceSideQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-6059.96191, 15.9868021, -4904.7373, -0.444992423, -3.0874483e-09, 0.895534337, -3.64098796e-08, 1, -1.4644522e-08, -0.895534337, -3.91229982e-08, -0.444992423)
      CFrameBoss = CFrame.new(-5115.72754, 23.7664986, -5338.2207, 0.251453817, 1.48345061e-08, -0.967869282, 4.02796978e-08, 1, 2.57916977e-08, 0.967869282, -4.54708946e-08, 0.251453817)
   elseif SelectBoss == "Cursed Captain [Lv. 1325] [Raid Boss]" then
      MsBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
      CFrameBoss = CFrame.new(916.928589, 181.092773, 33422, -0.999505103, 9.26310495e-09, 0.0314563364, 8.42916226e-09, 1, -2.6643713e-08, -0.0314563364, -2.63653774e-08, -0.999505103)
   elseif SelectBoss == "Awakened Ice Admiral [Lv. 1400] [Boss]" then
      MsBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
      NaemQuestBoss = "FrostQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(5669.33203, 28.2118053, -6481.55908, 0.921275556, -1.25320829e-08, 0.388910472, 4.72230788e-08, 1, -7.96414241e-08, -0.388910472, 9.17372489e-08, 0.921275556)
      CFrameBoss = CFrame.new(6407.33936, 340.223785, -6892.521, 0.49051559, -5.25310213e-08, -0.871432424, -2.76146022e-08, 1, -7.58250565e-08, 0.871432424, 6.12576301e-08, 0.49051559)
   elseif SelectBoss == "Tide Keeper [Lv. 1475] [Boss]" then
      MsBoss = "Tide Keeper [Lv. 1475] [Boss]"
      NaemQuestBoss = "ForgottenQuest"             
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-3053.89648, 236.881363, -10148.2324, -0.985987961, -3.58504737e-09, 0.16681771, -3.07832915e-09, 1, 3.29612559e-09, -0.16681771, 2.73641976e-09, -0.985987961)
      CFrameBoss = CFrame.new(-3570.18652, 123.328949, -11555.9072, 0.465199202, -1.3857326e-08, 0.885206044, 4.0332897e-09, 1, 1.35347511e-08, -0.885206044, -2.72606271e-09, 0.465199202)
      -- Old World
   elseif SelectBoss == "Saber Expert [Lv. 200] [Boss]" then
      MsBoss = "Saber Expert [Lv. 200] [Boss]"
      CFrameBoss = CFrame.new(-1458.89502, 29.8870335, -50.633564, 0.858821094, 1.13848939e-08, 0.512275636, -4.85649254e-09, 1, -1.40823326e-08, -0.512275636, 9.6063415e-09, 0.858821094)
   elseif SelectBoss == "The Gorilla King [Lv. 25] [Boss]" then
      MsBoss = "The Gorilla King [Lv. 25] [Boss]"
      NaemQuestBoss = "JungleQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
      CFrameBoss = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
   elseif SelectBoss == "Bobby [Lv. 55] [Boss]" then
      MsBoss = "Bobby [Lv. 55] [Boss]"
      NaemQuestBoss = "BuggyQuest1"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
      CFrameBoss = CFrame.new(-1147.65173, 32.5966301, 4156.02588, 0.956680477, -1.77109952e-10, -0.29113996, 5.16530874e-10, 1, 1.08897802e-09, 0.29113996, -1.19218679e-09, 0.956680477)
   elseif SelectBoss == "Yeti [Lv. 110] [Boss]" then
      MsBoss = "Yeti [Lv. 110] [Boss]"
      NaemQuestBoss = "SnowQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(1384.90247, 87.3078308, -1296.6825, 0.280209213, 2.72035177e-08, -0.959938943, -6.75690828e-08, 1, 8.6151708e-09, 0.959938943, 6.24481444e-08, 0.280209213)
      CFrameBoss = CFrame.new(1221.7356, 138.046906, -1488.84082, 0.349343032, -9.49245944e-08, 0.936994851, 6.29478194e-08, 1, 7.7838429e-08, -0.936994851, 3.17894653e-08, 0.349343032)
   elseif SelectBoss == "Mob Leader [Lv. 120] [Boss]" then
      MsBoss = "Mob Leader [Lv. 120] [Boss]"
      CFrameBoss = CFrame.new(-2848.59399, 7.4272871, 5342.44043, -0.928248107, -8.7248246e-08, 0.371961564, -7.61816636e-08, 1, 4.44474857e-08, -0.371961564, 1.29216433e-08, -0.928248107)
      --The Gorilla King [Lv. 25] [Boss]
   elseif SelectBoss == "Vice Admiral [Lv. 130] [Boss]" then
      MsBoss = "Vice Admiral [Lv. 130] [Boss]"
      NaemQuestBoss = "MarineQuest2"
      LevelQuestBoss = 2
      CQUESTBoss = CFrame.new(-5035.42285, 28.6520386, 4324.50293, -0.0611100644, -8.08395768e-08, 0.998130739, -1.57416586e-08, 1, 8.00271849e-08, -0.998130739, -1.08217701e-08, -0.0611100644)
      CFrameBoss = CFrame.new(-5078.45898, 99.6520691, 4402.1665, -0.555574954, -9.88630566e-11, 0.831466436, -6.35508286e-08, 1, -4.23449258e-08, -0.831466436, -7.63661632e-08, -0.555574954)
   elseif SelectBoss == "Warden [Lv. 175] [Boss]" then
      MsBoss = "Warden [Lv. 175] [Boss]"
      NaemQuestBoss = "ImpelQuest"
      LevelQuestBoss = 1
      CQUESTBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
      CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
   elseif SelectBoss == "Chief Warden [Lv. 200] [Boss]" then
      MsBoss = "Chief Warden [Lv. 200] [Boss]"
      NaemQuestBoss = "ImpelQuest"
      LevelQuestBoss = 2
      CQUESTBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
      CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
   elseif SelectBoss == "Flamingo [Lv. 225] [Boss]" then
      MsBoss = "Flamingo [Lv. 225] [Boss]"
      NaemQuestBoss = "ImpelQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
      CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
   elseif SelectBoss == "Magma Admiral [Lv. 350] [Boss]" then
      MsBoss = "Magma Admiral [Lv. 350] [Boss]"
      NaemQuestBoss = "MagmaQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-5317.07666, 12.2721891, 8517.41699, 0.51175487, -2.65508806e-08, -0.859131515, -3.91131572e-08, 1, -5.42026761e-08, 0.859131515, 6.13418294e-08, 0.51175487)
      CFrameBoss = CFrame.new(-5530.12646, 22.8769703, 8859.91309, 0.857838571, 2.23414389e-08, 0.513919294, 1.53689133e-08, 1, -6.91265853e-08, -0.513919294, 6.71978384e-08, 0.857838571)
   elseif SelectBoss == "Fishman Lord [Lv. 425] [Boss]" then
      MsBoss = "Fishman Lord [Lv. 425] [Boss]"
      NaemQuestBoss = "FishmanQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(61123.0859, 18.5066795, 1570.18018, 0.927145958, 1.0624845e-07, 0.374700129, -6.98219367e-08, 1, -1.10790765e-07, -0.374700129, 7.65569368e-08, 0.927145958)
      CFrameBoss = CFrame.new(61351.7773, 31.0306778, 1113.31409, 0.999974668, 0, -0.00714713801, 0, 1.00000012, 0, 0.00714714266, 0, 0.999974549)
   elseif SelectBoss == "Wysper [Lv. 500] [Boss]" then
      MsBoss = "Wysper [Lv. 500] [Boss]"
      NaemQuestBoss = "SkyExp1Quest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-7862.94629, 5545.52832, -379.833954, 0.462944925, 1.45838088e-08, -0.886386991, 1.0534996e-08, 1, 2.19553424e-08, 0.886386991, -1.95022007e-08, 0.462944925)
      CFrameBoss = CFrame.new(-7925.48389, 5550.76074, -636.178345, 0.716468513, -1.22915289e-09, 0.697619379, 3.37381434e-09, 1, -1.70304748e-09, -0.697619379, 3.57381835e-09, 0.716468513)
   elseif SelectBoss == "Thunder God [Lv. 575] [Boss]" then
      MsBoss = "Thunder God [Lv. 575] [Boss]"
      NaemQuestBoss = "SkyExp2Quest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-7902.78613, 5635.99902, -1411.98706, -0.0361216255, -1.16895912e-07, 0.999347389, 1.44533963e-09, 1, 1.17024491e-07, -0.999347389, 5.6715117e-09, -0.0361216255)
      CFrameBoss = CFrame.new(-7917.53613, 5616.61377, -2277.78564, 0.965189934, 4.80563429e-08, -0.261550069, -6.73089886e-08, 1, -6.46515304e-08, 0.261550069, 8.00056768e-08, 0.965189934)
   elseif SelectBoss == "Cyborg [Lv. 675] [Boss]" then
      MsBoss = "Cyborg [Lv. 675] [Boss]"
      NaemQuestBoss = "FountainQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(5253.54834, 38.5361786, 4050.45166, -0.0112687312, -9.93677887e-08, -0.999936521, 2.55291371e-10, 1, -9.93769547e-08, 0.999936521, -1.37512213e-09, -0.0112687312)
      CFrameBoss = CFrame.new(6041.82813, 52.7112198, 3907.45142, -0.563162148, 1.73805248e-09, -0.826346457, -5.94632716e-08, 1, 4.26280238e-08, 0.826346457, 7.31437524e-08, -0.563162148)
   elseif SelectBoss == "Stone [Lv. 1550] [Boss]" then
      MsBoss = "Stone [Lv. 1550] [Boss]"
      NaemQuestBoss = "PiratePortQuest"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-288.003815, 43.7675667, 5573.12012, -0.959750533, 1.11968195e-08, 0.280853927, -1.77952231e-08, 1, -1.00677937e-07, -0.280853927, -1.01623563e-07, -0.959750533)
      CFrameBoss = CFrame.new(-1086.11621, 38.8425903, 6768.71436, 0.0231462717, -0.592676699, 0.805107772, 2.03251839e-05, 0.805323839, 0.592835128, -0.999732077, -0.0137055516, 0.0186523199)
   elseif SelectBoss == "Island Empress [Lv. 1675] [Boss]" then
      MsBoss = "Island Empress [Lv. 1675] [Boss]"
      NaemQuestBoss = "AmazonQuest2"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(5447.27734375, 601.68060302734, 750.61822509766)
      CFrameBoss = CFrame.new(5713.98877, 601.922974, 202.751251, -0.101080291, -0, -0.994878292, -0, 1, -0, 0.994878292, 0, -0.101080291)
   elseif SelectBoss == "Kilo Admiral [Lv. 1750] [Boss]" then
      MsBoss = "Kilo Admiral [Lv. 1750] [Boss]"
      NaemQuestBoss = "MarineTreeIsland"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(2179.8757324219, 28.705436706543, -6739.759765625)
      CFrameBoss = CFrame.new(2877.61743, 423.558685, -7207.31006, -0.989591599, -0, -0.143904909, -0, 1.00000012, -0, 0.143904924, 0, -0.989591479)
   elseif SelectBoss == "Captain Elephant [Lv. 1875] [Boss]" then
      MsBoss = "Captain Elephant [Lv. 1875] [Boss]"
      NaemQuestBoss = "DeepForestIsland"
      LevelQuestBoss = 3
      CQUESTBoss = CFrame.new(-13231.1602, 333.744446, -7624.40723, -0.0901302397, 8.36351219e-08, 0.995930016, 2.76566414e-08, 1, -8.14740204e-08, -0.995930016, 2.02008046e-08, -0.0901302397)
      CFrameBoss = CFrame.new(-13485.0283, 331.709259, -8012.4873, 0.714521289, 7.98849911e-08, 0.69961375, -1.02065748e-07, 1, -9.94383065e-09, -0.69961375, -6.43015241e-08, 0.714521289)
   elseif SelectBoss == "Beautiful Pirate [Lv. 1950] [Boss]" then
    MsBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
    NaemQuestBoss = "DeepForestIsland2"
    LevelQuestBoss = 3
    CQUESTBoss = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
    CFrameBoss = CFrame.new(5312.3598632813, 20.141201019287, -10.158538818359)
    end 
 end

spawn(function()
pcall(function()
while wait() do
if _G.AutoFarmLv or _G.AutoDungeonFarm or _G.AutoSecondSea or _G.AutoThirdSea then
        for i, v in pairs(game.Workspace["_WorldOrigin"]:GetChildren()) do
            if v.Name == "CurvedRing" or v.Name == "SlashHit" or v.Name == "SwordSlash" or v.Name == "Sounds" then
                v:Destroy() 
            end
        end
end
end
end)
end)

spawn(function()
    pcall(function()
        while game:GetService("RunService").Heartbeat:wait() do
            if _G.AutoFarmLv or _G.AutoDungeonFarm or _G.AutoSecondSea or _G.AutoThirdSea then
                if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Y <= 1 then
                    if not game:GetService("Workspace"):FindFirstChild("Water") then
                        local Water = Instance.new("Part", game.Workspace)
                        Water.Name = "Water"
                        Water.Size = Vector3.new(50,0.5,50)
                        Water.Transparency = 1
                        Water.Anchored = true
                        game:GetService("Workspace").Water.CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.X,game:GetService("Workspace").Camera["Water;"].CFrame.Y,game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
                    else
                        game:GetService("Workspace").Water.CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.X,game:GetService("Workspace").Camera["Water;"].CFrame.Y,game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
                    end
                elseif game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Y >= 1 and game:GetService("Workspace"):FindFirstChild("Water") then
                    game:GetService("Workspace"):FindFirstChild("Water"):Destroy()
                end
            else
                if game:GetService("Workspace"):FindFirstChild("Water") then
                    game:GetService("Workspace"):FindFirstChild("Water"):Destroy()
                end
            end
        end
    end)
end)

local CombatFrameworkROld = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework) 
local CombatFrameworkR = getupvalues(CombatFrameworkROld)[2]
local CameraShakerR = require(game.ReplicatedStorage.Util.CameraShaker)
CameraShakerR:Stop()

spawn(function()
    game:GetService("RunService").Stepped:Connect(function()
        pcall(function()
            CombatFrameworkR.activeController.hitboxMagnitude = 55
            if Usefastattack or SuperFastAttack then
                if fastattect then
                    if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") then
                        CombatFrameworkR.activeController.timeToNextAttack = 3
                    elseif game.Players.LocalPlayer.Character:FindFirstChild("Electro") then
                        CombatFrameworkR.activeController.timeToNextAttack = 2
                    else
                        CombatFrameworkR.activeController.timeToNextAttack = 0
                    end
                    CombatFrameworkR.activeController.attacking = false
                    CombatFrameworkR.activeController.increment = 3
                    CombatFrameworkR.activeController.blocking = false
                    CombatFrameworkR.activeController.timeToNextBlock = 0
                    game.Players.LocalPlayer.Character.Humanoid.Sit = false						
                end
            end
        end)
    end)
end)

spawn(function()
    while wait() do
        pcall(function()
            if Usefastattack or SuperFastAttack then
                if fastattect then
                    if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") then
                        CombatFrameworkR.activeController.timeToNextAttack = 3
                    elseif game.Players.LocalPlayer.Character:FindFirstChild("Electro") then
                        CombatFrameworkR.activeController.timeToNextAttack = 2
                    else
                        CombatFrameworkR.activeController.timeToNextAttack = 0
                    end
                    CombatFrameworkR.activeController.attacking = false
                    CombatFrameworkR.activeController.increment = 3
                    CombatFrameworkR.activeController.blocking = false
                    CombatFrameworkR.activeController.timeToNextBlock = 0
                    game.Players.LocalPlayer.Character.Humanoid.Sit = false		
                end
            end
        end)
    end
end)
spawn(function()
    while wait() do
        pcall(function()
            if Usefastattack or SuperFastAttack then
                if fastattect then
                    if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") then
                        CombatFrameworkR.activeController.timeToNextAttack = 3
                    elseif game.Players.LocalPlayer.Character:FindFirstChild("Electro") then
                        CombatFrameworkR.activeController.timeToNextAttack = 2
                    else
                        CombatFrameworkR.activeController.timeToNextAttack = 0
                    end
                    CombatFrameworkR.activeController.attacking = false
                    CombatFrameworkR.activeController.increment = 3
                    CombatFrameworkR.activeController.blocking = false
                    CombatFrameworkR.activeController.timeToNextBlock = 0
                    game.Players.LocalPlayer.Character.Humanoid.Sit = false		
                end
            end
        end)
    end
end)
spawn(function()
    while wait() do
        pcall(function()
            if  SuperFastAttack then
                if fastattect then
                    if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") then
                        CombatFrameworkR.activeController.timeToNextAttack = 3
                    elseif game.Players.LocalPlayer.Character:FindFirstChild("Electro") then
                        CombatFrameworkR.activeController.timeToNextAttack = 2
                    else
                        CombatFrameworkR.activeController.timeToNextAttack = 0
                    end
                    CombatFrameworkR.activeController.attacking = false
                    CombatFrameworkR.activeController.increment = 3
                    CombatFrameworkR.activeController.blocking = false
                    CombatFrameworkR.activeController.timeToNextBlock = 0
                    game.Players.LocalPlayer.Character.Humanoid.Sit = false		
                end
            end
        end)
    end
end)

spawn(function()
    while wait() do
       pcall(function()
          for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                     if _G.AutoFarmLv and MagnetActive and Magnet then
                if v.Name == Ms and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
                   if v.Name == "Factory Staff [Lv. 800]" then
                      if (v.HumanoidRootPart.Position - PosMon.Position).Magnitude <= 250 then
                         v.Head.CanCollide = false
                         v.Humanoid.JumpPower = 0
                         v.Humanoid.WalkSpeed = 0
                         v.Humanoid:ChangeState(14)
                         v.HumanoidRootPart.CanCollide = false
                         v.Head.CanCollide = false
                         v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                         if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                         v.HumanoidRootPart.CFrame = PosMon
                         sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                      end
                   elseif v.Name == Ms then
                      if (v.HumanoidRootPart.Position - PosMon.Position).Magnitude <= 275 then
                         v.Head.CanCollide = false
                         v.Humanoid.JumpPower = 0
                         v.Humanoid.WalkSpeed = 0
                         v.Humanoid:ChangeState(14)
                         v.HumanoidRootPart.CanCollide = false
                         v.Head.CanCollide = false
                         v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                         if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                         v.HumanoidRootPart.CFrame = PosMon
                         sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                      end
                   end
                end
                elseif _G.Auto_Bone and StartMagnetBoneMon and Magnet then
                    if (v.Name == "Reborn Skeleton [Lv. 1975]" or v.Name == "Living Zombie [Lv. 2000]" or v.Name == "Demonic Soul [Lv. 2025]" or v.Name == "Posessed Mummy [Lv. 2050]") and (v.HumanoidRootPart.Position - PosMonBone.Position).Magnitude <= 250 and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                        v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                        v.Humanoid.JumpPower = 0
                        v.Humanoid.WalkSpeed = 0
                        v.Humanoid:ChangeState(14)
                        v.HumanoidRootPart.CanCollide = false
                        v.Head.CanCollide = false
                        v.HumanoidRootPart.CFrame = PosMonBone
                        if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                        sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                    end
 end
 end
 end)
 end
 end)
