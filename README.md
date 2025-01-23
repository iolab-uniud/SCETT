# SCETP

This repository contains the dataset related to the paper "A Two-Stage Stochastic Programming Approach Against Uncertain Student Capacity in Examination Timetabling." It includes the instance files as well as the 50 scenarios used to test the method presented in the paper.

## Formats
### Instances
The instance format follows the structure used by Carter et al. in the paper "Examination timetabling: Algorithmic strategies and applications" with one exception: the header includes the total number of seats available (i.e. the sum of all individual room capacities) making the problem a Capacitated Examination Timetabling problem.

### Scenarios

A single file contains the disruptions for all 50 scenarios. The file begins with a header indicating the total number of scenarios. Following the header, each scenario specifies the reduction in seats per period, preceded by its corresponding scenario index. The format is as follows:

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


