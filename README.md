# Passenger-Traffic-Regression

The purpose of this project is to assess how well the suggested passenger traffic model predicts passenger traffic based on model inputs and in comparison with existing intra-African air passenger traffic values to and from Kenya. The data is contained in an excel file and contains different variables that are assummed to have an effect on air passenger traffic numbers.
The model is based on the following relationship between traffic and the chosen variables:

    𝑇𝑟𝑎𝑓𝑓𝑖𝑐 = 𝐹(𝐺𝐷𝑃,𝐷𝑖𝑠𝑡𝑎𝑛𝑐𝑒,𝐴𝑆𝐴,𝑉𝑖𝑠𝑎 𝑅𝑒𝑔𝑢𝑙𝑎𝑡𝑖𝑜𝑛𝑠,𝐵𝑢𝑠.𝐷𝑒𝑠𝑡.,𝑇𝑜𝑢𝑟.𝐷𝑒𝑠𝑡.,𝐿𝑎𝑛𝑔𝑢𝑎𝑔𝑒)

This model is expressed in the following log-linear form: 

    𝑙𝑛(𝑇𝑟𝑎𝑓𝑓𝑖𝑐) = 𝛽 + 𝛽1𝑙𝑛(𝐺𝐷𝑃) + 𝛽2𝑙𝑛(𝐷𝑖𝑠𝑡𝑎𝑛𝑐𝑒) + 𝛽3 𝐴𝑆𝐴 + 𝛽3 𝑉𝑖𝑠𝑎 𝑅𝑒𝑔𝑢𝑙𝑎𝑡𝑖𝑜𝑛𝑠 + 𝛽5 𝐵𝑢𝑠𝐷𝑒𝑠𝑡 + 𝛽6 𝑇𝑜𝑢𝑟𝐷𝑒𝑠𝑡 + 𝛽7 𝐿𝑎𝑛𝑔𝑢𝑎𝑔𝑒 + 𝜀

𝑮𝑫𝑷 is the GDP product of the two countries in the country-pair while 𝑑𝑖𝑠𝑡𝑎𝑛𝑐𝑒 is the great Circle distance between the two major airports in the country-pair. 𝑽𝒊𝒔𝒂 𝒓𝒆𝒈𝒖𝒍𝒂𝒕𝒊𝒐𝒏 is a dummy variable that refers to whether citizens of that country need a visa before departure to visit Kenya and whether Kenyan citizens need a visa before departure to visit a specific country. The 𝑨𝑺𝑨 dummy variable captures the liberalization degree for the market provisions Capacity, Designation and Fifth Freedom Rights as well as the overall restrictiveness or liberalness of an ASA. 𝑩𝒖𝒔𝑫𝒆𝒔𝒕 and 𝑻𝒐𝒖𝒓𝑫𝒆𝒔𝒕 are the variables that categorise a country as a tourist or business destination. 𝑳𝒂𝒏𝒈𝒖𝒂𝒈𝒆 is the dummy variable for whether a country has English as one of its official languages or not. 𝜺 is the error term, and 𝒍𝒏 is the natural logarithm.
This study shall perform two panel OLS regression models. The first model (Model A) shall incorporate a single ASA variable which captures the overall liberalness or restrictiveness across the three market provisions, namely capacity, designation and fifth freedom rights. The second model (Model B) shall use the dummy variables for the market provisions capacity, designation and fifth freedom rights The model predictions are then compared to see how well each of the models performs and if there is one model that has a better performance than the other.
