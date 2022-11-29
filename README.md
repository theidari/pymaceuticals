<p align="center">
<img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-2.png" width="980"></br>
<a href="https://github.com/theidari/pymaceuticals#overview-of-project-"><img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-10.png" width="180"></a>
<a href="https://github.com/theidari/pymaceuticals/blob/main/pymaceuticals.ipynb"><img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-12.png" width="80"></a>
<a href="https://github.com/theidari/pymaceuticals#result-"><img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-9.png" width="100"></a>
<a href="https://github.com/theidari/pymaceuticals#documents--references-"><img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-11.png" width="245"></a>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSf8thoYWMUQ24ftGdSdEvC7Ilkm1dbplhM5USAkPDs4Qp3InA/viewform?usp=sf_link"><img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/gif%201.gif" width="160"></a></br>
<img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-3.png" width="980"></br>
</p>



<b>Pymaceuticals, Inc.</b>, a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for <b><a href="https://www.skincancer.org/skin-cancer-information/squamous-cell-carcinoma/">squamous cell carcinoma (SCC)</a></b>, a commonly occurring form of skin cancer. In this study, <b>249</b> mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured.

### Overview of Project <img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-3.png" width="625"></br>
This project used python programming language and a Jupiter notebook to analyze and compare the performance of Pymaceuticals’ drug of interest, <b>Capomulin</b>, against the other treatment regimens.

#### Objective:</br>
> Data Cleaning:</br>

  - Merge all data into a single DataFrame.
  - Display the number of unique mice IDs in the data.
  - Check for any mouse ID with duplicate time points.
  - Display the data associated with that mouse ID.
  - Create a new dataframe where this data is removed.
  - Use this cleaned dataframe for the remaining steps.
  
> Summary Statistic:
  - Create a dataframe of summary statistics (Methods:  ➊ groupby ➋ aggregation) including:
    - A row for each drug regimen.
    - A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.
  - Generate <b>bar charts</b> that show <ins>the number of mice tested for each drug regimen</ins> and <b>pie charts</b> that show the distribution of <ins>females versus males</ins> with both Pandas `DataFrame.plot()` and Matplotlib's `pyplot` methods.
  - Calculate Quartiles, Find Outliers, and Create a <b>Box Plot</b> for the four treatment groups, Capomulin, Ramicane, Infubinol, and Ceftamin.
  - Generate line plot is generated that shows the <ins>tumor volume vs. time point</ins> for one mouse treated with <b>Capomulin</b>.
  - Generate scatter plot is generated that shows the average <ins>tumor volume vs. mouse weight</ins> for the <b>Capomulin regimen</b> And Calculate <i>Correlation</i> and <i>Regression</i>.

#### Methods and Software:</br>
  - The analyses were performed using the <a href="https://github.com/theidari/pandas-challenge/main/README.md#resources">Resources</a> dataset. and correlation checked by <a href="https://www.ibm.com/topics/linear-regression#:~:text=Resources-,What%20is%20linear%20regression%3F,is%20called%20the%20independent%20variable.">Linear Reression</a> method.</br>
  
  
  - Following programming languages, software, and libraries were used in this project:
    * <b>python v.3.9.13</b>
    * <b>jupyter notebook v.6.4.12</b>
    * <b>Visual Studio v.1.73.1</b>
    * <b>PowerPoint v.16.0. 14026.20298.</b>
    * <b>pandas v.1.4.4</b>
    * <b>SciPy v.1.9.3</b>
    * <b>Matplotlib v.3.6.0</b>
    * <b>NumPy v.1.23.4</b>
   
<p align="right">
<a href="https://github.com/theidari/pymaceuticals#overview-of-project-"><sup>TOP PAGE</sup></a>
</P>

### Result <img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-3.png" width="745"></br>
#### Data Cleaning:

After the left merge of data (1893 rows), the results of <a href="https://github.com/theidari/pymaceuticals/blob/main/Results/micebefore.png"><b>| 249 |</b></a> mice show that the mouse with <ins>ID g989</ins> had a duplicate by mouse ID and timepoint. due to cleaning data of mouse ID g989 (13 rows)<a href="https://github.com/theidari/pymaceuticals/edit/main/README.md#-fig-1-data-for-the-duplicate-mouse-id"><sup>Table [1]</sup></a>, results show <a href="https://github.com/theidari/pymaceuticals/blob/main/Results/miceafter.png"><b>| 248 |</b></a> mice in 1880 rows <a href="https://github.com/theidari/pymaceuticals/blob/main/README.md#-fig-2-new-dataframe"><sup>Table [2]</sup></a>
.</br>

<h6> Table [1]: data for the duplicate mouse ID</h6>

<p align="center">
<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/duplicatedataformiceid.png" width="800">
</p>

<h6> Table [2]: new dataframe</h6>

<p align="center">
<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/dataframe.png" width="700"></br>
</p>

#### Summary Statistic:

  - According to the following tables, <ins>Capomulin mean tumor volume was significantly smaller than other treatments</ins>. Moreover, Ramicane treatment was just can compete with capomulin. This pattern also was the same in median, variance standard deviation, and standard error.<a href="https://github.com/theidari/pymaceuticals#-table-4-aggregation-method"><sup>Table [3,4]</sup></a>.</br>


<h6> Table [3]: groupby method</h6>

<p align="center">
<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/summarystatisticstable.png" width="850">
</p>

<h6> Table [4]: aggregation method</h6>

<p align="center">
<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/summarystatisticstableagg.png" width="450">
</p>


  - Results indicate that the Number of mice tested by Capomulin was equal to Ramicane and more than other treatments, but we can not verify difference was significant. Also, 51% of mice were male.
  

<table align="center">
  <tr>
    <th>Pandas <sup>DataFrame.plot()</sup></th>
    <th>Matplotlib's <sup>pyplot</sup></th>
  </tr>
  <tr>
    <td><img src="https://github.com/theidari/pymaceuticals/blob/main/Results/pandasbarchart.png" width="400"></td>
    <td><img src="https://github.com/theidari/pymaceuticals/blob/main/Results/pyplotbarchart.png" width="400"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/theidari/pymaceuticals/blob/main/Results/pandaspiechart.png" width="300"></td>
    <td><img src="https://github.com/theidari/pymaceuticals/blob/main/Results/pyplotpiechart.png" width="270"></td>
  </tr>
</table>

outliers:

<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/outliers.png">


distrubution of the tumor volume for each treatment group:

<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/boxplot.png" width="550">

tumor volume vs. time point for a mouse treated with Capomulin:

<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/Capomulintreatmentofmousel509.png" width="500"><img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/mice.gif" width="250"></br>

average tumor volume vs. mouse weight for the Capomulin regimen

<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/averagetumorvolumevsmouseweight.png">

linear regression

<img src="https://github.com/theidari/pymaceuticals/blob/main/Results/linear%20regression.png">





### Documents & References <img src="https://github.com/theidari/pymaceuticals/blob/main/Pic/Madule5-3.png" width="575"></br>

#### Documents:</br>

<table align="center" table border="1px" bordercolor="b">
<tr>
<td>
<table border="2px" bordercolor="#F35557">
<h4 align="center"><b><ins>Resources</ins></b></h4>
<tr>
<td><a href="https://github.com/theidari/pymaceuticals/blob/main/Resources/Mouse_metadata.csv">Mouse Metadata</a></td>
<td><a href="https://github.com/theidari/pymaceuticals/blob/main/Resources/Study_results.csv">Study Results</a></td>
</tr>
</table>
</td>
<td>
<table border="2px" bordercolor="#F35557">
<h4 align="center"><b><ins>Results</ins></b></h4>
<tr>
<td><a href="https://github.com/theidari/pymaceuticals/tree/main/Results">Images</a></td>
</tr>
</table>
</td>
</tr>
</table>


#### References:</br>
<sup>[1]</sup> Data generated by [Mockaroo, LLC](https://mockaroo.com/), (2022). Realistic Data Generator.</br>


<p align="right">
<a href="https://github.com/theidari/pandas-challenge#-overview-of-project"><sup><b>⬆ BACK TO TOP ⬆</b></sup></a>
</P>
