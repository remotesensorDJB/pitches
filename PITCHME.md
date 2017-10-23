# SPATIAL DATA CONCEPTS AND VISUALIZATION
## GEOG 350 - FALL 2017

### Donald J. Biddle
---
### The Plan 
- Talk about Geographic Scale |
 - What is it? How do we represent it? Large scale vs small scale.
 - What are the effects/limitations of scale?
 - How do we make decisions about scale in our mapping efforts?
- Talk about Scale of Measurement | 
 - What are *levels* of data?
 - What is data normalization?
---
### The Plan
- Talk about Thematic Mapping |
 - Data Classification > Choropleth Mapping 
 - Ways to classify data
 - The role of color/shading
- Other ways to represent data |
 - Dot Density
 - Proportional Symbols
 - Cartograms
 - Vector Fields
---
## Geographic *(Map)* Scale
  >*The ratio of a distance on a map to the corresponding distance on the ground* 
---
### Representing Map Scale
- Representative Fraction |
 - 1:24,000
- Textual Scale |
 - *One inch equals 24,000 inches*
 - *1" = 2,000'*
- Graphical Scale |
 - Scale Bars
 - ![Scale](http://faculty.chemeketa.edu/afrank1/topo_maps/scale/scale.jpg)
---
### Large or Small Scale?? 
- #### Easy way to remember: 
 - >*Features appear **larger** in **large** scale maps, and **smaller** in **small** scale maps* 
- #### CAUTION! |
 - >A large denominator ≠ a large scale map! |
---
![ScaleHeadache](http://blog.chartandmapshop.com.au/wp-content/uploads/2015/02/scale.png)
---
#### Examples of large vs. small scale maps
![Scale Example Image](http://blog.chartandmapshop.com.au/wp-content/uploads/2015/02/scales.png)
---
### Limitations/Effects of Scale
#### Simply put: Tradeoff between detail and extent
- ###### Large Scale Maps > High detail, limited area |
- ###### Small Scale Maps > Large extent, limited detail |
---
### Scale Effects
- **Cartographic Generalization**
 - Deriving a smaller scale map from large scale map data |
 - Abstraction of higher level data to lower level data |
 - Loss of detail/Omission of key features |
 - The "Baltimore Phenomenon" |
---
### Generalization
![Generalization Examples Image 1](images/generalization1.png)
Note: Simplification – Removing points
Smoothing – Replacing sharp and complex bends with smoother ones
Collapse – Areas become combinations of lines and points
Aggregation – individual objects are replaced by a smaller number of new objects
---
### Generalization
![Generalization Examples Image 2](images/generalization2.png)
Note: Amalgamation – Several Area objects become one single area
Merge – Several lines become one line
Refinement – Replacing complex patterns with a simple pattern preserving general form
Exaggeration – Enlarging object to preserve it at smaller scales
---
### The Coastline Paradox
> The measured length of a feature is inversely proportional to its unit of measure.
> The smaller the unit of measure, the longer the measured length!

https://youtu.be/I_rw-AJqpCM 
--- 
## DATA SCALE
### or SCALE OF MEASUREMENT
> How are *attributes* measured? 

- Four main scales of data:
 - Nominal: Each value is a unique meaning |
 - Ordinal: Each value is ranked in relation to other values |
 - Interval: The scale unit is fixed |
 - Ratio: The scale has a true zero value |
---
#### Nominal Data
- Categorical/Descriptive 
- Numbers have no mathematical value, only used as labels 
- Operations: = , ≠
- Example: Land Use Classification
---
#### Ordinal Data
- Rankings
- 1st, 2nd, 3rd, etc. 
- Distance between adjacent values could vary widely
- Operations: < , >
- Example: Top ten countries by population
---
#### Interval Data
- Data points are measured on a fixed scale
- Data scale **has no true zero value**, and negatives are possible
- Operations: + , - 
- Examples: Temperature on Celsius Scale, Time/Date from 0CE  
---
#### Ratio Data
- Data scale has a true/absolute zero value
- Negative values not possible
- Operations: * , /
- Examples: Daily precipitation, population, Temp in Kelvin
---
#### Scales of Spatial Data
![Spatial Data Scales](images/data_levels_maps.JPG)
---
### THEMATIC MAPS
- Display information about a single attribute/phenomenon
- As opposed to a *reference map*, showing general information about an area
- Can be designed to show data in any scale...
---
#### THEMATIC MAP: NOMINAL DATA
![Geology Map](http://www.uky.edu/KGS/geoky/images/kygeo.jpg)
##### Geologic Map
---
#### THEMATIC MAP: ORDINAL DATA
![Cancer Risk Map](https://pbs.twimg.com/media/B0Zk1D9CAAEmROA.jpg)
##### Cancer Risk Map
---
#### THEMATIC MAP: INTERVAL DATA
![Soil pH Map](http://www.cropnutrition.com/Images/median-soil-ph.png?v=3)
##### Soil pH Map
---
#### THEMATIC MAP: RATIO DATA
![Population Density Map](https://www.google.com/url?sa=i&rct=j&q=&esrc=s&source=images&cd=&cad=rja&uact=8&ved=0ahUKEwj-iJ3lgIfXAhVM6yYKHYp5BN8QjRwIBw&url=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FPopulation_density&psig=AOvVaw2BzmOTHDrkE0QMsg9L6HEz&ust=1508857072285991)
##### Population Density Map
---
### CHOROPLETH MAPS
- Thematic mapping on a single numerical attribute
- Use coloring, shading, or different symbols to represent the average value over an area
- The "bar chart" of the mapping world
---
![Bar Chart and Map](https://thumbnails-visually.netdna-ssl.com/us-map-choropleth-with-bar-chart_5411f4ef92636.png)
---
### DATA CLASSIFICATION
- Breaking a range (distribution) of values into *n* classes
- Reducing the complexity of a dataset into something more interpretable
- Rescaling data from interval/ratio data > ordinal data
- The basis for choropleth mapping
---
### DATA DISTRIBUTIONS
###### the "shape" of our data
- ![Data Shapes](images/datashapes.jpg)
---
### HISTOGRAMS
###### Depict the distribution of data values
![Hotel Data Hisogram](images/hotel_data.png)
---
### CLASSIFICATION METHODS
- Where do we define the breakpoints in our dataset?
- Three main methods:
 - Equal Interval: divides the range of attribute values into equal-sized subranges. **Rectangular distributions**
 - Quantile: Each class contains an equal number of features. **Recatangular distributions**
 - Natural Breaks: based on natural groupings of data. Maximizes in group similarity, minimizes out of group differences. **Uneven/skewed/multimodal distributions**
---
 ![Classification Methods](http://axismaps.github.io/thematic-cartography/images/histogram_examples.png) |

	