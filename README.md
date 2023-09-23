local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("YouTube Example Hub", "Ocean")
    
    
    -- MAIN
    local Main = Window:NewTab("Main")
    local MainSection = Main:NewSection("Main")


    MainSection:NewButton("FlyScript", "Gives your flying script.", function()
        loadstring(game:HttpGet('https://pastebin.com/raw/wKKxxg2e'))()
    end)
    MainSection:NewSlider("Walkspeed", "SPEED!!", 500, 16, function(s)
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
    end)

    MainSection:NewSlider("Jumppower", "JUMP HIGH!!", 350, 50, function(s)
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
    end)

    MainSection:NewButton("Reset WS/JP", "Resets to all defaults", function()
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 50
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
    end)


    --Combat
    local Combat = Window:NewTab("Combat")
    local CombatSection = Combat:NewSection("Combat")
    
    
    CombatSection:NewButton("COMBAT ESP", "Gives you a combatesp script.", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/Varap228/Hitbox-by-Varap/main/Code%20hitbox.lua', true))()
    end)

end

end "" 
