# Belly Button Biodiversity

## Overview of the Project
The purpose of this analysis is to create a responsive webpage using javascript, Plotly, HTML, and CSS customizations. The page displays three visualizations using data from a json file. The dataset contains results of bacteria samples taken from the belly buttons of volunteers whose names have been replaced using anonymous ID numbers. The json dataset is loaded using the `d3.json()` method that results in a data object structured with three keys each associated with an array: metadata, names, and samples. The names array contains the ID numbers of the volunteers. The metadata array contains the demographic information provided by each volunteer. And the samples array contains the results of the bacteria sample taken from their belly buttons. 

Using `d3.select`, the webpage references the drop down option (ID numbers) selected by the user. Then the `optionChanged` function fetches new data from the json file for the selected ID number. Each time a new ID number is selected, the `buildMetadata` function pulls the demographic information from the metadata array. And the `buildCharts` function builds the bar chart, bubble chart, and gauge diagram for the selected ID. 


## Customizations
* An image was added to the jumbotron
* The text in the jumbotron was changed to white for contrast against the image and the font to Georgia
* A paragraph was added to the top of the page describing the purpose and functionality of the page to the volunteers
* The page's has a cohesive blue colorscheme by changing the text color to blue, the gauge diagram to various shades of blue, and the bar chart to teal
