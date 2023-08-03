# National-Park-Biodiversity
An investigation into biodiversity across US National Parks

---

An analysis into `species_info.csv` and `observations.csv` where:


*Species Info*:
| Header | |
| --- | --- |
| category | Taxonomic category e.g. mammal, plant, etc. |
| scientific name | Scientific or Latin name of a species within [binomial nomeclature](https://en.wikipedia.org/wiki/Binomial_nomenclature)
| common names | Everyday name of a given species |
| conservation status | The given species conservation status at time of file creation |


*Observations*:
| Header | |
| --- | --- |
| scientific name | See above |
| park name | Name of US National Park species observations took place |
| observations | Number of obseravtions of a given species across a one week period |

Before deeper analysis takes place, the data is explored using exploratory data analysis with the data in `species_info.csv` being looked at first. Here duplicated `scientific_name` rows were found.

Then `observations.csv` is explored again using EDA techniques, again with duplicate entries found.

For duplications in `observations.csv`, all the data was taken to be correct and as a result, all the duplicate entries collated into a single entry.

Duplications in `species_info.csv` fell into two categories depending on which column the data differed:
- Common names: In this case, the rows shared all the same information except the common names. The corresdonding rows were combined and common names collected together.
- Conservation Status: Without more information, it is impossible to ascertain why such duplications occured. It could be that a given species has a different status across each park. Without more information, these such duplications were left as is.

TODO 

What is the distribution of conservation status for animals?
Are certain types of species more likely to be endangered?
Are the differences between species and their conservation status significant?
Which species were spotted the most at each park?

---
### Dependencies
- Pandas
- Numpy
- Matplotlib
- Seaborn

---

Data provided by [CodeCademy.com](https://www.codecademy.com/) and is inspired by true data.
