# Toronto_Shelter_Optimization
## Aims to use optimization method to solve the shelter shortage problem in Toronto, with the limited resources and government budget.

We mainly collected the data from the City of Toronto open data repository, with additional data
from news and papers released by the housing & shelter department (SSHA) under the city of
Toronto. We modified the data based on the logistics that we thought about the project. 
1. Firstly, We have a shelter table which includes 75 existing shelters and their capacity.
2. We then categorized those shelters into small, medium, and large based on the capacity, where the small shelters only have the
capacity up to 50, the medium have up to 100 and large shelters have the capacity more than 100.
3. Additionally, we have a cost table that is categorized based on the three sizes, including the
construction cost (one time cost), maintenance cost (per day per person), and empty spot fee cost (per day per empty spot).
4. To further consider building new shelters, we assume the three sizes of new shelters are at exactly the capacity of 50, 100, 200 respectively.

- The objective function: to minimize the total cost of building new shelters and maintaining new and existing shelters for
a given year
- The constraints:
  1. Current shelters occupancy must be less than or equal to the capacity of the shelter.
  2. The total capacity of current and new shelter should satisfy the demand of 8700, which is the number of people experiencing homlessness in a given day in the city of Toronto.
  3. Total expenditure of the shelter allocation should not exceed the government budget.
  4. The number of capacity should be non-negative.
 
#### See Toronto Shelter Optimization Jupyter Notebook for detailed analysis.
#### Data information mentioned above can be found in Info_overview table.
