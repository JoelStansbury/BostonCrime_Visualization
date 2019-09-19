# BostonCrime_Visualization
Visualization using OpenStreetMap, Leaflet, and D3 to show crime distribution throughout Boston Massachusetts.

## View Here
<a href='https://joelstansbury.github.io/BostonCrime_Visualization/'>https://joelstansbury.github.io/BostonCrime_Visualization/</a>

## Usage Example
If you want to view only Traffic Violations you would...
* Press the `-` button next to the `Time of Day` slider. This removes the TOD filter, allowing incidents from all hours of the day to be displayed
* Press the `+` button to the left of `Crime Categories` to enable the category filter.
* Scroll down the list until you find `Traffic Violation` and Left Click. It will highlight when selected
* Press the `Update Map` button and wait a few seconds for all of the markers to be drawn

![picture](images/Capture.PNG)

## Other Interesting Searches
* Prostitution
* Alcohol
* Riot/Party/Strike
* Assault @ 2am

You can also select multiple crime categories to be displayed by holding `ctrl` or `shift`. This may cause issues however as the searching algorithm worst-case running time is O(n*num_categories) and can cause the browser to timeout. If this were running on a normal server all of the searching would be done in SQL or SQLite which would speed this up a great deal.

### Disclaimer
These categories were made by me in order to simplify the searching process. There may be mistakes, and some groupings admitedly don't make much sense Riot/Party/Strike for example, the reason for this particular grouping was that these are _groups_ of offenders as opposed to a single offender. The point is, don't take them too seriously, the alternative is selecting individual crime_codes from a list of 576, though I'll be adding this functionality as well.

## TODO
Still working on the user interface.


