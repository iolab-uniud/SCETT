# SCETT

This repository contains the dataset used to the paper "A Two-Stage Stochastic Programming Approach Against Uncertain Student Capacity in Examination Timetabling", by Sara Ceschia, Daniele Manerba, Andrea Schaerf, Eugenia Zanazzo, and Roberto Zanotti, currenty submitted for publication. It includes the instance files as well as the disruption files used to test the PH method presented in the paper.

## Formats
### Instances
The instance format follows the structure used by Carter et al. in the paper "[Examination timetabling: Algorithmic strategies and applications](https://www.tandfonline.com/doi/abs/10.1057/jors.1996.37)" with one exception: the header includes the total number of seats available (i.e. the sum of all individual room capacities) making the problem a Capacitated Examination Timetabling problem. 
The dataset is divided into four subsets (D0, D1, D2, D3). D0 contains 20 instances and was used to perform an in-sample stability analysis of the generated instances. 
The remaining subsets (D1, D2, D3) each contain 10 instances, with increasing sizes, along with the corresponding 10 disruption files that describe the disruptions for each of the 50 scenarios.

### Scenarios

A single file contains the disruptions for all scenarios. The file begins with a header indicating the number of scenarios. Following the header, each scenario specifies the reduction in seats per period, preceded by its corresponding scenario index. The format is as follows:

```
50
1
S(1, -7)  
S(2, -13)  
S(3, -15)  
S(4, -7)  
S(5, -2)  
S(6, -22)  
S(7, -17)  
S(8, -10)  
S(9, -10)  
S(10, -1)  
2
...
```


