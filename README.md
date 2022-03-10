ModIDS = { 
   1819673174,
   79287609,
    2828200349,
     15893719,
   3150684934,
   3215776050, 
   3211439829,
    3245366071,
     290495126,
    3167962445,
    1261255280,
     490432634,
     97710388,
     2037237498,
    3243685679,
    572632422,
   121588554,
  3323456791,
 28346134,
 2553294052,
3247793465,
130001960,
2795701619,
2309750621,
688350923,
1853772442,
360645202,
2564411817,

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
