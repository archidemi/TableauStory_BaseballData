# A Tableau Story of Baseball Data

The initial version: https://public.tableau.com/profile/ssni#!/vizhome/baseball_v1_1/Story1

The final version: https://public.tableau.com/profile/ssni#!/vizhome/baseball_v2_1/Baseball_Story

### Summary
The dataset (baseball.csv) consists of 1157 players' following attributes:
+ Handedness: left, right or both
+ Height: in inches
+ Weight: in pounds
+ Avg: batting average
+ HR: number of home runs
+ ID: integer sequence as primary key

I'm interested in finding what features contribute to high batting average, successful home runs, and the relationship between batting average and home runs.

The percentage of left-handed people are much higher than in ordinary population (widely considered 10%). Are lefties doing greater job than righties on baseball fields?

### Design
1. Top players are displayed in bar charts to present a straightforward view and the comparable differences between each person. In the fianl version, the axis and titles are refined to provide a more enunciating visualization. Two bar charts are laid out side by side instead of up and down, so readers can compare the names more easily.
  
2. Scatter plots are best for displaying relationships. Height and weight are positively correlated. Different coloring are applied to indicate the batting average and home run changes over the grid, in order to tell us a second relationship between the performance and the physical attributes.

3. Histograms are used to show the distribution of the players' height and weight. The distributions look pretty normal, with most people in the middle. By coloring the bins with gradient palette, it's quite obvious to grasp which bin gets the highest average score, and even trends.

4. Another scatter plot of batting average vs. home runs also tells the relationship between the two. I first added two layers of height and weight on the points, but the graph turned out to be too crammed and losing information when zoomed in. So in the final version, a single layer of handedness is applied, all data included. Then an important relationship shows up (good batting average is essential for more successful home runs).

5. The handedness is categorical, so in order to look at how different types of handedness work, a box plot is decided. It gives us the quantiles, maxes and mins, and where major people fall in each group. A bar chart only showing the average sits together for people who have difficulties reading box plots.

6. One more dashboard is added in the final version to draw conclusions. Several key plots are put together to filter and play around.

### Feedback
Questions are gathered from readers with no data analysis background against the first sketch.

#### Plot 1
1. What does the "avg" take average on? What does "HR" mean? Count?
1. Are there easier ways to present no overlap exists?
1. "Runner" sounds different from "home runner".

#### Plot 2
1. What's the "Avg.Avg."?
1. No idea how to read the box plot.

#### Plot 3
1. This is a good one!

#### Plot 4
1. What does the color mean?

#### Plot 5
1. The plot names "h-bat-hist", "w-bat-hist" seem mysterious...

#### Plot 6
1. Only encoding with color or size may be more straightforward instead of the two indicating the same thing.

#### Plot 7
1. The same problem as in Plot 5.

#### Plot 8
1. Lots of presentation but lack of information.

### Resources
https://onlinehelp.tableau.com/current/pro/desktop/en-us/buildexamples_histogram.html  
https://en.wikipedia.org/wiki/Batting_average
