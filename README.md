# Project6
## Summary
This visualisation shows the migration to Europe in 2015 using Eurostat's data containing monthly number of persons applying for asylym  per country. The purpose is to show how quickly the migration became a crisis, how different countries were affected and how the crisis ended.

## Design
The visualisation consists on a map of Europe and the number of persons is represented by bubbles. The color of the bubble represents the change from previous month (in %).

Every country has a bubble. The center of the bubble is roughly at the center of the country on the map. There is one bubble representing the EU total. Note that only the EU member states (28 countries) are calculated in the total. I used absolute figures and not relative to the country's population. The idea is to show how migrants moved around Europe especially when countries closed borders one by one and some even built fences. 

I decided to represent the map as a background so that the focus is on the bubbles. The map's color is white and only the borders are shown as light grey.  The bubbles are transparent as I'm using alpha to represent the change. The red color represents positive change and blue represents negative chnage. If the change is 100 % or greater the alpha is 1 otherwise alpha is between 0.2 - and 1.0. If change is below 15% the alpha is 0.2 and the color is purple. This prevents the bubbles becoming too colorless.

First I created an animation which shows the bubbles grow bigger towards the autumn and then became smaller towards the end of the year. Then I included Prev and Next -buttons for changing the month. After that I showed the first version to the personnel in the college where I work as a volunteer IT support.

To fix the problem with overlapping bubbles, I sorted the data so that smaller bubbles are on top of bigger ones. The fix the problem with bubbles hiding the country, I added Hide/Show bubbles -button which makes it easy to click on a country.

I didn't add any explanation about the countries' actions beacuse I couldn't find any one reliable, EU-wide source. 

## Feedback

What do you notice in the visualization?
 - all bubbles seem to have roughly the same red color in the spring and summer which means that number of migrants was growing steadily in every country
 - the crisis was at it's height in August - September
 - In September - October some bubbles turned blue which mean some countries managed to stop the migration
 - In December most bubbles are blue and the crisis is more or less over

What questions do you have about the data?
- are the figures absolute or per country's population
- is it possible to scale the bubbles differently to make them more visible (for example Iceland)
- are Spain's and UK's figures correct (the bubbles seem to be too small)

What relationships do you notice?
- the size of the bubble and the size of the country don't correlate
- after Hungary closed borders in September the migrants moved North 

What do you think is the main takeaway from this visualization?
- it demonstrates the disproportional burden: how some small countries were hit hard and some big coutries were not affected

Is there something you don’t understand in the graphic?
- some bubbles overlap and are difficult to see
- some bubbles hide the country so that it's not possible to click the country
- there is no explanation on the actions that individual countries or EU made, for example closed borders or built fences

## Resources
- https://developer.mozilla.org/en-US/docs/Web
- https://github.com/mbostock/d3/wiki/API-Reference
- http://ec.europa.eu/eurostat/web/asylum-and-managed-migration/data/main-tables

