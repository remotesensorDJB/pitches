## Representiing Spatial Data
## GEOG 558 - Intro to GIS

#### Donald J. Biddle, GISP
---
### The Plan 
- Basics of Symbology |
 - Fundamental properties
 - Types of maps
- Scale of Measurement | 
 - What are *levels* of data?
 - What is data normalization?
---
### The Plan
- Talk about Thematic Mapping |
 - Data Classification > Choropleth Mapping 
 - Ways to classify data
 - The role of color/shading
---
## Basics of map symbols

We are mainly trying to differentiate features based on **category** or **quantity**. 

Depending on feature geometry we have several ways to do so... 

![Symbol Prop](images/symbol_prop.jpg) 
+++
### Types of maps

Different maps for different types of data...

- For nominal/categorical or ordinal data
    - single symbol
	- unique values
- For numerical data
    - graduated color
	- graduated symbol
	- dot density
	- chart maps


--- 
## DATA SCALE
### or SCALE OF MEASUREMENT
> How are *attributes* measured? 

- Four main scales of data:
 - Nominal: Each value is a unique meaning |
 - Ordinal: Each value is ranked in relation to other values |
 - Interval: The scale unit is fixed |
 - Ratio: The scale has a true zero value |
+++
@snap[west span-40]
![unique value](images/unique_value.jpg)
@snapend

@snap[east span-40]
@box[bg-blue text-white waved box-padding](Nominal Data# - Categorical or Descriptive <br/>- Numbers have no mathematical value, only used as labels<br/>- Operations: = , ≠<br/>- Example: Land Use Classification)
@snapend
+++

@snap[west span-40]
![ordinal](images/habitat_suit.jpg)
@snapend

@snap[east span-40]
@box[bg-blue text-white waved box-padding](Ordinal Data# - Rankings<br/>- 1st, 2nd, 3rd, etc. <br/>- Distance between adjacent values could vary widely<br/>- Operations: < , > <br/>- Example: Habitat Suitability)
@snapend
+++
@snap[west span-40]
![interval](images/elevation.jpg)
@snapend

@snap[east span-40]
@box[bg-blue text-white waved box-padding](Interval Data# - Measured on a fixed scale<br/>- **No true zero** <br/>- Negative values possible<br/>- Operations: + , - <br/>- Example: Elevation)
@snapend
+++
@snap[west span-40]
![ratio](images/pop_dot.jpg)
@snapend

@snap[east span-40]
@box[bg-blue text-white waved box-padding](Ratio Data# - **Has true zero**<br/>- Negatives not possible <br/>- Operations: x , / <br/>- Population)
@snapend
+++
	#### Scales of Spatial Data
![Spatial Data Scales](images/data_levels_maps.JPG)
---
### THEMATIC MAPS
- Display information about a single attribute/phenomenon
- As opposed to a *reference map*, showing general information about an area
- Can be designed to show data in any scale...
+++
#### THEMATIC MAP: NOMINAL DATA
![Geology Map](http://www.uky.edu/KGS/geoky/images/kygeo.jpg)
##### Geologic Map
+++
#### THEMATIC MAP: ORDINAL DATA
![Cancer Risk Map](https://pbs.twimg.com/media/B0Zk1D9CAAEmROA.jpg)
##### Cancer Risk Map
+++
#### THEMATIC MAP: INTERVAL DATA
![height=600px](https://forages.oregonstate.edu/sites/forages.oregonstate.edu/files/ph.jpg)
##### Soil pH Map
+++
#### THEMATIC MAP: RATIO DATA
![height=600px](https://i.redd.it/gew2qvfe6h511.png)
##### Population Density Map
---
### CHOROPLETH MAPS
- Thematic mapping on a single numerical attribute
- Use coloring, shading, or different symbols to represent a quantity or average value over an area
- The "bar chart" of the mapping world
+++
![Bar Chart and Map](https://thumbnails-visually.netdna-ssl.com/us-map-choropleth-with-bar-chart_5411f4ef92636.png)
+++
### DATA CLASSIFICATION
- Breaking a range (distribution) of values into *n* classes
- Reducing the complexity of a dataset into something more interpretable
- Rescaling data from interval/ratio data > ordinal data
- The basis for choropleth mapping
+++
### DATA DISTRIBUTIONS
###### the "shape" of our data
![Data Shapes](images/datashapes.jpg)
+++
### HISTOGRAMS
###### Depict the distribution of data values
![Hotel Data Histogram](images/hotel_data.png)
+++
### CLASSIFICATION METHODS
- Where do we define the breakpoints in our dataset? **How many classes are appropriate?**
- Four main methods:
 - Equal Interval: divides the range of attribute values into equal-sized subranges. **Rectangular distributions**
 - Quantile: Each class contains an equal number of features. **Recatangular distributions**
 - Natural Breaks: based on natural groupings of data. Maximizes in group similarity, minimizes out of group differences. **Uneven/skewed/multimodal distributions**
 - Standard Deviations: Classifies data with respect to mean value. 
+++
 ![Classification Methods](http://axismaps.github.io/thematic-cartography/images/histogram_examples.png)
+++
### EQUAL INTERVAL
![Equal Interval](images/election2016-ei5.jpg)
+++
### QUANTILE
![Quantiles](images/election2016-q5.jpg)
+++
### NATURAL BREAKS
![NATURAL BREAKS](images/election2016-nb5.jpg)
+++
### STANDARD DEVIATION
![Standard Deviation](images/election2016-sd1.jpg)
+++
### MANUAL BREAKS
![Two Classes](images/election2016-2class.jpg)
+++
### GUIDING THOUGHTS
- Classification decisions dictate how your audience interprets the data. 
- Your opportunity to control the narrative! 
- Select a classification method and number of classes that highlight **your** message.
- Visual impact dominates perception! Color and size are first impression.
- How to lie with maps! http://www.markmonmonier.com/how_to_lie_with_maps_14880.htm 
+++
### THE ROLE OF COLOR
- Color impacts the way a reader interprets data
 - Use different colors for unique values 
 - Use shades of same hue for sequential data
 - Use shades of two colors for divergent data
 - Most can't distinguish more than seven colors...classes begin to blur
+++
![colo](images/color.jpg)
+++
### THE ROLE OF COLOR 
- Avoid bold/brash colors...pastel hues more eye pleasing
- Blues/greens easier to differentiate than reds/oranges
- Use greyscale tones to de-emphasize unimportant data
- Pay attention to prevailing color associations 
 - e.g. radar maps
+++
### INCORRECT USE OF COLOR!
![Bad colors](images/election2016-badcolor.jpg)
+++
### NON-INTUITIVE USE OF COLOR
![Wrong Colors](images/election2016-blue.jpg)
+++
### BETTER CHOICE
![Good Color](images/election2016-red.jpg)
+++
### COLOR BREWER
##### http://colorbrewer2.org/
---
### Unclassed Maps
To avoid subjective groupings or breaks in data...
- **Proportional symbol** maps increase size in proportion to the data value.
- **Dot density** maps place random points within a polygon based on a specified ratio (1 dot: 1000 people).
+++
##### Proportional Symbols
![proportional symbol](images/prop_symbol.jpg)
+++
##### Dot Density
![dot density](images/dot_density.jpg)
+++
### The End


 
 
 

	