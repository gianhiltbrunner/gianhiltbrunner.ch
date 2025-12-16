+++
title="Gian's Shoyu Ramen"
description="My best ramen recipe so far - a rich double soup with homemade tare and perfectly cooked eggs"
date=2025-12-16T20:00:00+01:00
tldr="A comprehensive shoyu ramen recipe with detailed timing and dependency graphs"
draft=false
tags=["ramen", "recipe", "japanese", "cooking"]
+++

My best ramen recipe so far. Takes a bit of time to make. But the tare can be made in large batches and refrigerated.

## Dependency Graph

{{< mermaid >}}
graph TD;
    Eggs-->Bowl;
    Sofrito --> Tare --> Bowl;
    Dashi --> Soup;
    Stock --> Soup;
    Soup --> Bowl;
{{< /mermaid >}}

## Timing

{{< mermaid >}}
gantt
    dateFormat mm
    tickInterval 1hour
    axisFormat %Hh
    section Tare
        Sofrito: sofrito, 0, 420m
        Tare: tare, after sofrito, 10m
    section Soup
        Dashi : 0, 40m
        Stock (pressure cooker) :stock, 0, 60m
        Stock (normal pot) :stock, 0, 360m
        Soup :after stock, 10m
    section Eggs
        Eggs : 0, 360m
    section Bowl
        Bowl: after tare, 30m
{{< /mermaid >}}

## Sources

> Ivan Ramen: Love, Obsession, and Recipes From Tokyo's Most Unlikely Noodle Joint; Ivan Orkin

> The Book of Ramen; Michael T. Satinover and Scott J. Satinover

## Ramen Bowl

Makes 1 bowl (plan 1 - 2 bowls / person)

- 10 - 20 milliliters (2 - 4 teaspoons) warm FAT (chicken or pork)
- 30 milliliters (2 tablespoons) room-temperature SHIO TARE
- 2.5 grams (0.5 tablespoon) SALT, by taste
- 270 milliliters DOUBLE SOUP, simmering
- 130 grams RAMEN NOODLES
- 1 room-temperature HALF-COOKED EGG
- Finely shredded green onions or negi (Japanese green onions), for garnish
- 1 optional pinch of MSG

## Double Soup

- 500 milliliters CHICKEN STOCK
- 500 milliliters DASHI

## Chicken Stock

- 1 large (2-kilo) whole chicken (or 2 small whole chickens)
- Water (1 part chicken to 2 parts water by volume)

1. Start cooking until scum rises to the top. Remove scum and cook according to method below.

> Chicken (whole, backs, feet, all chicken)
> Pot: 6 hours
> Pressure Cooker: 45 minutes (or 30 minutes with 30-minute natural release)

2. Drain and filter the stock.

## Dashi

- 1 L cold water
- 10 g kombu
- 25 g katsuobushi (or replace with niboshi, or shiitake, as desired)

1. Add the cold water and kombu to a pot (if using niboshi or shiitake, add with the kombu).
2. Heat over medium-low heat until just below simmer, around 80 °C. Turn off the heat and allow it to steep for 10 minutes.
3. Remove the kombu, add the katsuobushi (if using).
4. Bring up to a simmer, then turn off the heat again, cover, and allow to steep until flavored to your liking, anywhere from 5 minutes to 30 minutes.
5. Strain through a fine-mesh strainer and reserve until needed.

> Dashi degrades quickly in flavor, so it only keeps for a few days in the fridge if you decide to make it in advance. Luckily, it's relatively simple to put together.

## Shio Tare

- 48 grams (4 tablespoons) sea salt
- 340 milliliters boiling water
- 275 grams SOFRITO

## Sofrito

- 325 grams Fuji apples, peeled
- 1.2 kilos yellow onions
- 160 grams garlic
- 65 grams fresh ginger, peeled
- About 1 liter vegetable oil

1. Preheat the oven to 110°C.
2. Cut the apples and onions into a small dice. (Or, since everything is going to cook down for hours anyway, you could use a food processor: cut the onions and apples into coarse chunks, then process them separately, pulsing in short bursts to achieve a small dice without turning things into mush.) Dice the garlic and ginger very fine, close to a mince.
3. Put the onions and apples into a deep sauté pan or roasting pan that will hold all the ingredients in a 13-millimeter layer. Pour in the oil, set the pan over medium heat, and cook until the oil begins to bubble and the vegetables begin to sweat. Cover the pan, transfer it to the oven, and cook for about 3 hours. You want the onions and apples to cook very slowly, taking on color only toward the end of cooking. The cooking time will vary depending on how much water is in the onions and apples. Stir the ingredients and rotate the pan regularly to prevent burning.
4. After the onions and apples have cooked down and begun to brown slightly, add the garlic and ginger and continue to cook for another 2 or 3 hours, stirring and rotating the pan from time to time, until everything has a uniformly light brown color and a soft, creamy consistency. Try to prevent the onions and apples from developing dark or crisp edges.
5. Cool the sofrito completely, then refrigerate. It should keep for at least 2 weeks in a tightly sealed container.

## Half-Cooked Eggs

- Refrigerated Eggs

1. Bring a large pot of water to a full boil.
2. In a large bowl or container, fill with ice and cold water to make an ice bath. Reserve.
3. Remove eggs from the refrigerator.
4. Working in batches of 4-6 eggs at a time, to avoid the water temperature dropping too quickly, lower your eggs into the boiling water.
5. Boil the eggs, stirring occasionally during the first minute or so of cooking, for 6-7 minutes, depending on how firm you'd like the yolk. I like 7, the yolk gets juuuust a tad cooked, and slightly custardy. Others like a completely liquid yolk, which is around 6 minutes to 6 minutes 30 seconds.
6. After the time is up, quickly remove the eggs from the water and place them in the ice bath from step 2, hold for 15 minutes, or until thoroughly chilled.

**Marinade:**

- One part soy sauce
- One part mirin
- One part water

1. Place peeled eggs in an airtight container, like a hard plastic container or a sealable bag.
2. Pour the above ingredients into the container to cover (you may not need to use all the brine, reduce the amount as necessary)
3. Soak, jostling contents every hour or so, for 4-6 hours.
4. Remove from brine, reserve in the fridge until needed.
