---
layout: post
title: "Design for Understanding"
author: "Ally Smith"
categories: journal
tags: [documentation,sample]
image: ds2.webp
---

We investigated the difference between analytical and persuasive data visualizations. We brainstormed analytical and persuasive visualizations for a Movie dataset using the Five Design Sheet method. Then, we coded our finalized designs using CSS and HTML.

---

Hold onto your popcorn, because movie data analysis just got that much better! In this project, we sought to provide users with the ability to analyze a number of movie performance metrics in both an analytical and persuasive way. We wanted to provide users the ability to explore how different genres stack up over time, which movies won hearts (and wallets), and how budgets really influence those blockbuster hits. This post shows our team’s process as we built dynamic visuals to display this data.

![Intro Pic](assets/img/ds2intro.webp "Intro Pic")

## The Designs

We are excited to share a series of visuals for users to use and learn more about various aspects of movie production, profits, and popularity!

Click the hotlink to see the final designs: 
[Final Designs](https://allysmith.dcreate.domains/ "Final Designs")

## The Data Set

The dataset we utilized was pulled from Kaggle and consists of several key variables related to movies, offering insights into their production, financial performance, and public reception. The variables that we used are below with a short description of each:

* **title:** The movie's name.
* **release_year:** The year when the movie was officially released to the public.
* **revenue:** The total amount of money the movie generated globally, representing its financial success.
* **budget:** The cost associated with the movie's production, indicating the resources allocated for its creation.
* **popularity:** A score reflecting the movie’s overall appeal, derived from various sources such as user ratings, social media buzz, or online engagement metrics.
* **genres:** A comma-separated list of categories (e.g., action, drama, comedy) that classify the movie’s thematic content.
* **production_countries:** A comma-separated list of countries where the movie was produced, providing geographical context to its origins.

![Data Set Pic](assets/img/ds2production.webp "Data Set Pic")

Initially, the dataset consisted of nearly 1 million film productions from 1913 to 2023, many of which contained incomplete or irrelevant information or were TV productions (ex. NFL games). We applied a threshold of 1,000 for both budget and revenue, removing entries that did not meet this minimum, which helped focus our analysis on legitimate and relevant movie productions.

Additionally, we consolidated the genre classifications. The original data allowed each movie to be ranked into multiple genres. To simplify and create more easily readable visualizations, we selected the eight most prevalent genres and filtered out movies that did not fall into any of these categories. This consolidation ensured that the dataset remained manageable and lead to more interesting analysis.

After applying these cleaning steps, we reduced the dataset to approximately 10,000 movies (which can be seen here: Cleaned Data), making it more suitable for visualization and analysis. This cleaned dataset was then used to create both unbiased visualizations for neutral interpretation and more targeted visuals to steer users toward specific conclusions, as part of our exploration into how data representation can influence perception.

## The Task
Using this dataset, we had two layers to the assignment: first, to create visualizations that would allow users to analyze the data in an objective and unbiased manner, providing clear and transparent insights into movie production and performance and allowing the user to provide some sort of customization over their inquiries.

Second, we aimed to design three additional visuals with the intention to persuade the user. We wanted to make it clear which counties and movies in each respective genre were most popular. This approach allowed us to explore how data representation can influence perception while still remaining grounded in factual information.

## Design Process
### Analysis: 5 Design Sheets

**Sheet 1:** 

The purpose of sheet one was to get all of our ideas out there. The way we laid it out helped us stay organized; we described the data we had available to us and then identified ways we hoped to analyze the data. In the bottom we broke up our organization into ways to filter, ways to categorize, then experimented with some ways to combine the two. In sketches 2–4, the sheet was very helpful in helping us stay organized and allign with the original task.

![Analysis Sheet 1](assets/img/ds2sheet1.webp "Analysis Sheet 1")

**Sheet 2:** 

In this design we have three dynamic visuals, each of which adjusts based on the time period selected via a time slider at the top. In addition to the time slider, there is a genre dropdown menu that filters two of the graphs according to the selected genre.

The first graph, located on the left, is a pie chart that displays the distribution of the total number of movies produced within the selected time frame. It displays an overview of the volume of movie production over time according to genre.

To the right of the pie chart are two similar bar charts. The top bar chart highlights the top 10 and bottom 10 movies within the selected genre, based on their revenue-to-budget ratio. The top 10 movies are shown in blue, while the bottom 10, which likely will have negative ratios, are displayed in red and may fall below the zero line. Users can hover over each bar to view the movie’s poster, name, and exact revenue-to-budget ratio.

The bottom bar chart is structured similarly to the one above but focuses on popularity ratings. It showcases the top 10 and bottom 10 movies based on popularity within the selected genre, with blue representing the top 10 and red representing the bottom 10. Hover functionality is also included, providing additional details such as the movie poster, title, and precise popularity score.

![Analysis Sheet 2](assets/img/ds2sheet2.webp "Analysis Sheet 2")

**Sheet 3:**

On the left is a bar chart displaying the volume of movies produced per genre over time. This chart presents data across all available years and shows a comprehensive look at how movie production trends have evolved for each genre. Each is displayed individually making it easily observable for them to see each genres volume.

In the middle, a bar chart representing each genre shows the average budget for each film across each 20-year span. It enables the user to see how movie budgets have changed over time across genres. Users can filter the chart by genre using the dropdown menu to explore specific trends.

On the right, another scatter plot shows genre averages plotted according to their budget (x-axis) and revenue (y-axis), with a break-even line indicating where movies have 0 profit. This graph highlights which genres have been particularly profitable. Similar to the middle graph, this plot can also be filtered by genre using the dropdown menu, allowing users to focus on specific genres when analyzing profitability.

![Analysis Sheet 3](assets/img/ds2sheet3.webp "Analysis Sheet 3")

**Sheet 4:**

On the left, a stacked line graph presents the volume of movies produced across all genres over time. Each genre is represented by a different color within the stacked lines, providing a clear view of the total number of films produced, as well as the distribution across genres. This setup allows users to see both individual genre volumes and the aggregate movie production.

In the middle, a bar chart displays the average popularity score for each genre. Each genre has its own bar, making it easy to compare the relative popularity of different genres across the dataset.

On the right, another bar chart shows the average revenue-to-budget ratio for each genre. This chart highlights the financial efficiency of movies within each genre, indicating which genres tend to generate the highest returns on their budgets.

A genre dropdown filter is available, allowing users to focus on a specific genre in all three charts, tailoring the analysis to more targeted insights.

![Analysis Sheet 4](assets/img/ds2sheet4.webp "Analysis Sheet 4")

**Sheet 5:**

For our final sketch, we consulted some of our roommates to find the visuals they thought would be most helpful. They appreciated the separate line graphs for volume and the line plot reflecting popularity and budget. Finally, they liked a line graoh showing the relationship between revenue and budget.

On the left is a bar chart displaying the volume of movies produced per genre over time. This chart presents data across all available years and shows a comprehensive look at how movie production trends have evolved for each genre. Each is displayed individually making it easily observable for them to see each genre’s volume.

In the middle, a scatter plot visualizes individual movies as points, color-coded by genre. The x-axis represents time, and the y-axis represents the budget for each movie. The size of each point reflects the movie’s popularity score, giving a visual representation of how budget influences popularity over time. Users can filter the chart by genre using the dropdown menu to explore specific trends.

On the right, another scatter plot shows movies plotted according to their budget (x-axis) and revenue (y-axis), with a break-even line indicating where movies have 0 profit. This graph highlights which movies were particularly profitable. Similar to the middle graph, this plot can also be filtered by genre using the dropdown menu, allowing users to focus on specific genres when analyzing profitability.

![Analysis Sheet 5](assets/img/ds2sheet5.webp "Analysis Sheet 5")

### Persuasion: 5 Design Sheets

**Sheet 1:**

The goal of Sheet 1 was to explore our dataset and brainstorm various ways to visualize the data effectively. We began by analyzing our data to identify key elements that could be related or compared to each other. This helped us pinpoint topics that could be compelling and persuasive to users. We sketched preliminary visualizations to explore the potential direction of our designs, allowing room for iteration and refinement.

Next, we filtered the dataset and visualizations to align with our focus on persuasion and storytelling. Our aim is to create memorable representations that resonate with users long after they’ve left the page. To achieve this, we selected key elements: title, year, revenue, budget, revenue-to-budget ratio, genre, production countries, popularity, and release date. We then refined our designs into visualizations such as bar graphs, multi-line graphs, bubble charts, choropleth maps, word clouds, and movie clips or trailers. These formats use color, size, and even audio to create a lasting impression on the audience.

After filtering the data, we categorized the chosen visualizations. Bar charts and line graphs are ideal for displaying amounts over time or by category. Bubble charts and word clouds leverage color and size to highlight category differences, while choropleth maps and audio clips reveal geographic trends in movie data. The missing element in these visualizations is interactivity, which would further enhance user engagement and retention of the information.

To address this, we decided to combine and refine our visualizations. For example, pairing a bubble chart with a bar or line graph would show relationships between elements like popularity or budget over time. Clicking on a bubble could change the data displayed in the accompanying chart. Additionally, combining a bar chart with movie clips or audio would use sound to reinforce the data, making it more memorable. Finally, we paired the choropleth map with a word cloud to illustrate geographic differences in genre preferences and production budgets, with interactivity allowing users to explore data by location.

![Persuasive Sheet 1](assets/img/ds2sheet12.webp "Persuasive Sheet 1")

**Sheet 2:**

In Sheet 2, we refined our ideas around the question: Does production budget correlate with average popularity across movie genres? We designed two bubble charts — one showing the average budget for each genre, and the other showing average popularity. Users can interact with the bubbles, clicking one or more to display corresponding data in line graphs. Clicking a second time on a bubble will deselect it and remove it from the graphs. By hovering over the line graphs, users can see details such as genre, year, and popularity over time. The line graphs represent trends in the popularity or budget of genres throughout time. A third chart to the right compares genre budgets and popularity over time, providing a comprehensive view of the trends.

![Persuasive Sheet 2](assets/img/ds2sheet22.webp "Persuasive Sheet 2")

**Sheet 3:**

For Sheet 3, we focused on visualizing where movies are produced and when they are released. We designed a world map where users can click on a country to view its average production budget. Instead of using a traditional choropleth map, we opted for a more interactive design where a money bag icon fills up based on the selected country’s data. Upon clicking a country, the word clouds automatically update to display the most popular genres and release months, with size and color indicating the significance of each. Additionally, an audio clip that relates to the most popular genre in the country plays. To ensure accessibility, we considered alternatives for users with hearing or visual impairments, such as contrast adjustments for the word cloud and text alternatives for the audio.

![Persuasive Sheet 3](assets/img/ds2sheet32.webp "Persuasive Sheet 3")

**Sheet 4:**

In Sheet 4, we designed a unique way to display the “best” movies in each genre. The first bar chart features movie posters as bars, with the size of the poster representing the popularity of each genre. Each bar is a specific genre and the movie poster is for the most popular movie in that genre. Users can click on a poster to reveal another chart, showing the top 10 most popular movies in that genre, ordered by release date. Hovering over the posters provides additional information such as movie name, release date, popularity, and profit. When a user clicks on a genre, a video frame will play clips from the top 10 movies, while a popcorn bucket icon dynamically fills based on the currently displayed movie’s popularity, adding an engaging and memorable visual element.

![Persuasive Sheet 4](assets/img/ds2sheet42.webp "Persuasive Sheet 4")

**Sheet 5:**

The final sheet brings together our visualizations into a cohesive design plan. We combined elements from the first four sheets, ensuring a blend of graphs and multimedia stimuli to create a memorable and interactive experience for users. In our final design, we strived to portray our claim that the U.S. dominates global film production, particularly with family-friendly movies, which drive revenue. Family films appeal to larger audiences — often attracting families of four or more — leading to higher ticket sales compared to genres that cater to individuals or smaller groups. The final design includes a bubble chart, world map, and movie clip player. For the map, hovering over a country now fills the money bag icon, making it easier for users to compare production budgets across countries. The bubble chart retains its functionality from Sheet 2, but now users click on a bubble to be taken to a new page. This new page shows the selected genre’s top movie trailer and a popcorn bucket filled based on the genre’s popularity. Users can then interact with the page by playing the trailer or using the arrows to see the other genres’ pages.

![Persuasive Sheet 5](assets/img/ds2sheet52.webp "Persuasive Sheet 5")

## Final Designs
### Analysis

For the final version of our project, we decided to keep the three visualizations separate, as making them fully dynamic presented more of a challenge than anticipated. Instead, we hosted them on a clean GitHub page, where users can explore each chart along with descriptions of the project and the data visualizations.

The first visualization is a series of line graphs that show the volume of movies produced in each genre over time. By keeping them separate, users can easily distinguish and compare trends across genres without clutter.

The second graph is a dot plot where each movie is represented by a dot, with the size of the dot corresponding to the movie’s popularity. Users can filter this plot by genre, making it easier to focus on specific categories of films.

The third plot displays each movie’s revenue against its budget, allowing users to quickly spot which films were particularly successful. Hovering over the points reveals the movie’s name, adding an interactive layer to explore the data in more detail.

We followed the original design for the visuals closely and ensured the page is intuitive and user-friendly, making it simple for users to dive into the data and draw their own insights.

![Number of Movies Produced Past 100 Years](assets/img/ds2trends.webp "Number of Movies Produced Past 100 Years")
![Movie Budget, Popularity, Genre Trends](assets/img/ds2circles.webp "Movie Budget, Popularity, Genre Trends")
![Budget vs Revenue](assets/img/ds2budrev.webp "Budget vs Revenue")

### Pursuasion

Our process for actually creating and implementing our design ideas also occurred incrementally. Unsure if we had the technical skills to compete with our imagination, we started with the basics and advanced our web design as we completed simpler tasks. For example, in the creation of our theater page, we started by embedding the movie trailers for each genre and creating buttons that would allow us to click through each trailer. After accomplishing that feat, we attempted to create a visualization that would show a popularity comparison between the genres. Previously imagined as a popcorn bucket that changed fullness levels based on the popularity of the genre currently displayed, creating this visualization proved too difficult. So, we came up with an alternative, by using the number of individual popcorn kernels that lay beside a full popcorn bucket to visualize the differences in popularity across movie genres. Following user feedback, we incorporated additional text on the site so that users would understand what the popcorn kernels represented and why they changed on each slide. We also added a home button in the top left corner for users to return to the bubble chart page more easily.

When creating the map visualization, we also had to alter our design idea to fit our actual time and skills. Similar to the theater scene, we had the idea of creating a bag of money that would increase and decrease in fullness based on the average budget of the country the user was currently hovering over. As making the fullness level fluctuate was not an attainable goal given the context of the problem, we reassessed and chose to make the size of the bag change based on the average budget. Also, in creating our storyline, we decided to include a country comparison piece by providing a static money bag that reflected the average budget for movies produced in the U.S. Then, when the user hovers over a country, another money bag will appear next to the U.S. bag for comparison purposes. By providing a reflection point, the visualization communicates more than it would if it just displayed the average budgets for each country in isolation. Also, following user feedback, we included the name of the country the user was currently hovering over and the country’s average budget below the money bag so that the user’s focus during the comparison could remain in one place.

![Movie Popularity Bubble Chart](assets/img/ds2bubbles.webp "Movie Popularity Bubble Chart")
![Stage Model with popcorn bucket](assets/img/ds2stage.webp "Stage")
![World Map and money bags](assets/img/ds2map.webp "Map")

## Analysis vs Pursuasion
Our persuasion graphs had a clear and focused purpose: to emphasize America’s dominance in film production and persuade users to watch the most popular movies in each genre. Through a visually engaging design, we highlighted family-friendly films’ prominence in the industry and showcased the most popular movie trailers, reinforcing the message. Additionally, the graphs illustrated how the U.S. spends significantly more on film production compared to other countries, creating a compelling narrative around the influence of American cinema.

In contrast, our analytical graphs were designed to give users the freedom to explore the data on their own. These graphs offered a range of insights, from production trends to profitability and popularity, without directing users toward a specific conclusion. Instead, they provided interactive tools and genre filters, that allowed users to tailor their exploration and draw their own insights from the data. This approach empowered users to analyze trends and relationships in the film industry based on their interests.

## Demo Video
Click here to see the demo video for clearer instructions on how to use the visualizations!

Click the hotlink to see the final designs: 
[Final Designs](https://allysmith.dcreate.domains/ "Final Designs")

## Conclusion
In this project, we took on the challenge of turning a complicated set of movie data into visuals that anyone could enjoy both in an analytical and predetermined persuasive way. We created a series of visuals (pie charts, bar graphs, scatter plots, and maps) that let users dive deep into trends over time and across genres. With interactive features like sliders and filters, we made it easy for users to play director and pull out the key scenes from all that data. In the end, we think we’ve turned this data from a boring B-movie into an Oscar-worthy hit. That’s a wrap!