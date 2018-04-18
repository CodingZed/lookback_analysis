# Lookback_Window_analysis

Verify XXXX Client 3 days Look Back Window

## Getting Started

I have the sample data uploaded. **NOTICE: The data was different from the actual data.**
For the survival analysis, I use the **[lifelines](https://github.com/CamDavidsonPilon/lifelines)** package.
Besides, I use Pandas, Numpy, maplotlib, datetime, warnings, pylab.

### Prerequisites

You can install lifelines using

```
pip install lifelines
```


### AB Testing

I implemented Bootstrapping AB testing because of the unbalance data. 

```
df.sample(frac=0.5, replace=True)
```

And draw the Kernel Density Estimation(kde) of the two groups difference. 
* **Minimum Detectable effer**: Unknown <br>
So I will draw the conclusion based on the 95% confidence interval. <br>

Please refer the chart below on how I draw conclusion on significant or not.
![CI](https://github.com/CodingZed/lookback_analysis/blob/master/Embrace.png)
