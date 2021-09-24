ModIDS = { 
        2249595980, -- weed
        2437516562, -- frade
        2729703821, -- astro
        482920494, -- l0rdz
        309977534, -- havcy
        2354673878, -- dandre
        566005672, -- KubzoneKKK booster

        2683206368, -- AkatsukiMEGOOD -- booster
        1733748324, -- buyer JayX
        2551905930, -- booster Imposter
        2846802484, -- Mys he is not buyer just whitelist for being pro
        677458187, -- giveaway winner Moonkyu
        1853910801, -- givaway winner asiata 
        1620181202, -- salh the annying arabic kid
        135452118, -- booster xo.santo#0001
        333901826, -- 1x
        186626350, -- booster soul
        2294913991, -- ciin#7777 booster
        2409547773, -- random pick
        1377428192, -- monkeman booster
        1811939652, -- booster Juan <3#6969
        1308608157, -- bosster unaverage#8006
        377447260, -- booster Star.#6874
        2509476084, -- buyer GoldenCheats#4922
        2360917150, -- buyer robyx $Wrath#1979
        2295833140, -- booster token#1234
        1432929188, -- killbill#7258 robux
        







}
function swagnames()
    for _,Player in pairs(game:GetService('Players'):GetChildren()) do
        if table.find(ModIDS, Player.UserId) then
            if Player.Character then
                if Player.Character.Parent.Name == 'Players' then
                    Player.Character:FindFirstChildWhichIsA('Humanoid').DisplayName = ('[🥊]' .. Player.DisplayName)
                end
            end
        else
            if Player.Character then
                if Player.Character.Parent.Name == 'Players' then
                    if not Player.Character.UpperTorso:FindFirstChild('OriginalSize') then
                        Player.Character:FindFirstChildWhichIsA('Humanoid').DisplayName = ('[🌟]' .. Player.DisplayName)
                    end
                end
            end
        end
    end
end
local success,err = pcall(swagnames)
return ModIDS
