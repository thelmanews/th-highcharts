# th-highcharts

See the [component page](http://thelmanews.github.io/th-highcharts) for more information.

# Update Instructions for WSJ Styles

## Component

1) For each type of chart, find the WSJ JS file associated with it: 
   - th-highcharts-bar: https://github.com/dowjones/custom-data-charts/blob/master/_js/defaults.types.bar.js 
   - th-highcharts-column: https://github.com/dowjones/custom-data-charts/blob/master/_js/defaults.types.column.js
   - th-highcharts-line: 
   - th-highcharts-pie: https://github.com/dowjones/custom-data-charts/blob/master/_js/defaults.types.pie.js

2) In the component, replace the wsjOptions object with the object in the WSJ file.

3) Replace any jQuery with vanilla JS

4) In each component there is also a `_formatTooltipValues` method, which needs to be adjusted. 
This method was created to override the tooltip formatter function in WSJ code in order to pass in custom number format options. 
Please see the notes in documentation for this method on how to update.

## Styles

1) Find the compiled CSS in `style.css` for http://charts.d2.xoxco.com/ and paste it into th-highcharts.css in the 'WSJ STYLES' section. 
Note, below this section, there is 'COMPONENT STYLES' section. Please make sure to leave that in tact.





