# 🚀 Assignment 6: Global Energy Insights – Line Chart, Bar Chart, and Scatter Plot

(I have included the README.md and cleaned dataset on my github in a public repo since Canvas would not let me upload a .csv file: https://github.com/VM25/478_Assignment6)

In this assignment, you will explore global energy trends and relationships using the D3.js library. You will create three interactive visualizations:
1. 📈 **Line Chart**: Analyze energy consumption trends over time.
2. 📊 **Bar Chart**: Compare renewable energy contributions across countries.
3. 🟢 **Scatter Plot**: Examine the relationship between economic factors and energy consumption.

The purpose of this assignment is to test your ability to:
- Build and customize multiple visualizations using D3.js.
- Apply transitions, scales, and interactivity.
- Analyze and communicate data insights through visualizations.

---

## 📂 Dataset Description

We will use the **Global Energy Consumption Dataset** from Kaggle (https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption), which contains data on energy production and consumption by country and year. The dataset has been preprocessed for this assignment and includes the following columns:
- 🗓️ `year`: Year of observation.
- 🌍 `country`: Name of the country.
- ⚡ `primary_energy_consumption`: Total energy consumption (in TWh).
- ♻️ `renewables_share_energy`: Percentage of total energy derived from renewable sources.
- 👥 `population`: Total population of the country.
- 💵 `gdp`: Gross domestic product (in USD).

You should include the dataset in a `data` folder of the repository, named `dataset.csv`, thus making the path to the dataset: `data/dataset.csv`

---

## 🛠️ Getting Started

1. Clone this repository to your local machine.
2. Create the source code files (`index.html`, `style.css`, and `[Your ASUrite].js (example: cbryan16.js)`) to implement the assignment requirements.
3. Use a local server (e.g., HTTP Simple Server) to open `index.html`.
💡 **Important**: Remember that homeworks will be graded in Chrome using VS Code’s Live Server.

---

## 📝 Assignment Steps

### Step 0: Setup 🧰
- Create a `index.html` file and add your **Full Name** (example: Chris Bryan) and **ASU Email** (example: cbryan16@asu.edu) to the top of the page.

---

### Step 1: Line Chart – Energy Trends 📈
1. **Create an SVG**:
   - Add a responsive SVG to the `line-chart` section of the page.
2. **Set Up Axes**:
   - Use the **x-axis** for `year` and the **y-axis** for `primary_energy_consumption`.
   - Map the axes using `d3.scaleTime` for the x-axis and `d3.scaleLinear` for the y-axis.
3. **Dropdown Menu**:
   - Add a dropdown to select a `country`. When the user changes the selection, update the line chart to display energy trends for the chosen country.
4. **Tooltips**:
   - Add interactive tooltips that display the year and energy consumption when hovering over the line.
5. **Transitions**:
   - Animate the transition when switching countries for a smooth user experience.

---

### Step 2: Bar Chart – Renewable Energy Contributions 📊
1. **Create an SVG**:
   - Add a responsive SVG to the `bar-chart` section.
2. **Set Up Axes**:
   - Use the **x-axis** for `country` and the **y-axis** for `renewables_share_energy`.
3. **Dropdown Menu**:
   - Add a dropdown to select a `year`. Update the bar chart to show renewable energy contributions for all countries in that year.
4. **Color Coding**:
   - Use distinct colors for each bar to represent countries clearly.
5. **Tooltips**:
   - Display the country name and renewable energy percentage on hover.
6. **Highlighting**:
   - Highlight the country with the highest renewable share dynamically.

---

### Step 3: Scatter Plot – Economic Factors and Energy Use 🟢
1. **Create an SVG**:
   - Add a responsive SVG to the `scatter-plot` section.
2. **Set Up Axes**:
   - Use the **x-axis** for `gdp` and the **y-axis** for `primary_energy_consumption`.
3. **Bubble Sizes**:
   - Represent `population` using the size of each bubble.
4. **Dropdown Menu**:
   - Add a dropdown to filter the scatter plot by `region`. Only points for countries in the selected region should be displayed.
5. **Tooltips**:
   - Show the country name, GDP, energy consumption, and population when hovering over a point.
6. **Legend**:
   - Include a legend to explain bubble sizes and colors.

---

## ⭐ Extra Credit

There are three ways you can potentially receive extra credit for this assignment. A maximum of 2 extra credit points can be added to this assignment.

1. 🌟 **Animations**:
   - Add smooth transitions for updates to the line chart, bar chart, and scatter plot. (+1)
2. ⚙️ **Normalization**:
   - Allow users to toggle between absolute values and normalized metrics (e.g., energy consumption per capita). (+1)
3. 🌟 **Dynamic Highlights**:
   - Highlight countries with the highest or lowest energy metrics dynamically. (+1)

---

## 💡 Hints & Resources

### Hints
- 🛠️ Use `d3.axisBottom` and `d3.axisLeft` to create and update axes dynamically.
- 🎨 Explore color scales from [D3 Scale Chromatic](https://github.com/d3/d3-scale-chromatic) for consistent and appealing designs.
- 🖱️ Tooltips can be implemented using an invisible `<div>` that appears on hover and follows the mouse.

### Resources
- 📘 [D3 Line Chart Documentation](https://observablehq.com/@d3/line-chart)
- 📘 [D3 Bar Chart Examples](https://observablehq.com/@d3/bar-chart)
- 📘 [D3 Scatter Plot Examples](https://observablehq.com/@d3/scatterplot)

---

## 📤 Submission Instructions

Submit the following files:
1. `index.html`: Your main HTML file.
2. `style.css`: Styling for your visualizations.
3. `[ASUrite].js`: D3.js code for the assignment.
4. `data/dataset.csv`: Preprocessed dataset or a link to the raw dataset.

**Ensure your visualizations render correctly in Chrome using VS Code’s Live Server.**

---

## 📊 Grading

This assignment is worth up to 10 points, with extra credit contributing an additional 2 points. The grading breakdown is as follows:

- Step 0 is worth 1 point
- Step 1 is worth 3 points
- Step 2 is worth 3 points
- Step 3 is worth 3 points
- ⭐ The Extra Credit is worth up to 2 bonus points

Good luck! 🎉