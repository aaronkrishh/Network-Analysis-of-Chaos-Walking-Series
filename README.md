![Alt text](https://scrollonline.net/wp-content/uploads/2018/03/chaos-walking.png)
# Network-Analysis-of-Chaos-Walking-Series: Project Overview
- Analyze relevancy and significance of characters and character relationships throughout the series
- Scrap character names from fandom wiki pages
- Visualize relationships and characters as a networks graph to express importance of characters and relationshops (Characters as nodes and relationship as an edge)
- Perform Louvain Community Detection Algorithm to determine the different communites through out the series.
- Analyze the accuracy of graph based on the knowledge of reading the series.

## Dataset and Data Cleaning
- The data was scrapped using selenium and performed using this script. Information on how to scrape data from wiki fandom pages are found [here](https://chaoswalking.fandom.com/wiki/Category:Characters)
- Data was filtered for unique characters and characters containing First and Last names were split into new columns. Abbreviations and punctuation were removed
- Entities were detected for each sentence and converted into dataframe. Dataframe was then filtered with only character entitites
- Relationships between 2 entitites within a 5 sentence rolling window were recorded and turned into a dataframe. 

## Exploratory Network Analysis
XNA was performed on the given txt files. Entities were detected using spacy and were filtered leaving only characters Entities. Connections were also established between characters if 2 characters were mentioned within 5 sentences. 
![graph1](https://user-images.githubusercontent.com/79017977/210680872-97f78443-f916-4063-a9ed-c238b6ff9948.png)
###  Graphs
[Knife of Never Letting Go]
[The Ask and The Answer]
[Monsters of Men]



## Code and Resourced Used
- Python Version 3.8
- Packages: Pandas, Numpy, Spacy, Matplotlib, Selenium, Regex, Spacy, Networkx
- [[Character Data]](https://chaoswalking.fandom.com/wiki/Category:Characters)
- [[Structure and Formating of Project]](https://github.com/thu-vu92/the_witcher_network)

