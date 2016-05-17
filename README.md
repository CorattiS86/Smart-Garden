# Smart-Garden
In this repository there is all the material that describe how it was possible to build a system able to manage the watering of a garden.

The garden consists of 3 plants, for our choice we select:
 - Cactus plant
 - Rosemary plant
 - Tomato plant

The reason of such 3 plants is that they present 3 different characteristics from the point of view of watering.

For watering we decided to use drip irrigation. 
The biggest challenge in drip irrigation is accurately determining how much and when to water.

Based on a reasearch, that you can find in the follow link 

  "http://ucanr.edu/sites/scmg/files/30917.pdf" 
  
it is possible to see what influence irrigation for several kind of plant:
  - ET (Evapotranspiration) factor
  - Crop coefficent
  - Density
  - Exposure factor
  - Planted area
  - Irrigation efficency
 

CROP EFFICENT
Crop coefficients, or species factors range from 0.1 to 0.9 and are
divided into four categories:
  - Very low      < 0.1 (10% of ET°)
  - Low       0.1 - 0.3 (10-30%)
  - Moderate  0.4 - 0.6 (40-60%)
  - High      0.7 - 0.9 (70-90%) 
 
PLANTING DENSITY
The planting density factor ranges in value from 0.5 to 1.3.
This range is separated into three categories:
  - Low—sparse                 0.5 - 0.9
  - Average—moderate coverage  1.0
  - High--complete coverage    1.1 - 1.3  
 
EXPOSURE FACTOR
The microclimate or exposure factor ranges from 0.5 to 1.4, and is divided into three categories: 
Average is open field, lowmoderate wind, part sun. Higher winds and greater exposure take a
higher factor, and a protected, shady location would use a lower factor.
  - Low     0.5 - 0.9
  - Average 1.0
  - High    1.1 - 1.4 
 
Returning to what was said before, the choice of 3 plants is due to the fact that they have different values
of CROP EFFICENT and PLANTING DENSITY

 PLANT     | CROP EFF. | PLANT DENSITY
------------------------------------
  fat       |           |
  rosemary  |           |
  tomato    |           |   

from which it is established a formula that says the amount of water necessary for the plant for a month

  (ET° x crop coeff. x density x exposure factor x planted area x .623) / (Irrigation efficiency)

such formula expresses the amount of water in gallons we translate such formula in liters, 
and use a conversion to compute daily amount of water. 

We use such informations to independently configure the 3 plants to obtain for each one an efficiently irrigation
using the least amount of water possible. 

