local windows = loadstring(game:HttpGet("https://raw.githubusercontent.com/BunnySalf/UiLib/main/uione"))()
local window = windows.new('a')
local tgd = window:Tap("NemorosHub")
tgd:Label("")
tgd:Label("-  Welcome to NEMOROS HUB's  -")
tgd:Label("")
tgd:Label("-  Thank you for purchasing our products.  -")
tgd:Label("")
local CloseIcon = Instance.new("ImageLabel")
	CloseIcon.Name = "CloseIcon"
	CloseIcon.Parent = game:GetService("CoreGui").Whiteui.MainSceen.Page.pagesFolder["NemorosHubPage"]
	CloseIcon.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	CloseIcon.BackgroundTransparency = 1.000
	CloseIcon.Position = UDim2.new(0.2, 0, 0.128935531, 0)
	CloseIcon.Size = UDim2.new(0, 17, 0, 17)
	CloseIcon.Image = "http://www.roblox.com/asset/?id=1615699542"
	CloseIcon.ImageColor3 = Color3.fromRGB(220, 221, 222)
tgd:Button('Join Discord',function()
    local InviteCode = "WD59jFF3WX"
	syn.request({
            Url = "http://127.0.0.1:6463/rpc?v=1",
            Method = "POST",
            Headers = {
                ["Content-Type"] = "application/json",
                ["Origin"] = "https://discord.com"
            },
            Body = game:GetService("HttpService"):JSONEncode({
                cmd = "INVITE_BROWSER",
                args = {
                    code = InviteCode
                },
                nonce = game:GetService("HttpService"):GenerateGUID(false)
            }),
          })
end)
local placeId = game.PlaceId
if placeId == 2753915549 then
	world1 = true
elseif placeId == 4442272183 then
	world2 = true
elseif placeId == 7449423635 then
	world3 = true
end

function cq()
    local MyLevel =  game.Players.LocalPlayer.Data.Level.Value
    if world1 then
		Dis = 300
		if MyLevel == 1 or MyLevel <= 9 then -- Bandit
            magbring = 400
			Ms = "Bandit [Lv. 5]"
			NameQuest = "BanditQuest1"
			LevelQuest = 1
			NameMon = "Bandit"
			CFrameQuest = CFrame.new(1061.66699, 16.5166187, 1544.52905, -0.942978859, -3.33851502e-09, 0.332852632, 7.04340497e-09, 1, 2.99841325e-08, -0.332852632, 3.06188177e-08, -0.942978859)
			CFrameMon = CFrame.new(1199.31287, 52.2717781, 1536.91516, -0.929782331, 6.60215846e-08, -0.368109822, 3.9077392e-08, 1, 8.06501603e-08, 0.368109822, 6.06023249e-08, -0.929782331)
		elseif MyLevel == 10 or MyLevel <= 14 then -- Monkey
            magbring = 400
			Ms = "Monkey [Lv. 14]"
			NameQuest = "JungleQuest"
			LevelQuest = 1
			NameMon = "Monkey"
			CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
			CFrameMon = CFrame.new(-1502.74609, 98.5633316, 90.6417007, 0.836947978, 0, 0.547282517, -0, 1, -0, -0.547282517, 0, 0.836947978)
		elseif MyLevel == 15 or MyLevel <= 29 then -- Gorilla
            magbring = 240
			Ms = "Gorilla [Lv. 20]"
			NameQuest = "JungleQuest"
			LevelQuest = 2
			NameMon = "Gorilla"
			CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
			CFrameMon = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
		elseif MyLevel == 30 or MyLevel <= 39 then -- Pirate
			Dis = 150
			Ms = "Pirate [Lv. 35]"
			NameQuest = "BuggyQuest1"
			LevelQuest = 1
			NameMon = "Pirate"
			CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
			CFrameMon = CFrame.new(-1219.32324, 4.75205183, 3915.63452, -0.966492832, -6.91238853e-08, 0.25669381, -5.21195496e-08, 1, 7.3047012e-08, -0.25669381, 5.72206496e-08, -0.966492832)
		elseif MyLevel == 40 or MyLevel <= 59 then -- Brute
			Dis = 150
			Ms = "Brute [Lv. 45]"
			NameQuest = "BuggyQuest1"
			LevelQuest = 2
			NameMon = "Brute"
			CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
			CFrameMon = CFrame.new(-1146.49646, 96.0936813, 4312.1333, -0.978175163, -1.53222057e-08, 0.207781896, -3.33316912e-08, 1, -8.31738873e-08, -0.207781896, -8.82843523e-08, -0.978175163)
		elseif MyLevel == 60 or MyLevel <= 74 then -- Desert Bandit
			Ms = "Desert Bandit [Lv. 60]"
			NameQuest = "DesertQuest"
			LevelQuest = 1
			NameMon = "Desert Bandit"
			CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
			CFrameMon = CFrame.new(932.788818, 6.4503746, 4488.24609, -0.998625934, 3.08948351e-08, 0.0524050146, 2.79967303e-08, 1, -5.60361286e-08, -0.0524050146, -5.44919629e-08, -0.998625934)
		elseif MyLevel == 75 or MyLevel <= 89 then -- Desert Officre
			Ms = "Desert Officer [Lv. 70]"
			NameQuest = "DesertQuest"
			LevelQuest = 2
			NameMon = "Desert Officer"
			CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
			CFrameMon = CFrame.new(1580.03198, 4.61375761, 4366.86426, 0.135744005, -6.44280718e-08, -0.990743816, 4.35738308e-08, 1, -5.90598574e-08, 0.990743816, -3.51534837e-08, 0.135744005)
		elseif MyLevel == 90 or MyLevel <= 99 then -- Snow Bandits
			Ms = "Snow Bandit [Lv. 90]"
			NameQuest = "SnowQuest"
			LevelQuest = 1
			NameMon = "Snow Bandits"
			CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
			CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
		elseif MyLevel == 100 or MyLevel <= 119 then -- Snowman
			Ms = "Snowman [Lv. 100]"
			NameQuest = "SnowQuest"
			LevelQuest = 2
			NameMon = "Snowman"
			CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
			CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
		elseif MyLevel == 120 or MyLevel <= 149 then -- Chief Petty Officer
			Ms = "Chief Petty Officer [Lv. 120]"
			NameQuest = "MarineQuest2"
			LevelQuest = 1
			NameMon = "Chief Petty Officer"
			CFrameQuest = CFrame.new(-5035.0835, 28.6520386, 4325.29443, 0.0243340395, -7.08064647e-08, 0.999703884, -6.36926814e-08, 1, 7.23777944e-08, -0.999703884, -6.54350671e-08, 0.0243340395)
			CFrameMon = CFrame.new(-4882.8623, 22.6520386, 4255.53516, 0.273695946, -5.40380647e-08, -0.96181643, 4.37720793e-08, 1, -4.37274998e-08, 0.96181643, -3.01326679e-08, 0.273695946)
		elseif MyLevel == 150 or MyLevel <= 174 then -- Sky Bandit
			Ms = "Sky Bandit [Lv. 150]"
			NameQuest = "SkyQuest"
			LevelQuest = 1
			NameMon = "Sky Bandit"
			CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
			CFrameMon = CFrame.new(-4970.74219, 294.544342, -2890.11353, -0.994874597, -8.61311236e-08, -0.101116329, -9.10836206e-08, 1, 4.43614923e-08, 0.101116329, 5.33441664e-08, -0.994874597)
		elseif MyLevel == 175 or MyLevel <= 224 then -- Dark Master
			Ms = "Dark Master [Lv. 175]"
			NameQuest = "SkyQuest"
			LevelQuest = 2
			NameMon = "Dark Master"
			CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
			CFrameMon = CFrame.new(-5220.58594, 430.693298, -2278.17456, -0.925375521, 1.12086873e-08, 0.379051805, -1.05115507e-08, 1, -5.52320891e-08, -0.379051805, -5.50948407e-08, -0.925375521)
		elseif MyLevel == 225 or MyLevel <= 274 then -- Toga Warrior
			Ms = "Toga Warrior [Lv. 225]"
			NameQuest = "ColosseumQuest"
			LevelQuest = 1
			NameMon = "Toga Warrior"
			CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
			CFrameMon = CFrame.new(-1779.97583, 44.6077499, -2736.35474, 0.984437346, 4.10396339e-08, 0.175734788, -3.62286876e-08, 1, -3.05844168e-08, -0.175734788, 2.3741821e-08, 0.984437346)
		elseif MyLevel == 275 or MyLevel <= 299 then -- Gladiato
			Ms = "Gladiator [Lv. 275]"
			NameQuest = "ColosseumQuest"
			LevelQuest = 2
			NameMon = "Gladiato"
			CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
			CFrameMon = CFrame.new(-1274.75903, 58.1895943, -3188.16309, 0.464524001, 6.21005611e-08, 0.885560572, -4.80449414e-09, 1, -6.76054768e-08, -0.885560572, 2.71497012e-08, 0.464524001)
		elseif MyLevel == 300 or MyLevel <= 329 then -- Military Soldier
			Ms = "Military Soldier [Lv. 300]"
			NameQuest = "MagmaQuest"
			LevelQuest = 1
			NameMon = "Military Soldier"
			CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
			CFrameMon = CFrame.new(-5363.01123, 41.5056877, 8548.47266, -0.578253984, -3.29503091e-10, 0.815856814, 9.11209668e-08, 1, 6.498761e-08, -0.815856814, 1.11920997e-07, -0.578253984)
		elseif MyLevel == 300 or MyLevel <= 374 then -- Military Spy
            FM = false
			Ms = "Military Spy [Lv. 330]"
			NameQuest = "MagmaQuest"
			LevelQuest = 2
			NameMon = "Military Spy"
			CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
			CFrameMon = CFrame.new(-5787.99023, 120.864456, 8762.25293, -0.188358366, -1.84706277e-08, 0.982100308, -1.23782129e-07, 1, -4.93306951e-09, -0.982100308, -1.22495649e-07, -0.188358366)
		elseif MyLevel == 375 or MyLevel <= 399 then -- Fishman Warrior
            FM = true
			Ms = "Fishman Warrior [Lv. 375]"
			NameQuest = "FishmanQuest"
			LevelQuest = 1
			NameMon = "Fishman Warrior"
			CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
			CFrameMon = CFrame.new(60946.6094, 48.6735229, 1525.91687, -0.0817126185, 8.90751153e-08, 0.996655822, 2.00889794e-08, 1, -8.77269599e-08, -0.996655822, 1.28533992e-08, -0.0817126185)
		elseif MyLevel == 400 or MyLevel <= 449 then -- Fishman Commando
            FM = true
			Ms = "Fishman Commando [Lv. 400]"
			NameQuest = "FishmanQuest"
			LevelQuest = 2
			NameMon = "Fishman Commando"
			CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
			CFrameMon = CFrame.new(61885.5039, 18.4828243, 1504.17896, 0.577502489, 0, -0.816389024, -0, 1.00000012, -0, 0.816389024, 0, 0.577502489)
		elseif MyLevel == 450 or MyLevel <= 474 then -- God's Guards
            FM = false
			Ms = "God's Guard [Lv. 450]"
			NameQuest = "SkyExp1Quest"
			LevelQuest = 1
			NameMon = "God's Guards"
			CFrameQuest = CFrame.new(-4721.71436, 845.277161, -1954.20105, -0.999277651, -5.56969759e-09, 0.0380011722, -4.14751478e-09, 1, 3.75035256e-08, -0.0380011722, 3.73188307e-08, -0.999277651)
			CFrameMon = CFrame.new(-4716.95703, 853.089722, -1933.92542, -0.93441087, -6.77488776e-09, -0.356197298, 1.12145182e-08, 1, -4.84390199e-08, 0.356197298, -4.92565206e-08, -0.93441087)
		elseif MyLevel == 475 or MyLevel <= 524 then -- Shandas
            sky = false
			Ms = "Shanda [Lv. 475]"
			NameQuest = "SkyExp1Quest"
			LevelQuest = 2
			NameMon = "Shandas"
			CFrameQuest = CFrame.new(-7863.63672, 5545.49316, -379.826324, 0.362120807, -1.98046344e-08, -0.93213129, 4.05822291e-08, 1, -5.48095125e-09, 0.93213129, -3.58431969e-08, 0.362120807)
			CFrameMon = CFrame.new(-7685.12354, 5601.05127, -443.171509, 0.150056243, 1.79768236e-08, -0.988677442, 6.67798661e-09, 1, 1.91962481e-08, 0.988677442, -9.48289181e-09, 0.150056243)
		elseif MyLevel == 525 or MyLevel <= 549 then -- Royal Squad
            sky = true
			Ms = "Royal Squad [Lv. 525]"
			NameQuest = "SkyExp2Quest"
			LevelQuest = 1
			NameMon = "Royal Squad"
			CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
			CFrameMon = CFrame.new(-7685.02051, 5606.87842, -1442.729, 0.561947823, 7.69527464e-09, -0.827172697, -4.24974544e-09, 1, 6.41599973e-09, 0.827172697, -9.01838604e-11, 0.561947823)
		elseif MyLevel == 550 or MyLevel <= 624 then -- Royal Soldier
            Dis = 240
            sky = true
			Ms = "Royal Soldier [Lv. 550]"
			NameQuest = "SkyExp2Quest"
			LevelQuest = 2
			NameMon = "Royal Soldier"
			CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
			CFrameMon = CFrame.new(-7864.44775, 5661.94092, -1708.22351, 0.998389959, 2.28686137e-09, -0.0567218624, 1.99431383e-09, 1, 7.54200258e-08, 0.0567218624, -7.54117195e-08, 0.998389959)
		elseif MyLevel == 625 or MyLevel <= 649 then -- Galley Pirate
            Dis = 240
            sky = false
			Ms = "Galley Pirate [Lv. 625]"
			NameQuest = "FountainQuest"
			LevelQuest = 1
			NameMon = "Galley Pirate"
			CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
			CFrameMon = CFrame.new(5595.06982, 41.5013695, 3961.47095, -0.992138803, -2.11610267e-08, -0.125142589, -1.34249509e-08, 1, -6.26613996e-08, 0.125142589, -6.04887518e-08, -0.992138803)
		elseif MyLevel >= 650 then -- Galley Captain
            Dis = 240
			Ms = "Galley Captain [Lv. 650]"
			NameQuest = "FountainQuest"
			LevelQuest = 2
			NameMon = "Galley Captain"
			CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
			CFrameMon = CFrame.new(5658.5752, 38.5361786, 4928.93506, -0.996873081, 2.12391046e-06, -0.0790185928, 2.16989656e-06, 1, -4.96097414e-07, 0.0790185928, -6.66008248e-07, -0.996873081)
		end
    elseif world2 then
		Dis = 240
		if MyLevel == 700 or MyLevel <= 724 then -- Raider [Lv. 700]
			Ms = "Raider [Lv. 700]"
			NameQuest = "Area1Quest"
			LevelQuest = 1
			NameMon = "Raider"
			CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
			CFrameMon = CFrame.new(-737.026123, 39.1748352, 2392.57959, 0.272128761, 0, -0.962260842, -0, 1, -0, 0.962260842, 0, 0.272128761)
		elseif MyLevel == 725 or MyLevel <= 774 then -- Mercenary [Lv. 725]
			Ms = "Mercenary [Lv. 725]"
			NameQuest = "Area1Quest"
			LevelQuest = 2
			NameMon = "Mercenary"
			CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
			CFrameMon = CFrame.new(-973.731995, 95.8733215, 1836.46936, 0.999135971, 2.02326991e-08, -0.0415605344, -1.90767793e-08, 1, 2.82094952e-08, 0.0415605344, -2.73922804e-08, 0.999135971)
		elseif MyLevel == 775 or MyLevel <= 799 then -- Swan Pirate [Lv. 775]
			Ms = "Swan Pirate [Lv. 775]"
			NameQuest = "Area2Quest"
			LevelQuest = 1
			NameMon = "Swan Pirate"
			CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
			CFrameMon = CFrame.new(970.369446, 142.653198, 1217.3667, 0.162079468, -4.85452638e-08, -0.986777723, 1.03357589e-08, 1, -4.74980872e-08, 0.986777723, -2.50063148e-09, 0.162079468)
		elseif MyLevel == 800 or MyLevel <= 874 then -- Factory Staff [Lv. 800]
			Ms = "Factory Staff [Lv. 800]"
			NameQuest = "Area2Quest"
			LevelQuest = 2
			NameMon = "Factory Staff"
			CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
			CFrameMon = CFrame.new(296.786499, 72.9948196, -57.1298141, -0.876037002, -5.32364979e-08, 0.482243896, -3.87658332e-08, 1, 3.99718729e-08, -0.482243896, 1.63222538e-08, -0.876037002)
		elseif MyLevel == 875 or MyLevel <= 899 then -- Marine Lieutenant [Lv. 875]
			Ms = "Marine Lieutenant [Lv. 875]"
			NameQuest = "MarineQuest3"
			LevelQuest = 1
			NameMon = "Marine Lieutenant"
			CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
			CFrameMon = CFrame.new(-2913.26367, 73.0011826, -2971.64282, 0.910507619, 0, 0.413492233, 0, 1.00000012, 0, -0.413492233, 0, 0.910507619)
		elseif MyLevel == 900 or MyLevel <= 949 then -- Marine Captain [Lv. 900]
			Ms = "Marine Captain [Lv. 900]"
			NameQuest = "MarineQuest3"
			LevelQuest = 2
			NameMon = "Marine Captain"
			CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
			CFrameMon = CFrame.new(-1868.67688, 73.0011826, -3321.66333, -0.971402287, 1.06502087e-08, 0.237439692, 3.68856199e-08, 1, 1.06050372e-07, -0.237439692, 1.11775684e-07, -0.971402287)
		elseif MyLevel == 950 or MyLevel <= 974 then -- Zombie [Lv. 950]
			Ms = "Zombie [Lv. 950]"
			NameQuest = "ZombieQuest"
			LevelQuest = 1
			NameMon = "Zombie"
			CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
			CFrameMon = CFrame.new(-5634.83838, 126.067039, -697.665039, -0.992770672, 6.77618939e-09, 0.120025545, 1.65461245e-08, 1, 8.04023372e-08, -0.120025545, 8.18070234e-08, -0.992770672)
		elseif MyLevel == 975 or MyLevel <= 999 then -- Vampire [Lv. 975]
			Ms = "Vampire [Lv. 975]"
			NameQuest = "ZombieQuest"
			LevelQuest = 2
			NameMon = "Vampire"
			CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
			CFrameMon = CFrame.new(-6030.32031, 6.4377408, -1313.5564, -0.856965423, 3.9138893e-08, -0.515373945, -1.12178942e-08, 1, 9.45958547e-08, 0.515373945, 8.68467822e-08, -0.856965423)
		elseif MyLevel == 1000 or MyLevel <= 1049 then -- Snow Trooper [Lv. 1000] **
			Ms = "Snow Trooper [Lv. 1000]"
			NameQuest = "SnowMountainQuest"
			LevelQuest = 1
			NameMon = "Snow Trooper"
			CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
			CFrameMon = CFrame.new(535.893433, 401.457062, -5329.6958, -0.999524176, 0, 0.0308452044, 0, 1, -0, -0.0308452044, 0, -0.999524176)
		elseif MyLevel == 1050 or MyLevel <= 1099 then -- Winter Warrior [Lv. 1050]
			Ms = "Winter Warrior [Lv. 1050]"
			NameQuest = "SnowMountainQuest"
			LevelQuest = 2
			NameMon = "Winter Warrior"
			CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
			CFrameMon = CFrame.new(1223.7417, 454.575226, -5170.02148, 0.473996818, 2.56845354e-08, 0.880526543, -5.62456428e-08, 1, 1.10811016e-09, -0.880526543, -5.00510211e-08, 0.473996818)
		elseif MyLevel == 1100 or MyLevel <= 1124 then -- Lab Subordinate [Lv. 1100]
			Ms = "Lab Subordinate [Lv. 1100]"
			NameQuest = "IceSideQuest"
			LevelQuest = 1
			NameMon = "Lab Subordinate"
			CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
			CFrameMon = CFrame.new(-5769.2041, 37.9288292, -4468.38721, -0.569419742, -2.49055017e-08, 0.822046936, -6.96206541e-08, 1, -1.79282633e-08, -0.822046936, -6.74401548e-08, -0.569419742)
		elseif MyLevel == 1125 or MyLevel <= 1174 then -- Horned Warrior [Lv. 1125]
			Ms = "Horned Warrior [Lv. 1125]"
			NameQuest = "IceSideQuest"
			LevelQuest = 2
			NameMon = "Horned Warrior"
			CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
			CFrameMon = CFrame.new(-6400.85889, 24.7645149, -5818.63574, -0.964845479, 8.65926566e-08, -0.262817472, 3.98261392e-07, 1, -1.13260398e-06, 0.262817472, -1.19745812e-06, -0.964845479)
		elseif MyLevel == 1175 or MyLevel <= 1199 then -- Magma Ninja [Lv. 1175]
			Ms = "Magma Ninja [Lv. 1175]"
			NameQuest = "FireSideQuest"
			LevelQuest = 1
			NameMon = "Magma Ninja"
			CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
			CFrameMon = CFrame.new(-5496.65576, 58.6890411, -5929.76855, -0.885073781, 0, -0.465450764, 0, 1.00000012, -0, 0.465450764, 0, -0.885073781)
		elseif MyLevel == 1200 or MyLevel <= 1249 then -- Lava Pirate [Lv. 1200]
			Ms = "Lava Pirate [Lv. 1200]"
			NameQuest = "FireSideQuest"
			LevelQuest = 2
			NameMon = "Lava Pirate"
			CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
			CFrameMon = CFrame.new(-5169.71729, 34.1234779, -4669.73633, -0.196780294, 0, 0.98044765, 0, 1.00000012, -0, -0.98044765, 0, -0.196780294)
		elseif MyLevel == 1250 or MyLevel <= 1274 then -- Ship Deckhand [Lv. 1250]
			Ms = "Ship Deckhand [Lv. 1250]"
			NameQuest = "ShipQuest1"
			LevelQuest = 1
			NameMon = "Ship Deckhand"
			CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
			CFrameMon = CFrame.new(1163.80872, 138.288452, 33058.4258, -0.998580813, 5.49076979e-08, -0.0532564968, 5.57436763e-08, 1, -1.42118655e-08, 0.0532564968, -1.71604082e-08, -0.998580813)
		elseif MyLevel == 1275 or MyLevel <= 1299 then -- Ship Engineer [Lv. 1275]
			Ms = "Ship Engineer [Lv. 1275]"
			NameQuest = "ShipQuest1"
			LevelQuest = 2
			NameMon = "Ship Engineer"
			CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
			CFrameMon = CFrame.new(916.666504, 44.0920448, 32917.207, -0.99746871, -4.85034697e-08, -0.0711069331, -4.8925461e-08, 1, 4.19294288e-09, 0.0711069331, 7.66126895e-09, -0.99746871)
		elseif MyLevel == 1300 or MyLevel <= 1324 then -- Ship Steward [Lv. 1300]
			Ms = "Ship Steward [Lv. 1300]"
			NameQuest = "ShipQuest2"
			LevelQuest = 1
			NameMon = "Ship Steward"
			CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
			CFrameMon = CFrame.new(918.743286, 129.591064, 33443.4609, -0.999792814, -1.7070947e-07, -0.020350717, -1.72559169e-07, 1, 8.91351277e-08, 0.020350717, 9.2628369e-08, -0.999792814)
		elseif MyLevel == 1325 or MyLevel <= 1349 then -- Ship Officer [Lv. 1325]
			Ms = "Ship Officer [Lv. 1325]"
			NameQuest = "ShipQuest2"
			LevelQuest = 2
			NameMon = "Ship Officer"
			CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
			CFrameMon = CFrame.new(786.051941, 181.474106, 33303.2969, 0.999285698, -5.32193063e-08, 0.0377905183, 5.68968588e-08, 1, -9.62386864e-08, -0.0377905183, 9.83201005e-08, 0.999285698)
		elseif MyLevel == 1350 or MyLevel <= 1374 then -- Arctic Warrior [Lv. 1350]
			Ms = "Arctic Warrior [Lv. 1350]"
			NameQuest = "FrostQuest"
			LevelQuest = 1
			NameMon = "Arctic Warrior"
			CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
			CFrameMon = CFrame.new(5995.07471, 57.3188477, -6183.47314, 0.702747107, -1.53454167e-07, -0.711440146, -1.08168464e-07, 1, -3.22542007e-07, 0.711440146, 3.03620908e-07, 0.702747107)
		elseif MyLevel == 1375 or MyLevel <= 1424 then -- Snow Lurker [Lv. 1375]
			Ms = "Snow Lurker [Lv. 1375]"
			NameQuest = "FrostQuest"
			LevelQuest = 2
			NameMon = "Snow Lurker"
			CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
			CFrameMon = CFrame.new(5518.00684, 60.5559731, -6828.80518, -0.650781393, -3.64292951e-08, 0.759265184, -4.07668654e-09, 1, 4.44854642e-08, -0.759265184, 2.58550248e-08, -0.650781393)
		elseif MyLevel == 1425 or MyLevel <= 1449 then -- Sea Soldier [Lv. 1425]
			Ms = "Sea Soldier [Lv. 1425]"
			NameQuest = "ForgottenQuest"
			LevelQuest = 1
			NameMon = "Sea Soldier"
			CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
			CFrameMon = CFrame.new(-3029.78467, 66.944252, -9777.38184, -0.998552859, 1.09555076e-08, 0.0537791774, 7.79564235e-09, 1, -5.89660658e-08, -0.0537791774, -5.84614881e-08, -0.998552859)
		elseif MyLevel >= 1450 then -- Water Fighter [Lv. 1450]
			Ms = "Water Fighter [Lv. 1450]"
			NameQuest = "ForgottenQuest"
			LevelQuest = 2
			NameMon = "Water Fighter"
			CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
			CFrameMon = CFrame.new(-3262.00098, 298.699615, -10553.6943, -0.233570755, -4.57538185e-08, 0.972339869, -5.80986068e-08, 1, 3.30992194e-08, -0.972339869, -4.87605725e-08, -0.233570755)
		end
    elseif world3 then
		Dis = 240
		if MyLevel == 1500 or MyLevel <= 1524 then
			Ms = "Pirate Millionaire [Lv. 1500]"
			NameQuest = "PiratePortQuest"
			LevelQuest = 1
			NameMon = "Pirate Millionaire"
			CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
			CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
		elseif MyLevel == 1525 or MyLevel <= 1574 then
			Ms = "Pistol Billionaire [Lv. 1525]"
			NameQuest = "PiratePortQuest"
			LevelQuest = 2
			NameMon = "Pistol Billionaire"
			CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
			CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
		elseif MyLevel == 1575 or MyLevel <= 1599 then
			Ms = "Dragon Crew Warrior [Lv. 1575]"
			NameQuest = "AmazonQuest"
			LevelQuest = 1
			NameMon = "Dragon Crew Warrior"
			CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
			CFrameMon = CFrame.new(6241.9951171875, 51.522083282471, -1243.9771728516)
		elseif MyLevel == 1600 or MyLevel <= 1624 then
			Ms = "Dragon Crew Archer [Lv. 1600]"
			NameQuest = "AmazonQuest"
			LevelQuest = 2
			NameMon = "Dragon Crew Archer"
			CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
			CFrameMon = CFrame.new(6488.9155273438, 383.38375854492, -110.66246032715)
		elseif MyLevel == 1625 or MyLevel <= 1649 then
			Ms = "Female Islander [Lv. 1625]"
			NameQuest = "AmazonQuest2"
			LevelQuest = 1
			NameMon = "Female Islander"
			CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
			CFrameMon = CFrame.new(4770.4990234375, 758.95520019531, 1069.8680419922)
		elseif MyLevel == 1650 or MyLevel <= 1699 then
			Ms = "Giant Islander [Lv. 1650]"
			NameQuest = "AmazonQuest2"
			LevelQuest = 2
			NameMon = "Giant Islander"
			CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
			CFrameMon = CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789)
		elseif MyLevel == 1700 or MyLevel <= 1724 then
			Ms = "Marine Commodore [Lv. 1700]"
			NameQuest = "MarineTreeIsland"
			LevelQuest = 1
			NameMon = "Marine Commodore"
			CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
			CFrameMon = CFrame.new(2490.0844726563, 190.4232635498, -7160.0502929688)
		elseif MyLevel == 1725 or MyLevel <= 1774 then
			Ms = "Marine Rear Admiral [Lv. 1725]"
			NameQuest = "MarineTreeIsland"
			LevelQuest = 2
			NameMon = "Marine Rear Admiral"
			CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
			CFrameMon = CFrame.new(3951.3903808594, 229.11549377441, -6912.81640625)
		elseif MyLevel == 1775 or MyLevel <= 1799 then
			Ms = "Fishman Raider [Lv. 1775]"
			NameQuest = "DeepForestIsland3"
			LevelQuest = 1
			NameMon = "Fishman Raider"
			CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
			CFrameMon = CFrame.new(-10322.400390625, 390.94473266602, -8580.0908203125)
		elseif MyLevel == 1800 or MyLevel <= 1824 then
			Ms = "Fishman Captain [Lv. 1800]"
			NameQuest = "DeepForestIsland3"
			LevelQuest = 2
			NameMon = "Fishman Captain"
			CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
			CFrameMon = CFrame.new(-11194.541992188, 442.02795410156, -8608.806640625)
		elseif MyLevel == 1825 or MyLevel <= 1849 then
			Ms = "Forest Pirate [Lv. 1825]"
			NameQuest = "DeepForestIsland"
			LevelQuest = 1
			NameMon = "Forest Pirate"
			CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
			CFrameMon = CFrame.new(-13225.809570313, 428.19387817383, -7753.1245117188)
		elseif MyLevel == 1850 or MyLevel <= 1899 then
			Ms = "Mythological Pirate [Lv. 1850]"
			NameQuest = "DeepForestIsland"
			LevelQuest = 2
			NameMon = "Mythological Pirate"
			CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
			CFrameMon = CFrame.new(-13869.172851563, 564.95251464844, -7084.4135742188)
		elseif MyLevel == 1900 or MyLevel <= 1924 then
			Ms = "Jungle Pirate [Lv. 1900]"
			NameQuest = "DeepForestIsland2"
			LevelQuest = 1
			NameMon = "Jungle Pirate"
			CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
			CFrameMon = CFrame.new(-11982.221679688, 376.32522583008, -10451.415039063)
		elseif MyLevel == 1925 or MyLevel <= 1974 then
			Ms = "Musketeer Pirate [Lv. 1925]"
			NameQuest = "DeepForestIsland2"
			LevelQuest = 2
			NameMon = "Musketeer Pirate"
			CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
			CFrameMon = CFrame.new(-13282.3046875, 496.23684692383, -9565.150390625)
        elseif MyLevel == 1975 or MyLevel <= 1999 then
			Ms = "Reborn Skeleton [Lv. 1975]"
			NameQuest = "HauntedQuest1"
			LevelQuest = 1
			NameMon = "Reborn Skeleton"
			CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
			CFrameMon = CFrame.new(-8761.3154296875, 164.85829162598, 6161.1567382813)
        elseif MyLevel == 2000 or MyLevel <= 2024 then
			Ms = "Living Zombie [Lv. 2000]"
			NameQuest = "HauntedQuest1"
			LevelQuest = 2
			NameMon = "Living Zombie"
			CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
			CFrameMon = CFrame.new(-10093.930664063, 237.38233947754, 6180.5654296875)
		elseif MyLevel == 2025 or MyLevel <= 2049 then
			Ms = "Demonic Soul [Lv. 2025]"
			NameQuest = "HauntedQuest2"
			LevelQuest = 1
			NameMon = "Demonic Soul"
			CFrameQuest = CFrame.new(-9514.78027, 171.162918, 6078.82373, 0.301918149, 7.4535027e-09, 0.953333855, -3.22802141e-09, 1, -6.79604995e-09, -0.953333855, -1.02553133e-09, 0.301918149)
			CFrameMon = CFrame.new(-9466.72949, 171.162918, 6132.01514)
		elseif MyLevel == 2050 or MyLevel <= 2074 then
			Ms = "Posessed Mummy [Lv. 2050]" 
			NameQuest = "HauntedQuest2"
			LevelQuest = 2
			NameMon = "Posessed Mummy"
			CFrameQuest = CFrame.new(-9514.78027, 171.162918, 6078.82373, 0.301918149, 7.4535027e-09, 0.953333855, -3.22802141e-09, 1, -6.79604995e-09, -0.953333855, -1.02553133e-09, 0.301918149)
			CFrameMon = CFrame.new(-9589.93848, 4.85058546, 6190.27197)
        elseif MyLevel == 2075 or MyLevel <= 2099 then
            Ms = "Peanut Scout [Lv. 2075]"
            NameQuest = "NutsIslandQuest"
            LevelQuest = 1
            NameMon = "Peanut Scout"
            CFrameMon = CFrame.new(-2124, 123, -10435)
            CFrameQuest = CFrame.new(-2104, 38, -10192)
        elseif MyLevel == 2100 or MyLevel <= 2124 then
            Ms = "Peanut President [Lv. 2100]"
            NameQuest = "NutsIslandQuest"
            LevelQuest = 2
            NameMon = "Peanut President"
            CFrameMon = CFrame.new(-2124, 123, -10435)
            CFrameQuest = CFrame.new(-2104, 38, -10192)
        elseif MyLevel == 2125 or MyLevel <= 2149 then
            Ms = "Ice Cream Chef [Lv. 2125]"
            NameQuest = "IceCreamIslandQuest"
            LevelQuest = 1
            NameMon = "Ice Cream Chef"
            CFrameMon = CFrame.new(-641, 127, -11062)
            CFrameQuest = CFrame.new(-822, 66, -10965)
        elseif MyLevel >= 2150 then
            Ms = "Ice Cream Commander [Lv. 2150]"
            NameQuest = "IceCreamIslandQuest"
            LevelQuest = 2
            NameMon = "Ice Cream Commander"
            CFrameMon = CFrame.new(-641, 127, -11062)
            CFrameQuest = CFrame.new(-822, 66, -10965)
		end
    end
end

if _G.SelectToolWeapon == nil then
    _G.SelectToolWeapon = ""
end
local tgls = window:Tap('Auto Farm',6031094670)
if _G.Team == "Pirate" then
	for i,v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.MouseButton1Click)) do
		v.Function()
	end
elseif _G.Team == "Marine" then
	for i,v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Marines.Frame.ViewportFrame.TextButton.MouseButton1Click)) do
		v.Function()
	end
else
	for i,v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.MouseButton1Click)) do
		v.Function()
	end
end
if _G.HideGui then
	game:GetService("VirtualInputManager"):SendKeyEvent(true, Enum.KeyCode.RightControl, false, game)
end
if _G.RedeemAllCode then
	function UseCode(Text)
		game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Text)
	end
	UseCode("FUDD10")
	UseCode("BIGNEWS")
	UseCode("THEGREATACE")
	UseCode("SUB2NOOBMASTER123")
	UseCode("Sub2Daigrock")
	UseCode("Axiore")
	UseCode("TantaiGaming")
	UseCode("STRAWHATMAINE")
	UseCode("Sub2OfficialNoobie")
end
Magnet = true
if _G.FPSBOOST then
	local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
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
end
setfflag("HumanoidParallelRemoveNoPhysics", "False")
setfflag("HumanoidParallelRemoveNoPhysicsNoSimulate2", "False")
setfflag("CrashPadUploadToBacktraceToBacktraceBaseUrl", "")
setfflag("CrashUploadToBacktracePercentage", "0")
setfflag("CrashUploadToBacktraceBlackholeToken", "")
setfflag("CrashUploadToBacktraceWindowsPlayerToken", "")

spawn(function()
    while true do game:GetService("RunService").RenderStepped:Wait()
        if _G.AutoFarmCandy or _G.AutoSoulReaper or _G.AutoRaidhop or _G.AutoCavenderHop or _G.AutoCavender or _G.MusketeeHat or _G.AutoObservationHakiV2 or _G.AutoHakiRainbow or _G.AutoEliteHunter or _G.HolyTorch or _G.AutoYama or _G.AutoBuddySwords or _G.AutoFramEctoplasm or _G.AutoRengoku or _G.AutoQuestBartilo or _G.AutoEvoRace2 or _G.AutoPoleHOP or _G.AutoPole or _G.AutoSaber or _G.FramBoss or _G.AutoThird or _G.AutoNew or _G.FarmLevel or _G.AutoHallowScythe or _G.AutoFarmBone then
            if not KRNL_LOADED and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
                game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
            end
        else
            Workspace.Gravity = 197
        end
    end
end)
spawn(function()
    while wait() do
        if setscriptable then
            setscriptable(game.Players.LocalPlayer, "SimulationRadius", true)
            game.Players.LocalPlayer.SimulationRadius = math.huge * math.huge, math.huge * math.huge * 1 / 0 * 1 / 0 * 1 / 0 * 1 / 0 * 1 / 0
        end
    end
end)
spawn(function()
    game:GetService("RunService").Stepped:Connect(function()
        kkii = require(game.ReplicatedStorage.Util.CameraShaker)
        kkii:Stop()
        if _G.AutoFarmCandy or _G.AutoSoulReaper or _G.AutoRaidhop or _G.AutoCavenderHop or _G.AutoCavender or _G.MusketeeHat or _G.AutoObservationHakiV2 or _G.AutoHakiRainbow or _G.AutoEliteHunter or _G.HolyTorch or _G.AutoYama or _G.AutoBuddySwords or _G.AutoFramEctoplasm or _G.AutoRengoku or _G.AutoQuestBartilo or _G.AutoEvoRace2 or _G.AutoPoleHOP or _G.AutoPole or _G.AutoSaber or _G.FramBoss or _G.AutoThird or _G.AutoNew or _G.FarmLevel or _G.AutoHallowScythe or _G.AutoFarmBone then
            for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
                if v:IsA("BasePart") then
                    v.CanCollide = false
                    Workspace.Gravity = 0
                end
            end
        end
    end)
end)

function EquipWeapon(ToolSe)
	if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
		getgenv().tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
		wait(.1)
		game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end
end

function toTarget(targetPos, targetCFrame)
    local tweenfunc = {}
    local tween_s = game:service"TweenService"
    local info = TweenInfo.new((targetPos - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).Magnitude/300, Enum.EasingStyle.Linear)
    local tween = tween_s:Create(game:GetService("Players").LocalPlayer.Character["HumanoidRootPart"], info, {CFrame = targetCFrame * CFrame.fromAxisAngle(Vector3.new(1,0,0), math.rad(0))})
    tween:Play()

    function tweenfunc:Stop()
        tween:Cancel()
        return tween
    end

    if not tween then return tween end
    return tweenfunc
end

function TPFF(P1)
    Distance = (CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
    if Distance < 250 then
        Speed = 1000
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

function TP2FF(P1)
	Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
	if Distance < 1000 then
		Speed = 400
	elseif Distance >= 1000 then
		Speed = 250
	end
    game:GetService("TweenService"):Create(
        game.Players.LocalPlayer.Character.HumanoidRootPart,
        TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
        {CFrame = P1}
    ):Play()
    wait(Distance/Speed)
end

function autofarm()
    if _G.FarmLevel and game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then
        cq()
        kkii = require(game.ReplicatedStorage.Util.CameraShaker)
        kkii:Stop()
        if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
            cq()
            StartMagnetAutoFarm = false
            Questtween = toTarget(CFrameQuest.Position,CFrameQuest)
            if world1 and (Ms == "Fishman Commando [Lv. 400]" or Ms == "Fishman Warrior [Lv. 375]") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
                if Questtween then
                    Questtween:Stop()
                end
                local TouchInterest = game:GetService("Workspace").Map.TeleportSpawn.Entrance
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                local string_1 = "SetSpawnPoint";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1);
            elseif world1 and not (Ms == "Fishman Commando [Lv. 400]" or Ms == "Fishman Warrior [Lv. 375]") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
                if Questtween then
                    Questtween:Stop()
                end
                local TouchInterest = game:GetService("Workspace").Map.TeleportSpawn.Exit
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                local string_1 = "SetSpawnPoint";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1);
            elseif world2 and string.find(Ms, "Ship") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 30000 then
                if Questtween then
                    Questtween:Stop()
                end
                local TouchInterest = game:GetService("Workspace").Map.GhostShip.Teleport
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                wait(.5)
                local string_1 = "SetSpawnPoint";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1);
            elseif world2 and not string.find(Ms, "Ship") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 30000 then
                if Questtween then
                    Questtween:Stop()
                end
                local TouchInterest = game:GetService("Workspace").Map.GhostShipInterior.Teleport
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                wait(.5)
                local string_1 = "SetSpawnPoint";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1);
            elseif (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                if Questtween then
                    Questtween:Stop()
                end
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
                wait(1)
                local string_1 = "StartQuest";
                local string_2 = NameQuest;
                local number_1 = LevelQuest;
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1, string_2, number_1);
                local string_1 = "SetSpawnPoint";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1);
            end 
        elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
            cq()
            if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                    if _G.FarmLevel and v.Name == Ms and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
                        if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
                            repeat wait()
                                if world1 and (Ms == "Fishman Commando [Lv. 400]" or Ms == "Fishman Warrior [Lv. 375]") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
                                    local TouchInterest = game:GetService("Workspace").Map.TeleportSpawn.Entrance
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                                    local string_1 = "SetSpawnPoint";
                                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                                    Target:InvokeServer(string_1);
                                    StartMagnetAutoFarm = false
                                elseif world1 and not (Ms == "Fishman Commando [Lv. 400]" or Ms == "Fishman Warrior [Lv. 375]") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
                                    local TouchInterest = game:GetService("Workspace").Map.TeleportSpawn.Exit
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                                    local string_1 = "SetSpawnPoint";
                                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                                    Target:InvokeServer(string_1);
                                    StartMagnetAutoFarm = false
                                elseif world2 and string.find(Ms, "Ship") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 30000 then
                                    local TouchInterest = game:GetService("Workspace").Map.GhostShip.Teleport
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                                    wait(.5)
                                    local string_1 = "SetSpawnPoint";
                                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                                    Target:InvokeServer(string_1);
                                    StartMagnetAutoFarm = false
                                elseif world2 and not string.find(Ms, "Ship") and (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 30000 then
                                    local TouchInterest = game:GetService("Workspace").Map.GhostShipInterior.Teleport
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                                    wait(.5)
                                    local string_1 = "SetSpawnPoint";
                                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                                    Target:InvokeServer(string_1);
                                    StartMagnetAutoFarm = false
                                elseif v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 250 then
                                    Farmtween = toTarget(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
                                    StartMagnetAutoFarm = false
                                elseif v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
                                    EquipWeapon(_G.SelectToolWeapon)
                                    if Farmtween then
                                        Farmtween:Stop()
                                    end
                                    if Modstween then
                                        Modstween:Stop()
                                    end
                                    PosMonAutoFarm = v.HumanoidRootPart.CFrame
                                    if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
                                        local args = {
                                            [1] = "Buso"
                                        }
                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                                    end
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 0, -20)
                                 
                                        game:GetService'VirtualUser':CaptureController()
                                        game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
                              
                                    StartMagnetAutoFarm = true
                                end
                            until not _G.FarmLevel or not v.Parent or v.Humanoid.Health <= 0 or not string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
                            if not string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
                                local l__Remotes__11 = game.ReplicatedStorage:WaitForChild("Remotes");
                                l__Remotes__11.CommF_:InvokeServer("AbandonQuest");
                            end
                            StartMagnetAutoFarm = false
                            Modstween = toTarget(CFrameMon.Position,CFrameMon)
                            if (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                                if Modstween then
                                    Modstween:Stop()
                                end
                                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
                            end 
                        else
                            local l__Remotes__11 = game.ReplicatedStorage:WaitForChild("Remotes");
                            l__Remotes__11.CommF_:InvokeServer("AbandonQuest");
                        end 
                    end
                end
            else
                if not string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
                    local l__Remotes__11 = game.ReplicatedStorage:WaitForChild("Remotes");
                    l__Remotes__11.CommF_:InvokeServer("AbandonQuest");
                end
                StartMagnetAutoFarm = false
                Modstween = toTarget(CFrameMon.Position,CFrameMon)
                if world1 and (Ms == "Fishman Commando [Lv. 400]" or Ms == "Fishman Warrior [Lv. 375]") and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
                    if Modstween then
                        Modstween:Stop()
                    end
                    local TouchInterest = game:GetService("Workspace").Map.TeleportSpawn.Entrance
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                    local string_1 = "SetSpawnPoint";
                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                    Target:InvokeServer(string_1);
                elseif world1 and not (Ms == "Fishman Commando [Lv. 400]" or Ms == "Fishman Warrior [Lv. 375]") and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
                    if Modstween then
                        Modstween:Stop()
                    end
                    local TouchInterest = game:GetService("Workspace").Map.TeleportSpawn.Exit
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                    local string_1 = "SetSpawnPoint";
                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                    Target:InvokeServer(string_1);
                elseif world2 and string.find(Ms, "Ship") and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 30000 then
                    if Modstween then
                        Modstween:Stop()
                    end
                    local TouchInterest = game:GetService("Workspace").Map.GhostShip.Teleport
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                    wait(.5)
                    local string_1 = "SetSpawnPoint";
                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                    Target:InvokeServer(string_1);
                elseif world2 and not string.find(Ms, "Ship") and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 30000 then
                    if Modstween then
                        Modstween:Stop()
                    end
                    local TouchInterest = game:GetService("Workspace").Map.GhostShipInterior.Teleport
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
                    wait(.5)
                    local string_1 = "SetSpawnPoint";
                    local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                    Target:InvokeServer(string_1);
                elseif (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                    if Modstween then
                        Modstween:Stop()
                    end
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
                end 
            end
        end 
    end
end
spawn(function()
    game:GetService("RunService").Stepped:Connect(function()
        if _G.FarmLevel and StartMagnetAutoFarm then
            for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
                if StartMagnetAutoFarm and _G.FarmLevel and v.Name == Ms and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                    v.HumanoidRootPart.CFrame = PosMonAutoFarm
                    v.HumanoidRootPart.CanCollide = false
                    -- v.Humanoid:ChangeState(11)
                end
            end
        end
    end)
end)

spawn(function()
	while wait() do
        if _G.FarmLevel then
            autofarm()
        end
    end
end)

-------------- Change Sate
game:GetService("RunService").Heartbeat:Connect(
function()
	if _G.FarmLevel or _G.Observation or _G.AutoNew or _G.Factory or _G.Superhuman or _G.FullSuperhuman  or _G.DeathStep or _G.FruitMastery or _G.GunMastery or FramBoss or FramAllBoss or _G.AutoBartilo or AutoNear or _G.AutoRengoku or _G.AutoSharkman or _G.AutoFramEctoplasm then
		if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Humanoid") then
			game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end
end)



---- Select Wapon
function EquipWeapon(ToolSe)
	if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
		getgenv().tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
		wait(.1)
		game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end
end



tgls:Label("--AutoFarm--")
tgls:Toggle("Auto Farm on /off 20 minute",false,function(vu)
	_G.OnOff = vu
end)
spawn(function()
	while wait() do
		if _G.OnOff then
			wait(1200)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest") 
                _G.FarmLevel = false
			wait(.8)
			_G.FarmLevel = true
		end
	end
end)
tgls:Toggle("Auto Farm",false,function(t)
	_G.FarmLevel = t
end)
tgls:Toggle("Auto New World",false,function(vu)
	_G.AutoNew = vu
end)
tgls:Toggle("Auto Third Sea", false, function(vu)
	_G.AutoThird = vu
end)
tgls:Toggle("Auto Factory",false,function(vu)
	_G.Factory = vu
	while _G.Factory do wait()
		if game.Workspace.Enemies:FindFirstChild("Core") then
			Core = true
			_G.FarmLevel = false
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if Core and v.Name == "Core" and v.Humanoid.Health > 0 then
					repeat wait(.1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(448.46756, 199.356781, -441.389252)
						EquipWeapon(SelectToolWeapon)
						game:GetService'VirtualUser':CaptureController()
						game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
					until not Core or v.Humanoid.Health <= 0  or _G.Factory == false
				end
			end
		elseif game.ReplicatedStorage:FindFirstChild("Core") then
			Core = true
            _G.FarmLevel= false
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(448.46756, 199.356781, -441.389252)
		elseif AFMMain then
			Core = false
            _G.FarmLevel = true
		end
	end
end)
tgls:Toggle("Auto Superhuman",false,function(vu)
	_G.Superhuman = vu
end)
tgls:Toggle("Full Superhuman",false,function(vu)
	_G.FullSuperhuman = vu
end)
tgls:Toggle("Auto DeathStep",false,function(vu)
	_G.DeathStep = vu
end)
tgls:Toggle("Auto Electric Claw",false, function(vu)
	AutoElectricClaw = vu
	if AutoElectricClaw then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
	end
end)
tgls:Toggle("Auto Fram Ectoplasm",false,function(A)
	_G.AutoFramEctoplasm = A
end)
tgls:Toggle("Auto Pole",false,function(vu)
	_G.Pole = vu
end)
tgls:Toggle("Auto Pole+Hop",false,function(eiei)
	_G.PoleHop = eiei
end)
tgls:Toggle("Auto SwanGlasses",false,function(vu)
	_G.SwanGlasses = vu
end)
tgls:Toggle("Auto SwanGlasses+Hop",false,function(eiei)
	_G.SwanGlassesHop = eiei
end)
tgls:Toggle("Auto Dark Code",false,function(vu)
	_G.DarkCode = vu
end)
tgls:Toggle("Auto DarkCode+Hop",false,function(eiei)
	_G.DarkCodeHop = eiei
end)
tgls:Toggle("Auto Bisento v2",false,function(vu)
	_G.Bisentov2 = vu
end)
tgls:Toggle("Auto Bisento v2 + Hop",false,function(vu)
	_G.Bisentov2Hop = vu
end)
tgls:Toggle("Auto Elite Hunter",false,function (t)
	_G.EliteHunter = t
end)
tgls:Toggle("Auto Yama(30 Elite Hunter Only)",false,function(t)
	yama = t
end)
tgls:Toggle("Auto RainBow Haki",false,function(vu)
	_G.AutoRainbow = vu
end)
tgls:Toggle("Auto Saber",false,function(Value)
	_G.AutoOpenSaber = Value
end)
tgls:Toggle("Auto Citizen Quest", false, function(vu)
	CheckCitizen = vu
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Musketeer Hat") then
		CTCH = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Musketeer Hat") then
		CTCH = true
	end
	if CTCH and CheckCitizen then
		CNPPaid:Notification("Notification","Auto Quest Citizen","Successfully")
	elseif CheckCitizen and MiscFarmWeapon == "" then
		CNPPaid:Notification("Notification","SelectWeapon First","Okay")
	elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 3 and CheckCitizen then
		CNPPaid:Notification("Notification","Auto Quest Citizen","Successfully")
	else
		_G.AutoCitizen = vu
	end
end)
tgls:Toggle("AutoFarmChest", false, function(vu)
	_G.AutoFarmChest = vu
end)
tgls:Toggle("Auto Farm Chest Hop",false,function(vu)
	_G.AutoFarmChestHop = vu
end)
tgls:Toggle("Fast Attack",true,function(Value)
	_G.FastAttack = Value  
end)
_G.Delay_FastAttack = 1
tgls:Slider("Delay_FastAttack", 1, 100,1,function(t)
	_G.Delay_FastAttack = t
end)
tgls:Toggle("Equitp All Weapon",false,function(value)
	_G.Equitp = value
end)


-------------- ------------- Select Weapon
Wapon = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
	if v:IsA("Tool") then
		table.insert(Wapon ,v.Name)
	end
end
local SelectWeapona = tgls:Dropdown("Select Weapon",Wapon,function(Value)
	_G.SelectToolWeapon = Value
	SelectToolWeaponOld = Value
end)
tgls:Button("Refresh Weapon", function()
	SelectWeapona:Clear()
	Wapon = {}
	for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
		if v:IsA("Tool") then
			SelectWeapona:Add(v.Name)
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
		if v:IsA("Tool") then
			SelectWeapona:Add(v.Name)
		end
	end
end)



-------------- ------------- Auto Accessories

tgls:Label("-- Auto Accessories --")
WaponAccessories = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
	if v:IsA("Tool") then 
		if v.ToolTip == "Wear" then    
			table.insert(WaponAccessories, v.Name)
		end
	end
end
tgls:Toggle("Auto Accessories",false,function(Value)
	if SelectTooAccessories == "" and Value then
		CNPPaid:Notification("Notification","Select Accessories First", "Ok")
	else
		AutoAccessories = Value 
	end
end)
local SelectAccessories = tgls:Dropdown("Select Accessories",WaponAccessories,function(Value)
	SelectTooAccessories = Value
end)
tgls:Button("Refresh Accessories", function()
	SelectAccessories:Clear()
	for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
		if v:IsA("Tool") then 
			if v.ToolTip == "Wear" then    
				SelectAccessories:Add(v.Name)
			end
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
		if v:IsA("Tool") then 
			if v.ToolTip == "Wear" then    
				SelectAccessories:Add(v.Name)
			end
		end
	end
end)

----------------------- AutoQuestLuccy
tgls:Label("--AutoQuestLuccy--", true)
local args = {
	[1] = "getInventoryWeapons"
}
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
game:GetService("RunService").Heartbeat:Connect(
function()
	if _G.AutoBartilo then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)
tgls:Toggle("Auto Quest Bartilo",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Warrior Helmet") then
		HaveWarriorHelmet = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Warrior Helmet") then
		HaveWarriorHelmet = true
	end
	if HaveWarriorHelmet and Bool == true then
		CNPPaid:Notification("Notification","Quest Bartilo Successfully", "Alright")
	elseif WeaponBartilo == "" and Bool == true then
		CNPPaid:Notification("Notification","Select Weapon", "Alright")
	elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 3 and Bool == true then
		CNPPaid:Notification("Notification","Quest Bartilo Successfully", "Alright")
	else
		_G.AutoBartilo = v
	end
end)
local BartiloWeapon = tgls:Dropdown("Select Weapon",Wapon,function(A)
	WeaponBartilo = A
end) 
tgls:Button("Refresh Weapon", function()
	BartiloWeapon:Clear()
	for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
		if v:IsA("Tool") then
			BartiloWeapon:Add(v.Name)
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
		if v:IsA("Tool") then
			BartiloWeapon:Add(v.Name)
		end
	end
end)
---------------------- hide ----------------
pcall(function()
game:GetService("ReplicatedStorage").Assets.GUI:Destroy()
game:GetService("ReplicatedStorage").Assets.SlashHit:Destroy()
end)
---------- AutoNew --------------------------
spawn(function()
	while wait(.1) do
		if _G.AutoNew then
			local MyLevel = game.Players.localPlayer.Data.Level.Value
			if MyLevel >= 700 and OldWorld then
				_G.FarmLevel = false
				_G.SelectToolWeapon = "Key"
				tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(10, Enum.EasingStyle.Linear)
tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(4849.29883, 5.65138149, 719.611877)})
tween:Play()
				wait(10)
				local args = {
					[1] = "DressrosaQuestProgress",
					[2] = "Detective"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				wait(0.5)
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Key") then
					getgenv().tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Key")
					wait(.4)
					game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
				end
				tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(15, Enum.EasingStyle.Linear)
tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(1347.7124, 37.3751602, -1325.6488)})
tween:Play()
				wait(15)
				function click()
					game:GetService'VirtualUser':CaptureController()
					game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
				end
				if game.Workspace.Enemies:FindFirstChild("Ice Admiral [Lv. 700] [Boss]") and game.Workspace.Map.Ice.Door.CanCollide == false and game.Workspace.Map.Ice.Door.Transparency == 1 then
					CheckBoss = true
					_G.SelectToolWeapon = SelectToolWeaponOld
					for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
						if CheckBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == "Ice Admiral [Lv. 700] [Boss]" then
							repeat wait(.1)
								pcall(function() 
									v.HumanoidRootPart.Transparency = 0.5
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									v.HumanoidRootPart.BrickColor = BrickColor.new("White")
									v.HumanoidRootPart.CanCollide = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0, 10, 10)
									click()
								end)
							until not CheckBoss or not v.Parent or v.Humanoid.Health <= 0
						end
					end
					CheckBoss = false
					wait(0.5)
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(15, Enum.EasingStyle.Linear)
tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-1166.23743, 7.65220165, 1728.36487)})
tween:Play()
print("Pss")
					wait(15)
					local args = {
						[1] = "TravelDressrosa" -- OLD WORLD to NEW WORLD
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				else
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Key") then
						getgenv().tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Key")
						wait(.4)
						game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
					end
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(15, Enum.EasingStyle.Linear)
tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(1347.7124, 37.3751602, -1325.6488)})
tween:Play()
print("Pss")
				end 
			end
		end 
	end
end)



----------- AutoThird --------------------------
spawn(function()
	while wait() do
		if _G.AutoThird then
			if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1500 and NewWorld then
				_G.FarmLevel = false
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016)
				wait(1.1)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Begin")
				wait(1.1)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016)
				if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") then
					for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "rip_indra [Lv. 1500] [Boss]" then
							repeat wait(.1)
								pcall(function()
									EquipWeapon(_G.SelectToolWeapon)
									AutoHaki()
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,25)
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Transparency = 0.8
									v.HumanoidRootPart.Size = Vector3.new(70,70,70)
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								end)
							until _G.AutoThird == false or v.Humanoid.Health <= 0 or not v.Parent
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016)
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016)
				end
			end
		end
	end
end)
game:GetService("RunService").Heartbeat:Connect(function()
	if _G.AutoThird then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)



----------- Fast Attack --------------------------
spawn(function()
	while wait() do
		if _G.FastAttack then
			pcall(function()
					local RigC = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework)
					require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut = 2,Sustained = 0,Inactive =1}
					RigC.activeController.timeToNextAttack = 0
					RigC.activeController.attacking = false
					RigC.activeController.increment = 3
					RigC.activeController.hitboxMagnitude = 55
			end)
		end
	end
end)
-------- Farm Chest ----
spawn(function()
	while wait() do
		if _G.AutoFarmChest then
			for i,v in pairs(game.Workspace:GetChildren()) do
				if v.Name == "Chest1" or v.Name == "Chest2" or v.Name == "Chest3" then
					v.CanCollide = false
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(1.5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.CFrame})
					tween:Play()
				end
			end
		end
	end
end)
spawn(function()
	while wait() do
		if _G.AutoFarmChest then
			game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end
end)

spawn(function()
	while wait() do
		if _G.AutoFarmChestHop then
			for i,v in pairs(game.Workspace:GetChildren()) do
				if v.Name == "Chest1" or v.Name == "Chest2" or v.Name == "Chest3" then
					v.CanCollide = false
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(1.5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.CFrame * CFrame.new(0,0,0)})
					tween:Play()
				elseif not game.Workspace:FindFirstChild("Chest1") and not game.Workspace:FindFirstChild("Chest2") and game.Workspace:FindFirstChild("Chest3") then
					local PlaceID = game.PlaceId
					local AllIDs = {}
					local foundAnything = ""
					local actualHour = os.date("!*t").hour
					local Deleted = false
					function TPReturner()
						local Site;
						if foundAnything == "" then
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
						else
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
						end
						local ID = ""
						if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
							foundAnything = Site.nextPageCursor
						end
						local num = 0;
						for i,v in pairs(Site.data) do
							local Possible = true
							ID = tostring(v.id)
							if tonumber(v.maxPlayers) > tonumber(v.playing) then
								for _,Existing in pairs(AllIDs) do
									if num ~= 0 then
										if ID == tostring(Existing) then
											Possible = false
										end
									else
										if tonumber(actualHour) ~= tonumber(Existing) then
											local delFile = pcall(function()
												-- delfile("NotSameServers.json")
												AllIDs = {}
												table.insert(AllIDs, actualHour)
											end)
										end
									end
									num = num + 1
								end
								if Possible == true then
									table.insert(AllIDs, ID)
									wait()
									pcall(function()
										-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
										wait()
										game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
									end)
									wait(.1)
								end
							end
						end
					end
					function Teleport() 
						while wait() do
							pcall(function()
								TPReturner()
								if foundAnything ~= "" then
									TPReturner()
								end
							end)
						end
					end
					Teleport()
				end
			end
		end
	end
end)
spawn(function()
	while wait() do
		if _G.AutoFarmChestHop then
			game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end
end)
-------- No Clip ----
game:GetService("RunService").RenderStepped:Connect(function()
	if  _G.DarkCode == true then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)



-------- Equitp All Weapon ----
spawn(function()
	while wait() do
		if _G.Equitp then
			for i,v in ipairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
				if v:IsA("Tool") then
					v.Parent = game:GetService("Players").LocalPlayer.Character
				end
			end
		end
	end
end)



-------- EliteHunter ----
spawn(function()
	while wait() do
		if _G.EliteHunter then
			if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true and string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Diablo") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Urban") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Deandre") then
				if game:GetService("ReplicatedStorage"):FindFirstChild("Diablo [Lv. 1750]") or game:GetService("ReplicatedStorage"):FindFirstChild("Urban [Lv. 1750]") or game:GetService("ReplicatedStorage"):FindFirstChild("Deandre [Lv. 1750]") then
					for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
						if v.Name == "Diablo [Lv. 1750]" or v.Name == "Urban [Lv. 1750]" or v.Name == "Deandre [Lv. 1750]" then
							repeat wait(.1)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,15)
								if HideHit then
									v.HumanoidRootPart.Transparency = 1
								else
									v.HumanoidRootPart.Transparency = 0.8
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(60,60,60)
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							until _G.EliteHunter == false or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5418.392578125, 313.74130249023, -2824.9157714844)
				end
			else
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5418.392578125, 313.74130249023, -2824.9157714844)
				wait(1.5)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter")
				wait(1.1)
			end
		end
	end
end)

game:GetService("RunService").Heartbeat:Connect(function()
	if _G.EliteHunter then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)


------------- AutoElectricClaw
spawn(function()
	while wait(.1) do
		if AutoElectricClaw then
			pcall(function()
				if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 400 then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
				end
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 400 then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
				end
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 399 then
					_G.SelectToolWeapon = "Electro"
				end
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Electric Claw") then
					_G.SelectToolWeapon = "Electric Claw"
				end
			end)
		end
	end
end)

------------- AutoRainbow
spawn(function()
	while wait(.1) do
		if _G.AutoRainbow then
			if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true and string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Stone") then
				if game:GetService("ReplicatedStorage"):FindFirstChild("Stone [Lv. 1550] [Boss]") then
					for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
						if v.Name == "Stone [Lv. 1550] [Boss]" then
							repeat wait()
								if sethiddenproperty then
									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								end
								if HideHitBlox then
									v.HumanoidRootPart.Transparency = 1
								else
									v.HumanoidRootPart.Transparency = 1
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							until _G.AutoRainbow == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11892.0703125, 930.57672119141, -8760.1591796875)
				end
			elseif game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true and string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Island Empress") then
				if game:GetService("ReplicatedStorage"):FindFirstChild("Island Empress [Lv. 1675] [Boss]") then
					for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
						if v.Name == "Island Empress [Lv. 1675] [Boss]" then
							repeat wait()
								if sethiddenproperty then

									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								end
								if HideHitBlox then
									v.HumanoidRootPart.Transparency = 1
								else
									v.HumanoidRootPart.Transparency = 1
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							until _G.AutoRainbow == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11892.0703125, 930.57672119141, -8760.1591796875)
				end
			elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Kilo Admiral") then
				if game:GetService("ReplicatedStorage"):FindFirstChild("Kilo Admiral [Lv. 1750] [Boss]") then
					for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
						if v.Name == "Kilo Admiral [Lv. 1750] [Boss]" then
							repeat wait()
								if sethiddenproperty then

									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								end
								if HideHitBlox then
									v.HumanoidRootPart.Transparency = 1
								else
									v.HumanoidRootPart.Transparency = 1
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							until _G.AutoRainbow == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11892.0703125, 930.57672119141, -8760.1591796875)
				end
			elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Captain Elephant") then
				if game:GetService("ReplicatedStorage"):FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
					for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
						if v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
							repeat wait()
								if sethiddenproperty then

									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								end
								if HideHitBlox then
									v.HumanoidRootPart.Transparency = 1
								else
									v.HumanoidRootPart.Transparency = 1
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							until _G.AutoRainbow == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11892.0703125, 930.57672119141, -8760.1591796875)
				end
			elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Beautiful Pirate") then
				if game:GetService("ReplicatedStorage"):FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") then
					for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
						if v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" then
							repeat wait()
								if sethiddenproperty then

									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								end
								if HideHitBlox then
									v.HumanoidRootPart.Transparency = 1
								else
									v.HumanoidRootPart.Transparency = 1
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							until _G.AutoRainbow == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11892.0703125, 930.57672119141, -8760.1591796875)
				end
			else
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11892.0703125, 930.57672119141, -8760.1591796875)
				wait(1.5)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("HornedMan","Bet")
			end
		end
	end
end)



------------- yama
spawn(function()
	while wait() do
		if yama then
			fireclickdetector(game:GetService("Workspace").Map.Waterfall.SealedKatana.Handle.ClickDetector)
		end
	end
end)


------------- AutoCitizen
spawn(function()
	while wait() do
		pcall(function()
			if _G.AutoCitizen then
				if game.Players.LocalPlayer.Data.Level.Value >= 1875 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 0 then
					if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Forest Pirate") and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "50") and game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if game:GetService("Workspace").Enemies:FindFirstChild("Forest Pirate [Lv. 1825]") then
							CitizenMagnet = true
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Forest Pirate [Lv. 1825]" then
									repeat wait(.1)
										game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,0)
										if HideHit then
											v.HumanoidRootPart.Transparency = 1
										else
											v.HumanoidRootPart.Transparency = .8
										end
										v.HumanoidRootPart.CanCollide = false
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										game:GetService'VirtualUser':CaptureController()
										game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										PosMonCitizen = v.HumanoidRootPart.CFrame
										CitizenMagnet = true
									until _G.AutoCitizen == false or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
								end
							end
						else
							CitizenMagnet = false
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13459.065429688, 412.68927001953, -7783.1860351563)
						end
					else
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125)
						wait(1.5)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest","CitizenQuest")
					end
				elseif game.Players.LocalPlayer.Data.Level.Value >= 1875 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 1 then
					if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Captain Elephant") and game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if game:GetService("ReplicatedStorage"):FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
							for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
								if v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
									repeat wait(.1)
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,10)
										if HideHit then
											v.HumanoidRootPart.Transparency = 1
										else
											v.HumanoidRootPart.Transparency = .8
										end
										v.HumanoidRootPart.CanCollide = false
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										game:GetService("VirtualUser"):CaptureController()
										game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
										sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
									until _G.AutoCitizen == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
								end
							end
						end
					else
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125)
						wait(1.5)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen")
					end
				elseif game.Players.LocalPlayer.Data.Level.Value >= 1875 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 2 then
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12512.138671875, 340.39279174805, -9872.8203125)
				end
			end
		end)
	end
end)
game:GetService("RunService").Heartbeat:Connect(function()
	if _G.AutoCitizen then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)


_G.fnz = true
-------------- ------------- AutoSuperhuman
spawn(function()
	while wait(.1) do
		if _G.Superhuman then
			if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
				local args = {
					[1] = "BuyBlackLeg"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
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
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300 then
					local args = {
						[1] = "BuyElectro"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
				if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300 then
					local args = {
						[1] = "BuyElectro"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 300 then
					local args = {
						[1] = "BuyFishmanKarate"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
				if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300 then
					local args = {
						[1] = "BuyFishmanKarate"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300 then
					local args = {
						[1] = "BlackbeardReward",
						[2] = "DragonClaw",
						[3] = "1"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					local args = {
						[1] = "BlackbeardReward",
						[2] = "DragonClaw",
						[3] = "2"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
				end
				if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300 then
					local args = {
						[1] = "BlackbeardReward",
						[2] = "DragonClaw",
						[3] = "1"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					local args = {
						[1] = "BlackbeardReward",
						[2] = "DragonClaw",
						[3] = "2"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
				end
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300 then
					local args = {
						[1] = "BuySuperhuman"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
				if game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 300 then
					_G.fnz = false
					local args = {
						[1] = "BuySuperhuman"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
			end
		end
	end
end)

-------------- ------------- FullSuperhuman
spawn(function()
	while wait(.1) do
		if _G.FullSuperhuman and _G.fnz then
			pcall(function()
				local args = {
					[1] = "BlackbeardReward",
					[2] = "DragonClaw",
					[3] = "1"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				local args = {
					[1] = "BlackbeardReward",
					[2] = "DragonClaw",
					[3] = "2"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
				-----------------
				local MyLevel = game.Players.LocalPlayer.Data.Level.Value
				if MyLevel >= 1100 then
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") then
						_G.autoraid = false
						_G.FarmLevel = true
					else
						_G.FarmLevel = false
						_G.autoraid = true
						local args = {
							[1] = "BlackbeardReward",
							[2] = "DragonClaw",
							[3] = "1"
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
						local args = {
							[1] = "BlackbeardReward",
							[2] = "DragonClaw",
							[3] = "2"
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
					end
				end
			end)
		end
	end
end)

-------------- ------------- AutoDeathStep
spawn(function()
	while wait(.1) do
		if _G.DeathStep then
			if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 450 then
				local args = {
					[1] = "BuyDeathStep"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end  
			if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 450 then
				local args = {
					[1] = "BuyDeathStep"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end  
			if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 449 then
				_G.SelectToolWeapon = "Black Leg"
			end   
		end
	end
end)


-------------- ------------- AutoOpenSaber
spawn(function()
	while wait(.1) do
		if _G.AutoOpenSaber then
			local off = game:GetService("Workspace").Map.Jungle.Final:FindFirstChild("Part")
			local MyLevel = game.Players.localPlayer.Data.Level.Value
			if MyLevel >= 200 and _G.FarmLevel == true then
				repeat wait(.1)
					_G.FarmLevel = false
					function accept1()
						local string_1 = "ProQuestProgress";
						local string2 = "SickMan";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF"];
						Target:InvokeServer(string_1, string_2);
					end

					function accept2()
						local string_1 = "ProQuestProgress";
						local string2 = "RichSon";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF"];
						Target:InvokeServer(string_1, string2);
					end
					function saber()
						if game:GetService("Workspace").Enemies:FindFirstChild("Mob Leader [Lv. 120] [Boss]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Mob Leader [Lv. 120] [Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
									repeat wait()
										pcall(function()
											if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
												local args = {
													[1] = "Buso"
												}
												game:GetService("ReplicatedStorage").Remotes.CommF:InvokeServer(unpack(args))
											end
											EquipWeapon(_G.SelectToolWeapon)
											v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
											v.HumanoidRootPart.CanCollide = false
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0, 10, 10)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										end)
									until v.Humanoid.Health == 0
								end
							end
						end

						function accept3()
							local string_1 = "ProQuestProgress";
							local string2 = "RichSon";
							local Target = game:GetService("ReplicatedStorage").Remotes["CommF"];
							Target:InvokeServer(string_1, string_2);
						end

						wait(.1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1421.87024, 55.4666862, 21.7750397)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1647.19556, 29.1544189, 438.299408)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1324.10144, 31.4560413, -461.404114)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1152.38464, 9.74718285, -700.309875)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1180.89563, 21.0007095, 187.861374)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1610.00757, 11.5049858, 164.001587)
						wait(2)
						local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Torch")
						wait(.4)
						game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
						wait(.1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1114.55762, 4.9214654, 4349.2334, -0.618430376, -1.56903435e-09, 0.785839617, -5.04992048e-09, 1, -1.97748973e-09, -0.785839617, -5.19136734e-09, -0.618430376)
						wait(5.5)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1114.26721, 4.16943789, 4366.15332)
						wait(1)
						local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Cup")
						wait(.4)
						game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1397.0614, 37.3480072, -1321.03955, -0.0699888021, -5.05999473e-08, 0.997547925, -7.48410045e-08, 1, 4.54734241e-08, -0.997547925, -7.14748296e-08, -0.0699888021)
						wait(4.5)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1457.87976, 88.2521744, -1390.39575)
						wait(1.5)
						accept1()
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-909.106689, 13.7520342, 4077.34888)
						wait(1.1)
						accept2()
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2852.90234, 7.56227827, 5367.72412)
						wait(1.5)
						EquipWeapon(_G.SelectToolWeapon)
						wait(1)
						saber()
						wait(2)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-909.106689, 13.7520342, 4077.34888)
						wait(1.1)
						accept3()
						wait(1)
						local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Relic")
						wait(.4)
						game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
						wait(1)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1405.84094, 29.8519993, 5.05432224, 0.859020233, -4.18967083e-08, 0.511941671, 4.07572731e-09, 1, 7.49999103e-08, -0.511941671, -6.23399004e-08, 0.859020233)
						wait(1)
						if off.CanCollide == false then
							_G.AutoOpenSaber = false
							_G.FarmLevel = true
						end
					end
				until _G.AutoOpenSaber == false or off.CanCollide == false or _G.FarmLevel == true

			elseif MyLevel >= 200 then
				repeat wait(.1)
					function accept1()
						local string_1 = "ProQuestProgress";
						local string2 = "SickMan";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF"];
						Target:InvokeServer(string_1, string_2);
					end

					function accept2()
						local string_1 = "ProQuestProgress";
						local string2 = "RichSon";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF"];
						Target:InvokeServer(string_1, string2);
					end
					function saber()
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v.Name == "Mob Leader [Lv. 120] [Boss]" then
								repeat wait()
									for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == "Mob Leader [Lv. 120] [Boss]" then
											if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
												local args = {
													[1] = "Buso"
												}
												game:GetService("ReplicatedStorage").Remotes.CommF:InvokeServer(unpack(args))
											end
											EquipWeapon(_G.SelectToolWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.HumanoidRootPart.Size = Vector3.new(50,50,50)
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
											game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
										end
									end
								until v.Humanoid.Health == 0
							end
						end
					end

					function accept3()
						local string_1 = "ProQuestProgress";
						local string2 = "RichSon";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF"];
						Target:InvokeServer(string_1, string_2);
					end

					wait(.1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1421.87024, 55.4666862, 21.7750397)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1647.19556, 29.1544189, 438.299408)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1324.10144, 31.4560413, -461.404114)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1152.38464, 9.74718285, -700.309875)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1180.89563, 21.0007095, 187.861374)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1610.00757, 11.5049858, 164.001587)
					wait(2)
					local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Torch")
					wait(.4)
					game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
					wait(.1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1114.55762, 4.9214654, 4349.2334, -0.618430376, -1.56903435e-09, 0.785839617, -5.04992048e-09, 1, -1.97748973e-09, -0.785839617, -5.19136734e-09, -0.618430376)
					wait(5.5)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1114.26721, 4.16943789, 4366.15332)
					wait(1)
					local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Cup")
					wait(.4)
					game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1397.0614, 37.3480072, -1321.03955, -0.0699888021, -5.05999473e-08, 0.997547925, -7.48410045e-08, 1, 4.54734241e-08, -0.997547925, -7.14748296e-08, -0.0699888021)
					wait(4.5)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1457.87976, 88.2521744, -1390.39575)
					wait(1.5)
					accept1()
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-909.106689, 13.7520342, 4077.34888)
					wait(1.1)
					accept2()
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2852.90234, 7.56227827, 5367.72412)
					wait(1.5)
					EquipWeapon(_G.SelectToolWeapon)
					wait(1)
					saber()
					wait(2)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-909.106689, 13.7520342, 4077.34888)
					wait(1.1)
					accept3()
					wait(1)
					local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Relic")
					wait(.4)
					game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1405.84094, 29.8519993, 5.05432224, 0.859020233, -4.18967083e-08, 0.511941671, 4.07572731e-09, 1, 7.49999103e-08, -0.511941671, -6.23399004e-08, 0.859020233)
					wait(1)
					if off.CanCollide == false then
						_G.AutoOpenSaber = false
					end
				until G.AutoOpenSaber == false or off.CanCollide == false
				if game:GetService("Workspace").Enemies:FindFirstChild("Saber Expert [Lv. 200] [Boss]") then
					for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Saber Expert [Lv. 200] [Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
							repeat wait()
								pcall(function()
									if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
										local args = {
											[1] = "Buso"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF:InvokeServer(unpack(args))
									end
									EquipWeapon(_G.SelectToolWeapon)
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									v.HumanoidRootPart.CanCollide = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0, 15, 10)
									game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
								end)
							until _G.AutoOpenSaber == true or v.Humanoid.Health <= 0
						end
					end
				end
			end
		end
	end
end)

-------------- ------------- AutoPole
spawn(function()
	while wait() do
		if _G.Pole then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v.Name == "Thunder God [Lv. 575] [Boss]" then
						repeat wait()
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
						until v.Humanoid.Health == 0 or not _G.Pole
					else
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-7911.14453, 5613.89795, -2272.67822, -0.585544586, -6.38371889e-09, 0.810640216, -2.4883267e-08, 1, -1.00988613e-08, -0.810640216, -2.60847095e-08, -0.585544586)
					end
				end
			end)
		end
	end
end)
------------------------------- Pole Hop
spawn(function()
	while wait() do
		if _G.PoleHop then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				if game:GetService("Workspace").Enemies:FindFirstChild("Thunder God [Lv. 575] [Boss]") then
					for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Thunder God [Lv. 575] [Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
							repeat wait()
								pcall(function()
									if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
										local args = {
											[1] = "Buso"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									v.HumanoidRootPart.CanCollide = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
								end)
							until _G.PoleHop == false or v.Humanoid.Health <= 0
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-7911.14453, 5613.89795, -2272.67822, -0.585544586, -6.38371889e-09, 0.810640216, -2.4883267e-08, 1, -1.00988613e-08, -0.810640216, -2.60847095e-08, -0.585544586)
					wait(3)
					if not game:GetService("Workspace").Enemies:FindFirstChild("Thunder God [Lv. 575] [Boss]") then
						local PlaceID = game.PlaceId
						local AllIDs = {}
						local foundAnything = ""
						local actualHour = os.date("!*t").hour
						local Deleted = false
						function TPReturner()
							local Site;
							if foundAnything == "" then
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
							else
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
							end
							local ID = ""
							if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
								foundAnything = Site.nextPageCursor
							end
							local num = 0;
							for i,v in pairs(Site.data) do
								local Possible = true
								ID = tostring(v.id)
								if tonumber(v.maxPlayers) > tonumber(v.playing) then
									for _,Existing in pairs(AllIDs) do
										if num ~= 0 then
											if ID == tostring(Existing) then
												Possible = false
											end
										else
											if tonumber(actualHour) ~= tonumber(Existing) then
												local delFile = pcall(function()
													-- delfile("NotSameServers.json")
													AllIDs = {}
													table.insert(AllIDs, actualHour)
												end)
											end
										end
										num = num + 1
									end
									if Possible == true then
										table.insert(AllIDs, ID)
										wait()
										pcall(function()
											-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
											wait()
											game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
										end)
										wait(.1)
									end
								end
							end
						end
						function Teleport() 
							while wait() do
								pcall(function()
									TPReturner()
									if foundAnything ~= "" then
										TPReturner()
									end
								end)
							end
						end
						Teleport()
					end
				end
			end) 
		end
	end
end)

-------------- ------------- AutoSwanGlasses
spawn(function()
	while wait() do
		if _G.SwanGlasses then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v.Name == "Don Swan [Lv. 1000] [Boss]" then
						repeat wait()
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
						until v.Humanoid.Health == 0 or not _G.SwanGlasses
					else
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2302.19019, 15.1778421, 663.811035)
					end
				end
			end)
		end
	end
end)
----------------- Auto Swan Hop
spawn(function()
	while wait() do
		if _G.SwanGlassesHop then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				if game:GetService("Workspace").Enemies:FindFirstChild("Don Swan [Lv. 1000] [Boss]") then
					for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Don Swan [Lv. 1000] [Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
							repeat wait()
								game:GetService'VirtualUser':CaptureController()
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
								pcall(function()
									if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
										local args = {
											[1] = "Buso"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									v.HumanoidRootPart.CanCollide = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
								end)
							until _G.SwanGlassesHop == false or v.Humanoid.Health <= 0
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2302.19019, 15.1778421, 663.811035)
					wait(3)
					if not game:GetService("Workspace").Enemies:FindFirstChild("Don Swan [Lv. 1000] [Boss]") then
						local PlaceID = game.PlaceId
						local AllIDs = {}
						local foundAnything = ""
						local actualHour = os.date("!*t").hour
						local Deleted = false
						function TPReturner()
							local Site;
							if foundAnything == "" then
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
							else
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
							end
							local ID = ""
							if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
								foundAnything = Site.nextPageCursor
							end
							local num = 0;
							for i,v in pairs(Site.data) do
								local Possible = true
								ID = tostring(v.id)
								if tonumber(v.maxPlayers) > tonumber(v.playing) then
									for _,Existing in pairs(AllIDs) do
										if num ~= 0 then
											if ID == tostring(Existing) then
												Possible = false
											end
										else
											if tonumber(actualHour) ~= tonumber(Existing) then
												local delFile = pcall(function()
													-- delfile("NotSameServers.json")
													AllIDs = {}
													table.insert(AllIDs, actualHour)
												end)
											end
										end
										num = num + 1
									end
									if Possible == true then
										table.insert(AllIDs, ID)
										wait()
										pcall(function()
											-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
											wait()
											game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
										end)
										wait(.1)
									end
								end
							end
						end
						function Teleport() 
							while wait() do
								pcall(function()
									TPReturner()
									if foundAnything ~= "" then
										TPReturner()
									end
								end)
							end
						end
						Teleport()
					end
				end
			end) 
		end
	end
end)
-------------- ------------- AutoDarkCode
spawn(function()
	while wait() do
		if _G.DarkCode then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v.Name == "Darkbeard [Lv. 1000] [Raid Boss]" then
						repeat wait()
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(15,15,15)
						until v.Humanoid.Health == 0 or not _G.DarkCode
					else
						game.Players.localPlayer.Character.HumanoidRootPart.CFrame = game.Workspace["_WorldOrigin"].Locations["Dark Arena"].CFrame
					end
				end
			end)
		end
	end
end)
----------------- Dark Code Hop

spawn(function()
	while wait() do
		if _G.DarkCodeHop then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				if game:GetService("Workspace").Enemies:FindFirstChild("Darkbeard [Lv. 1000] [Raid Boss]") then
					for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Darkbeard [Lv. 1000] [Raid Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
							repeat wait()
								pcall(function()
									if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
										local args = {
											[1] = "Buso"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									v.HumanoidRootPart.CanCollide = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
								end)
							until _G.DarkCodeHop == false or v.Humanoid.Health <= 0
						end
					end
				else
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = game.Workspace["_WorldOrigin"].Locations["Dark Arena"].CFrame
					wait(3)
					if not game:GetService("Workspace").Enemies:FindFirstChild("Darkbeard [Lv. 1000] [Raid Boss]") then
						local PlaceID = game.PlaceId
						local AllIDs = {}
						local foundAnything = ""
						local actualHour = os.date("!*t").hour
						local Deleted = false
						function TPReturner()
							local Site;
							if foundAnything == "" then
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
							else
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
							end
							local ID = ""
							if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
								foundAnything = Site.nextPageCursor
							end
							local num = 0;
							for i,v in pairs(Site.data) do
								local Possible = true
								ID = tostring(v.id)
								if tonumber(v.maxPlayers) > tonumber(v.playing) then
									for _,Existing in pairs(AllIDs) do
										if num ~= 0 then
											if ID == tostring(Existing) then
												Possible = false
											end
										else
											if tonumber(actualHour) ~= tonumber(Existing) then
												local delFile = pcall(function()
													-- delfile("NotSameServers.json")
													AllIDs = {}
													table.insert(AllIDs, actualHour)
												end)
											end
										end
										num = num + 1
									end
									if Possible == true then
										table.insert(AllIDs, ID)
										wait()
										pcall(function()
											-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
											wait()
											game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
										end)
										wait(.1)
									end
								end
							end
						end
						function Teleport() 
							while wait() do
								pcall(function()
									TPReturner()
									if foundAnything ~= "" then
										TPReturner()
									end
								end)
							end
						end
						Teleport()
					end
				end
			end) 
		end
	end
end)
------------------ Auto Bisentov2
spawn(function()
	while wait() do
		if _G.Bisentov2 then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v.Name == "Greybeard [Lv. 750] [Raid Boss]" then
						repeat wait()
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
						until v.Humanoid.Health == 0 or not _G.Bisentov2
					else
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4970.26904, 20.6520348, 4258.50537, 0.27719146, -4.41324488e-09, 0.960814714, -1.61775908e-08, 1, 9.26040666e-09, -0.960814714, -1.81105726e-08, 0.27719146)
					end
				end
			end)
		end
	end
end)
-------------------- Auto Bisentov2Hop
spawn(function()
	while wait() do
		if _G.Bisentov2Hop then
			pcall(function()
				EquipWeapon(_G.SelectToolWeapon)
				if game:GetService("Workspace").Enemies:FindFirstChild("Greybeard [Lv. 750] [Raid Boss]") then
					for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Greybeard [Lv. 750] [Raid Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
							repeat wait()
								pcall(function()
									if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
										local args = {
											[1] = "Buso"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									v.HumanoidRootPart.CanCollide = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
								end)
							until _G.Bisentov2Hop == false or v.Humanoid.Health <= 0
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4970.26904, 20.6520348, 4258.50537, 0.27719146, -4.41324488e-09, 0.960814714, -1.61775908e-08, 1, 9.26040666e-09, -0.960814714, -1.81105726e-08, 0.27719146)
					wait(3)
					if not game:GetService("Workspace").Enemies:FindFirstChild("Greybeard [Lv. 750] [Raid Boss]") then
						local PlaceID = game.PlaceId
						local AllIDs = {}
						local foundAnything = ""
						local actualHour = os.date("!*t").hour
						local Deleted = false
						function TPReturner()
							local Site;
							if foundAnything == "" then
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
							else
								Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
							end
							local ID = ""
							if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
								foundAnything = Site.nextPageCursor
							end
							local num = 0;
							for i,v in pairs(Site.data) do
								local Possible = true
								ID = tostring(v.id)
								if tonumber(v.maxPlayers) > tonumber(v.playing) then
									for _,Existing in pairs(AllIDs) do
										if num ~= 0 then
											if ID == tostring(Existing) then
												Possible = false
											end
										else
											if tonumber(actualHour) ~= tonumber(Existing) then
												local delFile = pcall(function()
													-- delfile("NotSameServers.json")
													AllIDs = {}
													table.insert(AllIDs, actualHour)
												end)
											end
										end
										num = num + 1
									end
									if Possible == true then
										table.insert(AllIDs, ID)
										wait()
										pcall(function()
											-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
											wait()
											game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
										end)
										wait(.1)
									end
								end
							end
						end
						function Teleport() 
							while wait() do
								pcall(function()
									TPReturner()
									if foundAnything ~= "" then
										TPReturner()
									end
								end)
							end
						end
						Teleport()
					end
				end
			end) 
		end
	end
end)



-------------- ------------- AutoAccessories



spawn(function()
	while wait() do
		if AutoAccessories then
			CheckAccessories = game.Players.LocalPlayer.Character 
			if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid").Health > 0 then
				if CheckAccessories:FindFirstChild("CoolShades") or CheckAccessories:FindFirstChild("BlackSpikeyCape") or CheckAccessories:FindFirstChild("BlueSpikeyCape") or CheckAccessories:FindFirstChild("RedSpikeyCape") or CheckAccessories:FindFirstChild("Chopper") or CheckAccessories:FindFirstChild("MarineCape") or CheckAccessories:FindFirstChild("GhoulMask") or CheckAccessories:FindFirstChild("MarineCap") or CheckAccessories:FindFirstChild("PinkCape") or CheckAccessories:FindFirstChild("SaboTopHat") or CheckAccessories:FindFirstChild("SwanGlasses") or CheckAccessories:FindFirstChild("UsoapHat") or CheckAccessories:FindFirstChild("Corrida") or CheckAccessories:FindFirstChild("ZebraCap") or CheckAccessories:FindFirstChild("TomoeRing") or CheckAccessories:FindFirstChild("BlackCape") or CheckAccessories:FindFirstChild("SwordsmanHat") or CheckAccessories:FindFirstChild("SantaHat") or CheckAccessories:FindFirstChild("ElfHat") or CheckAccessories:FindFirstChild("DarkCoat") then
				else
					EquipWeapon(SelectTooAccessories)
					wait(0.1)
					game:GetService'VirtualUser':CaptureController()
					game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
					wait(0.1)
					if game.Players.LocalPlayer.Character:FindFirstChild(SelectTooAccessories) then
						game.Players.LocalPlayer.Character:FindFirstChild(SelectTooAccessories).Parent = game.Players.LocalPlayer:FindFirstChild("Backpack")
					end
					wait(1)
				end
			end
		end
	end
end)
tgls:Label("--AutoFarmBoss--", true)
tgls:Toggle("Auto Farm Boss",false,function(Value)
	wait(.1)
	local args = {
		[1] = "AbandonQuest"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
	FramBoss = Value
end)
spawn(function()
	while wait(.1) do
		if FramBoss then
			EquipWeaponBoss()
		end
	end
end)
spawn(function()
	while wait(.1) do
		if FramBoss then
			AutoFramBoss()
		end 
	end
end)
function CheckQuestBoss()
	if SelectBoss == "Diamond [Lv. 750] [Boss]" then
		MsBoss = "Diamond [Lv. 750] [Boss]"
		NaemQuestBoss = "Area1Quest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
		CFrameBoss = CFrame.new(-1736.26587, 198.627731, -236.412857, -0.997808516, 0, -0.0661673471, 0, 1, 0, 0.0661673471, 0, -0.997808516)
	elseif SelectBoss == "Jeremy [Lv. 850] [Boss]" then
		MsBoss = "Jeremy [Lv. 850] [Boss]"
		NaemQuestBoss = "Area2Quest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
		CFrameBoss = CFrame.new(2203.76953, 448.966034, 752.731079, -0.0217453763, 0, -0.999763548, 0, 1, 0, 0.999763548, 0, -0.0217453763)
	elseif SelectBoss == "Fajita [Lv. 925] [Boss]" then
		MsBoss = "Fajita [Lv. 925] [Boss]"
		NaemQuestBoss = "MarineQuest3"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
		CFrameBoss = CFrame.new(-2297.40332, 115.449463, -3946.53833, 0.961227536, -1.46645796e-09, -0.275756449, -2.3212845e-09, 1, -1.34094433e-08, 0.275756449, 1.35296352e-08, 0.961227536)
	elseif SelectBoss == "Don Swan [Lv. 1000] [Boss]" then
		MsBoss = "Don Swan [Lv. 1000] [Boss]"
		CFrameBoss = CFrame.new(2288.802, 15.1870775, 863.034607, 0.99974072, -8.41247214e-08, -0.0227668174, 8.4774733e-08, 1, 2.75850098e-08, 0.0227668174, -2.95079072e-08, 0.99974072)
	elseif SelectBoss == "Smoke Admiral [Lv. 1150] [Boss]" then
		MsBoss = "Smoke Admiral [Lv. 1150] [Boss]"
		NaemQuestBoss = "IceSideQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-6059.96191, 15.9868021, -4904.7373, -0.444992423, -3.0874483e-09, 0.895534337, -3.64098796e-08, 1, -1.4644522e-08, -0.895534337, -3.91229982e-08, -0.444992423)
		CFrameBoss = CFrame.new(-5115.72754, 23.7664986, -5338.2207, 0.251453817, 1.48345061e-08, -0.967869282, 4.02796978e-08, 1, 2.57916977e-08, 0.967869282, -4.54708946e-08, 0.251453817)
	elseif SelectBoss == "Cursed Captain [Lv. 1325] [Raid Boss]" then
		MsBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
		CFrameBoss = CFrame.new(916.928589, 181.092773, 33422, -0.999505103, 9.26310495e-09, 0.0314563364, 8.42916226e-09, 1, -2.6643713e-08, -0.0314563364, -2.63653774e-08, -0.999505103)
	elseif SelectBoss == "Darkbeard [Lv. 1000] [Raid Boss]" then
		MsBoss = "Darkbeard [Lv. 1000] [Raid Boss]"
		CFrameBoss = CFrame.new(3876.00366, 24.6882591, -3820.21777, -0.976951957, 4.97356325e-08, 0.213458836, 4.57335361e-08, 1, -2.36868622e-08, -0.213458836, -1.33787044e-08, -0.976951957)
	elseif SelectBoss == "Order [Lv. 1250] [Raid Boss]" then
		MsBoss = "Order [Lv. 1250] [Raid Boss]"
		CFrameBoss = CFrame.new(-6221.15039, 16.2351036, -5045.23584, -0.380726993, 7.41463495e-08, 0.924687505, 5.85604774e-08, 1, -5.60738549e-08, -0.924687505, 3.28013137e-08, -0.380726993)
	elseif SelectBoss == "Awakened Ice Admiral [Lv. 1400] [Boss]" then
		MsBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
		NaemQuestBoss = "FrostQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(5669.33203, 28.2118053, -6481.55908, 0.921275556, -1.25320829e-08, 0.388910472, 4.72230788e-08, 1, -7.96414241e-08, -0.388910472, 9.17372489e-08, 0.921275556)
		CFrameBoss = CFrame.new(6407.33936, 340.223785, -6892.521, 0.49051559, -5.25310213e-08, -0.871432424, -2.76146022e-08, 1, -7.58250565e-08, 0.871432424, 6.12576301e-08, 0.49051559)
	elseif SelectBoss == "Tide Keeper [Lv. 1475] [Boss]" then
		MsBoss = "Tide Keeper [Lv. 1475] [Boss]"
		NaemQuestBoss = "ForgottenQuest"             
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-3053.89648, 236.881363, -10148.2324, -0.985987961, -3.58504737e-09, 0.16681771, -3.07832915e-09, 1, 3.29612559e-09, -0.16681771, 2.73641976e-09, -0.985987961)
		CFrameBoss = CFrame.new(-3570.18652, 123.328949, -11555.9072, 0.465199202, -1.3857326e-08, 0.885206044, 4.0332897e-09, 1, 1.35347511e-08, -0.885206044, -2.72606271e-09, 0.465199202)
		-- Old World
	elseif SelectBoss == "Saber Expert [Lv. 200] [Boss]" then
		MsBoss = "Saber Expert [Lv. 200] [Boss]"
		CFrameBoss = CFrame.new(-1458.89502, 29.8870335, -50.633564, 0.858821094, 1.13848939e-08, 0.512275636, -4.85649254e-09, 1, -1.40823326e-08, -0.512275636, 9.6063415e-09, 0.858821094)
	elseif SelectBoss == "The Saw [Lv. 100] [Boss]" then
		MsBoss = "The Saw [Lv. 100] [Boss]"
		CFrameBoss = CFrame.new(-683.519897, 13.8534927, 1610.87854, -0.290192783, 6.88365773e-08, 0.956968188, 6.98413629e-08, 1, -5.07531119e-08, -0.956968188, 5.21077759e-08, -0.290192783)
	elseif SelectBoss == "The Gorilla King [Lv. 25] [Boss]" then
		MsBoss = "The Gorilla King [Lv. 25] [Boss]"
		NaemQuestBoss = "JungleQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
		CFrameBoss = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
	elseif SelectBoss == "Bobby [Lv. 55] [Boss]" then
		MsBoss = "Bobby [Lv. 55] [Boss]"
		NaemQuestBoss = "BuggyQuest1"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
		CFrameBoss = CFrame.new(-1147.65173, 32.5966301, 4156.02588, 0.956680477, -1.77109952e-10, -0.29113996, 5.16530874e-10, 1, 1.08897802e-09, 0.29113996, -1.19218679e-09, 0.956680477)
	elseif SelectBoss == "Yeti [Lv. 110] [Boss]" then
		MsBoss = "Yeti [Lv. 110] [Boss]"
		NaemQuestBoss = "SnowQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(1384.90247, 87.3078308, -1296.6825, 0.280209213, 2.72035177e-08, -0.959938943, -6.75690828e-08, 1, 8.6151708e-09, 0.959938943, 6.24481444e-08, 0.280209213)
		CFrameBoss = CFrame.new(1221.7356, 138.046906, -1488.84082, 0.349343032, -9.49245944e-08, 0.936994851, 6.29478194e-08, 1, 7.7838429e-08, -0.936994851, 3.17894653e-08, 0.349343032)
	elseif SelectBoss == "Mob Leader [Lv. 120] [Boss]" then
		MsBoss = "Mob Leader [Lv. 120] [Boss]"
		CFrameBoss = CFrame.new(-2848.59399, 7.4272871, 5342.44043, -0.928248107, -8.7248246e-08, 0.371961564, -7.61816636e-08, 1, 4.44474857e-08, -0.371961564, 1.29216433e-08, -0.928248107)
		--The Gorilla King [Lv. 25] [Boss]
	elseif SelectBoss == "Vice Admiral [Lv. 130] [Boss]" then
		MsBoss = "Vice Admiral [Lv. 130] [Boss]"
		NaemQuestBoss = "MarineQuest2"
		LevelQuestBoss = 2
		CFrameQuestBoss = CFrame.new(-5035.42285, 28.6520386, 4324.50293, -0.0611100644, -8.08395768e-08, 0.998130739, -1.57416586e-08, 1, 8.00271849e-08, -0.998130739, -1.08217701e-08, -0.0611100644)
		CFrameBoss = CFrame.new(-5078.45898, 99.6520691, 4402.1665, -0.555574954, -9.88630566e-11, 0.831466436, -6.35508286e-08, 1, -4.23449258e-08, -0.831466436, -7.63661632e-08, -0.555574954)
	elseif SelectBoss == "Warden [Lv. 175] [Boss]" then
		MsBoss = "Warden [Lv. 175] [Boss]"
		NaemQuestBoss = "ImpelQuest"
		LevelQuestBoss = 1
		CFrameQuestBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
		CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
	elseif SelectBoss == "Chief Warden [Lv. 200] [Boss]" then
		MsBoss = "Chief Warden [Lv. 200] [Boss]"
		NaemQuestBoss = "ImpelQuest"
		LevelQuestBoss = 2
		CFrameQuestBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
		CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
	elseif SelectBoss == "Swan [Lv. 225] [Boss]" then
		MsBoss = "Swan [Lv. 225] [Boss]"
		NaemQuestBoss = "ImpelQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
		CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
	elseif SelectBoss == "Magma Admiral [Lv. 350] [Boss]" then
		MsBoss = "Magma Admiral [Lv. 350] [Boss]"
		NaemQuestBoss = "MagmaQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-5317.07666, 12.2721891, 8517.41699, 0.51175487, -2.65508806e-08, -0.859131515, -3.91131572e-08, 1, -5.42026761e-08, 0.859131515, 6.13418294e-08, 0.51175487)
		CFrameBoss = CFrame.new(-5530.12646, 22.8769703, 8859.91309, 0.857838571, 2.23414389e-08, 0.513919294, 1.53689133e-08, 1, -6.91265853e-08, -0.513919294, 6.71978384e-08, 0.857838571)
	elseif SelectBoss == "Fishman Lord [Lv. 425] [Boss]" then
		MsBoss = "Fishman Lord [Lv. 425] [Boss]"
		NaemQuestBoss = "FishmanQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(61123.0859, 18.5066795, 1570.18018, 0.927145958, 1.0624845e-07, 0.374700129, -6.98219367e-08, 1, -1.10790765e-07, -0.374700129, 7.65569368e-08, 0.927145958)
		CFrameBoss = CFrame.new(61351.7773, 31.0306778, 1113.31409, 0.999974668, 0, -0.00714713801, 0, 1.00000012, 0, 0.00714714266, 0, 0.999974549)
	elseif SelectBoss == "Wysper [Lv. 500] [Boss]" then
		MsBoss = "Wysper [Lv. 500] [Boss]"
		NaemQuestBoss = "SkyExp1Quest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-7862.94629, 5545.52832, -379.833954, 0.462944925, 1.45838088e-08, -0.886386991, 1.0534996e-08, 1, 2.19553424e-08, 0.886386991, -1.95022007e-08, 0.462944925)
		CFrameBoss = CFrame.new(-7925.48389, 5550.76074, -636.178345, 0.716468513, -1.22915289e-09, 0.697619379, 3.37381434e-09, 1, -1.70304748e-09, -0.697619379, 3.57381835e-09, 0.716468513)
	elseif SelectBoss == "Thunder God [Lv. 575] [Boss]" then
		MsBoss = "Thunder God [Lv. 575] [Boss]"
		NaemQuestBoss = "SkyExp2Quest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-7902.78613, 5635.99902, -1411.98706, -0.0361216255, -1.16895912e-07, 0.999347389, 1.44533963e-09, 1, 1.17024491e-07, -0.999347389, 5.6715117e-09, -0.0361216255)
		CFrameBoss = CFrame.new(-7917.53613, 5616.61377, -2277.78564, 0.965189934, 4.80563429e-08, -0.261550069, -6.73089886e-08, 1, -6.46515304e-08, 0.261550069, 8.00056768e-08, 0.965189934)
	elseif SelectBoss == "Cyborg [Lv. 675] [Boss]" then
		MsBoss = "Cyborg [Lv. 675] [Boss]"
		NaemQuestBoss = "FountainQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(5253.54834, 38.5361786, 4050.45166, -0.0112687312, -9.93677887e-08, -0.999936521, 2.55291371e-10, 1, -9.93769547e-08, 0.999936521, -1.37512213e-09, -0.0112687312)
		CFrameBoss = CFrame.new(6041.82813, 52.7112198, 3907.45142, -0.563162148, 1.73805248e-09, -0.826346457, -5.94632716e-08, 1, 4.26280238e-08, 0.826346457, 7.31437524e-08, -0.563162148)
		--Three World
	elseif SelectBoss == "Kilo Admiral [Lv. 1750] [Boss]" then
		MsBoss = "Kilo Admiral [Lv. 1750] [Boss]"
		NaemQuestBoss = "MarineTreeIsland"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
		CFrameBoss = CFrame.new(2955.1189, 423.584412, -7240.22217, -0.761679471, 7.01648872e-08, 0.647953987, 8.75833539e-09, 1, -9.79912755e-08, -0.647953987, -6.89629474e-08, -0.761679471)
	elseif SelectBoss == "Captain Elephant [Lv. 1875] [Boss]" then
		MsBoss = "Captain Elephant [Lv. 1875] [Boss]"
		NaemQuestBoss = "DeepForestIsland"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
		CFrameBoss = CFrame.new(-13592.9053, 332.23584, -8134.08643, -0.866908491, -1.7684858e-08, 0.498467356, -3.95491107e-08, 1, -3.33032872e-08, -0.498467356, -4.85848446e-08, -0.866908491)
	elseif SelectBoss == "Beautiful Pirate [Lv. 1950] [Boss]" then
		MsBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
		NaemQuestBoss = "DeepForestIsland2"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
		CFrameBoss = CFrame.new(5310.80957, 22.5622349, 129.390533, 1, -2.47274325e-08, 1.41872977e-13, 2.47274325e-08, 1, -4.55364528e-08, -1.40746979e-13, 4.55364528e-08, 1)
	elseif SelectBoss == "Longma [Lv. 2000] [Boss]" then
		MsBoss = "Longma [Lv. 2000] [Boss]"
		CFrameBoss = CFrame.new(-10293.208, 332.791351, -9450.625, 0.132661447, -0.213521436, -0.96788919, -0.0110089043, 0.976142585, -0.21685116, 0.991100252, 0.0394231752, 0.127145842)
	elseif SelectBoss == "Stone [Lv. 1550] [Boss]" then
		MsBoss = "Stone [Lv. 1550] [Boss]"
		NaemQuestBoss = "PiratePortQuest"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
		CFrameBoss = CFrame.new(-970.778564, 40.0068855, 6795.5249, -0.179641441, -2.87076816e-08, 0.983732164, -4.4126935e-08, 1, 2.11243023e-08, -0.983732164, -3.96142852e-08, -0.179641441)
	elseif SelectBoss == "Island Empress [Lv. 1675] [Boss]" then
		MsBoss = "Island Empress [Lv. 1675] [Boss]"
		NaemQuestBoss = "AmazonQuest2"
		LevelQuestBoss = 3
		CFrameQuestBoss = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
		CFrameBoss = CFrame.new(5813.94140625, 661.14862060547, 202.04710388184)
	end
end
local Boss = {}
for i, v in pairs(game.ReplicatedStorage:GetChildren()) do
	if string.find(v.Name, "Boss") then
		if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
		else
			table.insert(Boss, v.Name)
		end
	end
end
for i, v in pairs(game.workspace.Enemies:GetChildren()) do
	if string.find(v.Name, "Boss") then
		if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
		else
			table.insert(Boss, v.Name)
		end
	end
end
local BossName = tgls:Dropdown("Select Boss",Boss,function(Value)
	SelectBoss = Value
	Don = false
end)
local SelectWeaponBoss = "" 
local SelectWeaponKillBos = tgls:Dropdown("Select Weapon Kill Boss",Wapon,function(Value)
	_G.SelectWeaponBoss = Value
end)
tgls:Button("Refresh Weapon Boss",function()
	SelectWeaponKillBoss:Clear()
	for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
		if v:IsA("Tool") then
			SelectWeaponKillBoss:Add(v.Name)
		end
	end
	for i, v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
		if v:IsA("Tool") then
			SelectWeaponKillBoss:Add(v.Name)
		end
	end
end)
tgls:Button("Refresh Boss",function()
	BossName:Clear()
	for i, v in pairs(game.ReplicatedStorage:GetChildren()) do
		if string.find(v.Name, "Boss") then
			if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
			else
				BossName:Add(v.Name)
			end
		end
	end
	for i, v in pairs(game.workspace.Enemies:GetChildren()) do
		if string.find(v.Name, "Boss") then
			if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
			else
				BossName:Add(v.Name)
			end
		end
	end
end)
function AutoFramBoss()
	CheckQuestBoss()
	if SelectBoss == "Don Swan [Lv. 1000] [Boss]" or SelectBoss == "Cursed Captain [Lv. 1325] [Raid Boss]" or SelectBoss == "Saber Expert [Lv. 200] [Boss]" or SelectBoss == "Mob Leader [Lv. 120] [Boss]" or SelectBoss == "Darkbeard [Lv. 1000] [Raid Boss]" or SelectBoss == "Longma [Lv. 2000] [Boss]" then
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if FramBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
					repeat
						pcall(function() wait() 
							if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
								local args = {
									[1] = "Buso"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							EquipWeapon(_G.SelectWeaponBoss)
							if HideHitBlox then
								v.HumanoidRootPart.Transparency = 0.75
							else
								v.HumanoidRootPart.Transparency = 1
							end
							v.HumanoidRootPart.CanCollide = false
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 25, 0)
							game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
							VirtualUser:CaptureController()
							VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end)
					until not FramBoss or not v.Parent or v.Humanoid.Health <= 0
				end
			end
		else
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
		end
	elseif SelectBoss == "Order [Lv. 1250] [Raid Boss]" then
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if FramBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
					repeat 
						pcall(function() wait() 
							if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
								local args = {
									[1] = "Buso"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							EquipWeapon(_G.SelectWeaponBoss)
							if HideHitBlox then
								v.HumanoidRootPart.Transparency = 0.75
							else
								v.HumanoidRootPart.Transparency = 1
							end
							v.HumanoidRootPart.CanCollide = false
							v.HumanoidRootPart.Size = Vector3.new(80, 80, 80)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 25, 0)
							game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
							VirtualUser:CaptureController()
							VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end)
					until not FramBoss or not v.Parent or v.Humanoid.Health <= 0
				end
			end
		else
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
		end
	else
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) or game:GetService("ReplicatedStorage"):FindFirstChild(SelectBoss) then
			if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then
				print()
				CheckQuestBoss()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuestBoss
				wait(1.5)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuestBoss, LevelQuestBoss)
				wait(1)
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
			elseif game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
				for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
					if FramBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
						repeat
							pcall(function() wait() 
								if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
									local args = {
										[1] = "Buso"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end
								EquipWeapon(_G.SelectWeaponBoss)
								if HideHitBlox then
									v.HumanoidRootPart.Transparency = 0.75
								else
									v.HumanoidRootPart.Transparency = 1
								end
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
								game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
								game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
								VirtualUser:CaptureController()
								VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
							end)
						until not FramBoss or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
					end
				end
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
			end
		end
	end
end
tgls:Toggle("Auto Farm Boss",false,function(Value)
	local args = {
		[1] = "AbandonQuest"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	FramBoss = Value
	MsBoss = ""
	while FramBoss do wait()
		AutoFramBoss()
	end
end)
KillBossuse = true
function AutoFramAllBoss()
	for i, v in pairs(game.Workspace.Enemies:GetChildren()) do
		if KillBossuse then
			if v.Name == "Diamond [Lv. 750] [Boss]" then
				SelectBoss = "Diamond [Lv. 750] [Boss]"
			elseif v.Name == "Jeremy [Lv. 850] [Boss]" then
				SelectBoss = "Jeremy [Lv. 850] [Boss]"
			elseif v.Name == "Fajita [Lv. 925] [Boss]" then
				SelectBoss = "Fajita [Lv. 925] [Boss]"
			elseif v.Name == "Don Swan [Lv. 1000] [Boss]" and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TalkTrevor","1") == 0 then
				SelectBoss = "Don Swan [Lv. 1000] [Boss]" 
			elseif v.Name == "Smoke Admiral [Lv. 1150] [Boss]"  then
				SelectBoss = "Smoke Admiral [Lv. 1150] [Boss]"
			elseif v.Name == "Cursed Captain [Lv. 1325] [Raid Boss]"  then
				SelectBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
			elseif v.Name == "Awakened Ice Admiral [Lv. 1400] [Boss]" then
				SelectBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
			elseif v.Name == "Tide Keeper [Lv. 1475] [Boss]" then
				SelectBoss = "Tide Keeper [Lv. 1475] [Boss]"
			elseif v.Name == "Saber Expert [Lv. 200] [Boss]" then
				SelectBoss = "Saber Expert [Lv. 200] [Boss]"
			elseif v.Name == "The Gorilla King [Lv. 25] [Boss]"  then
				SelectBoss = "The Gorilla King [Lv. 25] [Boss]"
			elseif v.Name == "Bobby [Lv. 55] [Boss]" then
				SelectBoss = "Bobby [Lv. 55] [Boss]" 
			elseif v.Name == "Yeti [Lv. 110] [Boss]"  then
				SelectBoss = "Yeti [Lv. 110] [Boss]"
			elseif v.Name == "Mob Leader [Lv. 120] [Boss]" then
				SelectBoss = "Mob Leader [Lv. 120] [Boss]"
			elseif v.Name == "Vice Admiral [Lv. 130] [Boss]" then
				SelectBoss = "Vice Admiral [Lv. 130] [Boss]"
			elseif v.Name == "Warden [Lv. 175] [Boss]" then
				SelectBoss = "Warden [Lv. 175] [Boss]"
			elseif v.Name == "Chief Warden [Lv. 200] [Boss]"then
				SelectBoss = "Chief Warden [Lv. 200] [Boss]"
			elseif v.Name == "Swan [Lv. 225] [Boss]" then
				SelectBoss = "Swan [Lv. 225] [Boss]"
			elseif v.Name == "Magma Admiral [Lv. 350] [Boss]" then
				SelectBoss = "Magma Admiral [Lv. 350] [Boss]"
			elseif v.Name == "Fishman Lord [Lv. 425] [Boss]" then
				SelectBoss = "Fishman Lord [Lv. 425] [Boss]"
			elseif v.Name == "Wysper [Lv. 500] [Boss]" then
				SelectBoss = "Wysper [Lv. 500] [Boss]"
			elseif v.Name == "Thunder God [Lv. 575] [Boss]" then
				SelectBoss = "Thunder God [Lv. 575] [Boss]"
			elseif v.Name == "Cyborg [Lv. 675] [Boss]" then
				SelectBoss = "Cyborg [Lv. 675] [Boss]"
			elseif v.Name == "Kilo Admiral [Lv. 1750] [Boss]" then
				SelectBoss = "Kilo Admiral [Lv. 1750] [Boss]"
			elseif v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
				SelectBoss = "Captain Elephant [Lv. 1875] [Boss]"
			elseif v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" then
				SelectBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
			elseif v.Name == "Longma [Lv. 2000] [Boss]" then
				SelectBoss = "Longma [Lv. 2000] [Boss]"
			elseif v.Name == "Stone [Lv. 1550] [Boss]" then
				SelectBoss = "Stone [Lv. 1550] [Boss]"
			elseif v.Name == "Island Empress [Lv. 1675] [Boss]" then
				SelectBoss = "Island Empress [Lv. 1675] [Boss]"
			end
		end   
	end
	for i, v in pairs(game.ReplicatedStorage:GetChildren()) do
		if KillBossuse then
			if v.Name == "Diamond [Lv. 750] [Boss]" then
				SelectBoss = "Diamond [Lv. 750] [Boss]"
			elseif v.Name == "Jeremy [Lv. 850] [Boss]"then
				SelectBoss = "Jeremy [Lv. 850] [Boss]"
			elseif v.Name == "Fajita [Lv. 925] [Boss]"  then
				SelectBoss = "Fajita [Lv. 925] [Boss]"
			elseif v.Name == "Don Swan [Lv. 1000] [Boss]" and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TalkTrevor","1") == 0 then
				SelectBoss = "Don Swan [Lv. 1000] [Boss]" 
			elseif v.Name == "Smoke Admiral [Lv. 1150] [Boss]"  then
				SelectBoss = "Smoke Admiral [Lv. 1150] [Boss]"
			elseif v.Name == "Cursed Captain [Lv. 1325] [Raid Boss]"  then
				SelectBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
			elseif v.Name == "Awakened Ice Admiral [Lv. 1400] [Boss]"  then
				SelectBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
			elseif v.Name == "Tide Keeper [Lv. 1475] [Boss]"  then
				SelectBoss = "Tide Keeper [Lv. 1475] [Boss]"
			elseif v.Name == "Saber Expert [Lv. 200] [Boss]"then
				SelectBoss = "Saber Expert [Lv. 200] [Boss]"
			elseif v.Name == "The Gorilla King [Lv. 25] [Boss]" then
				SelectBoss = "The Gorilla King [Lv. 25] [Boss]"
			elseif v.Name == "Bobby [Lv. 55] [Boss]"  then
				SelectBoss = "Bobby [Lv. 55] [Boss]" 
			elseif v.Name == "Yeti [Lv. 110] [Boss]"   then
				SelectBoss = "Yeti [Lv. 110] [Boss]"
			elseif v.Name == "Mob Leader [Lv. 120] [Boss]" then
				SelectBoss = "Mob Leader [Lv. 120] [Boss]"
			elseif v.Name == "Vice Admiral [Lv. 130] [Boss]"  then
				SelectBoss = "Vice Admiral [Lv. 130] [Boss]"
			elseif v.Name == "Warden [Lv. 175] [Boss]" then
				SelectBoss = "Warden [Lv. 175] [Boss]"
			elseif v.Name == "Chief Warden [Lv. 200] [Boss]"  then
				SelectBoss = "Chief Warden [Lv. 200] [Boss]"
			elseif v.Name == "Swan [Lv. 225] [Boss]"  then
				SelectBoss = "Swan [Lv. 225] [Boss]"
			elseif v.Name == "Magma Admiral [Lv. 350] [Boss]"  then
				SelectBoss = "Magma Admiral [Lv. 350] [Boss]"
			elseif v.Name == "Fishman Lord [Lv. 425] [Boss]"  then
				SelectBoss = "Fishman Lord [Lv. 425] [Boss]"
			elseif v.Name == "Wysper [Lv. 500] [Boss]"   then
				SelectBoss = "Wysper [Lv. 500] [Boss]"
			elseif v.Name == "Thunder God [Lv. 575] [Boss]"   then
				SelectBoss = "Thunder God [Lv. 575] [Boss]"
			elseif v.Name == "Cyborg [Lv. 675] [Boss]" then
				SelectBoss = "Cyborg [Lv. 675] [Boss]"
			elseif v.Name == "Kilo Admiral [Lv. 1750] [Boss]" then
				SelectBoss = "Kilo Admiral [Lv. 1750] [Boss]"
			elseif v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
				SelectBoss = "Captain Elephant [Lv. 1875] [Boss]"
			elseif v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" then
				SelectBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
			elseif v.Name == "Longma [Lv. 2000] [Boss]" then
				SelectBoss = "Longma [Lv. 2000] [Boss]"
			elseif v.Name == "Stone [Lv. 1550] [Boss]" then
				SelectBoss = "Stone [Lv. 1550] [Boss]"
			elseif v.Name == "Island Empress [Lv. 1675] [Boss]" then
				SelectBoss = "Island Empress [Lv. 1675] [Boss]"
			end
		end   
	end
	KillBossuse = false
	if SelectBoss == "Don Swan [Lv. 1000] [Boss]" or SelectBoss == "Cursed Captain [Lv. 1325] [Raid Boss]" or SelectBoss == "Saber Expert [Lv. 200] [Boss]" or SelectBoss == "Mob Leader [Lv. 120] [Boss]" or SelectBoss == "Darkbeard [Lv. 1000] [Raid Boss]" then
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if FramAllBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
					CheckQuestBoss()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
					wait(1)
					repeat
						pcall(function() wait() 
							if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
								local args = {
									[1] = "Buso"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							EquipWeapon(_G.SelectWeaponBoss)
							if HideHitBlox then
								v.HumanoidRootPart.Transparency = 0.75
							else
								v.HumanoidRootPart.Transparency = 1
							end
							v.HumanoidRootPart.CanCollide = false
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
							game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
							VirtualUser:CaptureController()
							VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end)
					until not FramAllBoss or not v.Parent or v.Humanoid.Health <= 0
					KillBossuse = true
				end
			end
		else
			CheckQuestBoss()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
		end
	else
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if FramAllBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
					CheckQuestBoss()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
					wait(1)
					repeat
						pcall(function() wait() 
							if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
								local args = {
									[1] = "Buso"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							EquipWeapon(_G.SelectWeaponBoss)
							if HideHitBlox then
								v.HumanoidRootPart.Transparency = 0.75
							else
								v.HumanoidRootPart.Transparency = 1
							end
							v.HumanoidRootPart.CanCollide = false
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
							game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
							VirtualUser:CaptureController()
							VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end)
					until not FramAllBoss or not v.Parent or v.Humanoid.Health <= 0
					KillBossuse = true
				end
			end
		else
			CheckQuestBoss()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
		end
	end
	KillBossuse = true
end

function AutoFramAllBoss2()
	for i, v in pairs(game.Workspace.Enemies:GetChildren()) do
		if KillBossuse then
			if v.Name == "Diamond [Lv. 750] [Boss]" then
				SelectBoss = "Diamond [Lv. 750] [Boss]"
			elseif v.Name == "Jeremy [Lv. 850] [Boss]" then
				SelectBoss = "Jeremy [Lv. 850] [Boss]"
			elseif v.Name == "Fajita [Lv. 925] [Boss]" then
				SelectBoss = "Fajita [Lv. 925] [Boss]"
			elseif v.Name == "Don Swan [Lv. 1000] [Boss]" and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TalkTrevor","1") == 0 then
				SelectBoss = "Don Swan [Lv. 1000] [Boss]" 
			elseif v.Name == "Smoke Admiral [Lv. 1150] [Boss]"  then
				SelectBoss = "Smoke Admiral [Lv. 1150] [Boss]"
			elseif v.Name == "Cursed Captain [Lv. 1325] [Raid Boss]"  then
				SelectBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
			elseif v.Name == "Awakened Ice Admiral [Lv. 1400] [Boss]" then
				SelectBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
			elseif v.Name == "Tide Keeper [Lv. 1475] [Boss]" then
				SelectBoss = "Tide Keeper [Lv. 1475] [Boss]"
			elseif v.Name == "Saber Expert [Lv. 200] [Boss]" then
				SelectBoss = "Saber Expert [Lv. 200] [Boss]"
			elseif v.Name == "The Gorilla King [Lv. 25] [Boss]"  then
				SelectBoss = "The Gorilla King [Lv. 25] [Boss]"
			elseif v.Name == "Bobby [Lv. 55] [Boss]" then
				SelectBoss = "Bobby [Lv. 55] [Boss]" 
			elseif v.Name == "Yeti [Lv. 110] [Boss]"  then
				SelectBoss = "Yeti [Lv. 110] [Boss]"
			elseif v.Name == "Mob Leader [Lv. 120] [Boss]" then
				SelectBoss = "Mob Leader [Lv. 120] [Boss]"
			elseif v.Name == "Vice Admiral [Lv. 130] [Boss]" then
				SelectBoss = "Vice Admiral [Lv. 130] [Boss]"
			elseif v.Name == "Warden [Lv. 175] [Boss]" then
				SelectBoss = "Warden [Lv. 175] [Boss]"
			elseif v.Name == "Chief Warden [Lv. 200] [Boss]"then
				SelectBoss = "Chief Warden [Lv. 200] [Boss]"
			elseif v.Name == "Swan [Lv. 225] [Boss]" then
				SelectBoss = "Swan [Lv. 225] [Boss]"
			elseif v.Name == "Magma Admiral [Lv. 350] [Boss]" then
				SelectBoss = "Magma Admiral [Lv. 350] [Boss]"
			elseif v.Name == "Fishman Lord [Lv. 425] [Boss]" then
				SelectBoss = "Fishman Lord [Lv. 425] [Boss]"
			elseif v.Name == "Wysper [Lv. 500] [Boss]" then
				SelectBoss = "Wysper [Lv. 500] [Boss]"
			elseif v.Name == "Thunder God [Lv. 575] [Boss]" then
				SelectBoss = "Thunder God [Lv. 575] [Boss]"
			elseif v.Name == "Cyborg [Lv. 675] [Boss]" then
				SelectBoss = "Cyborg [Lv. 675] [Boss]"
			elseif v.Name == "Kilo Admiral [Lv. 1750] [Boss]" then
				SelectBoss = "Kilo Admiral [Lv. 1750] [Boss]"
			elseif v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
				SelectBoss = "Captain Elephant [Lv. 1875] [Boss]"
			elseif v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" then
				SelectBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
			elseif v.Name == "Longma [Lv. 2000] [Boss]" then
				SelectBoss = "Longma [Lv. 2000] [Boss]"
			elseif v.Name == "Stone [Lv. 1550] [Boss]" then
				SelectBoss = "Stone [Lv. 1550] [Boss]"
			elseif v.Name == "Island Empress [Lv. 1675] [Boss]" then
				SelectBoss = "Island Empress [Lv. 1675] [Boss]"
			end
		end   
	end
	for i, v in pairs(game.ReplicatedStorage:GetChildren()) do
		if KillBossuse then
			if v.Name == "Diamond [Lv. 750] [Boss]" then
				SelectBoss = "Diamond [Lv. 750] [Boss]"
			elseif v.Name == "Jeremy [Lv. 850] [Boss]"then
				SelectBoss = "Jeremy [Lv. 850] [Boss]"
			elseif v.Name == "Fajita [Lv. 925] [Boss]"  then
				SelectBoss = "Fajita [Lv. 925] [Boss]"
			elseif v.Name == "Don Swan [Lv. 1000] [Boss]" and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TalkTrevor","1") == 0 then
				SelectBoss = "Don Swan [Lv. 1000] [Boss]" 
			elseif v.Name == "Smoke Admiral [Lv. 1150] [Boss]"  then
				SelectBoss = "Smoke Admiral [Lv. 1150] [Boss]"
			elseif v.Name == "Cursed Captain [Lv. 1325] [Raid Boss]"  then
				SelectBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
			elseif v.Name == "Awakened Ice Admiral [Lv. 1400] [Boss]"  then
				SelectBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
			elseif v.Name == "Tide Keeper [Lv. 1475] [Boss]"  then
				SelectBoss = "Tide Keeper [Lv. 1475] [Boss]"
			elseif v.Name == "Saber Expert [Lv. 200] [Boss]"then
				SelectBoss = "Saber Expert [Lv. 200] [Boss]"
			elseif v.Name == "The Gorilla King [Lv. 25] [Boss]" then
				SelectBoss = "The Gorilla King [Lv. 25] [Boss]"
			elseif v.Name == "Bobby [Lv. 55] [Boss]"  then
				SelectBoss = "Bobby [Lv. 55] [Boss]" 
			elseif v.Name == "Yeti [Lv. 110] [Boss]"   then
				SelectBoss = "Yeti [Lv. 110] [Boss]"
			elseif v.Name == "Mob Leader [Lv. 120] [Boss]" then
				SelectBoss = "Mob Leader [Lv. 120] [Boss]"
			elseif v.Name == "Vice Admiral [Lv. 130] [Boss]"  then
				SelectBoss = "Vice Admiral [Lv. 130] [Boss]"
			elseif v.Name == "Warden [Lv. 175] [Boss]" then
				SelectBoss = "Warden [Lv. 175] [Boss]"
			elseif v.Name == "Chief Warden [Lv. 200] [Boss]"  then
				SelectBoss = "Chief Warden [Lv. 200] [Boss]"
			elseif v.Name == "Swan [Lv. 225] [Boss]"  then
				SelectBoss = "Swan [Lv. 225] [Boss]"
			elseif v.Name == "Magma Admiral [Lv. 350] [Boss]"  then
				SelectBoss = "Magma Admiral [Lv. 350] [Boss]"
			elseif v.Name == "Fishman Lord [Lv. 425] [Boss]"  then
				SelectBoss = "Fishman Lord [Lv. 425] [Boss]"
			elseif v.Name == "Wysper [Lv. 500] [Boss]"   then
				SelectBoss = "Wysper [Lv. 500] [Boss]"
			elseif v.Name == "Thunder God [Lv. 575] [Boss]"   then
				SelectBoss = "Thunder God [Lv. 575] [Boss]"
			elseif v.Name == "Cyborg [Lv. 675] [Boss]" then
				SelectBoss = "Cyborg [Lv. 675] [Boss]"
			elseif v.Name == "Kilo Admiral [Lv. 1750] [Boss]" then
				SelectBoss = "Kilo Admiral [Lv. 1750] [Boss]"
			elseif v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
				SelectBoss = "Captain Elephant [Lv. 1875] [Boss]"
			elseif v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" then
				SelectBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
			elseif v.Name == "Longma [Lv. 2000] [Boss]" then
				SelectBoss = "Longma [Lv. 2000] [Boss]"
			elseif v.Name == "Stone [Lv. 1550] [Boss]" then
				SelectBoss = "Stone [Lv. 1550] [Boss]"
			elseif v.Name == "Island Empress [Lv. 1675] [Boss]" then
				SelectBoss = "Island Empress [Lv. 1675] [Boss]"
			end
		end   
	end
	KillBossuse = false
	if SelectBoss == "Don Swan [Lv. 1000] [Boss]" or SelectBoss == "Cursed Captain [Lv. 1325] [Raid Boss]" or SelectBoss == "Saber Expert [Lv. 200] [Boss]" or SelectBoss == "Mob Leader [Lv. 120] [Boss]" or SelectBoss == "Darkbeard [Lv. 1000] [Raid Boss]" then
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if _G.AllBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
					CheckQuestBoss()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
					wait(1)
					repeat
						pcall(function() wait() 
							if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
								local args = {
									[1] = "Buso"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							EquipWeapon(_G.SelectWeaponBoss)
							if HideHitBlox then
								v.HumanoidRootPart.Transparency = 0.75
							else
								v.HumanoidRootPart.Transparency = 1
							end
							v.HumanoidRootPart.CanCollide = false
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
							game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
							VirtualUser:CaptureController()
							VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end)
					until not _G.AllBoss or not v.Parent or v.Humanoid.Health <= 0
					KillBossuse = true
				end
			end
		else
			CheckQuestBoss()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
		end
	else
		if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if _G.AllBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
					CheckQuestBoss()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
					wait(1)
					repeat
						pcall(function() wait() 
							if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
								local args = {
									[1] = "Buso"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							EquipWeapon(_G.SelectWeaponBoss)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 20, 0)
							game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
							VirtualUser:CaptureController()
							VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end)
					until not _G.AllBoss or not v.Parent or v.Humanoid.Health <= 0
					KillBossuse = true
				end
			end
		else
			CheckQuestBoss()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
		end
	end
	KillBossuse = true
end

game:GetService("RunService").Heartbeat:Connect(
function()
	if _G.AllBossNoHop or _G.AllBossHop then
		if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Humanoid") then
			game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end
end
)

tgls:Toggle("Auto Farm All Boss",_G.AllBossNoHop,function(Value)
	_G.FastBoss = Value
	_G.AllBossNoHop = Value
end)

tgls:Toggle("Auto Farm All Boss+Hop",_G.AllBossHop,function(Value)
	_G.FastBoss = Value
	_G.AllBossHop = Value
end)

---------------------------------
local RigC = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework) 
local VirtualUser = game:GetService('VirtualUser')
kkii = require(game.ReplicatedStorage.Util.CameraShaker)
spawn(function()
	game:GetService('RunService').Heartbeat:connect(function()
		if _G.FastBoss then
			pcall(function()
				pcall(function ()
					kkii:Stop()
				end)  
			end)
		end
	end)
end)
---------------------------------
spawn(function()
	game:GetService('RunService').Heartbeat:connect(function()
		if _G.FastBoss then
			pcall(function()
				pcall(function ()
					RigC.activeController.timeToNextAttack = 0
				end)  
			end)
		end
	end)
end)

spawn(function()
	game:GetService('RunService').Heartbeat:connect(function()
		if _G.FastBoss then
			pcall(function()
				pcall(function ()
					RigC.activeController.hitboxMagnitude = 25
					wait(.05)
				end)  
			end)
		end
	end)
end)

spawn(function()
	game:GetService('RunService').Heartbeat:connect(function()
		if _G.FastBoss then
			pcall(function()
				pcall(function ()

					RigC.activeController.increment = 3
				end)
			end)
		end
	end)
end)

spawn(function()
	game:GetService('RunService').Heartbeat:connect(function()
		if _G.FastBoss then
			pcall(function()
				pcall(function ()
					game:GetService'VirtualUser':CaptureController()
					game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
					wait(.05)
				end)
			end)
		end
	end)
end)
spawn(function()
	game:GetService('RunService').Heartbeat:connect(function()
		if _G.FastBoss then
			pcall(function()
				pcall(function ()
					game:GetService'VirtualUser':CaptureController()
					game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
					wait(.05)
				end)
			end)
		end
	end)
end)

---------------------------------

function Autoallbossnope()
	for i, v in pairs(game.ReplicatedStorage:GetChildren()) do
		if string.find(v.Name, "Boss") then
			if v.Name == "rip_indra True Form [Lv. 5000] [Raid Boss]" or v.Name == "Ice Admiral [Lv. 700] [Boss]" or v.Name == "Don Swan [Lv. 1000] [Boss]" or v.Name == "Longma [Lv. 2000] [Boss]" then
			else
				SelectBoss = v.Name
				CheckQuestBoss()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
				if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) or
					game:GetService("ReplicatedStorage"):FindFirstChild(SelectBoss) then
					CheckQuestBoss()
					if _G.AllBossNoHop and v:IsA("Model") and v:FindFirstChild("Humanoid") and
						v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
						repeat
							pcall(function()
								wait()
								game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
								if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
									local args = {
										[1] = "Buso"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end
								EquipWeapon(_G.SelectWeaponBoss)
								v.HumanoidRootPart.Transparency = 1
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
								game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 25, 0)
							end)
						until not _G.AllBossNoHop or not v.Parent or v.Humanoid.Health <= 0 
					end
				else
					CheckQuestBoss()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
				end
				CheckQuestBoss()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss

			end

		end
	end
end

function AutoallbossHope()
	for i, v in pairs(game.ReplicatedStorage:GetChildren()) do
		if string.find(v.Name, "Boss") then
			if v.Name == "rip_indra True Form [Lv. 5000] [Raid Boss]" or v.Name == "Ice Admiral [Lv. 700] [Boss]" or v.Name == "Don Swan [Lv. 1000] [Boss]" or v.Name == "Longma [Lv. 2000] [Boss]" then
			else
				SelectBoss = v.Name
				CheckQuestBoss()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
				if game:GetService("Workspace").Enemies:FindFirstChild(SelectBoss) or
					game:GetService("ReplicatedStorage"):FindFirstChild(SelectBoss) then
					CheckQuestBoss()
					if _G.AllBossHop and v:IsA("Model") and v:FindFirstChild("Humanoid") and
						v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == MsBoss then
						repeat
							pcall(function()
								wait()
								game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
								if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
									local args = {
										[1] = "Buso"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end
								EquipWeapon(_G.SelectWeaponBoss)
								v.HumanoidRootPart.Transparency = 1
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
								game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 25, 0)
								game:GetService 'VirtualUser':CaptureController()
								game:GetService 'VirtualUser':Button1Down(Vector2.new(1280, 672))                                   
							end)
						until not _G.AllBossHop or not v.Parent or v.Humanoid.Health <= 0 
					end
				else
					CheckQuestBoss()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
				end
				CheckQuestBoss()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss

			end

		end
	end
	if _G.AllBossHop and not game.ReplicatedStorage:FindFirstChild("Diamond [Lv. 750] [Boss]") and 
		not game.ReplicatedStorage:FindFirstChild("Jeremy [Lv. 850] [Boss]") and 
		not game.ReplicatedStorage:FindFirstChild("Fajita [Lv. 925] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Smoke Admiral [Lv. 1150] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Cursed Captain [Lv. 1325] [Raid Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Saber Expert [Lv. 200] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Bobby [Lv. 55] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Yeti [Lv. 110] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Mob Leader [Lv. 120] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Vice Admiral [Lv. 130] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Warden [Lv. 175] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Chief Warden [Lv. 200] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Swan [Lv. 225] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Magma Admiral [Lv. 350] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Fishman Lord [Lv. 425] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Wysper [Lv. 500] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Thunder God [Lv. 575] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Cyborg [Lv. 675] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Kilo Admiral [Lv. 1750] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") and
		not game.ReplicatedStorage:FindFirstChild("Stone [Lv. 1550] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Diamond [Lv. 750] [Boss]") and 
		not game:GetService("Workspace").Enemies:FindFirstChild("Jeremy [Lv. 850] [Boss]") and 
		not game:GetService("Workspace").Enemies:FindFirstChild("Fajita [Lv. 925] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Smoke Admiral [Lv. 1150] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Cursed Captain [Lv. 1325] [Raid Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Saber Expert [Lv. 200] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Bobby [Lv. 55] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Yeti [Lv. 110] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Mob Leader [Lv. 120] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Vice Admiral [Lv. 130] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Warden [Lv. 175] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Chief Warden [Lv. 200] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Swan [Lv. 225] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Magma Admiral [Lv. 350] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Fishman Lord [Lv. 425] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Wysper [Lv. 500] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Thunder God [Lv. 575] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Cyborg [Lv. 675] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Kilo Admiral [Lv. 1750] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") and
		not game:GetService("Workspace").Enemies:FindFirstChild("Stone [Lv. 1550] [Boss]") then
		Hopey()
	end
end

function Hopey()
	local PlaceID = game.PlaceId
	local AllIDs = {}
	local foundAnything = ""
	local actualHour = os.date("!*t").hour
	local Deleted = false
	function TPReturner()
		local Site;
		if foundAnything == "" then
			Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
		else
			Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
		end
		local ID = ""
		if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
			foundAnything = Site.nextPageCursor
		end
		local num = 0;
		for i,v in pairs(Site.data) do
			local Possible = true
			ID = tostring(v.id)
			if tonumber(v.maxPlayers) > tonumber(v.playing) then
				for _,Existing in pairs(AllIDs) do
					if num ~= 0 then
						if ID == tostring(Existing) then
							Possible = false
						end
					else
						if tonumber(actualHour) ~= tonumber(Existing) then
							local delFile = pcall(function()
								-- delfile("NotSameServers.json")
								AllIDs = {}
								table.insert(AllIDs, actualHour)
							end)
						end
					end
					num = num + 1
				end
				if Possible == true then
					table.insert(AllIDs, ID)
					wait()
					pcall(function()
						-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
						wait()
						game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
					end)
					wait(4)
				end
			end
		end
	end
	function Teleport() 
		while wait() do
			pcall(function()
				TPReturner()
				if foundAnything ~= "" then
					TPReturner()
				end
			end)
		end
	end
	Teleport()
end

spawn(function()
	while wait() do 
		if _G.AllBossNoHop then
			Autoallbossnope()
		end
	end
end)

spawn(function()
	while wait() do 
		if _G.AllBossHop then
			AutoallbossHope()
		end
	end
end)

--------------------- AutoBartilo
spawn(function()
	while wait() do
		pcall(function()
			if _G.AutoBartilo then
				if game.Players.LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 0 then
					if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Swan Pirates") and string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "50") and game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then 
						if game.Workspace.Enemies:FindFirstChild("Swan Pirate [Lv. 775]") then
							Ms = "Swan Pirate [Lv. 775]"
							for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
								for i,k in pairs(game.Workspace.Enemies:GetChildren()) do
									if v.Name == Ms then
										pcall(function()
											repeat wait()
												if sethiddenproperty then
													sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
												end
												if HideHitBlox then
													v.HumanoidRootPart.Transparency = 1
												else
													v.HumanoidRootPart.Transparency = 1
												end
												v.HumanoidRootPart.CanCollide = false
												v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
												v.HumanoidRootPart. CFrame = k.HumanoidRootPart.CFrame
												game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
												PosMonBarto =  v.HumanoidRootPart.CFrame
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
												AutoBartiloBring = true
											until not v.Parent or v.Humanoid.Health <= 0 or _G.AutoBartilo == false or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
											AutoBartiloBring = false
										end)
									end
								end
							end
						else
							CFramMon = CFrame.new(1057.92761, 137.614319, 1242.08069)
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFramMon
						end
					else
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-456.28952, 73.0200958, 299.895966)
						wait(1.1)
						local args = {
							[1] = "StartQuest",
							[2] = "BartiloQuest",
							[3] = 1
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					end 
				elseif game.Players.LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 1 then
					if game.Workspace.Enemies:FindFirstChild("Jeremy [Lv. 850] [Boss]") then
						Ms = "Jeremy [Lv. 850] [Boss]"
						for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
							if v.Name == Ms then
								repeat wait()
									if sethiddenproperty then

										sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
									end
									if HideHitBlox then
										v.HumanoidRootPart.Transparency = 1
									else
										v.HumanoidRootPart.Transparency = 1
									end
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
								until not v.Parent or v.Humanoid.Health <= 0 or _G.AutoBartilo == false
							end
						end
					elseif game.ReplicatedStorage:FindFirstChild("Jeremy [Lv. 850] [Boss]") then
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-456.28952, 73.0200958, 299.895966)
						wait(1.1)
						local args = {
							[1] = "BartiloQuestProgress",
							[2] = "Bartilo"
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
						wait(1)
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2099.88159, 448.931, 648.997375)
						wait(2)
					else
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2099.88159, 448.931, 648.997375)
					end
				elseif game.Players.LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 2 then
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1850.49329, 13.1789551, 1750.89685)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1858.87305, 19.3777466, 1712.01807)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1803.94324, 16.5789185, 1750.89685)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1858.55835, 16.8604317, 1724.79541)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1869.54224, 15.987854, 1681.00659)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1800.0979, 16.4978027, 1684.52368)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1819.26343, 14.795166, 1717.90625)
					wait(1)
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1813.51843, 14.8604736, 1724.79541)
				end
			end 
		end)
	end
end)



------------ AutoFramEctoplasm
spawn(function()
	while wait() do
		if _G.AutoFramEctoplasm then
			pcall(function()
				for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v.Name == "Ship Deckhand [Lv. 1250]" then
						repeat wait()
							v.HumanoidRootPart.Size = Vector3.new(50,50,50)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							BRING = v.HumanoidRootPart.CFrame
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
							if sethiddenproperty then
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							end
						until v.Humanoid.Health == 0 or not _G.AutoFramEctoplasm
					else
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1121.19312, 125.754921, 33019.2383, -0.823803723, 9.91749571e-10, 0.5668751, -4.56660265e-10, 1, -2.41313813e-09, -0.5668751, -2.24682162e-09, -0.823803723)
					end
				end
			end)
		end
	end
end)
spawn(function()
	while wait() do
		if _G.AutoFramEctoplasm then
			EquipWeapon(_G.SelectToolWeapon)
		end
	end
end)
spawn(function()
	while wait() do
		if _G.AutoFramEctoplasm then
			game:GetService'VirtualUser':Button1Down(Vector2.new(0.9,0.9))
			game:GetService'VirtualUser':Button1Up(Vector2.new(0.9,0.9))
		end
	end
end)

----------------  Auto Fram observhaki
tgls:Label("--Auto Fram observhaki--", true)
local ObservationVirtualUser = game:GetService('VirtualUser')
tgls:Toggle("Auto Fram Observation",false,function(a)
	_G.Observation = a
	if _G.Observation then
		ObservationVirtualUser:CaptureController()
		ObservationVirtualUser:SetKeyDown('0x65')
		wait(2)
		ObservationVirtualUser:SetKeyUp('0x65')
	end
	while _G.Observation do wait()
		if NewWorld then
			if game.Workspace.Enemies:FindFirstChild("Ship Engineer [Lv. 1275]") then
				if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
					repeat wait()
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Ship Engineer [Lv. 1275]").HumanoidRootPart.CFrame * CFrame.new(3,0,0)
					until _G.Observation == false or not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
				else
					repeat wait()
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Ship Engineer [Lv. 1275]").HumanoidRootPart.CFrame * CFrame.new(10,15,0)
					until _G.Observation == false or game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
				end
			else
				game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(918.558777, 40.0827065, 32766.498)
			end
		elseif OldWorld then
			if game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]") then
				if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
					repeat wait()
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.CFrame * CFrame.new(3,0,0)
					until _G.Observation == false or not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
				else
					repeat wait()
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.CFrame * CFrame.new(10,15,0)
					until _G.Observation == false or game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
				end
			else
				game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5533.29785, 88.1079102, 4852.3916)
			end
		end
	end
end)
spawn(function()
	while wait() do wait(40)
		pcall(function()
			if _G.Observation and not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
				ObservationVirtualUser:CaptureController()
				ObservationVirtualUser:SetKeyDown('0x65')
				wait(2)
				ObservationVirtualUser:SetKeyUp('0x65')
			end
		end)
	end
end)
tgls:Button("Check Observation Haki level","", function()
	CNPPaid:Notification("Notification","Observation Haki Level = "..game.Players.LocalPlayer.VisionRadius.Value, "Alright")
end)


--------------------- Auto Rengoku
if NewWorld then
	tgls:Label("-- Auto RenGoKu")
	RengokuWeapon = ""
	tgls:Toggle("Auto Rengoku",false,function(v)
		if OldWorld then
			CNPPaid:Notification("Notification","Use in New World","Okay")
		elseif RengokuWeapon == "" and v then
			CNPPaid:Notification("Notification","Select Wapon First","Okay")
		else
			_G.AutoRengoku = v
		end
	end)
end
spawn(function()
	pcall(function()
		while wait(.1) do
			if _G.AutoRengoku then
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Hidden Key") or  game.Players.LocalPlayer.Character:FindFirstChild("Hidden Key") then
					EquipWeapon("Hidden Key")
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(6571.1201171875, 299.23028564453, -6967.841796875)
				elseif game.Workspace.Enemies:FindFirstChild("Snow Lurker [Lv. 1375]") then
					for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
						if v.Name == "Snow Lurker [Lv. 1375]" and v.Humanoid.Health > 0 then
							repeat wait(.1)
								v.HumanoidRootPart.Size = Vector3.new(60,60,60)
								EquipWeapon(RengokuWeapon)
								function AutoHaki()
									if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
										local args = {
											[1] = "Buso"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
								end
								AutoHaki()
								if game.Workspace.Enemies:FindFirstChild("Snow Lurker [Lv. 1375]") then
									PosMonRengoku = v.HumanoidRootPart.CFrame
									game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 17, 0)
									game:GetService'VirtualUser':CaptureController()
									game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									RengokuMagnet = true
								else
									RengokuMagnet = false
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5525.7045898438, 262.90060424805, -6755.1186523438)
								end
							until game.Players.LocalPlayer.Backpack:FindFirstChild("Hidden Key") or _G.AutoRengoku == false or not v.Parent or v.Humanoid.Health <= 0
							RengokuMagnet = false
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5525.7045898438, 262.90060424805, -6755.1186523438)
						end
					end
				else
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5525.7045898438, 262.90060424805, -6755.1186523438)
				end
			end
		end
	end)
end)
local Rengoku = tgls:Dropdown("Select Weapon",Wapon,function(Value)
	RengokuWeapon = Value
end)
tgls:Button("Refresh Weapon",function()
	Rengoku:Clear()
	for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
		if v:IsA("Tool") then
			Rengoku:Add(v.Name)
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
		if v:IsA("Tool") then
			Rengoku:Add(v.Name)
		end
	end
end)
---------------- Auto Sharkman Katate
if NewWorld then
	tgls:Label("-- Auto Sharkman Katate -- ")
	tgls:Toggle("Auto Sharkman Katate",false,function(v)
		if OldWorld then
			CNPPaid:Notification("Notification","Use in New World","Okay")
		elseif SharkmanWeapon == "" and v then
			CNPPaid:Notification("Notification","Select Wapon First","Okay")
		else
			local args = {
				[1] = "BuyFishmanKarate"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			AutoSharkman = v
		end 
		while AutoSharkman do wait()
			if AutoSharkman then
				if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate"), "keys") then  
					if game.Players.LocalPlayer.Character:FindFirstChild("Water Key") or game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key") then
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2604.6958, 239.432526, -10315.1982, 0.0425701365, 0, -0.999093413, 0, 1, 0, 0.999093413, 0, 0.0425701365)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
					elseif game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 400 then
					else 
						Ms = "Tide Keeper [Lv. 1475] [Boss]"
						if game.Workspace.Enemies:FindFirstChild(Ms) then   
							for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
								if v.Name == Ms then    
									repeat wait()
										EquipWeapon(SharkmanWeapon)
										game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
										if setsimulationradius then 
											setsimulationradius(1e+1598, 1e+1599)
										end
										if HideHitBlox then
											v.HumanoidRootPart.Transparency = 1
										else
											v.HumanoidRootPart.Transparency = 0.75
										end
										v.HumanoidRootPart.CanCollide = false
										v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
										game:GetService'VirtualUser':CaptureController()
										game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
									until not v.Parent or v.Humanoid.Health <= 0 or AutoSharkman == false or game.Players.LocalPlayer.Character:FindFirstChild("Water Key") or game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key")
								end
							end
						else
							CFrameBoss = CFrame.new(-3570.18652, 123.328949, -11555.9072, 0.465199202, -1.3857326e-08, 0.885206044, 4.0332897e-09, 1, 1.35347511e-08, -0.885206044, -2.72606271e-09, 0.465199202)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameBoss
						end
					end
				else 
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
				end
			end
		end
	end)
	local Sharkman = tgls:Dropdown("Select Weapon",Wapon,function(Value)
		SharkmanWeapon = Value
	end)
	tgls:Button("Refresh Weapon",function()
		Sharkman:Clear()
		for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
			if v:IsA("Tool") then
				Sharkman:Add(v.Name)
			end
		end
		for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
			if v:IsA("Tool") then
				Sharkman:Add(v.Name)
			end
		end
	end)
end
-- ---------------------------------------------------------------------------------------------------------
function AutoDevilFruitMastery()
	if _G.FruitMastery then
		if LocalPlayer.PlayerGui.Main.Quest.Visible == false then
			StatrMagnetDevilFruitMastery = false
			CheckQuest()
			LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
			wait(1.1)
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
		elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
			CheckQuest()
			LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
			if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
				pcall(
					function()
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							CheckQuest()  
							if v.Name == Ms then
								repeat wait() CheckQuest()  
									if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
										if string.find(LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
											if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
												local args = {
													[1] = "Buso"
												}
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
											end
											HealthMin = v.Humanoid.MaxHealth*Persen/100
											PosMon = v.HumanoidRootPart.CFrame
											if v.Humanoid.Health <= HealthMin then
												UseDF = true
												EquipWeapon(game.Players.LocalPlayer.Data.DevilFruit.Value)
												v.HumanoidRootPart.CanCollide = false
												v.HumanoidRootPart.Size = Vector3.new(2, 2, 1)
												v.HumanoidRootPart.Transparency = 1
												if sethiddenproperty then
													sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
												end
												game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
												if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon-Dragon") then
													if SkillZ and v.Humanoid.Health <= HealthMin then
														local args = {
															[1] = v.HumanoidRootPart.Position
														}
														game:GetService("Players").LocalPlayer.Character["Dragon-Dragon"].RemoteEvent:FireServer(unpack(args))
														local args = {
															[1] = "Z",
															[2] = Vector3.new(0,0,0)
														}
														game:GetService("Players").LocalPlayer.Character["Dragon-Dragon"].RemoteFunction:InvokeServer(unpack(args))
													end
													if SkillX and v.Humanoid.Health <= HealthMin then
														local args = {
															[1] = v.HumanoidRootPart.Position
														}
														game:GetService("Players").LocalPlayer.Character["Dragon-Dragon"].RemoteEvent:FireServer(unpack(args))
														local args = {
															[1] = "X"
														}
														game:GetService("Players").LocalPlayer.Character["Dragon-Dragon"].RemoteFunction:InvokeServer(unpack(args))
													end   
												elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value) then
													if SkillZ and v.Humanoid.Health <= HealthMin then
														local args = {
															[1] = v.HumanoidRootPart.Position
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
														local args = {
															[1] = "Z",
															[2] = Vector3.new(0,0,0)
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteFunction:InvokeServer(unpack(args))
													end
													if SkillX and v.Humanoid.Health <= HealthMin then
														local args = {
															[1] = v.HumanoidRootPart.Position
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
														local args = {
															[1] = "X",
															[2] = Vector3.new(0,0,0)
														}

														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteFunction:InvokeServer(unpack(args))
													end
													if SkillC and v.Humanoid.Health <= HealthMin then
														local args = {
															[1] = v.HumanoidRootPart.Position
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
														local args = {
															[1] = "C",
															[2] = Vector3.new(0,0,0)
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteFunction:InvokeServer(unpack(args))
													end
													if SkillV and v.Humanoid.Health <= HealthMin then
														local args = {
															[1] = v.HumanoidRootPart.Position
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
														local args = {
															[1] = "V",
															[2] = Vector3.new(0,0,0)
														}
														game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Data.DevilFruit.Value].RemoteFunction:InvokeServer(unpack(args))
													end
												end   
											else
												UseDF = false
												EquipWeapon(WeaponMastery)
												if HideHitBlox then
													v.HumanoidRootPart.Transparency = 1
												else
													v.HumanoidRootPart.Transparency = 1
												end
												v.HumanoidRootPart.CanCollide = false
												v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
												game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))  
											end
											StatrMagnetDevilFruitMastery = true 
										else
											StatrMagnet = false
											CheckQuest()

											LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
											wait(1.5)
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
										end  
									else
										CheckQuest() 
										game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
									end 
								until not v.Parent or v.Humanoid.Health <= 0 or _G.FarmLevel == false or LocalPlayer.PlayerGui.Main.Quest.Visible == false
								StatrMagnetDevilFruitMastery = false
								CheckQuest() 
								game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
							end
						end
					end
				)
			else
				CheckQuest()
				game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
			end 
		end
	end
end
spawn(function()
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
function AutoGunMastery()
	if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then  
		CheckQuest()
		LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
		wait(1.1)
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NaemQuest, LevelQuest)
		wait(0.5)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
	elseif game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then  
		for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
			CheckQuest()
			pcall(function()
				if game.Workspace.Enemies:FindFirstChild(Ms) then
					if _G.GunMastery and v.Name == Ms then
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
						repeat wait()
							pcall(function()
								if game.Workspace.Enemies:FindFirstChild(Ms) then
									if string.find(LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
										HealthMin = v.Humanoid.MaxHealth*Persen/100
										PosMon = v.HumanoidRootPart.CFrame
										if v.Humanoid.Health <= HealthMin then
											EquipWeapon(SelectToolWeaponGun)
											v.HumanoidRootPart.CanCollide = false
											v.HumanoidRootPart.Size = Vector3.new(2, 2, 1)
											v.HumanoidRootPart.Transparency = 1
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
											local args = {
												[1] = v.HumanoidRootPart.Position,
												[2] = v.HumanoidRootPart
											}
											game:GetService("Players").LocalPlayer.Character[SelectToolWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
										else
											EquipWeapon(WeaponMastery)
											if HideHitBlox then
												v.HumanoidRootPart.Transparency = 1
											else
												v.HumanoidRootPart.Transparency = 1
											end
											v.HumanoidRootPart.CanCollide = false
											v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										end 
										StatrMagnet = true
									else
										CheckQuest()

										LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
										wait(1.1)

										wait(0.5)
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
									end
								else
									CheckQuest()
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
								end
							end)
						until game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or _G.GunMastery == false or v.Humanoid.Health <= 0 or not v.Parent or v.Humanoid.Health <= 0
					end
				else
					CheckQuest()
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
				end
			end)
		end
	end
end
tgls:Label("-- Auto Fram Mastery --")
game:GetService("RunService").Heartbeat:Connect(function()
	if _G.FruitMastery then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
	if _G.GunMastery then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)
WeaponMastery = ""
tgls:Toggle("Auto Fram Mastery  Fruit",false,function(v)
	if WeaponMastery == "" and v then
		CNPPaid:Notification("Notification","Select Wapon First","Okay")
	else
		CheckQuest()
		local args = {
			[1] = "AbandonQuest"
		}
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		_G.FruitMastery = v
		Ms = ""
	end	
	while _G.FruitMastery do wait()
		pcall(function()
			AutoDevilFruitMastery()
		end)
	end
end)
tgls:Toggle("Auto Fram Gun Mastery",false,function(v)
	if WeaponMastery == "" and v then
		CNPPaid:Notification("Notification","Select Wapon First","Okay")
	else 
		CheckQuest()

		_G.GunMastery = v
		Ms = ""
	end	
	while _G.GunMastery do wait()
		pcall(function()
			AutoGunMastery()
		end)
	end
end)
Persen = 15
tgls:Slider("Health %", 1, 100,Persen,function(v)
	Persen = v
end)
local AMS = tgls:Dropdown("Select Weapon",Wapon,function(v)
	WeaponMastery = v
	WeaponOldMastery = v
end)
tgls:Button("Refresh Weapon", function()
	AMS:Clear()
	for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
		if v:IsA("Tool") then
			AMS:Add(v.Name)
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
		if v:IsA("Tool") then
			AMS:Add(v.Name)
		end
	end
end)
-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet-- Magnet
spawn(function()
	while wait() do
		if _G.FarmLevel and StatrMagnet and Magnet then
			CheckQuest()
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if v.Name == Ms and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if v.Name == "Factory Staff [Lv. 800]" and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 200 then
						wait()
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
						v.HumanoidRootPart.CFrame = PosMon
					elseif v.Name == Ms and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 400 then
						wait()
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
						v.HumanoidRootPart.CFrame = PosMon
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
					end
				end
			end
		end 
		if _G.FruitMastery and StatrMagnetDevilFruitMastery and Magnet then
			for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
				CheckQuest()
				if v.Name == Ms and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if v.Name == "Factory Staff [Lv. 800]" and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 200 then
						wait()
						v.HumanoidRootPart.CanCollide = false
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						if UseDF then
							v.HumanoidRootPart.Size = Vector3.new(2, 2, 1)
						elseif UseDF == false then
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
						end   
						v.HumanoidRootPart.CFrame = PosMon
					elseif v.Name == Ms and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
						wait()
						v.HumanoidRootPart.CanCollide = false
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						if UseDF then
							v.HumanoidRootPart.Size = Vector3.new(2, 2, 1)
						elseif UseDF == false then
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
						end   
						v.HumanoidRootPart.CFrame = PosMon
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
					end
				end
			end
		end
		if _G.AutoBartilo and AutoBartiloBring and Magnet then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if v.Name == "Swan Pirate [Lv. 775]" and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if v.Name == "Swan Pirate [Lv. 775]" then
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
						v.HumanoidRootPart.CFrame = PosMonBarto
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
					end
				end
			end
		end
		if _G.AutoRengoku and RengokuMagnet and Magnet then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if v.Name ==  "Snow Lurker [Lv. 1375]" and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if v.Name == "Snow Lurker [Lv. 1375]" then
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 0.75
						end
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
						v.HumanoidRootPart.CFrame = PosMonRengoku
					end
				end
			end
		end
		if _G.AutoBartilo and AutoBartiloBring and Magnet then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if v.Name == "Swan Pirate [Lv. 775]" and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if v.Name == "Swan Pirate [Lv. 775]" then
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
						v.HumanoidRootPart.CFrame = PosMonBarto
						if sethiddenproperty then

							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
					end
				end
			end
		end
		if _G.AutoCitizen or CitizenMagnet or Magnet then
			for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
				if v.Name == "Forest Pirate [Lv. 1825]" and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if v.Name == "Forest Pirate [Lv. 1825]" and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 600 then
						if HideHit then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 0.8
						end
						v.Humanoid.WalkSpeed = 0
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
						v.HumanoidRootPart.CFrame = PosMonCitizen
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
					end
				end
			end
		end
		if _G.AutoFramEctoplasm and StatrMagnetEctoplasm and Magnet then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if v.Name == "Ship Deckhand [Lv. 1250]" and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
					if (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
						if HideHitBlox then
							v.HumanoidRootPart.Transparency = 1
						else
							v.HumanoidRootPart.Transparency = 1
						end
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
						v.HumanoidRootPart.CanCollide = false
						v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
						v.HumanoidRootPart.CFrame = BRING
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
					end
				end
			end
		end
	end
end)
-----------------------------------------------------------------------------------------------------------------
tgls:Label("--AutoBuyItem--")
tgls:Toggle("Auto Legendary Sword",false,function(Value)
	_G.LegebdarySword = Value    
end)
tgls:Toggle("Auto Legendary Sword + Hop",false,function(Value)
	_G.LegebdarySwordHop = Value    
end)
spawn(function()
	while wait(.1) do
		if _G.LegebdarySword then
			local args = {
				[1] = "LegendarySwordDealer",
				[2] = "1"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end 
	end
end)
spawn(function()
	while wait(.1) do
		if _G.LegebdarySword then
			local args = {
				[1] = "LegendarySwordDealer",
				[2] = "2"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end 
	end
end)
spawn(function()
	while wait(.1) do
		if _G.LegebdarySword then
			local args = {
				[1] = "LegendarySwordDealer",
				[2] = "3"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end 
	end
end)
spawn(function()
	while wait() do
		if _G.LegebdarySwordHop then
			local args = {
				[1] = "LegendarySwordDealer",
				[2] = "1"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			--
			local args = {
				[1] = "LegendarySwordDealer",
				[2] = "2"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			--
			local args = {
				[1] = "LegendarySwordDealer",
				[2] = "3"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			wait(20)
			local PlaceID = game.PlaceId
			local AllIDs = {}
			local foundAnything = ""
			local actualHour = os.date("!*t").hour
			local Deleted = false
			function TPReturner()
				local Site;
				if foundAnything == "" then
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
				else
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
				end
				local ID = ""
				if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
					foundAnything = Site.nextPageCursor
				end
				local num = 0;
				for i,v in pairs(Site.data) do
					local Possible = true
					ID = tostring(v.id)
					if tonumber(v.maxPlayers) > tonumber(v.playing) then
						for _,Existing in pairs(AllIDs) do
							if num ~= 0 then
								if ID == tostring(Existing) then
									Possible = false
								end
							else
								if tonumber(actualHour) ~= tonumber(Existing) then
									local delFile = pcall(function()
										-- delfile("NotSameServers.json")
										AllIDs = {}
										table.insert(AllIDs, actualHour)
									end)
								end
							end
							num = num + 1
						end
						if Possible == true then
							table.insert(AllIDs, ID)
							wait()
							pcall(function()
								-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
								wait()
								game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
							end)
							wait(.1)
						end
					end
				end
			end
			function Teleport() 
				while wait() do
					pcall(function()
						TPReturner()
						if foundAnything ~= "" then
							TPReturner()
						end
					end)
				end
			end
			Teleport()
		end
	end
end)
tgls:Toggle("Auto Haki Color",false,function(Value)
	_G.Enhancement = Value    
end)
spawn(function()
	while wait(.1) do
		if _G.Enhancement then
			local args = {
				[1] = "ColorsDealer",
				[2] = "2"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end 
	end
end)
tgls:Toggle("Auto Haki Color + Hop",false,function(Value)
	_G.EnhancementHop = Value    
end)
spawn(function()
	while wait(.1) do
		if _G.EnhancementHop then
			local args = {
				[1] = "ColorsDealer",
				[2] = "2"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			wait(20)
			local PlaceID = game.PlaceId
			local AllIDs = {}
			local foundAnything = ""
			local actualHour = os.date("!*t").hour
			local Deleted = false
			function TPReturner()
				local Site;
				if foundAnything == "" then
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
				else
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
				end
				local ID = ""
				if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
					foundAnything = Site.nextPageCursor
				end
				local num = 0;
				for i,v in pairs(Site.data) do
					local Possible = true
					ID = tostring(v.id)
					if tonumber(v.maxPlayers) > tonumber(v.playing) then
						for _,Existing in pairs(AllIDs) do
							if num ~= 0 then
								if ID == tostring(Existing) then
									Possible = false
								end
							else
								if tonumber(actualHour) ~= tonumber(Existing) then
									local delFile = pcall(function()
										-- delfile("NotSameServers.json")
										AllIDs = {}
										table.insert(AllIDs, actualHour)
									end)
								end
							end
							num = num + 1
						end
						if Possible == true then
							table.insert(AllIDs, ID)
							wait()
							pcall(function()
								-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
								wait()
								game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
							end)
							wait(.1)
						end
					end
				end
			end
			function Teleport() 
				while wait() do
					pcall(function()
						TPReturner()
						if foundAnything ~= "" then
							TPReturner()
						end
					end)
				end
			end
			Teleport()
		end 
	end
end)
local args = {
	[1] = "getInventoryWeapons"
}
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
for i,v in pairs(game.Players.LocalPlayer.PlayerGui.Main.Inventory.Container:GetDescendants()) do
	if v.Name == "Ghoul Mask" then
		AssGhoulMask = true
	end
	if v.Name == "Midnight Blade" then
		AssMidnightBlade = true
	end
	if v.Name == "Bizarre Rifle" then
		AssBizarreRifle = true
	end
end
tgls:Toggle("Auto Buy Bizarre Rifle",false,function(A)
	if NewWorld then
		AutoBuyBizarreRifle = A
		while AutoBuyBizarreRifle do wait()
			if AssBizarreRifle then
			else
				local args = {
					[1] = "Ectoplasm",
					[2] = "Buy",
					[3] = 1
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end
		end
	end
end)
tgls:Toggle("Auto Buy Ghoul Mask",false,function(A)
	if NewWorld then
		AutoBuyGhoulMask = A
		while AutoBuyGhoulMask do wait()
			if AssGhoulMask then

			else
				local args = {
					[1] = "Ectoplasm",
					[2] = "Buy",
					[3] = 2
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end
		end
	end
end)
tgls:Toggle("Auto Buy Midnight Blade",false,function(A)
	if NewWorld then
		AutoBuyMidnightBlade = A
		while AutoBuyMidnightBlade do wait()
			if AssMidnightBlade then

			else
				local args = {
					[1] = "Ectoplasm",
					[2] = "Buy",
					[3] = 3
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end
		end
	end
end)
local Stats =  window:Tap("Stats",6031094670)
local Point = Stats:Label("")
Stats:Toggle("Melee",false,function(Value)
	_G.Meleebf = Value    
end)
Stats:Toggle("Defense",false,function(value)
	_G.Defensebf = value
end)
Stats:Toggle("Sword",false,function(value)
	_G.Swordbf = value
end)
Stats:Toggle("Gun",false,function(value)
	_G.Gunbf = value
end)
Stats:Toggle("Devil Fruit",false,function(value)
	_G.Fruitbf = value
end)
Stats:Toggle("Max Point",false,function(value)
	_G.MaxPoint = value
end)

PointStats = 1
Stats:Slider("Point", 1, 100,PointStats,function(a)
	PointStats = a
end)

local Meleel = Stats:Label("")-- nil
local Defensel = Stats:Label("")-- nil
local swordl = Stats:Label("")-- nil
local gunl = Stats:Label("")-- nil
local demonfruitl = Stats:Label("") -- nil

---  variable
Point:change("Points Stats : "..game:GetService("Players")["LocalPlayer"].Data.Points.Value)
Meleel:change("Melee Points : "..game.Players.LocalPlayer.Data.Stats.Melee.Level.Value)
Defensel:change("Defense Points : "..game.Players.LocalPlayer.Data.Stats.Defense.Level.Value)
swordl:change("Sword Points : "..game.Players.LocalPlayer.Data.Stats.Sword.Level.Value)
gunl:change("Gun Points : "..game:GetService("Players").LocalPlayer.Data.Stats.Gun.Level.Value)
demonfruitl:change("Df Points : "..game.Players.LocalPlayer.Data.Stats["Demon Fruit"].Level.Value)


--- Loop
spawn(function()
	while wait(1) do 
		Point:change("Points Stats : "..game:GetService("Players")["LocalPlayer"].Data.Points.Value)
		Meleel:change("Melee Points : "..game.Players.LocalPlayer.Data.Stats.Melee.Level.Value)
		Defensel:change("Defense Points : "..game.Players.LocalPlayer.Data.Stats.Defense.Level.Value)
		swordl:change("Sword Points : "..game.Players.LocalPlayer.Data.Stats.Sword.Level.Value)
		gunl:change("Gun Points : "..game:GetService("Players").LocalPlayer.Data.Stats.Gun.Level.Value)
		demonfruitl:change("DevilFruit Points : "..game.Players.LocalPlayer.Data.Stats["Demon Fruit"].Level.Value)
	end
end)

spawn(function()
	while wait(.1) do
		if _G.MaxPoint then
			pcall(function()
				PointStats = game:GetService("Players").LocalPlayer.Data.Points.Value
			end)
		end
	end
end)

spawn(function()
	while wait(.1) do
		if _G.Meleebf then
			pcall(function()
				local args = {
					[1] = "AddPoint",
					[2] = "Melee",
					[3] = PointStats
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
spawn(function()
	while wait(.1) do
		if _G.Defensebf then
			pcall(function()
				local args = {
					[1] = "AddPoint",
					[2] = "Defense",
					[3] = PointStats
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
spawn(function()
	while wait(.1) do
		if _G.Gunbf then
			pcall(function()
				local args = {
					[1] = "AddPoint",
					[2] = "Gun",
					[3] = PointStats
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
spawn(function()
	while wait(.1) do
		if _G.Swordbf then
			pcall(function()
				local args = {
					[1] = "AddPoint",
					[2] = "Sword",
					[3] = PointStats
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
spawn(function()
	while wait(.1) do
		if _G.Fruitbf then
			pcall(function()
				local args = {
					[1] = "AddPoint",
					[2] = "Demon Fruit",
					[3] = PointStats
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
local Players = window:Tap("Players",6031094670)
PlayerName = {}
for i,v in pairs(game.Players:GetChildren()) do  
	table.insert(PlayerName ,v.Name)
end
local Player = Players:Dropdown("Selected Player",PlayerName,function(plys) --true/false, replaces the current title "Dropdown" with the option that t
	SelectedKillPlayer = plys
	SelectedPly:Refresh("Selected Player : "..SelectedKillPlayer)
end)
Players:Button("Refrsh Player",function()
	PlayerName = {}
	Player:Clear()
	for i,v in pairs(game.Players:GetChildren()) do  
		Player:Add(v.Name)
	end
end)
Wapon = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
	if v:IsA("Tool") then
		table.insert(Wapon ,v.Name)
	end
end
local HEE = Players:Dropdown("Select Weapon",Wapon,function(Value)
	_G.Select_Wapon_Bouty = Value
end)
Players:Button("Refresh Weapon", function()
	HEE:Clear()
	Wapon = {}
	for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
		if v:IsA("Tool") then
			HEE:Add(v.Name)
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
		if v:IsA("Tool") then
			HEE:Add(v.Name)
		end
	end
end)

-----function
function Hop()
	local PlaceID = game.PlaceId
	local AllIDs = {}
	local foundAnything = ""
	local actualHour = os.date("!*t").hour
	local Deleted = false
	function TPReturner()
		local Site;
		if foundAnything == "" then
			Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
		else
			Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
		end
		local ID = ""
		if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
			foundAnything = Site.nextPageCursor
		end
		local num = 0;
		for i,v in pairs(Site.data) do
			local Possible = true
			ID = tostring(v.id)
			if tonumber(v.maxPlayers) > tonumber(v.playing) then
				for _,Existing in pairs(AllIDs) do
					if num ~= 0 then
						if ID == tostring(Existing) then
							Possible = false
						end
					else
						if tonumber(actualHour) ~= tonumber(Existing) then
							local delFile = pcall(function()
								-- delfile("NotSameServers.json")
								AllIDs = {}
								table.insert(AllIDs, actualHour)
							end)
						end
					end
					num = num + 1
				end
				if Possible == true then
					table.insert(AllIDs, ID)
					wait()
					pcall(function()
						-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
						wait()
						game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
					end)
					wait(.1)
				end
			end
		end
	end
	function Teleport() 
		while wait() do
			pcall(function()
				TPReturner()
				if foundAnything ~= "" then
					TPReturner()
				end
			end)
		end
	end
	Teleport()
end
----



game:GetService("RunService").Heartbeat:Connect(
function()
	if _G.KillPlayer then
		game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)
Players:Toggle("Fast Attack 2", false,function(vu)
	_G.a = vu
end)
Players:Toggle("Kill Player + Hop", false,function(vu)
	_G.Bounty_Farm_Hop = vu
end)
Players:Toggle("Kill Player",false,function(bool)
	_G.KillPlayer = bool
	if _G.KillPlayer == false then
		game.Players:FindFirstChild(SelectedKillPlayer).Character.HumanoidRootPart.Size = Vector3.new(2, 2, 1)
	end
	while _G.KillPlayer do wait()
		repeat wait()
			EquipWeapon(_G.Select_Wapon_Bouty)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(SelectedKillPlayer).Character.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
			game.Players:FindFirstChild(SelectedKillPlayer).Character.HumanoidRootPart.Size = Vector3.new(60,60,60)
			game:GetService'VirtualUser':CaptureController()
			game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
		until not _G.KillPlayer or game.Players:FindFirstChild(SelectedKillPlayer).Character.Humanoid.Health == 0
		if NewWorld then
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
		end
		if NewWorld2 then
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
		end
		_G.KillPlayer = false
		_G.a = false
	end
end)

for i,v in pairs(game.Workspace:GetDescendants()) do
	if v.Name == "Lava" then   
		v:Destroy()
	end
end
for i,v in pairs(game.ReplicatedStorage:GetDescendants()) do
	if v.Name == "Lava" then   
		v:Destroy()
	end
end

Players:Toggle("Auto Farm Bounty (Gun Only)",false,function(value)
	_G.Bounty = value
end)

Players:Toggle("Kill Players No Spawn + Hop ( Gun )",false,function(t)
	_G.KillAndHop = t
end)




_G.Hop = false
spawn(function()
	while wait() do
		if _G.Bounty then
			pcall(function()
				wait(80)
				print("Hop la i sus")
				_G.Hop = true
			end)
		end
	end
end)

spawn(function()
	while wait(10) do
		pcall(function()
			if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.InCombat.Visible == false then
				wait(2)
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.InCombat.Visible == false then
					_G.Change = true
				end
			end
		end)
	end
end)

spawn(function()
	while wait(10) do
		pcall(function()
			if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.SafeZone.Visible == true then
				wait(2)
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.SafeZone.Visible == true then
					_G.Change = true
				end
			end
		end)
	end
end)

spawn(function()
	while wait(.1) do
		for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
			if v:IsA("Tool") then
				if v:FindFirstChild("RemoteFunctionShoot") then 
					_G.SelectToolWeaponGun = v.Name
				end
			end
		end
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.Bounty then
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == true then
					local args = {
						[1] = "EnablePvp"
					}

					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
			end
		end)
	end
end)

function EquipWeapon(ToolSe)
	if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
		local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
		wait()
		game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end
end

spawn(function()
	while wait() do
		if _G.Hop == true then
			pcall(function()
				_G.Bounty = false
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.InCombat.Visible == false then
					local PlaceID = game.PlaceId
					local AllIDs = {}
					local foundAnything = ""
					local actualHour = os.date("!*t").hour
					local Deleted = false
					function TPReturner()
						local Site;
						if foundAnything == "" then
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
						else
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
						end
						local ID = ""
						if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
							foundAnything = Site.nextPageCursor
						end
						local num = 0;
						for i,v in pairs(Site.data) do
							local Possible = true
							ID = tostring(v.id)
							if tonumber(v.maxPlayers) > tonumber(v.playing) then
								for _,Existing in pairs(AllIDs) do
									if num ~= 0 then
										if ID == tostring(Existing) then
											Possible = false
										end
									else
										if tonumber(actualHour) ~= tonumber(Existing) then
											local delFile = pcall(function()
												-- delfile("NotSameServers.json")
												AllIDs = {}
												table.insert(AllIDs, actualHour)
											end)
										end
									end
									num = num + 1
								end
								if Possible == true then
									table.insert(AllIDs, ID)
									wait()
									pcall(function()
										-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
										wait()
										game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
									end)
									wait(2)
								end
							end
						end
					end
					function Teleport()
						while wait() do
							pcall(function()
								TPReturner()
								if foundAnything ~= "" then
									TPReturner()
								end
							end)
						end
					end
					Teleport()
				end
			end)
		end
	end
end)
_G.Chennge = false

spawn(function ()
	while wait() do
		pcall(function()
			if _G.Bounty then
				if game:GetService("Players").localPlayer.PlayerGui.Notifications.NotificationTemplate then
					if game:GetService("Players").localPlayer.PlayerGui.Notifications.NotificationTemplate.Text:find("Cannot") or game:GetService("Players").Sixtiesgod.PlayerGui.Notifications.NotificationTemplate.Text:find("can't") then
						_G.Change = true
						for i, v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
							v:Destroy()
						end
					end
				end
			end
		end)	
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.Bounty then
				if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
					local args = {
						[1] = "Buso"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.Bounty then
				game:GetService'VirtualUser':Button1Down(Vector2.new(0.9,0.9))
				game:GetService'VirtualUser':Button1Up(Vector2.new(0.9,0.9))
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.Bounty then
				for i, v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
					if game:GetService("Players")[v.Name].Data.Level.Value >= 1200 and v.Name ~= game.Players.LocalPlayer.Name and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") then
						if game.Players.LocalPlayer.Character.Humanoid.Health > game.Players.LocalPlayer.Character.Humanoid.MaxHealth*35/100 then
							repeat wait()
								spawn(function()
									EquipWeapon(_G.SelectToolWeaponGun)
								end)
								NameRandom = v.Name
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50,50,50)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,-10,1)
							until _G.Bounty == false or v.Humanoid.Health == 0 or not v:FindFirstChild("HumanoidRootPart") or not v:FindFirstChild("Humanoid") or not v.Parent or _G.Change == true
							_G.Change = false
						else
							repeat wait()
								game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-390.096313, 331.886475, 673.464966)
								wait()
								game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2302.19019, 15.1778421, 663.811035)
								wait()
								game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2372.14697, 72.9919434, -3166.51416)
								wait()
								game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-385.250916, 73.0458984, 297.388397)
								wait()
								game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(430.42569, 210.019623, -432.504791)
								wait()
								game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-260.358917, 49325.7031, -35259.3008)
								wait()
							until _G.Bounty == false or game.Players.LocalPlayer.Character.Humanoid.Health >= game.Players.LocalPlayer.Character.Humanoid.MaxHealth
						end
					end
				end
			elseif _G.Hop == true then
				repeat wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-390.096313, 331.886475, 673.464966)
					wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2302.19019, 15.1778421, 663.811035)
					wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2372.14697, 72.9919434, -3166.51416)
					wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-385.250916, 73.0458984, 297.388397)
					wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(430.42569, 210.019623, -432.504791)
					wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-260.358917, 49325.7031, -35259.3008)
					wait()
				until _G.Bounty == false or _G.Hop == false
			end
		end)
	end
end)

spawn(function ()
	while wait(6) do
		pcall(function()
			if _G.Bounty then
				for i, v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
					if v.Name == NameRandom and v.Humanoid.Health == v.Humanoid.MaxHealth then
						_G.Change = true
					end
				end
			end
		end)	
	end
end)

local lp = game:GetService('Players').LocalPlayer
local mouse = lp:GetMouse()
mouse.Button1Down:Connect(function()
	if _G.Bounty and game.Players.LocalPlayer.Character:FindFirstChild(SelectToolWeaponGun).RemoteFunctionShoot then
		local args = {
			[1] = game:GetService("Players"):FindFirstChild(NameRandom).Character.HumanoidRootPart.Position,
			[2] = game:GetService("Players"):FindFirstChild(NameRandom).Character.HumanoidRootPart
		}
		game:GetService("Players").LocalPlayer.Character[SelectToolWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
	end 
end)

spawn(function()
	game:GetService('RunService').Stepped:connect(function()
		if _G.Bounty == true or _G.Hop == true then
			game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end)
end)

------ Kill No Spawn
function EquipWeapon(Tools)
	if game.Players.LocalPlayer.Backpack:FindFirstChild(Tools) then
		local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(Tools)
		wait()
		game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end
end

spawn(function()
	while wait() do
		for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
			if v:IsA("Tool") then
				if v:FindFirstChild("RemoteFunctionShoot") then 
					_G.WeaponUseKillGun = v.Name
				end
			end
		end
	end
end)

spawn(function()
	game:GetService('RunService').Stepped:connect(function()
		if _G.KillAndHop == true or _G.HopServerOn == true then
			game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end)
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.KillAndHop then
				wait(80)
				_G.HopServerOn = true
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.KillAndHop then
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == true then
					local args = {
						[1] = "EnablePvp"
					}

					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.KillAndHop then
				if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
					local args = {
						[1] = "Buso"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.KillAndHop then
				game:GetService'VirtualUser':CaptureController()
				game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
			end
		end)
	end
end)

spawn(function()
	while wait() do
		if _G.KillAndHop then
			if game.PlaceId == 2753915549 then
				game.Players.LocalPlayer:Kick("Not Support First Sea")
				break
			end
		end
	end
end)

if game.CoreGui:FindFirstChild("Ui Bounty") then
	game.CoreGui:FindFirstChild("Ui Bounty"):Destroy()
end
local ScreenGuiEz = Instance.new("ScreenGui")
local TextLabelsss = Instance.new("TextLabel")
local UIGradientsssss = Instance.new("UIGradient")

ScreenGuiEz.Parent = game.CoreGui
ScreenGuiEz.Name = "Ui Bounty"
ScreenGuiEz.Enabled = true
ScreenGuiEz.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

TextLabelsss.Parent = ScreenGuiEz
TextLabelsss.Active = true
TextLabelsss.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabelsss.BackgroundTransparency = 1.000
TextLabelsss.BorderColor3 = Color3.fromRGB(255, 255, 255)
TextLabelsss.Position = UDim2.new(0.424812019, 0, 0.1, 0) -- 
TextLabelsss.Size = UDim2.new(0, 200, 0, 50)
TextLabelsss.Font = Enum.Font.GothamBold
TextLabelsss.Text = ""
TextLabelsss.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabelsss.TextSize = 25.000
TextLabelsss.TextTransparency = 1
TextLabelsss.TextStrokeTransparency = 300.000

UIGradientsssss.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(245, 20, 65)), ColorSequenceKeypoint.new(0.50, Color3.fromRGB(245, 121, 20)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(245, 39, 20))}
UIGradientsssss.Parent = TextLabelsss

spawn(function()
	while wait() do
		if game.Players.LocalPlayer.Team ~= nil then
			_G.OldBounty = game:GetService("Players")["LocalPlayer"].leaderstats:FindFirstChild("Bounty/Honor").Value
			break
		end
	end
end)

local function UpdateTime()
	local GetBounty = game:GetService("Players")["LocalPlayer"].leaderstats:FindFirstChild("Bounty/Honor").Value - tonumber(_G.OldBounty)
	TextLabelsss.Text = ("Now You Get Bounty : "..GetBounty)
end

spawn(function()
	while true do
		pcall(function()
			if _G.KillAndHop then
				UpdateTime()
				TextLabelsss.TextTransparency = 0
			end
		end)
		wait()
	end
end)

_G.GodModeOn = false
spawn(function()
	while wait() do
		if _G.KillAndHop then
			wait(.1)
			game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-260.358917, 49325.7031, -35259.3008)
			wait(1)
			local player = game.Players.LocalPlayer
			if player.Character then
				if player.Character:FindFirstChild("Humanoid") then
					player.Character.Humanoid.Name = "1"
				end
				local l = player.Character["1"]:Clone()
				l.Parent = player.Character
				l.Name = "Humanoid"; wait(0.1)
				player.Character["1"]:Destroy()
				workspace.CurrentCamera.CameraSubject = player.Character.Humanoid
				player.Character.Animate.Disabled = true; wait(0.1)
				player.Character.Animate.Disabled = false
			end
			print("GodMode : on")
			_G.GodModeOn = true
			_G.Aimbot = true
			_G.HideCrew = true
			print("all function : on")
			break
		end
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if _G.KillAndHop then
				for i, v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
					if game:GetService("Players")[v.Name].Data.Level.Value >= 1200 and v.Name ~= game.Players.LocalPlayer.Name and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") then
						if game.Players.LocalPlayer.Backpack:FindFirstChild(_G.WeaponUseKillGun) or game.Players.LocalPlayer.Character:FindFirstChild(_G.WeaponUseKillGun) then
							repeat wait()
								if _G.GodModeOn then
									spawn(function()
										wait(.2)
										EquipWeapon(_G.WeaponUseKillGun)
									end)
									NameKill = v.Name
									KillHealt = v.Humanoid.Health
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Size = Vector3.new(50,50,50)
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,55,1)
								end
							until not v.Parent or not v:FindFirstChild("Humanoid") or not v:FindFirstChild("HumanoidRootPart") or _G.KillAndHop == false or v.Humanoid.Health == 0 or NextPlayer == true or _G.HopServerOn == true or (not game.Players.LocalPlayer.Backpack:FindFirstChild(_G.WeaponUseKillGun) and not game.Players.LocalPlayer.Character:FindFirstChild(_G.WeaponUseKillGun))
							NextPlayer = false
						else
							if not game.Players.LocalPlayer.Backpack:FindFirstChild(_G.WeaponUseKillGun) and not game.Players.LocalPlayer.Character:FindFirstChild(_G.WeaponUseKillGun) then
								if game.PlaceId == 4442272183 then
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(124.16289520264, 25.941701889038, 2853.5454101563)
								end
								if game.PlaceId == 7449423635 then
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-216.48155212402, 12.3963174819946, 5325.3149414063)
								end
								wait(.3)
								local args = {
									[1] = "StoreItem",
									[2] = tostring(_G.WeaponUseKillGun)
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								wait(1)
								local args = {
									[1] = "LoadItem",
									[2] = tostring(_G.WeaponUseKillGun)
								}

								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								wait()
							end
						end
					end
				end
			elseif _G.HopServerOn == true then
				repeat wait()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-390.096313, 331.886475, 673.464966)
				until _G.KillAndHop == false or _G.HopServerOn == false
			end
		end)
	end
end)

local mousee = game:GetService('Players').LocalPlayer:GetMouse()
mousee.Button1Down:Connect(function()
	if _G.KillAndHop and game.Players.LocalPlayer.Character:FindFirstChild(_G.WeaponUseKillGun).RemoteFunctionShoot then
		local args = {
			[1] = game:GetService("Players"):FindFirstChild(NameKill).Character.HumanoidRootPart.Position,
			[2] = game:GetService("Players"):FindFirstChild(NameKill).Character.HumanoidRootPart
		}
		game:GetService("Players").LocalPlayer.Character[_G.WeaponUseKillGun].RemoteFunctionShoot:InvokeServer(unpack(args))
	end 
end)


spawn(function()
	while wait(15) do
		if _G.HopServerOn == true then
			pcall(function()
				_G.KillAndHop = false
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.InCombat.Visible == false then
					local PlaceID = game.PlaceId
					local AllIDs = {}
					local foundAnything = ""
					local actualHour = os.date("!*t").hour
					local Deleted = false
					function TPReturner()
						local Site;
						if foundAnything == "" then
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
						else
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
						end
						local ID = ""
						if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
							foundAnything = Site.nextPageCursor
						end
						local num = 0;
						for i,v in pairs(Site.data) do
							local Possible = true
							ID = tostring(v.id)
							if tonumber(v.maxPlayers) > tonumber(v.playing) then
								for _,Existing in pairs(AllIDs) do
									if num ~= 0 then
										if ID == tostring(Existing) then
											Possible = false
										end
									else
										if tonumber(actualHour) ~= tonumber(Existing) then
											local delFile = pcall(function()
												-- delfile("NotSameServers.json")
												AllIDs = {}
												table.insert(AllIDs, actualHour)
											end)
										end
									end
									num = num + 1
								end
								if Possible == true then
									table.insert(AllIDs, ID)
									wait()
									pcall(function()
										-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
										wait()
										game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
									end)
									wait(2)
								end
							end
						end
					end
					function Teleport()
						while wait() do
							pcall(function()
								TPReturner()
								if foundAnything ~= "" then
									TPReturner()
								end
							end)
						end
					end
					Teleport()
				end
			end)
		end
	end
end)


spawn(function()
	while wait(9) do
		pcall(function()
			if _G.KillAndHop then
				for i, v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
					if v.Name == NameKill and (v.Humanoid.Health == v.Humanoid.MaxHealth or v.Humanoid.Health < KillHealt) then
						NextPlayer = true
					end
				end
			end
		end)
	end
end)

spawn(function()
	while wait(.1) do
		if _G.Bounty_Open then
			if BountyValue >= _G.Bounty_Lock then
				game.Players.localPlayer:Kick("\n Auto Farm Bounty Completed : "..game:GetService("Players").LocalPlayer.leaderstats["Bounty/Honor"].Value)
			end
		end
	end
end)
spawn(function()
	while wait() do
		if _G.Bounty_Farm_Hop then
			pcall(function()
				for i,v in pairs(game.Players:GetChildren()) do
					if v.Name ~= game.Players.LocalPlayer.Name then
						repeat wait()
							EquipWeapon(_G.Select_Wapon_Bouty)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(v.Name).Character.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
							game.Players:FindFirstChild(v.Name).Character.HumanoidRootPart.Size = Vector3.new(60,60,60)
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							local savezone = "Cannot attack players in a Safe Zone"
							local pvpnotopen = "PvP disabled for 10 minutes"
							local enemiepvpnot = "Player died recently, you can't attack them yet!"

							if game:GetService("Players").LocalPlayer.PlayerGui.Notifications:FindFirstChild("NotificationTemplate") then
								notifier = game:GetService("Players").LocalPlayer.PlayerGui.Notifications.NotificationTemplate.Text
							end

							for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
								if not game:GetService("Players").LocalPlayer.PlayerGui.Notifications:FindFirstChild("NotificationTemplate") then
									print("NO NOTIFIER")
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
									_G.Bounty_Farm_Hop = false
									if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.InCombat.Text,"ÃƒÆ’Ã‚Â¢Ãƒâ€¦Ã‚Â¡ÃƒÂ¢Ã¢â€šÂ¬Ã‚ÂÃƒÆ’Ã‚Â¯Ãƒâ€šÃ‚Â¸Ãƒâ€šÃ‚ÂIn Combat - Bounty at risk!ÃƒÆ’Ã‚Â¢Ãƒâ€¦Ã‚Â¡ÃƒÂ¢Ã¢â€šÂ¬Ã‚ÂÃƒÆ’Ã‚Â¯Ãƒâ€šÃ‚Â¸Ãƒâ€šÃ‚Â") then
										if NewWorld then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
										end
										if NewWorld2 then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
										end
									else
										Hop()
									end
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
								elseif string.find(notifier,savezone) then
									print("IN SAVEZONE")
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
									_G.Bounty_Farm_Hop = false
									if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.InCombat.Text,"ÃƒÆ’Ã‚Â¢Ãƒâ€¦Ã‚Â¡ÃƒÂ¢Ã¢â€šÂ¬Ã‚ÂÃƒÆ’Ã‚Â¯Ãƒâ€šÃ‚Â¸Ãƒâ€šÃ‚ÂIn Combat - Bounty at risk!ÃƒÆ’Ã‚Â¢Ãƒâ€¦Ã‚Â¡ÃƒÂ¢Ã¢â€šÂ¬Ã‚ÂÃƒÆ’Ã‚Â¯Ãƒâ€šÃ‚Â¸Ãƒâ€šÃ‚Â") then
										if NewWorld then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
										end
										if NewWorld2 then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
										end
									else
										Hop()
										if NewWorld then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
										end
										if NewWorld2 then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
										end
									end
								elseif string.find(notifier,pvpnotopen) then
									print("PVP NOT OPEN")
									if NewWorld then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
									end
									if NewWorld2 then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
									end
									_G.Bounty_Farm_Hop = false
									if NewWorld then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
									end
									if NewWorld2 then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
									end
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp")
									wait(5)
									_G.Bounty_Farm_Hop = true
								elseif string.find(notifier,enemiepvpnot) then
									print("ENEMIE PVP NOT OPEN")
									if NewWorld then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
									end
									if NewWorld2 then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
									end
									_G.Bounty_Farm_Hop = false
									if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.InCombat.Text,"ÃƒÆ’Ã‚Â¢Ãƒâ€¦Ã‚Â¡ÃƒÂ¢Ã¢â€šÂ¬Ã‚ÂÃƒÆ’Ã‚Â¯Ãƒâ€šÃ‚Â¸Ãƒâ€šÃ‚ÂIn Combat - Bounty at risk!ÃƒÆ’Ã‚Â¢Ãƒâ€¦Ã‚Â¡ÃƒÂ¢Ã¢â€šÂ¬Ã‚ÂÃƒÆ’Ã‚Â¯Ãƒâ€šÃ‚Â¸Ãƒâ€šÃ‚Â") then
										if NewWorld then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
										end
										if NewWorld2 then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
										end
									else
										Hop()
										if NewWorld then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
										end
										if NewWorld2 then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
										end
									end
								end
							end
						until _G.Bounty_Farm_Hop == false or game.Players:FindFirstChild(v.Name).Character.Humanoid.Health == 0
						_G.Bounty_Farm_Hop = false
						if NewWorld then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
						end
						if NewWorld2 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
						end
						wait()
						Hop()
					end
				end
			end)
		end
	end
end)
spawn(function()
	while wait() do
		if _G.Bounty_Farm_Hop then
			game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
		end
	end
end)
spawn(function()
	while wait() do
		if _G.a then
			pcall(function()
				for i = 1,math.huge do wait(math.huge)
					local RigC = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework)
					require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut = 2,Sustained = 0,Inactive =1}
					RigC.activeController.timeToNextAttack = 0
					RigC.activeController.attacking = false
					RigC.activeController.blocking = false
					RigC.activeController.timeToNextAttack = -9999
					RigC.activeController.timeToNextBlock = 0
					RigC.activeController.increment = 3
					RigC.activeController.hitboxMagnitude = 20
					game.Players.LocalPlayer.Character.Stun.Value = 0
					game.Players.LocalPlayer.Character.Humanoid.Sit = false
					wait(math.huge)
				end
			end)
		end
	end
end)
Players:Toggle("Safe Mode", false, function(vu)
	SafePlayer = vu
end)
Players:Toggle("God Mode",false,function(t)
	_G.GodMode = t
end)
Players:Toggle("Steal Players(use gun)",false,function(t)
	_G.StealPlayers = t
end)
spawn(function()
	if _G.GodMode or _G.StealPlayers then
		local player = game.Players.LocalPlayer
		if player.Character then
			if player.Character:FindFirstChild("Humanoid") then
				player.Character.Humanoid.Name = "1"
			end
			local l = player.Character["1"]:Clone()
			l.Parent = player.Character
			l.Name = "Humanoid"; wait(0.1)
			player.Character["1"]:Destroy()
			workspace.CurrentCamera.CameraSubject = player.Character.Humanoid
			player.Character.Animate.Disabled = true; wait(0.1)
			player.Character.Animate.Disabled = false
		end
		print("GodMode & Steal Players:on")
	end
end)
Players:Toggle("Ghost Mode ",false,function(b)
	if b == true then
		game.Players.LocalPlayer.Character.LowerTorso:Destroy()
	else
		game.Players.LocalPlayer.Character.Humanoid.Health = 0
	end
end)
spawn(function()
	while wait(.1) do
		if SafePlayer then
			pcall(function()
				local X = math.random(0,100000)
				local Z = math.random(0,100000)
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(X,3000,Y)
				game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
			end)
		end
	end
end)
Players:Toggle("Spectate Player",false,function(bool)
	Sp = bool
	local plr1 = game.Players.LocalPlayer.Character.Humanoid
	local plr2 = game.Players:FindFirstChild(SelectedKillPlayer)
	repeat wait(.1)
		game.Workspace.Camera.CameraSubject = plr2.Character.Humanoid
	until Sp == false 
	game.Workspace.Camera.CameraSubject = game.Players.LocalPlayer.Character.Humanoid
end)
_G.Bounty_Lock = 25000000
BountyValue = game:GetService("Players").LocalPlayer.leaderstats["Bounty/Honor"].Value
Players:Slider("Select Bounty", 0, 25000000, 1, function(value)
	_G.Bounty_Lock = value
end)

Players:Toggle("Lock Bounty",false,function(value)
	_G.Bounty_Open = value
end)
Players:Label("Click to Player")
Players:Button("Teleport Player", function()
	local plr1 = game.Players.LocalPlayer.Character
	local plr2 = game.Players:FindFirstChild(SelectedKillPlayer)
	plr1.HumanoidRootPart.CFrame = plr2.Character.HumanoidRootPart.CFrame
end)
Players:Button("copy Pant and Shirt", function()
	local plr1 = game.Players.LocalPlayer.Character
	local plr2 = game.Players:FindFirstChild(SelectedKillPlayer)
	plr1.Shirt.ShirtTemplate = plr2.Character.Shirt.ShirtTemplate
	plr1.Pants.PantsTemplate = plr2.Character.Pants.PantsTemplate
end)
Players:Label("--AIMBOT--")
Players:Toggle("Aimbot Gun",true,function(bool)
	_G.Aimbot = bool
end)
local lp = game:GetService('Players').LocalPlayer
local mouse = lp:GetMouse()
mouse.Button1Down:Connect(function()
	pcall(function()
		if _G.Aimbot and game.Players.LocalPlayer.Character:FindFirstChild(SelectToolWeaponGun) then
			for i,v in pairs(game:GetService("Players"):GetChildren()) do
				if v.Character:FindFirstChild("HumanoidRootPart") and v.Character:FindFirstChild("Humanoid") then
					if (v.Character.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude/3 <= RangeAimGun then
						if v.Name == game.Players.LocalPlayer.Name then
						else
							local args = {
								[1] = v.Character.HumanoidRootPart.Position,
								[2] = v.Character.HumanoidRootPart
							}
							game:GetService("Players").LocalPlayer.Character[SelectToolWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
						end
					end
				end
			end
		end
	end)
end)
game:GetService("RunService").Heartbeat:Connect(
function()
	if _G.Aimbot then
		pcall(function()
			local args = {
				[1] = game:GetService("Players"):FindFirstChild(SelectedKillPlayer).Character.HumanoidRootPart.Position,
				[2] = game:GetService("Players"):FindFirstChild(SelectedKillPlayer).Character.HumanoidRootPart
			}
			game:GetService("Players").LocalPlayer.Character[SelectToolWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
			game:GetService("Workspace").Characters.LocalPlayer[SelectToolWeaponGun].Cooldown = 0
		end)
	end
end)
Players:Toggle("Aimbot Skill",false,function(bool)
	AimbotSkill = bool
	while AimbotSkill do wait()
		pcall(function()
			game:GetService("Workspace").Characters.LocalPlayer[SelectToolWeaponGun].Cooldown = 0
			if game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool") and game.Players.LocalPlayer.Character[game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name]:FindFirstChild("MousePos") then
				local args = {
					[1] = game:GetService("Players"):FindFirstChild(SelectedKillPlayer).Character.HumanoidRootPart.Position
				}
				game:GetService("Players").LocalPlayer.Character[game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
			end
		end)
	end
end)
SpeesPlayer = 16
Players:Toggle("Use Speed",false,function(a)
	local name = game.Players.LocalPlayer.Name
	game.Workspace.Characters[name].Movement.Disabled = true
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 36
	speed = a
end)
Players:Slider("Speed", 36, 100000,36,function(t)
	sspeed = t
end)

spawn(function()
	while wait() do
		if speed then
			local name = game.Players.LocalPlayer.Name
			game.Workspace.Characters[name].Movement.Disabled = true
			game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = sspeed
		end
	end
end)
Players:Button("Set Speed", function()
	Speed:Change(36)
end)
Players:Toggle("Clone Players Is Lag Sever",false,function(vu)
	Lag = vu
	while Lag do wait()
		if Lag then
			spawn(function()
				local args = {
					[1] = "SetTeam",
					[2] = "Pirates"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
				local args = {
					[1] = "BartiloQuestProgress"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				local args = {
					[1] = "Buso"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
local Teleport = window:Tap("Teleport",6031094670)
Teleport:Toggle("Ctrl + Click = TP",false,function(vu)
	CTRL = vu
end)
local Plr = game:GetService("Players").LocalPlayer
local Mouse = Plr:GetMouse()
Mouse.Button1Down:connect(
	function()
		if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
			return
		end
		if not Mouse.Target then
			return
		end
		if CTRL then
			Plr.Character:MoveTo(Mouse.Hit.p)
		end
	end)
Teleport:Button("Teleport To Old World", function()
	local args = {
		[1] = "TravelMain" -- OLD WORLD to NEW WORLD
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

Teleport:Button("Teleport To NewWorld", function()
	local args = {
		[1] = "TravelDressrosa" -- NEW WORLD to OLD WORLD
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Teleport:Button("Teleport To Third World", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
end)
Teleport:Button("Teleport to SeaBeasts", function()
	for i,v in pairs(game.Workspace.SeaBeasts:GetChildren()) do
		if v:FindFirstChild("HumanoidRootPart") then
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,100,0)
		end
	end
end)
Teleport:Label("-----------------------------------------------------------------")
function tweenteleoirtzz(XXXXx)
	local Distance = (Vector3.new(XXXXx) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
local Speed = 300
game:GetService("TweenService"):Create(
  game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart,
  TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
  {CFrame = XXXXx}
):Play()
_G.NoClip = true
wait(Distance/Speed)
_G.NoClip = false
end
if OldWorld then
Teleport:Button("Start Island",function()
tweenteleoirtzz(CFrame.new(1071.2832, 16.3085976, 1426.86792))
end)
Teleport:Button("Marine Start",function()
tweenteleoirtzz(CFrame.new(-2573.3374, 6.88881969, 2046.99817))
end)
Teleport:Button("Middle Town",function()
tweenteleoirtzz(CFrame.new(-655.824158, 7.88708115, 1436.67908))
end)
Teleport:Button("Jungle",function()
tweenteleoirtzz(CFrame.new(-1249.77222, 11.8870859, 341.356476))
end)
Teleport:Button("Pirate Village",function()
tweenteleoirtzz(CFrame.new(-1122.34998, 4.78708982, 3855.91992))
end)
Teleport:Button("Desert",function()
tweenteleoirtzz(CFrame.new(1094.14587, 6.47350502, 4192.88721))
end)
Teleport:Button("Frozen Village",function()
tweenteleoirtzz(CFrame.new(1198.00928, 27.0074959, -1211.73376))
end)
Teleport:Button("MarineFord",function()
tweenteleoirtzz(CFrame.new(-4505.375, 20.687294, 4260.55908))
end)
Teleport:Button("Colosseum",function()
tweenteleoirtzz(CFrame.new(-1428.35474, 7.38933945, -3014.37305))
end)
Teleport:Button("Sky 1st Floor",function()
tweenteleoirtzz(CFrame.new(-4970.21875, 717.707275, -2622.35449))
end)
Teleport:Button("Sky 2st Floor",function()
tweenteleoirtzz(CFrame.new(-4813.0249, 903.708557, -1912.69055))
end)
Teleport:Button("Sky 3st Floor",function()
tweenteleoirtzz(CFrame.new(-7952.31006, 5545.52832, -320.704956))
end)
Teleport:Button("Prison",function()
tweenteleoirtzz(CFrame.new(4854.16455, 5.68742752, 740.194641))
end)
Teleport:Button("Magma Village",function()
tweenteleoirtzz(CFrame.new(-5231.75879, 8.61593437, 8467.87695))
end)
Teleport:Button("UndeyWater City",function()
tweenteleoirtzz(CFrame.new(61163.8516, 11.7796879, 1819.78418))
end)
Teleport:Button("Fountain City",function()
tweenteleoirtzz(CFrame.new(5132.7124, 4.53632832, 4037.8562))
end)
Teleport:Button("House Cyborg's",function()
tweenteleoirtzz(CFrame.new(6262.72559, 71.3003616, 3998.23047))
end)
Teleport:Button("Shank's Room",function()
tweenteleoirtzz(CFrame.new(-1442.16553, 29.8788261, -28.3547478))
end)
Teleport:Button("Mob Island",function()
tweenteleoirtzz(CFrame.new(-2850.20068, 7.39224768, 5354.99268))
end)
end
if NewWorld then
Teleport:Button("Dock",function()
tweenteleoirtzz(CFrame.new(82.9490662, 18.0710983, 2834.98779))
end)
Teleport:Button("Kingdom of Rose",function()
tweenteleoirtzz(CFrame.new(-394.983521, 118.503128, 1245.8446))
end)
Teleport:Button("Mansion",function()
tweenteleoirtzz(CFrame.new(-390.096313, 331.886475, 673.464966))
end)
Teleport:Button("Flamingo Room",function()
tweenteleoirtzz(CFrame.new(2302.19019, 15.1778421, 663.811035))
end)
Teleport:Button("Green Zone",function()
tweenteleoirtzz(CFrame.new(-2372.14697, 72.9919434, -3166.51416))
end)
Teleport:Button("Cafe",function()
tweenteleoirtzz(CFrame.new(-385.250916, 73.0458984, 297.388397))
end)
Teleport:Button("Factroy",function()
tweenteleoirtzz(CFrame.new(430.42569, 210.019623, -432.504791))
end)
Teleport:Button("Colosseum",function()
tweenteleoirtzz(CFrame.new(-1836.58191, 44.5890656, 1360.30652))
end)
Teleport:Button("GraveIsland",function()
tweenteleoirtzz(CFrame.new(-5411.47607, 48.8234024, -721.272522))
end)
Teleport:Button("Snow Mountain",function()
tweenteleoirtzz(CFrame.new(511.825226, 401.765198, -5380.396))
end)
Teleport:Button("Cold Island",function()
tweenteleoirtzz(CFrame.new(-6026.96484, 14.7461271, -5071.96338))
end)
Teleport:Button("Hot Island",function()
tweenteleoirtzz(CFrame.new(-5478.39209, 15.9775667, -5246.9126))
end)
Teleport:Button("Cursed Ship",function()
tweenteleoirtzz(CFrame.new(902.059143, 124.752518, 33071.8125))
end)
Teleport:Button("IceCastle",function()
tweenteleoirtzz(CFrame.new(5400.40381, 28.21698, -6236.99219))
end)
Teleport:Button("Forgotten Island",function()
tweenteleoirtzz(CFrame.new(-3043.31543, 238.881271, -10191.5791))
end)
Teleport:Button("Usoapp Island",function()
tweenteleoirtzz(CFrame.new(4748.78857, 8.35370827, 2849.57959))
end)
Teleport:Button("Minisky Island",function()
tweenteleoirtzz(CFrame.new(-260.358917, 49325.7031, -35259.3008))
end)
end
if NewWorld2 then 
Teleport:Button("Port Towen",function()
tweenteleoirtzz(CFrame.new(-610.309692, 57.8323097, 6436.33594, 1, 0, 0, 0, 1, 0, 0, 0, 1))
end)
Teleport:Button("Hydra Island",function()
tweenteleoirtzz(CFrame.new(5229.99561, 603.916565, 345.154022, -0.137452736, 6.26227887e-08, -0.990508318, 5.81512971e-08, 1, 5.51532295e-08, 0.990508318, -5.00183823e-08, -0.137452736))
end)
Teleport:Button("Great Tree",function()
tweenteleoirtzz(CFrame.new(2174.94873, 28.7312393, -6728.83154, 0.864815354, 2.51030592e-08, -0.502090037, -5.24263299e-09, 1, 4.09670555e-08, 0.502090037, -3.27966632e-08, 0.864815354))
end)
Teleport:Button("Castle on the Sea",function()
tweenteleoirtzz(CFrame.new(-5477.62842, 313.794739, -2808.4585, 0.914748192, -2.40542199e-08, 0.404024392, -8.97737973e-09, 1, 7.98621613e-08, -0.404024392, -7.66808483e-08, 0.914748192))
end)
Teleport:Button("Floating Turtle",function()
tweenteleoirtzz(CFrame.new(-10919.2998, 331.788452, -8637.57227, 0.606543362, 0, -0.795050383, -0, 1, -0, 0.795050383, 0, 0.606543362))
end)
Teleport:Button("Mansion",function()
tweenteleoirtzz(CFrame.new(-12553.8125, 332.403961, -7621.91748, -0.999466479, 2.33264661e-08, 0.0326608531, 2.2023519e-08, 1, -4.02529707e-08, -0.0326608531, -3.95121873e-08, -0.999466479))
end)
Teleport:Button("Secret Temple",function()
tweenteleoirtzz(CFrame.new(5217.35693, 6.56511116, 1100.88159, 0.00408430398, 7.00437894e-08, -0.999991655, 1.42367229e-08, 1, 7.01025229e-08, 0.999991655, -1.45229242e-08, 0.00408430398))
end)
Teleport:Button("Friendly Arena",function()
tweenteleoirtzz(CFrame.new(5220.28955, 72.8193436, -1450.86304, 1, 0, 0, 0, 1, 0, 0, 0, 1))
end)
Teleport:Button("Beautiful Pirate Domain",function()
tweenteleoirtzz(CFrame.new(5310.8095703125, 21.594484329224, 129.39053344727))
end)
	Teleport:Label("--TelePort NPC--", true)
	Teleport:Button("Sword Dealer", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(895.941956, 14.9845877, 1412.76782, -0.939700961, 0, -0.341998369, 0, 1, 0, 0.341998369, 0, -0.939700961)
	end)
	Teleport:Button("Weapon Dealer", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-700.12005615234, 7.8522434234619, 1512.2841796875)
	end)
	Teleport:Button("NPC randomfruit", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1441.53357, 61.1999283, 7.7518611, 0.499959469, -0, -0.866048813, 0, 1, -0, 0.866048813, 0, 0.499959469)
	end)
	Teleport:Button("Sword Dealer of the West", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1279.0747070313, 13.752041816711, 3990.2504882813)
	end)
	Teleport:Button("darkleg teacher", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-983.618103, 12.450016, 3990.46265, 0.358573437, 0, 0.933501542, 0, 1, 0, -0.933501542, 0, 0.358573437)
	end)
	Teleport:Button("Hasan", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1322.017578125, 15.891534805298, 4486.0834960938)
	end)
	Teleport:Button("ability teacher", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1488.6115722656, 37.829216003418, -1412.5043945313)
	end)
	Teleport:Button("Sick man", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1460.7014160156, 88.573440551758, -1392.4689941406)
	end)
	Teleport:Button("Sword dealer of the east", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1431.3474121094, 87.752792358398, -1388.0727539063)
	end)
	Teleport:Button("Advance Weapon Dealer", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4997.841796875, 41.252048492432, 4403.181640625)
	end)
	Teleport:Button("parlus", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4929.2255859375, 96.839538574219, 3868.7917480469)
	end)
	Teleport:Button("master sword dealer", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4750.6059570313, 717.65997314453, -2654.2487792969)
	end)
	Teleport:Button("usoap", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-8036.05859375, 5756.033203125, -1934.3215332031)
	end)
	Teleport:Button("Remove Fruit", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5665.552734375, 64.651931762695, 868.56658935547)
	end)
	Teleport:Button("caption to newworld", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1164.2852783203, 8.2123336791992, 1727.9249267578)
	end)
	Teleport:Button("Kung fu teacher", function()
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(61581.54296875, 18.870784759521, 985.88067626953)
	end)
end
local pppp = window:Tap("Misc",6031094670)
pppp:Button("Open Awakening", function()
	local args = {
		[1] = "AwakeningChanger",
		[2] = "Check"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	game.Players.localPlayer.PlayerGui.Main.AwakeningToggler.Visible = true
end)
pppp:Button("Open Inventory", function()
	local args = {
		[1] = "getInventoryWeapons"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	game.Players.localPlayer.PlayerGui.Main.Inventory.Visible = true
end)
pppp:Button("Open Devil Shop", function()
	local args = {
		[1] = "GetFruits"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	game.Players.localPlayer.PlayerGui.Main.FruitShop.Visible = true
end)
pppp:Button("Open Color Haki", function()
	game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
end)
pppp:Button("Open Title Name", function()
	local args = {
		[1] = "getTitles"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
end)
pppp:Label("Checking Status")
pppp:Button("Check Status", function()
	game.StarterGui:SetCore("SendNotification", {
		Title = "Level", 
		Text = "My Level = " ..game.Players.LocalPlayer.Data.Level.Value,
		Icon = "",
		Duration = 2.5
	})
	game.StarterGui:SetCore("SendNotification", {
		Title = "Melee", 
		Text = "My Beli = " ..game:GetService("Players")["LocalPlayer"].Data.Beli.Value,
		Icon = "",
		Duration = 2.5
	})
	game.StarterGui:SetCore("SendNotification", {
		Title = "Fragments", 
		Text = "My Fragments = " ..game:GetService("Players")["LocalPlayer"].Data.Fragments.Value,
		Icon = "",
		Duration = 2.5
	})
	game.StarterGui:SetCore("SendNotification", {
		Title = "Exp", 
		Text = "My Exp = " ..game:GetService("Players")["LocalPlayer"].Data.Exp.Value,
		Icon = "",
		Duration = 2.5
	})
	game.StarterGui:SetCore("SendNotification", {
		Title = "Race", 
		Text = "My Race = " ..game:GetService("Players")["LocalPlayer"].Data.Race.Value,
		Icon = "",
		Duration = 2.5
	})
	game.StarterGui:SetCore("SendNotification", {
		Title = "DevilFruit", 
		Text = "My DevilFruit = " ..game:GetService("Players")["LocalPlayer"].Data.DevilFruit.Value,
		Icon = "",
		Duration = 2.5
	})
end)
pppp:Label("Team")
pppp:Button("Join Pirates Team", function()
	local args = {
		[1] = "SetTeam",
		[2] = "Pirates"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
	local args = {
		[1] = "BartiloQuestProgress"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "Buso"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

pppp:Button("Join Marines Team", function()
	local args = {
		[1] = "SetTeam",
		[2] = "Marines"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "BartiloQuestProgress"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "Buso"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Label("--ESP--", true)
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
							name.TextColor3 = Color3.new(255, 255 ,255)
						else
							name.TextColor3 = Color3.new(255, 255 ,255)
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
								name.TextColor3 = Color3.fromRGB(255, 255, 255)
								name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							end
							if v.Name == "Chest2" then
								name.TextColor3 = Color3.fromRGB(255, 255, 255)
								name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							end
							if v.Name == "Chest3" then
								name.TextColor3 = Color3.fromRGB(255, 255 ,255)
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
						name.TextColor3 = Color3.fromRGB(255, 255 ,255)
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
						name.TextColor3 = Color3.fromRGB(255, 255 ,255)
						if v.Name == "Flower1" then 
							name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							name.TextColor3 = Color3.fromRGB(255, 255 ,255)
						end
						if v.Name == "Flower2" then
							name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							name.TextColor3 = Color3.fromRGB(255, 255 ,255)
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
pppp:Toggle("ESP Player",false,function(a)
	ESPPlayer = a
	while ESPPlayer do wait()
		UpdatePlayerChams()
	end
end)
pppp:Toggle("ESP Chest",false,function(a)
	ChestESP = a
	while ChestESP do wait()
		UpdateChestChams() 
	end
end)
pppp:Toggle("ESP Devil Fruit",false,function(a)
	DevilFruitESP = a
	while DevilFruitESP do wait()
		UpdateDevilChams() 
	end
end)
pppp:Toggle("ESP Flower",false,function(a)
	FlowerESP = a
	while FlowerESP do wait()
		UpdateFlowerChams() 
	end
end)
pppp:Label("--Character--", true)
nododgecool = false
function NoDodgeCool()
	if nododgecool then
		for i,v in next, getgc() do
			if game.Players.LocalPlayer.Character.Dodge then
				if typeof(v) == "function" and getfenv(v).script == game.Players.LocalPlayer.Character.Dodge then
					for i2,v2 in next, getupvalues(v) do
						if tostring(v2) == "0.4" then
							repeat wait(.1)
								setupvalue(v,i2,0)
							until not nododgecool
						end
					end
				end
			end
		end
	end
end
pppp:Button("Auto Torch", function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Waterfall.SecretRoom.Room.Door.Door.Hitbox.CFrame
	wait(2)
	EquipWeapon("Holy Torch")
	wait()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Turtle.QuestTorches.Torch1.CFrame
	wait(1)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Turtle.QuestTorches.Torch2.CFrame
	wait(1)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Turtle.QuestTorches.Torch3.CFrame
	wait(1)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Turtle.QuestTorches.Torch4.CFrame
	wait(1)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Turtle.QuestTorches.Torch5.CFrame
end)
pppp:Toggle("Hide Crew",false,function(t)
	if t == true then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CrewBBG.Frame.Visible = false
	else
		game.Players.LocalPlayer.Character.HumanoidRootPart.CrewBBG.Frame.Visible = true
	end
end)
pppp:Toggle("Fast Attack V.2",_G.FastAttk,function(value)
	_G.FastAttk = value
end)

local RigC = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework) 
local VirtualUser = game:GetService('VirtualUser')
kkii = require(game.ReplicatedStorage.Util.CameraShaker)

spawn(function()
	for i = 1,2 do 
		spawn(function()
			game:GetService('RunService').Heartbeat:connect(function()
				if _G.FastAttk then
					pcall(function()
						pcall(function ()
							kkii:Stop()
							wait()
						end)  
					end)
				end
			end)
		end)
		---------------------------------
		spawn(function()
			game:GetService('RunService').Heartbeat:connect(function()
				if _G.FastAttk then
					pcall(function()
						pcall(function ()
							RigC.activeController.timeToNextAttack = 0
							wait()
						end)  
					end)
				end
			end)
		end)

		spawn(function()
			game:GetService('RunService').Heartbeat:connect(function()
				if _G.FastAttk then
					pcall(function()
						pcall(function ()
							RigC.activeController.hitboxMagnitude = 25
							wait(.05)
						end)  
					end)
				end
			end)
		end)

		spawn(function()
			game:GetService('RunService').Heartbeat:connect(function()
				if _G.FastAttk then
					pcall(function()
						pcall(function ()
							RigC.activeController.increment = 3
							wait()
						end)
					end)
				end
			end)
		end)

		spawn(function()
			game:GetService('RunService').Heartbeat:connect(function()
				if _G.FastAttk then
					pcall(function()
						pcall(function ()
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							wait(.05)
						end)
					end)
				end
			end)
		end)
		spawn(function()
			game:GetService('RunService').Heartbeat:connect(function()
				if _G.FastAttk then
					pcall(function()
						pcall(function ()
							game:GetService'VirtualUser':CaptureController()
							game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
							wait(.05)
						end)
					end)
				end
			end)
		end)

	end
end)

pppp:Button("Invisible Mode", function()
	game.Players.LocalPlayer.Character.LowerTorso:Destroy()
end)
pppp:Toggle("Walk on Water",false,function(Value)
	_G.WalkWater = Value
	if _G.WalkWater == true then
		game.Players.LocalPlayer.Data.DevilFruit.Value = ("Ice-Ice")
	elseif _G.WalkWater == false then
		game.Players.LocalPlayer.Data.DevilFruit.Value = ("")
	end
end)
pppp:Button("TP to Flower", function()
	if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower1") or not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower1") then
		game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Flower1.CFrame
	end
	wait(1)
	if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower2") or not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower2") then
		game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Flower2.CFrame
	end
end, "")
pppp:Toggle("Dodge No Cooldown",false,function(Value)
	nododgecool = Value
	NoDodgeCool()
end)
pppp:Toggle("Infinits Energy",false,function(value)
	InfinitsEnergy = value
	originalstam = LocalPlayer.Character.Energy.Value
end)
local LocalPlayer = game:GetService'Players'.LocalPlayer
local originalstam = LocalPlayer.Character.Energy.Value
function infinitestam()
	LocalPlayer.Character.Energy.Changed:connect(function()
		if InfinitsEnergy then
			LocalPlayer.Character.Energy.Value = originalstam
		end
	end)
end
spawn(function()
	while wait(.1) do
		if InfinitsEnergy then
			wait(0.3)
			originalstam = LocalPlayer.Character.Energy.Value
			infinitestam()
		end
	end
end)
function infAb()
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	wait(.1)
	local inf = Instance.new("ParticleEmitter")
	inf.Acceleration = Vector3.new(0,0,0)
	inf.Archivable = true
	inf.Drag = 20
	inf.EmissionDirection = Enum.NormalId.Top
	inf.Enabled = true
	inf.Lifetime = NumberRange.new(0.2,0.2)
	inf.LightInfluence = 0
	inf.LockedToPart = true
	inf.Name = "Agility"
	inf.Rate = 500
	local numberKeypoints2 = {
		NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
		NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
	}

	inf.Size = NumberSequence.new(numberKeypoints2)
	inf.RotSpeed = NumberRange.new(999, 9999)
	inf.Rotation = NumberRange.new(0, 0)
	inf.Speed = NumberRange.new(30, 30)
	inf.SpreadAngle = Vector2.new(360,360)
	inf.Texture = "rbxassetid://243098098"
	inf.VelocityInheritance = 0
	inf.ZOffset = 2
	inf.Transparency = NumberSequence.new(0)
	inf.Color = ColorSequence.new(Color3.fromRGB(0, 255, 255),Color3.fromRGB(0, 255, 255))
	inf.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart

	local inf2 = Instance.new("ParticleEmitter")
	inf2.Acceleration = Vector3.new(0,0,0)
	inf2.Archivable = true
	inf2.Drag = 20
	inf2.EmissionDirection = Enum.NormalId.Top
	inf2.Enabled = true
	inf2.Lifetime = NumberRange.new(0.2,0.2)
	inf2.LightInfluence = 0
	inf2.LockedToPart = true
	inf2.Name = "Agility"
	local numberKeypoints3 = {
		NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
		NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
	}

	inf2.Size = NumberSequence.new(numberKeypoints3)
	inf2.Rate = 500
	inf2.RotSpeed = NumberRange.new(999, 9999)
	inf2.Rotation = NumberRange.new(0, 0)
	inf2.Speed = NumberRange.new(30, 30)
	inf2.SpreadAngle = Vector2.new(360,360)
	inf2.Texture = "rbxassetid://243098098"
	inf2.VelocityInheritance = 0
	inf2.Transparency = NumberSequence.new(0)
	inf2.Color = ColorSequence.new(Color3.fromRGB(255, 0, 0),Color3.fromRGB(255, 0, 0))
	inf2.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart

	local inf3 = Instance.new("ParticleEmitter")
	inf3.Acceleration = Vector3.new(0,0,0)
	inf3.Archivable = true
	inf3.Drag = 20
	inf3.EmissionDirection = Enum.NormalId.Top
	inf3.Enabled = true
	inf3.Lifetime = NumberRange.new(0.2,0.2)
	inf3.LightInfluence = 0
	inf3.LockedToPart = true
	inf3.Name = "Agility"
	local numberKeypoints4 = {
		NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
		NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
	}

	inf3.Size = NumberSequence.new(numberKeypoints4)
	inf3.Rate = 500
	inf3.RotSpeed = NumberRange.new(999, 9999)
	inf3.Rotation = NumberRange.new(0, 0)
	inf3.Speed = NumberRange.new(30, 30)
	inf3.SpreadAngle = Vector2.new(360,360)
	inf3.Texture = "rbxassetid://243098098"
	inf3.VelocityInheritance = 0
	inf3.Transparency = NumberSequence.new(0)
	inf3.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0),Color3.fromRGB(255, 255, 0))
	inf3.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart

	local inf4 = Instance.new("ParticleEmitter")
	inf4.Acceleration = Vector3.new(0,0,0)
	inf4.Archivable = true
	inf4.Drag = 20
	inf4.EmissionDirection = Enum.NormalId.Top
	inf4.Enabled = true
	inf4.Lifetime = NumberRange.new(0.2,0.2)
	inf4.LightInfluence = 0
	inf4.LockedToPart = true
	inf4.Name = "Agility"
	local numberKeypoints5 = {
		NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
		NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
	}

	inf4.Size = NumberSequence.new(numberKeypoints5)
	inf4.Rate = 500
	inf4.RotSpeed = NumberRange.new(999, 9999)
	inf4.Rotation = NumberRange.new(0, 0)
	inf4.Speed = NumberRange.new(30, 30)
	inf4.SpreadAngle = Vector2.new(360,360)
	inf4.Texture = "rbxassetid://243098098"
	inf4.VelocityInheritance = 0
	inf4.Transparency = NumberSequence.new(0)
	inf4.Color = ColorSequence.new(Color3.fromRGB(255, 255, 255),Color3.fromRGB(255, 6, 60))
	inf4.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
end

pppp:Toggle("Inf Ability",false,function(inf)
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
		game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
	end
	wait()
	getgenv().InfAbility = inf
end)

spawn(function()
	while wait(1) do
		pcall(function()
			if InfAbility then
				if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
					if InfAbility == true then
						infAb()
					elseif InfAbility == false then
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
					else
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
						end
					end
				end
			end
		end)
	end
end)
pppp:Toggle("Auto Click",false,function(value)
	AuctoClick = value
end)
spawn(function()
	while wait(.1) do
		if AuctoClick then
			game:GetService'VirtualUser':CaptureController()
			game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
		end
	end
end)
Fly = false
function activatefly()
	local mouse=game.Players.LocalPlayer:GetMouse''
	localplayer=game.Players.LocalPlayer
	game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")
	local torso = game.Players.LocalPlayer.Character.HumanoidRootPart
	local speed=180
	local keys={a=false,d=false,w=false,s=false}
	local e1
	local e2
	local function start()
		local pos = Instance.new("BodyPosition",torso)
		local gyro = Instance.new("BodyGyro",torso)
		pos.Name="EPIXPOS"
		pos.maxForce = Vector3.new(math.huge, math.huge, math.huge)
		pos.position = torso.Position
		gyro.maxTorque = Vector3.new(9e9, 9e9, 9e9)
		gyro.cframe = torso.CFrame
		repeat
			wait()
			localplayer.Character.Humanoid.PlatformStand=true
			local new=gyro.cframe - gyro.cframe.p + pos.position
			if not keys.w and not keys.s and not keys.a and not keys.d then
				speed=3
			end
			if keys.w then
				new = new + workspace.CurrentCamera.CoordinateFrame.lookVector * speed
				speed=speed+9.02
			end
			if keys.s then
				new = new - workspace.CurrentCamera.CoordinateFrame.lookVector * speed
				speed=speed+4.02
			end
			if keys.d then
				new = new * CFrame.new(speed,0,0)
				speed=speed+2.02
			end
			if keys.a then
				new = new * CFrame.new(-speed,0,0)
				speed=speed+3.02
			end
			if speed>5 then
				speed=9.5
			end
			pos.position=new.p
			if keys.w then
				gyro.cframe = workspace.CurrentCamera.CoordinateFrame*CFrame.Angles(-math.rad(speed*15),0,0)
			elseif keys.s then
				gyro.cframe = workspace.CurrentCamera.CoordinateFrame*CFrame.Angles(math.rad(speed*15),0,0)
			else
				gyro.cframe = workspace.CurrentCamera.CoordinateFrame
			end
		until not Fly
		if gyro then
			gyro:Destroy()
		end
		if pos then
			pos:Destroy()
		end
		flying=false
		localplayer.Character.Humanoid.PlatformStand=false
		speed=5
	end
	e1=mouse.KeyDown:connect(function(key)
		if not torso or not torso.Parent then
			flying=false e1:disconnect() e2:disconnect() return
		end
		if key=="w" then
			keys.w=true
		elseif key=="s" then
			keys.s=true
		elseif key=="a" then
			keys.a=true
		elseif key=="d" then
			keys.d=true
		end
	end)
	e2=mouse.KeyUp:connect(function(key)
		if key=="w" then
			keys.w=false
		elseif key=="s" then
			keys.s=false
		elseif key=="a" then
			keys.a=false
		elseif key=="d" then
			keys.d=false
		end
	end)
	start()
end
pppp:Toggle("Fly",false,function(Value)
	Fly = Value
	activatefly()
end)
pppp:Toggle("No Clip",false,function(value)
	NoClip = value
end)
game:GetService("RunService").Heartbeat:Connect(
function()
	if NoClip or _G.Pole or _G.SwanGlasses then
		game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)
pppp:Label("Fake")
pppp:TextBox("Fake Bouty","",true,function(t)
	game:GetService("Players")["LocalPlayer"].leaderstats["Bounty/Honor"].Value = t
end)
pppp:TextBox("Fake Beli","", true, function(FakeBeli)
	game:GetService("Players")["LocalPlayer"].Data.Beli.Value = FakeBeli
end)
pppp:TextBox("Fake Level","", true, function(FakeLevel)
	game:GetService("Players")["LocalPlayer"].Data.Level.Value = FakeLevel
end)
pppp:TextBox("Fake Exp ","", true, function(FakeExp)
	game:GetService("Players")["LocalPlayer"].Data.Exp.Value = FakeExp
end)
pppp:TextBox("Fake Fragments","", true, function(FakeFragments)
	game:GetService("Players")["Localplayer"].Data.Fragments.Value = FakeFragments
end)
pppp:Label("Fake Stats")
pppp:TextBox("Fake Melee","", true, function(FakeMelee)
	game:GetService("Players")["LocalPlayer"].Data.Stats.Melee.Level.Value = FakeMelee
end)
pppp:TextBox("Fake Defense","", true, function(FakeDefense)
	game:GetService("Players")["localPlayer"].Data.Stats.Defense.Level.Value = FakeDefense
end)
pppp:TextBox("Fake Sword","", true, function(FakeSword)
	game:GetService("Players")["LocalPlayer"].Data.Stats.Sword.Level.Value = FakeSword
end)
pppp:TextBox("Fake Gun","", true, function(FakeGun)
	game:GetService("Players")["LocalPlayer"].Data.Stats.Gun.Level.Value = FakeGun
end)
pppp:TextBox("Fake Fruit","", true, function(FakeFruit)
	game:GetService("Players")["LocalPlayer"].Data.Stats["Demon Fruit"].Level.Value = FakeFruit
end)
pppp:Label("Haki Stage Select")
pppp:Button("Stage 0", function()
	local args = {
		[1] = "ChangeBusoStage",
		[2] = 0
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Button("Stage 1", function()
	local args = {
		[1] = "ChangeBusoStage",
		[2] = 1
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Button("Stage 2", function()
	local args = {
		[1] = "ChangeBusoStage",
		[2] = 2
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Button("Stage 3", function()
	local args = {
		[1] = "ChangeBusoStage",
		[2] = 3
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Button("Stage 4", function()
	local args = {
		[1] = "ChangeBusoStage",
		[2] = 4
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Button("Stage 5", function()
	local args = {
		[1] = "ChangeBusoStage",
		[2] = 5
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
pppp:Button("Redeem All Code", function()
	function UseCode(Text)
		game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Text)
	end
	UseCode("2BILLION")
	UseCode("THIRDSEA")
	UseCode("UPD15")
	UseCode("FUDD10")
	UseCode("BIGNEWS")
	UseCode("THEGREATACE")
	UseCode("SUB2GAMERROBOT_RESET1")
	UseCode("SUB2GAMERROBOT_EXP1")
	UseCode("StrawHatMaine")
	UseCode("Sub2OfficialNoobie")
	UseCode("SUB2NOOBMASTER123")
	UseCode("Sub2Daigrock")
	UseCode("Axiore")
	UseCode("TantaiGaming")
	UseCode("STRAWHATMAINE")
end)
local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
	vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
	wait(1)
	vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
pppp:Button("Remove Lave", function()
	for i,v in pairs(game.Workspace:GetDescendants()) do
		if v.Name == "Lava" then
			v:Destroy()
		end
	end
	for i,v in pairs(game.ReplicatedStorage:GetDescendants()) do
		if v.Name == "Lava" then
			v:Destroy()
		end
	end
end)
pppp:Button("FPS Boost", function()
	local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
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
pppp:Button("Super FPS Boost", function()
	for i,v in pairs(game.Workspace.Map:GetDescendants()) do
		if v.Name == "Tavern" or v.Name == "SmileFactory" or v.Name == "Tree" or v.Name == "Rocks" or v.Name == "PartHouse" or v.Name == "Hotel" or v.Name == "WallPiece" or v.Name == "MiddlePillars" or v.Name == "Cloud" or v.Name == "PluginGrass" or v.Name == "BigHouse" or v.Name == "SmallHouse" or v.Name == "Detail" then
			v:Destroy()
		end
	end 
	for i,v in pairs(game.ReplicatedStorage.Unloaded:GetDescendants()) do
		if v.Name == "Tavern" or v.Name == "SmileFactory" or v.Name == "Tree" or v.Name == "Rocks" or v.Name == "PartHouse" or v.Name == "Hotel" or v.Name == "WallPiece" or v.Name == "MiddlePillars" or v.Name == "Cloud" or v.Name == "PluginGrass" or v.Name == "BigHouse" or v.Name == "SmallHouse" or v.Name == "Detail" then
			v:Destroy()
		end
	end
	for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
		if v:IsA("Accessory") or v.Name == "Pants" or v.Name == "Shirt" then
			v:Destroy()
		end
	end
	local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
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
pppp:Label("Auto Farm Level Lock")
LockLevelValue = 2000
OldLevel = game.Players.localPlayer.Data.Level.Value
pppp:Slider("Select Level Lock", 1, LockLevelValue,LockLevelValue,function(value)
	LockLevelValue = value
end)
pppp:Toggle("Lock Level",false,function(value)
	LockLevel = value
end)
spawn(function()
	while wait(.1) do
		if LockLevel then
			if game.Players.localPlayer.Data.Level.Value >= LockLevelValue then
				game.Players.localPlayer:Kick("\n Auto Fram Completed Level : "..game.Players.localPlayer.Data.Level.Value.."\n Old Level : "..OldLevel.."\nUsername : "..game.Players.LocalPlayer.Name)
			end
		end
	end
end)
spawn(function()
	while wait(.1) do
		if AuctoClick then
			game:GetService'VirtualUser':CaptureController()
			game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
		end
	end
end)
local btns = window:Tap("Dunguen",6031094670)
btns:Label("AutoRaid")
btns:Dropdown("Select Microchip To Auto Raid",{"Flame","Ice","Quake","Light","Dark","String","Rumble","Magma","Human: Buddha"},function(t)
	selectchip = t
end)
btns:Toggle("Auto Raid",false,function(t)
	_G.autoraid = t
end)
game:GetService("RunService").RenderStepped:Connect(function()
	if _G.autoraid then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)

spawn(function()
	while wait(.1) do
		if _G.autoraid then
			if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
				if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1")  then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", selectchip)
				end
				if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or  game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip")  then
					if NewWorld then
						fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
					elseif NewWorld2 then
						fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
					end
				end
			end
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if _G.autoraid and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 500 then
					pcall(function()
						repeat wait(.1)
							if sethiddenproperty then
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							end
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
							v.HumanoidRootPart.CanCollide = false
							if v.Humanoid.Health > 0 then
								v.Humanoid.Health = 0
							elseif v.Humanoid.Health == 0 then
								v.Humanoid.Health = v.Humanoid.MaxHealth
							else
								v.Humanoid.Health = 0
							end
						until not _G.autoraid or not v.Parent or v.Humanoid.Health <= 0
					end)
				end
			end
			spawn(function()
				while wait() do
					pcall(function()
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
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
					end)
				end
			end)
			for i,v in pairs(game.Workspace:GetChildren()) do
				if string.find(v.Name, "Fruit") then
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
				end
			end
			if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
				if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
					wait(15)
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				end
			end
		end
	end
end)
spawn(function()
	while wait() do
		if _G.autoraid then
			local args = {
				[1] = "Cousin",
				[2] = "Buy"
			}

			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end
	end
end)
btns:Toggle("Auto Raid + Hop",false,function(t)
	_G.AutoRaid_Hop = t
end)
game:GetService("RunService").RenderStepped:Connect(function()
	if _G.AutoRaid_Hop then
		game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)

spawn(function()
	while wait(.1) do
		if _G.AutoRaid_Hop then
			if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
				if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1")  then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", selectchip)
				end
				if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or  game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip")  then
					if NewWorld then
						fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
					elseif NewWorld2 then
						fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
					end
				end
			end
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if _G.AutoRaid_Hop and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 500 then
					pcall(function()
						repeat wait(.1)
							if sethiddenproperty then
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							end
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
							v.HumanoidRootPart.CanCollide = false
							if v.Humanoid.Health > 0 then
								v.Humanoid.Health = 0
							elseif v.Humanoid.Health == 0 then
								v.Humanoid.Health = v.Humanoid.MaxHealth
							else
								v.Humanoid.Health = 0
							end
						until not _G.AutoRaid_Hop or not v.Parent or v.Humanoid.Health <= 0
					end)
				end
			end
			spawn(function()
				while wait() do
					pcall(function()
						if sethiddenproperty then
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
						end
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
						local args = {
							[1] = "Cousin",
							[2] = "Buy"
						}

						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					end)
				end
			end)
			for i,v in pairs(game.Workspace:GetChildren()) do
				if v:IsA "Tool" then
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
				end
			end
			if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
				if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
					wait(15)
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				end
				if not game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") and not game.Workspace:FindFirstChild("Fruit") then
					local PlaceID = game.PlaceId
					local AllIDs = {}
					local foundAnything = ""
					local actualHour = os.date("!*t").hour
					local Deleted = false
					function TPReturner()
						local Site;
						if foundAnything == "" then
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
						else
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
						end
						local ID = ""
						if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
							foundAnything = Site.nextPageCursor
						end
						local num = 0;
						for i,v in pairs(Site.data) do
							local Possible = true
							ID = tostring(v.id)
							if tonumber(v.maxPlayers) > tonumber(v.playing) then
								for _,Existing in pairs(AllIDs) do
									if num ~= 0 then
										if ID == tostring(Existing) then
											Possible = false
										end
									else
										if tonumber(actualHour) ~= tonumber(Existing) then
											local delFile = pcall(function()
												-- delfile("NotSameServers.json")
												AllIDs = {}
												table.insert(AllIDs, actualHour)
											end)
										end
									end
									num = num + 1
								end
								if Possible == true then
									table.insert(AllIDs, ID)
									wait()
									pcall(function()
										-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
										wait()
										game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
									end)
									wait(.1)
								end
							end
						end
					end
					function Teleport() 
						while wait() do
							pcall(function()
								TPReturner()
								if foundAnything ~= "" then
									TPReturner()
								end
							end)
						end
					end
					Teleport()
				end
			end
		end
	end
end)
btns:Label("--NorMal Raid--")
btns:Toggle("Kill Arua",false,function(value)
	_G.KillAura = value
end)
btns:Toggle("Auto Next Island",false,function(value)
	_G.NextIsland = value
end)
btns:Toggle("Auto Awakener",false,function(value)
	_G.Awakener = value
end)
btns:Button("Labbatle",function()
	if NewWorld then
		game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-6438.73535, 250.645355, -4501.50684)
	end
	if NewWorld2 then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5093.0385742188, 314.97863769531, -2924.8054199219)
	end
end)
btns:Button("Awakening Room", function()
	if NewWorld then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(266.227783, 1.39509034, 1857.00732)
	end
	if NewWorld2 then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1)
	end
end)


spawn(function()
	while wait(.1) do
		if _G.Awakener then
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
spawn(function()
	while wait(.1) do
		if _G.NextIsland then
			game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
			if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
				if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
					wait(15)
					tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(5, Enum.EasingStyle.Linear)
					tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0,10,10)})
					tween:Play()
				end
			end
		end
	end
end)
game:GetService("RunService").Heartbeat:Connect(
function()
	if _G.NextIsland then
		game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
	end
end)
spawn(function()
	while wait(.1) do
		if _G.KillAura then
			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
				if _G.KillAura and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 500 then
					pcall(function()
						repeat wait(.1)
							if sethiddenproperty then
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							end
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
							v.HumanoidRootPart.CanCollide = false
							if v.Humanoid.Health > 0 then
								v.Humanoid.Health = 0
							elseif v.Humanoid.Health == 0 then
								v.Humanoid.Health = v.Humanoid.MaxHealth
							else
								v.Humanoid.Health = 0
							end
						until not _G.KillAura or not v.Parent or v.Humanoid.Health <= 0
					end)
				end
			end
		end
	end
end)
btns:Label("--Buy Microchip--", true)
btns:Dropdown("Select Microchip To Buy",{"Flame","Ice","Quake","Light","Dark","String","Rumble","Magma","Human: Buddha"},function(t)
	BuyChip = t
end)
btns:Button("Buy Chip", function()
	local A_1 = "RaidsNpc"
	local A_2 = "Select"
	local A_3 = BuyChip
	local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
	Event:InvokeServer(A_1, A_2, A_3)
end)
local BuyItem = window:Tap("BuyItem",6031094670)
BuyItem:Label("--abilytys--", true)
BuyItem:Button("Skyjump", function()
	local args = {
		[1] = "BuyHaki",
		[2] = "Geppo"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Buso Haki",function()
	local args = {
		[1] = "BuyHaki",
		[2] = "Buso"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Soru",function()
	local args = {
		[1] = "BuyHaki",
		[2] = "Soru"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Label("--Fightingstyle--", true)
BuyItem:Button("Black Leg",function()
	local args = {
		[1] = "BuyBlackLeg"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Electro",function()
	local args = {
		[1] = "BuyElectro"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Fishman Karate", function()
	local args = {
		[1] = "BuyFishmanKarate"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Dragon Claw", function()
	local args = {
		[1] = "BlackbeardReward",
		[2] = "DragonClaw",
		[3] = "1"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "BlackbeardReward",
		[2] = "DragonClaw",
		[3] = "2"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Superhuman",function()
	local args = {
		[1] = "BuySuperhuman"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Death Step",function()
	local args = {
		[1] = "BuyDeathStep"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Sharkman Karate", function()
	local args = {
		[1] = "BuySharkmanKarate",
		[2] = true
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "BuySharkmanKarate"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Electric Claw",  function()
	local args = {
		[1] = "BuyElectricClaw",
		[2] = true
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "BuyElectricClaw"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Label("--random race--", true)
BuyItem:Button("random race",function()
	local A_1 = "BlackbeardReward"
	local A_2 = "Reroll"
	local A_3 = "2"
	local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
	Event:InvokeServer(A_1, A_2, A_3)
end)
BuyItem:Button("buy Stat refound", function()
	local A_1 = "BlackbeardReward"
	local A_2 = "Refund"
	local A_3 = "2"
	local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
	Event:InvokeServer(A_1, A_2, A_3)
end)
BuyItem:Button("Race Ghoul", function()
	local args = {
		[1] = "Ectoplasm",
		[2] = "BuyCheck",
		[3] = 4
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "Ectoplasm",
		[2] = "Change",
		[3] = 4
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Race Cyborg", function()
	local args = {
		[1] = "CyborgTrainer",
		[2] = "Buy"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Label("--Buy Sword--", true)
BuyItem:Button("Katana",  function()
	local args = {
		[1] = "BuyItem",
		[2] = "Katana"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Cutlass",  function()
	local args = {
		[1] = "BuyItem",
		[2] = "Cutlass"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Duel Katana",  function()
	local args = {
		[1] = "BuyItem",
		[2] = "Duel Katana"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Iron Mace", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Iron Mace"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Pipe", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Pipe"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Triple Katana", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Triple Katana"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Dual-Headed Blade", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Dual-Headed Blade"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Bisento", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Bisento"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Soul Cane", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Soul Cane"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("MidnightBlade", function()
	local A_1 = "Ectoplasm"
	local A_2 = "Buy"
	local A_3 = 3
	local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
	Event:InvokeServer(A_1, A_2, A_3)
end)
BuyItem:Label("--Buy gun--", true)
BuyItem:Button("Bizarre Rifle", function()
	local A_1 = "Ectoplasm"
	local A_2 = "Buy"
	local A_3 = 1
	local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
	Event:InvokeServer(A_1, A_2, A_3)
end)
BuyItem:Button("Slingshot", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Slingshot"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Musket", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Musket"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Flintlock", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Flintlock"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Refined Flintlock",function()
	local args = {
		[1] = "BuyItem",
		[2] = "Refined Flintlock"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Cannon", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Cannon"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Kabucha", function()
	local args = {
		[1] = "BlackbeardReward",
		[2] = "Slingshot",
		[3] = "1"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	local args = {
		[1] = "BlackbeardReward",
		[2] = "Slingshot",
		[3] = "2"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Label("Accessory")

BuyItem:Button("Black Cape", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Black Cape"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
BuyItem:Button("Toemo Ring", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Tomoe Ring"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

BuyItem:Button("Swordsman Hat", function()
	local args = {
		[1] = "BuyItem",
		[2] = "Swordsman Hat"
	}

	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
local Fruit = window:Tap("Devil Fruit",6031094670)
function EquipWeapon(ToolSe)
	if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
		local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
		wait(.4)
		game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end
end
Fruit:Toggle("Auto Drop Fruit", false, function(vu)
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
Fruit:Button("Buy Random Devil Fruit", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
end)
Fruit:Toggle("Auto Buy Random Devil Fruit",false,function(v)
	DevilAutoBuy = v
end)
spawn(function()
	while wait() do
		if DevilAutoBuy then wait()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
		end
	end
end)
Fruit:Toggle("Teleport Devil Fruit",false,function(value)
	TeleportDF = value
	pcall(function()
		while TeleportDF do wait()
			for i,v in pairs(game.Workspace:GetChildren()) do
				if string.find(v.Name, "Fruit") then 
					game.Players.LocalPlayer.Character.Humanoid:ChageState(11)
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
				end
			end
		end
	end)
end)
Fruit:Toggle("Bring Fruit",false,function(t)
	_G.BringFruit = t
end)
spawn(function()
	while wait() do
		if _G.BringFruit then
			pcall(function()
				for i,v in pairs(game.Workspace:GetChildren()) do
					if v:IsA("Tool") then
						if (v.Handle.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 500 then
							v.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
						elseif (v.Handle.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude >= 501 then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
						end
					end
				end
			end)
		end
	end
end)
SelectDevil = ""
CheckF = false
Fruit:Dropdown("AutoBuy DevilFruit",
	{
		"Bomb-Bomb",
		"Spike-Spike",
		"Chop-Chop",
		"Spring-Spring",
		"Kilo-Kilo",
		"Spin-Spin",
		"Bird: Falcon",
		"Smoke-Smoke",
		"Flame-Flame",
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
		"Vemon-Vemon",
		"Control-Control",
		"Dragon-Dragon"
	}
	,function(ply)
		SelectDevil = ply
	end)
Fruit:Toggle("Buy Devil Fruit Sinper",false,function(value)
	BuyFruitSinper = vu
end)
spawn(function()
	while wait(.1) do
		if BuyFruitSinper then
			local args = {
				[1] = "GetFruits"
			}

			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			local args = {
				[1] = "PurchaseRawFruit",
				[2] = SelectDevil
			}

			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end 
	end
end)
local k = window:Tap("Setting",6031094670)
k:Label("--Setting--", true)
_G.X = 0
k:Slider("Position X", 1, 100,0,function(t)
	_G.X = t
end)
_G.Y = 0
k:Slider("Position Y", 1, 100,15,function(t)
	_G.Y = t
end)
_G.Z = 0
k:Slider("Position Z", 1, 100,0,function(t)
	_G.Z = t
end)
------------------------ MON ---------------------
_G.XM = 0
k:Slider("Position X MON", 1, 100,0,function(t)
	_G.XM = t
end)
_G.YM = 15
k:Slider("Position Y MON", 1, 100,15,function(t)
	_G.YM = t
end)
_G.ZM = 0
k:Slider("Position Z MON", 1, 100,0,function(t)
	_G.ZM = t
end)
k:Toggle("Bring Mob",true,function(t)
	_G.BringMob = t
end)
k:Toggle("Ghost Mob",false, function(vu)
	HiddenMon = vu
end)
spawn(function()
	while wait() do
		pcall(function()
			if _G.FarmLevel and HiddenMon then
				for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
					if v.ClassName == "MeshPart" then
						v.Transparency = 1
					end
				end
				for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
					if v.Name == "Head" then
						v.Transparency = 1
					end
				end
				for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
					if v.ClassName == "Accessory" then
						v.Handle.Transparency = 1
					end
				end
			end
		end)
	end
end)

spawn(function()
	while game:GetService("RunService").RenderStepped:wait() do
		if _G.BringMob then
			sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
		end
	end
end)
spawn(function()
	while game:GetService("RunService").RenderStepped:wait() do
		if _G.BringMob then
			pcall(function()
				repeat
					game:GetService("RunService").RenderStepped:wait()
					for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
						for k,x in pairs(game.Workspace.Enemies:GetChildren()) do
							if x.Name == "Ship Deckhand [Lv. 1250]" then
								if v.Name == "Ship Deckhand [Lv. 1250]" then
									x.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
									BRINGMOB = x.HumanoidRootPart.CFrame
									x.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.CanCollide = false
									if sethiddenproperty then
										sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
									end
								end
							end
						end
					end
				until
				game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false or _G.BringMob == false or game:GetService("Players").LocalPlayer.Character.Humanoid.Health <= 0
			end)
		end
	end
end)
k:Toggle("Anit AFK",true,function(vu)
	local vu = game:GetService("VirtualUser")
	game:GetService("Players").LocalPlayer.Idled:connect(function()
		vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
		wait(1)
		vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
	end)
end)
_G.AUTOHAKI = true
k:Toggle("Auto Haki",true,function(Value)
	_G.AUTOHAKI = Value
end)
k:Toggle("Auto Observation haki",false,function(Value)
	AUTOHAKIObs = Value  
end)
spawn(function()
	while wait(.1) do
		if _G.AUTOHAKI then
			if game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then

			else
				local args = {
					[1] = "Buso"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end
		end
		if AUTOHAKIObs then
			if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then

			else wait(1)
				local virtualUser = game:GetService('VirtualUser')
				virtualUser:CaptureController()

				virtualUser:SetKeyDown('0x65')
				wait(2)
				virtualUser:SetKeyUp('0x65')
			end
		end
	end
end)
k:Toggle("Hide HitBlox",true,function(Value)
	HideHitBlox = Value  
end)
k:Label("--Auto Skill Farm mastery--", true)
k:Toggle("Skill Z",true,function(a)
	SkillZ = a
end)
k:Toggle("Skill X",true,function(a)
	SkillX = a
end)
k:Toggle("Skill C",true,function(a)
	SkillC = a
end)
k:Toggle("Skill V",true,function(a)
	SkillV = a
end)
k:Button("Destroy GUI", function()
	local ui = game:GetService("CoreGui").Whiteui
	if ui then
		ui:Destroy()
	end
end)
k:Button("Rejoin", function()
	local ts = game:GetService("TeleportService")
	local p = game:GetService("Players").LocalPlayer
	ts:Teleport(game.PlaceId, p)
end)
local function HttpGet(url)
	return game:GetService("HttpService"):JSONDecode(htgetf(url))
end
k:Button("Server Hop", function()
	local PlaceID = game.PlaceId
	local AllIDs = {}
	local foundAnything = ""
	local actualHour = os.date("!*t").hour
	local Deleted = false
	function TPReturner()
		local Site;
		if foundAnything == "" then
			Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
		else
			Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
		end
		local ID = ""
		if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
			foundAnything = Site.nextPageCursor
		end
		local num = 0;
		for i,v in pairs(Site.data) do
			local Possible = true
			ID = tostring(v.id)
			if tonumber(v.maxPlayers) > tonumber(v.playing) then
				for _,Existing in pairs(AllIDs) do
					if num ~= 0 then
						if ID == tostring(Existing) then
							Possible = false
						end
					else
						if tonumber(actualHour) ~= tonumber(Existing) then
							local delFile = pcall(function()
								-- delfile("NotSameServers.json")
								AllIDs = {}
								table.insert(AllIDs, actualHour)
							end)
						end
					end
					num = num + 1
				end
				if Possible == true then
					table.insert(AllIDs, ID)
					wait()
					pcall(function()
						-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
						wait()
						game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
					end)
					wait(.1)
				end
			end
		end
	end
	function Teleport() 
		while wait() do
			pcall(function()
				TPReturner()
				if foundAnything ~= "" then
					TPReturner()
				end
			end)
		end
	end
	Teleport()
end)
k:Button("TelePort To Lower Server", function()
	getgenv().AutoTeleport = true
	getgenv().DontTeleportTheSameNumber = true --If you set this true it won't teleport to the server if it has the same number of players as your current server
	getgenv().CopytoClipboard = true


	if not game:IsLoaded() then
		rconsoleprint("\nGame is loading waiting... | Amnesia Empty Server Finder")
		repeat
			wait()
		until game:IsLoaded()
	end

	local maxplayers = math.huge
	local serversmaxplayer;
	local goodserver;
	local gamelink = "https://games.roblox.com/v1/games/" .. game.PlaceId .. "/servers/Public?sortOrder=Asc&limit=100"

	function serversearch()
		for _, v in pairs(game:GetService("HttpService"):JSONDecode(game:HttpGetAsync(gamelink)).data) do
			if type(v) == "table" and maxplayers > v.playing then
				serversmaxplayer = v.maxPlayers
				maxplayers = v.playing
				goodserver = v.id
			end
		end
		rconsoleprint("\nCurrently checking the servers with max this number of players : " .. maxplayers .. " | Amnesia Empty Server Finder")
	end

	function getservers()
		serversearch()
		for i,v in pairs(game:GetService("HttpService"):JSONDecode(game:HttpGetAsync(gamelink))) do
			if i == "nextPageCursor" then
				if gamelink:find("&cursor=") then
					local a = gamelink:find("&cursor=")
					local b = gamelink:sub(a)
					gamelink = gamelink:gsub(b, "")
				end
				gamelink = gamelink .. "&cursor=" ..v
				getservers()
			end
		end
	end

	getservers()

	rconsoleprint("\nAll of the servers are searched") 
	rconsoleprint("\nServer : " .. goodserver .. " Players : " .. maxplayers .. "/" .. serversmaxplayer .. " | Amnesia Empty Server Finder")
	if CopytoClipboard then
		rconsoleprint(goodserver)
	end
	if AutoTeleport then
		if DontTeleportTheSameNumber then 
			if #game:GetService("Players"):GetPlayers() - 1 == maxplayers then
				return rconsoleprint("\nIt has same number of players (except you)")
			elseif goodserver == game.JobId then
				return rconsoleprint("\nYour current server is the most empty server atm") 
			end
		end
		rconsoleprint("\nAutoTeleport is enabled. Teleporting to : " .. goodserver)
		game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId, goodserver)
	end
end)

spawn(function()
    while wait(.1) do
		pcall(function()
			if _G.hopme then
				for i,v in pairs(game.Players:GetChildren()) do
				if v.Name ~= game.Players.LocalPlayer.Name then
					if v.Name:find(_G.nameme) then
						print("Hop")
						local PlaceID = game.PlaceId
							local AllIDs = {}
							local foundAnything = ""
							local actualHour = os.date("!*t").hour
							local Deleted = false
							function TPReturner()
								local Site;
								if foundAnything == "" then
									Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
								else
									Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
								end
								local ID = ""
								if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
									foundAnything = Site.nextPageCursor
								end
								local num = 0;
								for i,v in pairs(Site.data) do
									local Possible = true
									ID = tostring(v.id)
									if tonumber(v.maxPlayers) > tonumber(v.playing) then
										for _,Existing in pairs(AllIDs) do
											if num ~= 0 then
												if ID == tostring(Existing) then
													Possible = false
												end
											else
												if tonumber(actualHour) ~= tonumber(Existing) then
													local delFile = pcall(function()
														-- delfile("NotSameServers.json")
														AllIDs = {}
														table.insert(AllIDs, actualHour)
													end)
												end
											end
											num = num + 1
										end
										if Possible == true then
											table.insert(AllIDs, ID)
											wait()
											pcall(function()
												-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
												wait()
												game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
											end)
											wait(2)
										end
									end
								end
							end
							function Teleport()
								while wait() do
									pcall(function()
										TPReturner()
										if foundAnything ~= "" then
											TPReturner()
										end
									end)
								end
							end
							Teleport()
					end
					end
				end
			end	
		end)
    end
end)



spawn(function()
    while wait() do
    pcall(function()
        if not game:IsLoaded() then
            game.Loaded:Wait()
        end
        game.CoreGui.RobloxPromptGui.promptOverlay.DescendantAdded:Connect(function()
            local GUI = game.CoreGui.RobloxPromptGui.promptOverlay:FindFirstChild("ErrorPrompt")
            if GUI then
                if GUI.TitleFrame.ErrorTitle.Text == "Disconnected" then
                    if #game.Players:GetPlayers() <= 1 then
                        game.Players.LocalPlayer:Kick("\nRejoining...")
                        wait()
                        game:GetService("TeleportService"):Teleport(game.PlaceId, game.Players.LocalPlayer)
                    else
                        game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId, game.JobId, game.Players.LocalPlayer)
                    end
                end
            end
        end)
    end)
    end
end)

