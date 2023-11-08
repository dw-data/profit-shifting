# Corporations win big in tax havens, but who loses?
This repository contains the code for the DW story about profit shifting.

It was written by Rodrigo Menegat Schuinski and edited by Gianna Grün and Andreas Becker.

The resulting article can be found [here](#).

## Data source
The data for this story comes from the  [Atlas of the Offshore World](https://atlas-offshore.world/), published by the EU Tax Observatory, as well as from their most recent report on tax evasion.

## Methodology

EU Tax Observatory researchers measure the taxes won and lost by different countries by analzying data from primary sources. Those include official reports by tax authorities and country-by-country balances published by multinational companies.
 
The researchers start by comparing the profit margins of a multinational local branch in, say, Bermuda, and the total wages it pays for workers stationed there.
 
In tax havens, foreign businesses often have a way higher profit vs wages ratio than the local companies. This means that they make large amounts of money without having an actual footprint in the country, as measured by the costs of their workforce. This suggests that this excess comes from profits that were booked there, but were actually made somewhere else.
 
In order to estimate how much money is being shifted towards each tax haven, the researchers estimate how much profit the international companies would be making if they had the same profit vs wages ratio of the local businesses. The difference between this measurement and the real declared profits is then considered to be the amount of profit that was shifted towards the low-tax jurisdiction in a given year.
 
In order to estimate how much money was lost in each source country, though, they first calculate how many "high risk exports" were sent from each tax haven to each high-tax country. Those are goods and services that are normally used to "move" profits from one country to the other, like patents, intelectual property, consulting and other immaterial goods and services. 

Then, they compare the real ammount of high risk exports with a prediction of what they should have been under regular trade conditions. The difference between both values is considered to be the ammount of profit shifted from the source country to the tax haven.
 
Finally, the total tax loss in each country is calculated by applying the corporate taxation rate to the total profits shifted from it – that is, it shows how much each country would make if it taxed the money sent to tax havens using their regular rates.

A detailed description of the methodology can be found on [this paper]https://gabriel-zucman.eu/files/TWZ2022Restud.pdf).

## Code structure
In this repository, all the source data files can be found on the `data` directory, which contains the source file for all figures in the story.

Both the data processing required to make the charts and the data analysis can be found in the `code` directory. The notebook `taxes-won` dives into the profits shifted to tax havens, while the notebook `taxes-lost` does the same for the countries where profits were shifted from.

Finally, the CSV files used for making the charts are available in the `output` directory.

