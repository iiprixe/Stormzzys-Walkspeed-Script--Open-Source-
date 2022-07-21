--// BY STORMZZY Stormzzy#4968 \\--

local ScreenGui = Instance.new("ScreenGui")
local Holder = Instance.new("Frame")
local HEADER = Instance.new("TextLabel")
local WS = Instance.new("TextBox")
local UICorner = Instance.new("UICorner")
local SETWS = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local SETJP = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local JP = Instance.new("TextBox")
local UICorner_4 = Instance.new("UICorner")
local UICorner_5 = Instance.new("UICorner")

ScreenGui.Parent = game.Players.LocalPlayer.PlayerGui

Holder.Name = "Holder"
Holder.Parent = ScreenGui
Holder.BackgroundColor3 = Color3.fromRGB(24, 24, 24)
Holder.BorderSizePixel = 0
Holder.Position = UDim2.new(0.157043844, 0, 0.550795615, 0)
Holder.Size = UDim2.new(0, 294, 0, 187)

HEADER.Name = "HEADER"
HEADER.Parent = Holder
HEADER.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
HEADER.BackgroundTransparency = 1.000
HEADER.Position = UDim2.new(0.157021835, 0, 0.0347593576, 0)
HEADER.Size = UDim2.new(0, 200, 0, 50)
HEADER.Font = Enum.Font.GothamBold
HEADER.Text = "Set WS/JP Gui, By Stormzzy"
HEADER.TextColor3 = Color3.fromRGB(255, 255, 255)
HEADER.TextSize = 24.000
HEADER.TextWrapped = true

WS.Name = "WS"
WS.Parent = Holder
WS.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
WS.BorderSizePixel = 0
WS.Position = UDim2.new(0.728450418, 0, 0.362490475, 0)
WS.Size = UDim2.new(0, 69, 0, 50)
WS.Font = Enum.Font.GothamBold
WS.PlaceholderText = "WS"
WS.Text = ""
WS.TextColor3 = Color3.fromRGB(255, 255, 255)
WS.TextSize = 13.000

UICorner.Parent = WS

SETWS.Name = "SETWS"
SETWS.Parent = Holder
SETWS.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
SETWS.Position = UDim2.new(0.0260032788, 0, 0.362490475, 0)
SETWS.Size = UDim2.new(0, 200, 0, 50)
SETWS.Font = Enum.Font.GothamBold
SETWS.Text = "Set WS"
SETWS.TextColor3 = Color3.fromRGB(255, 255, 255)
SETWS.TextSize = 14.000

UICorner_2.Parent = SETWS

SETJP.Name = "SETJP"
SETJP.Parent = Holder
SETJP.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
SETJP.Position = UDim2.new(0.0294046402, 0, 0.672650933, 0)
SETJP.Size = UDim2.new(0, 200, 0, 50)
SETJP.Font = Enum.Font.GothamBold
SETJP.Text = "Set JP"
SETJP.TextColor3 = Color3.fromRGB(255, 255, 255)
SETJP.TextSize = 14.000

UICorner_3.Parent = SETJP

JP.Name = "JP"
JP.Parent = Holder
JP.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
JP.BorderSizePixel = 0
JP.Position = UDim2.new(0.731851757, 0, 0.672650933, 0)
JP.Size = UDim2.new(0, 69, 0, 50)
JP.Font = Enum.Font.GothamBold
JP.PlaceholderText = "JP"
JP.Text = ""
JP.TextColor3 = Color3.fromRGB(255, 255, 255)
JP.TextSize = 13.000

UICorner_4.Parent = JP

UICorner_5.CornerRadius = UDim.new(0, 14)
UICorner_5.Parent = Holder

-- Scripts:

local function IDFXVRT_fake_script() -- SETWS.LocalScript 
	local script = Instance.new('LocalScript', SETWS)

	local ws = script.Parent.Parent.WS

	script.Parent.MouseButton1Down:Connect(function()
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = ws.Text
	end)
end
coroutine.wrap(IDFXVRT_fake_script)()
local function OOACMJU_fake_script() -- SETJP.LocalScript 
	local script = Instance.new('LocalScript', SETJP)

	local jp = script.Parent.Parent.JP

	script.Parent.MouseButton1Down:Connect(function()
		game.Players.LocalPlayer.Character.Humanoid.JumpPower = jp.Text
	end)
end
coroutine.wrap(OOACMJU_fake_script)()
local function FQFV_fake_script() -- Holder.Dragify 
	local script = Instance.new('LocalScript', Holder)

	local UIS = game:GetService("UserInputService")
	function dragify(Frame)
		dragToggle = nil
		local dragSpeed = 0.50
		dragInput = nil
		dragStart = nil
		local dragPos = nil
		function updateInput(input)
			local Delta = input.Position - dragStart
			local Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + Delta.X, startPos.Y.Scale, startPos.Y.Offset + Delta.Y)
			game:GetService("TweenService"):Create(Frame, TweenInfo.new(0.30), {Position = Position}):Play()
		end
		Frame.InputBegan:Connect(function(input)
			if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) and UIS:GetFocusedTextBox() == nil then
				dragToggle = true
				dragStart = input.Position
				startPos = Frame.Position
				input.Changed:Connect(function()
					if input.UserInputState == Enum.UserInputState.End then
						dragToggle = false
					end
				end)
			end
		end)
		Frame.InputChanged:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
				dragInput = input
			end
		end)
		game:GetService("UserInputService").InputChanged:Connect(function(input)
			if input == dragInput and dragToggle then
				updateInput(input)
			end
		end)
	end

	dragify(script.Parent)
end
coroutine.wrap(FQFV_fake_script)()
