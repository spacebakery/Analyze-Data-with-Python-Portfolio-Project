# Analyzing Endangered Species in US National Parks - Data Science Portfolio Project Example

## Project Overview
This project explores the conservation of species in the top 10 most visited US National Parks. We'll use Python to analyze the dataset, and use the pandas and scipy libraries to answer the following questions:

- How does conservation status differ across national parks?
- Are mammal species more likely to be protected than non-mammal species?
- Are native species more likely to be protected than non-native species?
- Are there any abundant species that are also classified as threatened or endangered?

The project code and results are contained in the Jupyter Notebook `national-park-species.ipynb`, with a summary of the conclusions below.

## Conclusion
Here are some key findings from the analysis: 

- The Great Smoky Mountains National Park has the most endangered species (9) in the dataset but the lowest percentage (20.2%) of protected species within their park. 
- Statistical tests indicate that there is not a consistent association favoring Mammals for protection status
- We found that 30.5% of native species are protected while only 17.6% of non-native are protected. Statistical tests further showed that this difference indicates a statistical association that favors native species.
- We found that the Rainbow Trout (scientifically known as the Oncorhynchus Mykiss) is a non-native fish in Yellowstone National Park that is abundant but is threatened.

## Data
The data used in this project was obtained from a real-world dataset provided by the US National Park Service via their [NPSecies Database](https://irma.nps.gov/NPSpecies/) and is stored in the `datasets` directory under the filename `datasets/NPS_species_info.csv`. The raw dataset was cleaned and re-purposed for this capstone project example.

The dataset contains 51,706 rows and 10 columns containing information about the species. Here's a quick summary of the columns:

- **Scientific Name**: the name of the species according to scientific nomenclature
- **Common Names**: common names or aliases the species is known by the general public
- **Order**: the taxonomic order the species belongs to
- **Family**: the taxonomic family the species belongs to
- **Category**: indicates the category or classification of the species
- **Park Name**: the name of the national park the species was observed in
- **Nativeness**: indicates whether the species is native or non-native to the national park it was observed in
- **Abundance**: describes the abundance of the species in the national park it was observed in
- **Observations**: the number of observations or sightings used as evidence for the species occurrences
- **Conservation Status**: provides the conservation status of the species

## Python Version and Library Dependencies
- Python (3.8.10)
- numpy==1.22.2
- pandas==1.4.1
- scipy==1.10.1
- matplotlib==3.7.0 
