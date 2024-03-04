# Roblox GUI Animation Modular

This project provides a modular script in Lua scripting language for animating GUI objects in Roblox. The script allows you to pass a GUI object that you want to animate as well as the duration of the animation as parameters. Additionally, you can specify special properties for each object to customize the animation.

## Usage

To use the provided modular script:

1. Create a new modular script file in ReplicatedStorage in your Roblox game.
2. Copy and paste the contents of the provided modular script into the new modular script file.
3. In any local script where you want to animate a GUI object, call the provided function with the necessary parameters:

the module script contains a main  function as setupButton(button,property,value,duration)
  # button
  the gui object that needs to be animate should pass here as an object
  # property
  the property of the gui object that need to be changed in orderto animate should pass here as an String. For example think you need to edit the imagetransparency on mouse   enter. the just pass the "ImageTransparency"
  # value
  the effect of the change of the property value is managed by here. pass the amount
  # duration
  the time duration of the animation is handled in here

  ## example code
```lua
local GuiEffectsModular = require(game.ServerScriptService.GuiEffectsModular)

-- Get the image button (assuming it's named "ImageButton")
local imageButton = script.Parent.ImageButton

-- Define animation properties
local property = "ImageTransparency"
local value = 0.5 -- Target transparency value
local duration = 0.2 -- Duration of the animation in seconds

-- Set up button effects
GuiEffectsModular.setupButton(imageButton, property, value, duration)
```

Contributing
Contributions to improve or extend the functionality of this script are welcome! Fork the repository, make your changes, and submit a pull request.

License
This project is licensed under the MIT License.

Contact
For any inquiries or support, please contact samupuff@gmail.com or open an issue in the GitHub repository.
