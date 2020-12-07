-- Gui to Lua
-- Version: 3.2

-- Instances:

local sitetestD = Instance.new("ScreenGui")
local Holder = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local Title = Instance.new("TextLabel")
local Descriptor = Instance.new("TextLabel")
local NameInput = Instance.new("TextBox")
local UICorner_2 = Instance.new("UICorner")
local DrawToConfirm = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")

--Properties:

sitetestD.Name = "sitetestD"
sitetestD.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
sitetestD.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Holder.Name = "Holder"
Holder.Parent = sitetestD
Holder.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
Holder.Position = UDim2.new(0.0143403448, 0, 0.685151994, 0)
Holder.Size = UDim2.new(0, 261, 0, 167)

UICorner.CornerRadius = UDim.new(0, 13)
UICorner.Parent = Holder

Title.Name = "Title"
Title.Parent = Holder
Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Title.BackgroundTransparency = 1.000
Title.Position = UDim2.new(0.114942528, 0, 0.0538922139, 0)
Title.Size = UDim2.new(0, 200, 0, 32)
Title.Font = Enum.Font.Roboto
Title.Text = "<b>Scuffed ESP</b>"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextSize = 20.000

Descriptor.Name = "Descriptor"
Descriptor.Parent = Holder
Descriptor.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Descriptor.BackgroundTransparency = 1.000
Descriptor.Position = UDim2.new(0.0613026805, 0, 0.245508984, 0)
Descriptor.Size = UDim2.new(0, 229, 0, 63)
Descriptor.Font = Enum.Font.Roboto
Descriptor.Text = "Please input the name of the user you want to draw a line to."
Descriptor.TextColor3 = Color3.fromRGB(255, 255, 255)
Descriptor.TextSize = 20.000
Descriptor.TextWrapped = true
Descriptor.TextYAlignment = Enum.TextYAlignment.Top

NameInput.Name = "NameInput"
NameInput.Parent = Holder
NameInput.BackgroundColor3 = Color3.fromRGB(42, 42, 42)
NameInput.Position = UDim2.new(0.0613026805, 0, 0.700599015, 0)
NameInput.Size = UDim2.new(0, 127, 0, 36)
NameInput.ClearTextOnFocus = false
NameInput.Font = Enum.Font.Roboto
NameInput.Text = ""
NameInput.TextColor3 = Color3.fromRGB(255, 255, 255)
NameInput.TextSize = 14.000

UICorner_2.Parent = NameInput

DrawToConfirm.Name = "DrawToConfirm"
DrawToConfirm.Parent = Holder
DrawToConfirm.BackgroundColor3 = Color3.fromRGB(37, 202, 106)
DrawToConfirm.Position = UDim2.new(0.609195352, 0, 0.700599015, 0)
DrawToConfirm.Size = UDim2.new(0, 86, 0, 36)
DrawToConfirm.Font = Enum.Font.Roboto
DrawToConfirm.Text = "DRAW LINE"
DrawToConfirm.TextColor3 = Color3.fromRGB(0, 0, 0)
DrawToConfirm.TextSize = 13.000

UICorner_3.CornerRadius = UDim.new(0, 6)
UICorner_3.Parent = DrawToConfirm

-- Scripts:

local function HXLN_fake_script() -- DrawToConfirm.LocalScript 
	local script = Instance.new('LocalScript', DrawToConfirm)

	-- Development used for upcoming Drawing instance for Roblox. Currently on sitetest1.
	-- documentation found on rblx.co/drawing
	script.Parent.MouseButton1Click:Connect(function() -- Connect a function which draws a line
	local Torso = game:GetService("Players")(script.Parent.Parent.NameInput.Text).Character.Torso -- What the beam hooks to.
	local LocalTorso = game:GetService("Players").LocalPlayer.Character.Torso
	
	local beamed = Instance.new("Beam") -- Creates new beam.
	-- BEAM CONFIG --
	beamed.Parent = LocalTorso
	beamed.Color = Color3.fromRGB(255, 255, 255)
	beamed.LightEmission = 0
	beamed.LightInfluence = 1
	beamed.Width0 = 0.1
	beamed.Width1 = 0.1
	
	local Attach1 = Instance.new("Attachment")
	-- ATTACHMENT1 CONFIG --
	Attach1.Parent = LocalTorso -- Only thing we basically need.
	
	local Attach2 = Instance.new("Attachment")
	-- ATTACHMENT2 CONFIG --
	Attach2.Parent = Torso -- Once again all we need for attaching.
	
	-- SETTING UP PLACEMENT --
	
	beamed.Attachment0 = Attach1
	beamed.Attachment1 = Attach2
	end
end
coroutine.wrap(HXLN_fake_script)()
