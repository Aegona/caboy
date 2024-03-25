local replicatedStorage = game:GetService("ReplicatedStorage")
local generalEvents = replicatedStorage:WaitForChild("GeneralEvents")
local robEvent = generalEvents:WaitForChild("Rob")
local hr = game.Players.LocalPlayer.Character.HumanoidRootPart
local cashRegister = workspace:WaitForChild("CashRegister")

function Rob()
	local args = {
		[1] = "Register",
		[2] = {
			["Part"] = cashRegister:WaitForChild("Union"),
			["Active"] = true,
			["ActiveValue"] = cashRegister:WaitForChild("Active"),
			["OpenPart"] = cashRegister:WaitForChild("Open")
		}
	}

	robEvent:FireServer(unpack(args))
end


function tp()
	hr.CFrame = CFrame.new(1477.5528564453125, 132.84959411621094, 1658.643310546875)
	wait(3)
	hr.CFrame = CFrame.new(1342.0335693359375, 126.75310516357422, 1883.2281494140625)
	wait(0.5)
	hr.CFrame = CFrame.new(1477.5528564453125, 132.84959411621094, 1658.643310546875)
	wait(1)
	hr.CFrame = CFrame.new(1342.0335693359375, 126.75310516357422, 1883.2281494140625)
	wait(20)
	hr.CFrame = CFrame.new(1477.5528564453125, 132.84959411621094, 1658.643310546875)
	wait(0.1)
end

while _G.Farm do
	Rob()
	tp()
end



local AegonaHub = Instance.new("ScreenGui")
local Toogle = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local TextButton = Instance.new("TextButton")
local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
local UITextSizeConstraint = Instance.new("UITextSizeConstraint")
local UIAspectRatioConstraint_2 = Instance.new("UIAspectRatioConstraint")
local BG = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local TextButton_2 = Instance.new("TextButton")
local UIAspectRatioConstraint_3 = Instance.new("UIAspectRatioConstraint")
local UITextSizeConstraint_2 = Instance.new("UITextSizeConstraint")
local TextLabel = Instance.new("TextLabel")
local UIAspectRatioConstraint_4 = Instance.new("UIAspectRatioConstraint")
local UITextSizeConstraint_3 = Instance.new("UITextSizeConstraint")
local UIAspectRatioConstraint_5 = Instance.new("UIAspectRatioConstraint")

--Properties:

AegonaHub.Name = "AegonaHub"
AegonaHub.Parent = game.CoreGui
AegonaHub.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Toogle.Name = "Toogle"
Toogle.Parent = AegonaHub
Toogle.BackgroundColor3 = Color3.fromRGB(65, 65, 65)
Toogle.BorderColor3 = Color3.fromRGB(0, 0, 0)
Toogle.BorderSizePixel = 0
Toogle.Position = UDim2.new(0.328000009, 0, -0.0149999997, 0)
Toogle.Size = UDim2.new(0.341623992, 0, 0.0150375944, 0)

UICorner.Parent = Toogle

TextButton.Parent = Toogle
TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton.BackgroundTransparency = 1.000
TextButton.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextButton.BorderSizePixel = 0
TextButton.Size = UDim2.new(1, 0, 1, 0)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = ""
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextScaled = true
TextButton.TextSize = 14.000
TextButton.TextWrapped = true

UIAspectRatioConstraint.Parent = TextButton
UIAspectRatioConstraint.AspectRatio = 38.917

UITextSizeConstraint.Parent = TextButton
UITextSizeConstraint.MaxTextSize = 14

UIAspectRatioConstraint_2.Parent = Toogle
UIAspectRatioConstraint_2.AspectRatio = 38.917

BG.Name = "BG"
BG.Parent = AegonaHub
BG.BackgroundColor3 = Color3.fromRGB(65, 65, 65)
BG.BorderColor3 = Color3.fromRGB(0, 0, 0)
BG.BorderSizePixel = 0
BG.Position = UDim2.new(0.328999996, 0, 0.999000013, 0)
BG.Size = UDim2.new(0.341623992, 0, 0.273182958, 0)
BG.Visible = false

UICorner_2.Parent = BG

TextButton_2.Parent = BG
TextButton_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton_2.BackgroundTransparency = 1.000
TextButton_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextButton_2.BorderSizePixel = 0
TextButton_2.Position = UDim2.new(0, 0, 0.229357794, 0)
TextButton_2.Size = UDim2.new(1, 0, 0.229357794, 0)
TextButton_2.Font = Enum.Font.SourceSansBold
TextButton_2.Text = "AutoFarm"
TextButton_2.TextColor3 = Color3.fromRGB(255, 255, 255)
TextButton_2.TextScaled = true
TextButton_2.TextSize = 14.000
TextButton_2.TextWrapped = true

UIAspectRatioConstraint_3.Parent = TextButton_2
UIAspectRatioConstraint_3.AspectRatio = 9.340

UITextSizeConstraint_2.Parent = TextButton_2
UITextSizeConstraint_2.MaxTextSize = 50

TextLabel.Parent = BG
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.BorderSizePixel = 0
TextLabel.Position = UDim2.new(0.323340476, 0, 0.536697268, 0)
TextLabel.Size = UDim2.new(0.351177722, 0, 0.188073397, 0)
TextLabel.Font = Enum.Font.SourceSansBold
TextLabel.Text = "Stats : OFF"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

UIAspectRatioConstraint_4.Parent = TextLabel
UIAspectRatioConstraint_4.AspectRatio = 4.000

UITextSizeConstraint_3.Parent = TextLabel
UITextSizeConstraint_3.MaxTextSize = 41

UIAspectRatioConstraint_5.Parent = BG
UIAspectRatioConstraint_5.AspectRatio = 2.142

-- Scripts:

local function POZU_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

	local bg = script.Parent.Parent.Parent.BG
	local de = true
	script.Parent.MouseButton1Click:Connect(function()
		if bg.Visible == false and de == true then
			de = false
			bg.Visible = true
			bg:TweenPosition(UDim2.new(0.328, 0,0.053, 0),Enum.EasingDirection.InOut,Enum.EasingStyle.Quad,1.5)
			wait(1)
			de = true
		elseif bg.Visible == true and de == true then
			de = false
			bg:TweenPosition(UDim2.new(0.328, 0,0.999, 0),Enum.EasingDirection.InOut,Enum.EasingStyle.Quad,1.5)
			wait(1.6)
			bg.Visible = false
			wait(1)
			de = true
		end		
	
	end)
end
coroutine.wrap(POZU_fake_script)()
local function YYNOHT_fake_script() -- TextButton_2.LocalScript 
	local script = Instance.new('LocalScript', TextButton_2)

	script.Parent.MouseButton1Click:Connect(function()
		if script.Parent.Parent.Value.Value == 0 then
			script.Parent.Parent.Value.Value = 1
			script.Parent.Parent.TextLabel.Text = "Stats : ON"
			_G.Farm = true
		elseif script.Parent.Parent.Value.Value == 1 then
			script.Parent.Parent.Value.Value = 0
			script.Parent.Parent.TextLabel.Text = "Stats : OFF"
			_G.Farm = false
		end
	end)
end
coroutine.wrap(YYNOHT_fake_script)()



