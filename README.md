# Data Set for the France Synthetic Control Study on Fertility Rate

In this repository you will find the data set we compiled for the study in a csv format. 

# Codebook 
This dataset is used to explore the question: What was the causal effect of the 1994 French Parental Leave Reform on France's total fertility rate (TFR)? It contains 15 countries including France and takes the form of panel data, each row describing different years.
The unit of analysis in this codebook is country. The only unit that has 1 as a treatment variable is France, and it is compared against other OECD countries meeting the donor pool criteria: Austria, Belgium, Canada, Finland, Greece, Iceland, Ireland, Italy, South Korea, Luxembourg, New Zealand, Norway, Spain, Switzerland.

| Variable category | Name | Description | Type | Source |
| --- | --- | --- | --- | --- |
| Time | `year` | Year |
| Treatment | `reform` | The 1994 French Parental Leave Reform | Categorical Binary dummy (0=no, 1=yes) | Independent research, OECD Family Database |
| Outcome | `tfr` | The total fertility rate (TFR) | Continuous On-average children per mother in her lifetime | The World Bank |
| Confounders | `gdp` | Gross Domestic Product (GDP) per capita | Continuous, Current US dollars | The World Bank | 
|  | `hdi` | The Human Development Index (HDI) score | Continuous, Unitless between 0 (lowest) and 1 (highest) | UNDP | 
| | `labor_rate_female` and `labor_rate_male` | Labor participation rate for female and male populations respectively | Continuous, %. Age between 15 and 64 | The World Bank |
| | `tertiary_school_enrollment_total` | Teritial education school enrollment rate | Continous, %. | The World Bank |
| | `avg_yrs_schooling_total` | Average years of schooling | Continuous, Number of years | The World Bank |
| | `life_expectancy` | Life expectancy | Continuous, Age (years) | The World Bank |
| | `infant_mortality` | Infant mortality rate | Continous, % | The World Bank |
| | `gini` | Wealth inequality (Gini coefficient) | Unitless from 0 (lowest) to 100 (highest) | The World Bank |

You can also find the Codebook in this Google document [here](https://docs.google.com/document/d/1ncTU9xzHVZOxNMTrs9IjocBpD53HZF1QtHawqTYrySU/). 

## Additional comments on the variables 

- `gdp` is GDP per capita
- `labor_rate_female` is Labor force participation rate, female (% of female population ages 15+) (national estimate) taken from the Worldbank [here](https://data.worldbank.org/indicator/SL.TLF.CACT.FE.NE.ZS)
- `labor_rate_male` is Labor force participation rate, males (national estimates) taken from the Worldbank [here](https://data.worldbank.org/indicator/SL.TLF.CACT.MA.NE.ZS)
- `tertiary_school_enrollment_total` is School enrollment, tertiary (% gross) taken from the Worldbank [here](https://data.worldbank.org/indicator/SE.TER.ENRR?end=2005&start=1984&view=chart). Gross enrollment ratio is the ratio of total enrollment, regardless of age, to the population of the age group that officially corresponds to the level of education shown. Tertiary education, whether or not to an advanced research qualification, normally requires, as a minimum condition of admission, the successful completion of education at the secondary level.
- `avg_yrs_schooling_total` (and similarly for `avg_yrs_schooling_female`) is taken from the Worldbank database [here](https://databank.worldbank.org/Average-years-of-schooling-age-15plus/id/fdfe8ea8).  From the Series choose these two indicators: Barro-Lee: Average years of total schooling, age 25+, female; Barro-Lee: Average years of total schooling, age 25+, total
- `life_expectancy` is from the Worldbank [here](https://data.worldbank.org/indicator/SP.DYN.LE00.IN)
- `infant_mortality` is Mortality rate, infant (per 1,000 live births) from the Worldbank [here](https://data.worldbank.org/indicator/SP.DYN.IMRT.IN). Estimates developed by the UN Inter-agency Group for Child Mortality Estimation ( UNICEF, WHO, World Bank, UN DESA)
- `gini` is from the WIID - World Income Inequality Database, UNU-WIDER, United Nations University World Institute for Development Economics Research found [here](https://www4.wider.unu.edu/?ind=1&type=table&year=35&iso=FRA,AUT,GRC,ESP,NOR,FIN,BEL,ITA,IRL,ISL,KOR,NZL,CHE,CAN,LUX&byCountry=false&slider=slider&yearRange=35,51)





