# Electric Vehicle Data Analysis: Hypothesis Testing, Correlation Analysis, and Clustering

This project utilizes an extensive electric vehicle (EV) specifications dataset to uncover meaningful patterns and relationships among key technical and performance indicators. The methodology integrates hypothesis testing, correlation analysis, and clustering techniques to provide actionable insights for manufacturers, researchers, and consumers interested in EV technology.

## Exploratory Data Analysis
Upon exploration of the dataset, the following insights are drawn.
We have 42 Mercedes-Benz vehicles which is the most in our dataset, with 19 SUVs, 14 sedans and 9 small passenger vans. There are 22 vehicles with 210 km/h as top speed(10 SUVs and 12 sedans). There is one SUV with a top speed of 240 km/h, 1 sedan each with 220 km/h and 250 km/h. There are 13 SUVs and 9 sedans with AWD, 3 SUVs and 5 sedans with RWD and 3 SUVs and 9 vans with FWD.
1. The model GranTurismo Folgore by Maserati is the fastest with speed 325 km/h, followed by Taycan Turbo GT Weissach by Porsche with the speed 305 km/h.
2. The model Spring Electric 45 by Dacia is the most efficient with 109 Wh/km, followed by Fiat's  500e Hatchback 24 kWh, 500e 3+1 24 kWh and 500e Cabrio 24 kWh with 112 Wh/km.
3. The model, EQS 450+ by Mercedez-Benz has the highest driving range of 685 km, followed by Lucid's Air Grand Touring with 665 km under ideal or test conditions.

## Data Visualization

<img width="566" height="457" alt="output-speeddistribution" src="https://github.com/user-attachments/assets/4645c2ff-a84d-4441-b363-acc4bc36045a" />
<img width="1183" height="784" alt="top10brands-output" src="https://github.com/user-attachments/assets/b9661a35-42d6-4fc7-8f0f-80dea14543e7" />
<img width="575" height="589" alt="output-carbodydistribution" src="https://github.com/user-attachments/assets/8c85bfaa-5c9e-4a4e-a811-ff745959d310" />

## Hypothesis Testing

The first stage involves formulating and testing hypotheses on performance differences among various EV body types. There's a very strong positive correlation between battery capacity and range. As battery capacity (in kWh) increases, the driving range (in km) increases significantly — which makes intuitive sense and is statistically supported.

<img width="984" height="584" alt="hypothesistest" src="https://github.com/user-attachments/assets/ac51df66-d8f1-4f78-baf6-26e9562fb5f0" />

## Correlation Analysis

The second phase focuses on exploring quantitative relationships between numerical features. Pearson correlation coefficient(-0.82) is calculated between variables such as top speed and acceleration. Looking at the values, they are inversely correlated. That is, the vehicles that has the highest top speeds, takes less time to reach 100 km/h from standstill. This step reveals which technical factors most influence the overall performance and efficiency of EVs, highlighting where improvements could have substantial effects.

## Clustering Analysis

Finally, K-Means clustering algorithm is used to group vehicles into categories based on their specifications (e.g., range, battery size, acceleration, and power). By standardizing the data and defining optimal cluster numbers, the analysis uncovers natural groupings, such as high-performance sports EVs, long-range family vehicles, and affordable urban commuters. Each cluster's profile is analyzed, providing a basis for market segmentation and targeted product development.
<img width="984" height="684" alt="cluster-output" src="https://github.com/user-attachments/assets/843b3311-dbc6-4dec-b325-add582e4e2ee" />
<img width="909" height="384" alt="heatmap-cluster-meansoutput" src="https://github.com/user-attachments/assets/ce769866-08f3-4201-93c4-377b1580b340" />

## Conclusion

This comprehensive approach leverages statistical inference and machine learning to transform raw data into knowledge. Hypothesis testing validates or refutes preconceived notions, correlation analysis elucidates key relationships, and clustering uncovers hidden market segments. The findings enable better engineering decisions, more informed consumer choices, and targeted improvements in EV design and marketing.
