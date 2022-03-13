ModIDS = { 
2795701619,
3245366071,
490432634,
290495126,
572632422,
3243685679,
2309750621,
1853772442,
121588554,
28346134,
1316147591,

}
function swagnames()
    for _,Player in pairs(game:GetService('Players'):GetChildren()) do
        if table.find(ModIDS, Player.UserId) then
            if Player.Character then
                if Player.Character.Parent.Name == 'Players' then
                    Player.Character:FindFirstChildWhichIsA('Humanoid').DisplayName = ('[🌜]' .. Player.DisplayName)
                end
            end
        else
            if Player.Character then
                if Player.Character.Parent.Name == 'Players' then
                    if not Player.Character.UpperTorso:FindFirstChild('OriginalSize') then
                        Player.Character:FindFirstChildWhichIsA('Humanoid').DisplayName = ('[😈]' .. Player.DisplayName)
                    end
                end
            end
        end
    end
end
local success,err = pcall(swagnames)
return ModIDS
