#WATER LEVEL INDICATOR

 - The Water Level Indicator employs a simple mechanism to detect and indicate the water level in  an overhead tank or any other water container.
 - The sensing is done by using a set of nine probes which are placed at nine different levels on the tank walls (with probe 9 to probe 1 placed in increasing order of height, common probe (i.e. a supply carrying probe) is placed at the base of the tank).
 - The level 8 represents the “tank full” condition while level 0 represents the “tank empty” condition.

 - In this project we show the water level indicator using eight transistors which conducts as level rises, a buzzer is also added which will automatically start as the water level becomes full, auto buzzer start with the help of microcontroller. With the help of this project we not only show the level of water on seven segment display but also indicate the water full condition using a buzzer.

Block Diagram :- 
         
          %3CmxGraphModel%3E%3Croot%3E%3CmxCell%20id%3D%220%22%2F%3E%3CmxCell%20id%3D%221%22%20parent%3D%220%22%2F%3E%3CmxCell%20id%3D%222%22%20value%3D%22%26lt%3Bb%26gt%3BM%26lt%3Bbr%26gt%3BI%26lt%3Bbr%26gt%3BC%26lt%3Bbr%26gt%3BR%26lt%3Bbr%26gt%3BO%26lt%3Bbr%26gt%3BC%26lt%3Bbr%26gt%3BO%26lt%3Bbr%26gt%3BN%26lt%3Bbr%26gt%3BT%26lt%3Bbr%26gt%3BR%26lt%3Bbr%26gt%3BO%26lt%3Bbr%26gt%3BL%26lt%3Bbr%26gt%3BL%26lt%3Bbr%26gt%3BE%26lt%3Bbr%26gt%3BR%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D0%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3Balign%3Dcenter%3BfillColor%3D%23d5e8d4%3BgradientColor%3D%2397d077%3BstrokeColor%3D%2382b366%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22380%22%20y%3D%22100%22%20width%3D%22120%22%20height%3D%22380%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%223%22%20value%3D%22%26lt%3Bb%26gt%3BWATER%20LEVEL%26lt%3Bbr%26gt%3BSENSORS%26lt%3Bbr%26gt%3BS1%2CS2%2CS3%2CS4%2C%26lt%3Bbr%26gt%3BS5%2CS6%2CS7%2CS8%26lt%3Bbr%26gt%3B%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22590%22%20y%3D%22110%22%20width%3D%22120%22%20height%3D%2290%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%224%22%20value%3D%22%26lt%3Bb%26gt%3BBUZZER%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23f8cecc%3BstrokeColor%3D%23b85450%3BgradientColor%3D%23ea6b66%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22590%22%20y%3D%22340%22%20width%3D%22120%22%20height%3D%2260%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%225%22%20value%3D%22%26lt%3Bb%26gt%3BSEVEN%20SEGMENT%26lt%3Bbr%26gt%3BDISSPLAY%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23e51400%3BfontColor%3D%23ffffff%3BstrokeColor%3D%23B20000%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22590%22%20y%3D%22240%22%20width%3D%22120%22%20height%3D%2260%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%226%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BentryX%3D0%3BentryY%3D0.5%3BentryDx%3D0%3BentryDy%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20target%3D%225%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22500%22%20y%3D%22270%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22470%22%20y%3D%22150%22%20as%3D%22targetPoint%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%227%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BentryX%3D0%3BentryY%3D0.5%3BentryDx%3D0%3BentryDy%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20target%3D%224%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22500%22%20y%3D%22370%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22470%22%20y%3D%22150%22%20as%3D%22targetPoint%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%228%22%20value%3D%22Power%20Supply%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%2360a917%3BstrokeColor%3D%232D7600%3BfontColor%3D%23ffffff%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22240%22%20y%3D%22110%22%20width%3D%2290%22%20height%3D%2230%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%229%22%20value%3D%22%26lt%3Bb%26gt%3BS1%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfontStyle%3D0%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22150%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2210%22%20value%3D%22%26lt%3Bb%26gt%3BS2%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22180%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2211%22%20value%3D%22%26lt%3Bb%26gt%3BS3%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22210%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2212%22%20value%3D%22%26lt%3Bb%26gt%3BS4%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22240%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2213%22%20value%3D%22%26lt%3Bb%26gt%3BS5%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22270%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2214%22%20value%3D%22%26lt%3Bb%26gt%3BS7%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22300%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2215%22%20value%3D%22%26lt%3Bb%26gt%3BS8%26lt%3B%2Fb%26gt%3B%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3BfontSize%3D13%3BfillColor%3D%23ffe6cc%3BstrokeColor%3D%23d79b00%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22280%22%20y%3D%22330%22%20width%3D%2250%22%20height%3D%2220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2216%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BfontStyle%3D1%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%2290%22%20y%3D%22130%22%20width%3D%22150%22%20height%3D%22340%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2217%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22100%22%20y%3D%22160%22%20width%3D%22180%22%20height%3D%22300%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2218%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22110%22%20y%3D%22190%22%20width%3D%22170%22%20height%3D%22260%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2219%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22120%22%20y%3D%22220%22%20width%3D%22160%22%20height%3D%22220%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2220%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22130%22%20y%3D%22250%22%20width%3D%22150%22%20height%3D%22180%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2221%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22140%22%20y%3D%22280%22%20width%3D%22140%22%20height%3D%22140%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2222%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22150%22%20y%3D%22310%22%20width%3D%22130%22%20height%3D%22100%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2223%22%20value%3D%22%22%20style%3D%22shape%3DpartialRectangle%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3Bbottom%3D0%3Bright%3D0%3BfillColor%3Dnone%3BfontSize%3D13%3BstrokeWidth%3D2%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%22160%22%20y%3D%22340%22%20width%3D%22120%22%20height%3D%2260%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2224%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BentryX%3D0.017%3BentryY%3D0.066%3BentryDx%3D0%3BentryDy%3D0%3BentryPerimeter%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20source%3D%228%22%20target%3D%222%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22420%22%20y%3D%22310%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22370%22%20y%3D%22125%22%20as%3D%22targetPoint%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2225%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20source%3D%229%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22420%22%20y%3D%22310%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22380%22%20y%3D%22160%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2226%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20source%3D%2210%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22340%22%20y%3D%22170%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22380%22%20y%3D%22190%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%3E%3CmxPoint%20x%3D%22360%22%20y%3D%22190%22%2F%3E%3CmxPoint%20x%3D%22380%22%20y%3D%22190%22%2F%3E%3C%2FArray%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2227%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20source%3D%2211%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22350%22%20y%3D%22180%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22380%22%20y%3D%22220%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2228%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3BentryX%3D0%3BentryY%3D0.395%3BentryDx%3D0%3BentryDy%3D0%3BentryPerimeter%3D0%3B%22%20edge%3D%221%22%20source%3D%2212%22%20target%3D%222%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22360%22%20y%3D%22190%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22410%22%20y%3D%22190%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2229%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3BentryX%3D0%3BentryY%3D0.471%3BentryDx%3D0%3BentryDy%3D0%3BentryPerimeter%3D0%3B%22%20edge%3D%221%22%20source%3D%2213%22%20target%3D%222%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22370%22%20y%3D%22200%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22420%22%20y%3D%22200%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2230%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3BentryX%3D0%3BentryY%3D0.55%3BentryDx%3D0%3BentryDy%3D0%3BentryPerimeter%3D0%3B%22%20edge%3D%221%22%20source%3D%2214%22%20target%3D%222%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22340%22%20y%3D%22290%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22390%22%20y%3D%22288.98%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2231%22%20value%3D%22%22%20style%3D%22endArrow%3Dclassic%3Bhtml%3D1%3Brounded%3D0%3BfontSize%3D13%3BexitX%3D1%3BexitY%3D0.5%3BexitDx%3D0%3BexitDy%3D0%3BstrokeWidth%3D2%3B%22%20edge%3D%221%22%20source%3D%2215%22%20parent%3D%221%22%3E%3CmxGeometry%20width%3D%2250%22%20height%3D%2250%22%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22350%22%20y%3D%22300%22%20as%3D%22sourcePoint%22%2F%3E%3CmxPoint%20x%3D%22380%22%20y%3D%22340%22%20as%3D%22targetPoint%22%2F%3E%3CArray%20as%3D%22points%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2232%22%20value%3D%22%26lt%3Bb%26gt%3B%26amp%3Bnbsp%3B%20%26amp%3Bnbsp%3B%20%26amp%3Bnbsp%3B%20%26amp%3Bnbsp%3B%20%26amp%3Bnbsp%3B%20%26amp%3Bnbsp%3B%20%26amp%3Bnbsp%3BWATER%26lt%3B%2Fb%26gt%3B%22%20style%3D%22strokeWidth%3D2%3Bhtml%3D1%3Bshape%3Dmxgraph.flowchart.annotation_1%3Balign%3Dcenter%3BpointerEvents%3D1%3BfontSize%3D13%3Bdirection%3Dnorth%3BstrokeColor%3Ddefault%3B%22%20vertex%3D%221%22%20parent%3D%221%22%3E%3CmxGeometry%20x%3D%2270%22%20y%3D%22350%22%20width%3D%22160%22%20height%3D%22130%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3C%2Froot%3E%3C%2FmxGraphModel%3E