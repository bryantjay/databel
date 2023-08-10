# Data Prep

### Calculating Churn

###### Convert "Churn Label" to an easier-to-work-with numeric format, "Churned". Then, use this field to calcuate "Number of Churned Customers" and "Churn Rate".

**Churned** <- IF [Churn Label] = 'Yes' THEN 1 ELSE 0 END

**Churned Customers** <- SUM([Churned])

**Churn Rate** <- [Number of Churned Customers] / [Number of Unique Customers]

**Avg Customer Service Calls Per Customers** <- SUM([Customer Service Calls]) / [Number of Customers]

### Age bins

Automatically generate bins for the Age variable, using "Create > Bins" in the data pane.

### Data Groups

Create new group for Monthly Data GB Downloads, in order to convert it to a easier-to-analyze discrete format.

### Metric Parameter

Make a parameter and corresponding calculated field to easily change between different numeric metrics. This will be used in the following age and group plan visuals.
