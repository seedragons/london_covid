# London Covid Data

This dataset was built to provide some clarity into what % of Omicron cases we are catching in official case counts relative to prior waves.

Data Explanation/Sources: 
* ons_modeled_pct_positive: this comes from the ONS Coronavirus (COVID-19) Infection Survey: England[1]. My understanding of the methodology[3] is that this represents the % of London which would be expected to test positive on a PCR collected on the specified date. Historical data was taken from sheet 1p. There is repetition of dates ove rsuccessive publication dates, so I took the average accross all publications. They didn't deviate too much, but always taking the newest publication date would probably make more sense. I also filled in data from the latest interim report that was missing from the 1p sheet.
* reported_cases: daily reported cases downloaded from gov.uk[2]
* ons_total_case_estimate: ons_modeled_pct_positive/100 * 8,716,258. This # came from backing out the London population used by the ONS in [1].

[1]: https://www.ons.gov.uk/peoplepopulationandcommunity/healthandsocialcare/conditionsanddiseases/datasets/coronaviruscovid19infectionsurveydata/2021
[2]: https://coronavirus.data.gov.uk/details/cases?areaType=region&areaName=London 
[3]: https://www.ons.gov.uk/peoplepopulationandcommunity/healthandsocialcare/conditionsanddiseases/methodologies/covid19infectionsurveypilotmethodsandfurtherinformation 
