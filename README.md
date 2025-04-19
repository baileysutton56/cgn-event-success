# Which Event Is Most Important to a Team’s Success?
This article is part of College Gym News's [Data Deep Dive](https://collegegymnews.com/category/data/) series. [College Gym News](https://collegegymnews.com/) is "a one-stop-shop for college gymnastics news" and provides a wide-variety of coverage from more than 30 contributors. 

The full article can be found [here](https://collegegymnews.com/2024/02/12/data-deep-dive-which-event-is-most-important-to-a-teams-success/). Statistical analysis and writing was completed by Bailey Sutton with additional writing contributions by Dara Tan. 

## Navigation
- **:computer: code:** Files for scraping data from [Road to Nationals (RTN)](https://roadtonationals.com/results/index.php) and statistical analysis
- **:file_folder: data:** Team and event ranking data files
- **:bar_chart: plots:** Faceted line charts

## Methods
### Data
The data for this project comes from [Road to Nationals (RTN)](https://roadtonationals.com/results/index.php), the official statistical site of NCAA Gymnastics.

2023 Team and event rankings were scraped using the scraping_rtn Python package developed by CGN Senior Data Editor Claire Harmon.

### Programs
Data scraping was done with Python using Google Colab. Analysis was done in R and graphics were created using `ggplot2`.

## Results
The purpose of this project is to compare a team's final ranking to their final event ranking from the 2023 season to determine if one of the four events has a greater impact on a team's overall ranking than the others.

When looking at the relationships between each event ranking and the final team ranking, nearly all events have a 1:1 relationship with final team ranking with uneven bars having the strongest relationship. At the top and bottom of the rankings on each event, tight clustering indicates that those teams perform about as expected given their overall team ranking. The variation in the middle of each graph shows that mid-ranked teams have a greater tendency to overperform (be above the expected performance line) or underperform (be below the line).

<p align="center">
<img src="https://github.com/user-attachments/assets/cb0ef741-1422-48d0-9d2e-dc487e54091c" width=50% height=50%>
</p>

When breaking this out by conference, some trends appear when looking at overperformers and underperformers. The SEC, NCGA East, WIAC, and three independent teams all perform about as expected while the Big Ten, Big 12, EAGL, MPSF, and MAC conferences all have 70% or more of their teams with at least one major deviation. 

<p align="center">
<img src="https://github.com/user-attachments/assets/0ec68782-071c-4fa8-9f57-9f244291ade3" width=50% height=50%>
</p>

While no one event can determine a team's final ranking, especially at the top and bottom of the rankings, teams in the middle can climb the rankings with a couple standout events.
