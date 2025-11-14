#  **  TITANIC DATASET ANALYSIS**

This repository contains the full set of visualization tasks and instructions for the Titanic Dataset and Coffee Dataset.

All visualizations are created using Tableau Desktop, with clear steps for reproducing each chart.

Tasks Included




#### (i) Bar Chart — Passengers vs Gender
- **Drag:** Sex → Columns, PassengerId → Rows.
- **Modify:** Change PassengerId to **Count**.
- **View:** Select **Bar Chart**.



#### (ii) Survival Count by Gender
- **Drag:** Sex → Columns, Survived → Rows.
- **Add:** PassengerId → Rows → Set to **Count**.
- **View:** Choose **Stacked Bar Chart**.



#### (iii) Survival Rate by Passenger Class
- **Drag:** Pclass → Columns, Survived → Rows.
- **Modify:** Change aggregation of Survived **SUM → AVG** (survival rate).
- **View:** Bar Chart.



#### (iv) Age Distribution (Histogram)
- **Drag:** Age → Columns, PassengerId → Rows (Count).
- **Create:** Right-click Age → **Create → Bins** → bin size = **5 or 10**.
- **View:** Histogram.



#### (v) Average Fare by Class
- **Drag:** Pclass → Columns, Fare → Rows.
- **Modify:** Change Fare aggregation to **Average**.
- **View:** Bar Chart.



#### (vi) Scatter Plot — Fare vs Age
- **Drag:** Age → Columns, Fare → Rows.
- **Modify:** Mark Type → **Circle**.



#### (vii) Passenger Count by Embarkation Port
- **Drag:** Embarked → Columns, PassengerId → Rows → Set to **Count**.
- **View:** Bar Chart.



#### (viii) Survival Heatmap — Gender vs Class
- **Drag:** Sex → Columns, Pclass → Rows.
- **Add:** Survived → Color → Set aggregation = **AVG**.
- **Modify:** Mark Type → **Square (Heatmap)**.



#### (ix) Box Plot — Age vs Survival
- **Drag:** Survived → Columns, Age → Rows.
- **Add:** Analysis → **Box Plot**.



#### (x) Pie Chart — Dimension + Measure
**Example:** Gender distribution of passengers  
- **Drag:** Sex → Color, PassengerId → Rows → Set to **Count**.
- **Modify:** Mark Type → **Pie**.
- **Label:** Add Sex + Count to Label.

---















#  **  COFFEE CHAIN DATASET ANALYSIS**

Tasks Included 

#### (i) Heat Map — Product Type, State, and Profit  
- **Drag:** Product Type → Rows, State → Columns, Profit → Color.  
- **Identify:** The state with the *lowest profit* for **Espresso** by checking the darkest (lowest) color.

#### (ii) Box Plot — Espresso Sales Distribution  
- **Drag:** Product → Columns, Sales → Rows, Filter Product Type = Espresso.  
- **Add:** Analysis → Box Plot.  
- **Identify:** The Espresso product with the *highest spread* in sales.

#### (iii) Bar Chart — Product Type, Product, and Profit  
- **Drag:** Product Type → Columns, Product → Color, Profit → Rows.  
- **Conclusion:** Shows which product types drive profit or loss.

#### (iv) Scatter Plot — State, Sales, and Profit  
- **Drag:** State → Columns, Sales → Rows, Profit → Color, Mark Type → Circle.  
- **Conclusion:** States with high sales but low profit can be identified easily.

#### (v) Identify Highest & Lowest Profit State  
- **Create View:** Drag State → Rows, Profit → Columns.  
- Sort descending to find **highest** and **lowest** profit states.

#### (vi) Sales in Nevada for Decaf Espresso  
- Apply **Filters:** State = Nevada, Product = Decaf Espresso.  
- Observe total **Sales** in the view.

#### (vii) Contribution of Tea to Overall Profit (%)  
- **Filter:** Product Type = Tea.  
- Compute: `SUM(Profit for Tea) / SUM(Profit for All)` × 100.

#### (viii) Average Marketing in Area Codes 660 and 818  
- Filter Area Code = 660, 818 → Drag Marketing → Rows → Measure = Average.

#### (ix) Highest & Lowest Profit Product in California  
- Filter State = California → Drag Product → Rows, Profit → Columns.  
- Sort to identify top and bottom products.

#### (x) Side-by-Side Circles — Minimum Marketing for Coffee Beans (Colombian)  
- Filter Product = Coffee Beans Colombian → Drag Marketing → Rows, Market → Columns, Mark = Circle.  
- Identify the minimum marketing value visually.

#### (xi) Contribution of Sales in East Market for Decaf  
- Filter Product Type = Decaf → Market = East.  
- Compute `(Sales in East for Decaf / Total Sales) × 100`.

#### (xii) Contribution of Decaf Sales in East Market (2012)  
- Add filter for **Order Date (Year = 2012)**.  
- Repeat the above percentage calculation.

#### (xiii) Average Profit for Products Starting with “C”  
- Apply **Filter → Product → Starts With “C”**.  
- Drag Profit → Rows → Measure = Average.

#### (xiv) Central Region — Top 5 Products by Sales  
- Filter Region = Central → Sort by Sales → Keep Top 5.  
- Compute `(Sales of Top 5 / Total Sales) × 100`.

#### (xv) 2013 — Highest Profit State in West Market  
- Filter Year = 2013 and Market = West.  
- Sort Profit by descending → identify top state.

#### (xvi) Total Expenses-to-Sales Ratio of State with Lowest Profit  
- Identify state with lowest profit → Create Calculated Field:  
  `SUM(Expenses) / SUM(Sales)`.

#### (xvii) Distinct Count of Area Codes — Lowest Budget Margin, Small Markets  
- Filter Market Size = Small → Identify lowest Budget Margin state.  
- Drag Area Code → Rows → Measure = Count (Distinct).

#### (xviii) 2013 — % of Profit for Caffe Mocha (Major Market)  
- Filter Year = 2013, Product = Caffe Mocha, Market = Major.  
- Compute `(Profit of Caffe Mocha Major / Total Profit 2013) × 100`.

#### (xix) Month-Year when Decaf Sales Crossed $1,100 (Colorado & Florida)  
- Filter Product Type = Decaf, State = Colorado & Florida.  
- Drag Order Date → Columns → Set to Month/Year, Sales → Rows.  
- Add reference line at 1100 → Identify the bars crossing that line.

#### (xx) Tree Map — Market by Budget Sales  
- Drag Market → Label, Budget Sales → Size & Color → Mark Type = Tree Map.  
- Identify market with the **largest rectangle** (maximum budget sales).

---

