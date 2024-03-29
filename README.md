# Dependencies
pytorch == 1.10.0 scikit-learn == 1.0.2 numpy == 1.20.3

# Dataset
We made our experiments on the MIMIC-III and eICU datasets. In order to access the datasets, please refer to 
https://mimic.physionet.org/gettingstarted/access/  and  https://eicu-crd.mit.edu/gettingstarted/access/. 


<table>
	<tr>
	    <th colspan="3">MIMIC-III</th>
	    <th colspan="3">eICU</th>  
	</tr >
	<tr>
	    <td>Feature</td>
	    <td>Type</td>
		  <td>Missingness (%)</td>
		  <td>Feature</td>
	    <td>Type</td>
      <td>Missingness (%)</td>
	</tr>
  <tr>
	    <td>Capillary refill rate</td>
	    <td>categorical</td>
		  <td>99.78</td>
		  <td>-</td>
	    <td>-</td>
      <td>-</td>
	</tr>
  <tr>
	    <td>Diastolic blood pressure</td>
	    <td>continuous</td>
		  <td>30.90</td>
		  <td>Diastolic blood pressure</td>
	    <td>continuous</td>
      <td>33.80</td>
	</tr>
  <tr>
	    <td>Fraction inspired oxygen</td>
	    <td>continuous</td>
		  <td>94.33</td>
		  <td>Fraction inspired oxygen</td>
	    <td>continuous</td>
      <td>98.14</td>
	</tr>
  <tr>
	    <td>Glasgow coma scale eye</td>
	    <td>categorical</td>
		  <td>82.84</td>
		  <td>Glasgow coma scale eye</td>
	    <td>categorical</td>
      <td>83.42</td>
	</tr>
  <tr>
	    <td>Glasgow coma scale motor</td>
	    <td>categorical</td>
		  <td>81.74</td>
		  <td>Glasgow coma scale motor</td>
	    <td>categorical</td>
      <td>83.43</td>
	</tr>
  <tr>
	    <td>Glasgow coma scale total</td>
	    <td>categorical</td>
		  <td>89.16</td>
		  <td>Glasgow coma scale total</td>
	    <td>categorical</td>
      <td>81.70</td>
	</tr>
  <tr>
	    <td>Glasgow coma scale verbal</td>
	    <td>categorical</td>
		  <td>81.72</td>
		  <td>Glasgow coma scale verbal</td>
	    <td>categorical</td>
      <td>83.54</td>
	</tr>
  <tr>
	    <td>Glucose</td>
	    <td>continuous</td>
		  <td>83.04</td>
		  <td>Glucose</td>
	    <td>continuous</td>
      <td>83.89</td>
	</tr>
  <tr>
	    <td>Heart Rate</td>
	    <td>continuous</td>
		  <td>27.43</td>
		  <td>Heart Rate</td>
	    <td>continuous</td>
      <td>27.45</td>
	</tr>
  <tr>
	    <td>Height</td>
	    <td>continuous</td>
		  <td>99.77</td>
		  <td>Height</td>
	    <td>continuous</td>
      <td>99.19</td>
	</tr>
  <tr>
	    <td>Mean blood pressure</td>
	    <td>continuous</td>
		  <td>31.38</td>
		  <td>Mean arterial pressure</td>
	    <td>continuous</td>
      <td>96.53</td>
	</tr>
  <tr>
	    <td>Oxygen saturation</td>
	    <td>continuous</td>
		  <td>26.86</td>
		  <td>Oxygen saturation</td>
	    <td>continuous</td>
      <td>38.12</td>
	</tr>
  <tr>
	    <td>Respiratory rate</td>
	    <td>continuous</td>
		  <td>26.80</td>
		  <td>Respiratory rate</td>
	    <td>continuous</td>
      <td>33.11</td>
	</tr>
  <tr>
	    <td>Systolic blood pressure</td>
	    <td>continuous</td>
		  <td>30.87</td>
		  <td>Systolic blood pressure</td>
	    <td>continuous</td>
      <td>33.80</td>
	</tr>
  <tr>
	    <td>Temperature</td>
	    <td>continuous</td>
		  <td>78.06</td>
		  <td>Temperature</td>
	    <td>continuous</td>
      <td>76.35</td>
	</tr>
  <tr>
	    <td>Weight</td>
	    <td>continuous</td>
		  <td>97.89</td>
		  <td>Weight</td>
	    <td>continuous</td>
      <td>98.65</td>
	</tr>
  <tr>
	    <td>pH</td>
	    <td>continuous</td>
		  <td>91.56</td>
		  <td>pH</td>
	    <td>continuous</td>
      <td>97.91</td>
	</tr>
</table>

After downloading MIMIC-III, you can use the following zenodo repo for the pre-processing: https://doi.org/10.5281/zenodo.1306527 . \
After downloading eICU, you can use the following github repo for the pre-processing: https://github.com/mostafaalishahi/eICU_Benchmark_updated. 

# Main Entrance 
train.py contains training code. test.py contains evaluation code.
