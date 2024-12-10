---
layout: post
title: "Re-Design and Extend"
author: "Ally Smith"
categories: journal
tags: [documentation,sample]
image: ds4.jpg
---

To further understand the design process, we needed to learn about re-designing products and ensuring they are accessible. So, we created physical visualizations of our Design for Understanding data visualizations that are accessible for visually impaired or blind users.

---

For this design sprint, our group has been tasked with redesigning data visualizations that we worked on earlier in the semester, as data physicalizations. The visualizations that we chose visualized a movie dataset from Kaggle. This data set contains information on the number of movies made for each genre, the budget of each movie, the revenue of each movie, ratings, popularity, and much more.

Our digital visualizations were created using D3 and hosted locally on a webpage. For the analysis portion of the assignment our visualizations consisted of multiple line charts showing the number of movies made in each genre in the past century, a dot plot that shows the budget versus revenue for each movie genre, and a scaled dot plot showing the popularity and budget of each movie genre over time. For the persuasive visualizations, we created a bubble chart where each bubble represented a movie genre and the size and shade of each bubble represented the popularity of that specific genre. This visualization was also interactive. By clicking on a bubble you would be redirected to a movie-themed page where the trailer for the most popular movie in that genre is shown as well as a popcorn bucket that visualizes the genre’s overall popularity by the amount of kernels lying beside the bucket. Next, we will dive into our evaluation and analysis methodology.

## Evaluation

To evaluate our digital visualizations, we employed usability testing as our primary methodology. This involved asking users to complete a series of tasks and answer specific questions while interacting with our visualizations. The goal was to observe how effectively users could navigate, understand, and extract insights from the visualizations, while also identifying any areas of confusion or difficulty.

We chose usability testing because it provides direct feedback from real users, allowing us to assess the practical effectiveness of our visualizations in a controlled yet realistic environment. Unlike heuristic evaluations, which identify potential issues based on design principles, usability testing focuses on how end users actually interact with the product. This makes it particularly valuable for uncovering issues that might not be immediately apparent to designers. Through usability testing, we were able to observe users’ natural reactions and interactions with the visualizations, allowing us to pinpoint specific areas where users struggled.

The insights gathered from usability testing will be instrumental as we transition from digital visualizations to physical representations (physicalizations) of the data. By understanding where users found the digital visualizations easy or difficult to navigate, we can apply these lessons to the design of physical artifacts. For example, if users had trouble distinguishing between similar data points in digital form, we might consider using distinct tactile features or larger physical scales in a physicalization. Usability testing helps us identify which design elements need refinement, ultimately guiding us toward creating more effective and user-friendly physical representations of data.

To evaluate our existing data visualizations, we reached out to numerous individuals and asked them a series of questions to examine the usability of our work. The series of questions included the following:

* Compare the popularity of the horror genre and the family genre.
* What was the most popular comedy movie?
* Compared to the rest of the world, does the U.S. spend a lot of money per movie?
* What is the most popular movie genre in the last 10 years?
* Do higher-budget action movies tend to have higher revenue than higher-budget romance movies or vice versa?
* In 2000, what movie genre made the most movies?

These questions were developed as basic usability tests, to evaluate whether users with little previous use of the site could navigate through it and glean basic information. Overall, participants were successful in correctly answering the questions posed to them and found the site intuitive and easy to navigate. Below, we have included a breakdown of the feedback we received for each question asked.

## Usability Testing Results

### Compare the popularity of the horror genre and the family genre.

When asked to “Compare the popularity of the horror genre and the family genre” all participants navigated to the bubble chart visualization and either hovered over the horror and family genre bubbles to compare the popularity in the pop ups that appear when hovered over, or clicked on each bubble and compared the popularity of each genre on the movie theater site that is linked when you click a bubble. Participants answered this question very quickly. Feedback included praise for showing the differences in popularity between movie genres both by size and color of the bubble. More constructive criticism suggested we add a more direct explanation of what our popularity metric meant and how it was measured.

### What was the most popular comedy movie?

All participants were again able to answer quickly and accurately. Some participants hovered over the comedy bubble on the bubble chart page, and then clicked to be rerouted to the movie theater page where the trailers for the top movies in each genre were displayed. With the #1 ribbon attached to each movie trailer, participants quickly understood that the movies showcased were the top movie for each genre. Other participants used the budget and popularity visualization from the analysis section of the project. Here, the process for finding the most popular comedy movie was more difficult, as one had to first isolate all of the comedy movies by clicking on the comedy genre in the legend of the chart, and then visually compare the sizes of the remaining bubbles scattered across the chart. One participant acknowledged that they were able to find the correct answer quickly, but only because the difference in popularity between Barbie and the next most popular comedy movie was so stark. Additionally, users wanted the ability to click on each bubble on the chart to find out more information about the movie the data point represented, instead of simply hovering over the bubble to get the name of the movie to appear.

### Compared to the rest of the world, does the U.S. spend a lot of money per movie?

After navigating to the map visualization and taking some time to read the directions and fully understand the visualization, all participants spent time hovering over different countries on the map to compare to the reference point of the U.S. budget per movie that remained on the page at all times. All were able to come to the same conclusion that the U.S. spends a lot more money per movie than the rest of the world. One individual even pointed out the few countries that spent more than the U.S., but still acknowledged the general trend. The primary critique received on this visualization was related to how the comparison was being shown and the visibility of the visualization as a whole. One participant requested a zoom button so that they could better see individual countries on the map as they explored the visualization. Another thought there may be a better way to visualize the comparison between average budget per movie in the U.S. and the average movie budget in each country a user hovered over, than the scalable money bag. Another suggested including differences in shading of each country as an additional comparison point to visualize the budget differences.

### What was the most popular movie genre in the last 10 years?

Participants had the most difficulty finding the answer to this question and using the visualizations correctly. We expected users to use the Budget and Popularity visualization to answer this question, yet it was not clear to many users where to look. Once viewing the Budget and Popularity chart, users did not know how to use all of the features of the visualization, including that they could hover over or click the genre name in the legend and only the data points corresponding to that genre would appear on the chart. In addition, the bubbles would change transparency without a clear signal of what the user did to cause this or how to undo this action. Many noted that the visualization was not very intuitive to interpret either, as they did not understand that the size of the bubbles correlated to their popularity, even with instructions in the legend. Users also wished they could filter the chart to only show data points within a certain time frame, which would have allowed them to more easily answer this question. Other users never navigated to the correct visualization and failed to answer this question properly.

### Do higher-budget action movies tend to have higher revenue than higher-budget romance movies or vice versa?

We expected participants to navigate to the Budget vs. Revenue visualization to answer this question. While most navigated to the correct site, once there, many had difficulty interpreting the graph. Using the drop-down menu to change between the action graph being visible and the romance graph being visual, users wished there was a way for them both to be on the screen together for easier comparison. Many also did not know how to interpret the line of best fit and so didn’t have the intuition needed to understand the graph, while those who had the math background to understand this metric, found it very useful. Others thought the graph and data points were too small to easily analyze and wished there were numbers they could reference to answer this question instead of trying to figure this out solely by looking at the visual differences between the two charts.

### In 2000, what movie genre made the most movies?

Finally, we asked, “In 2000, what movie genre made the most movies?” Users navigated quickly to the correct visualization to answer this question and then slowly looked at each graph to try and identify which genre made the most movies in 2000. One user scanned through each graph while holding a finger on the highest value they currently had found to compare the current highest number to the values they found on each following graph. All users were able to correctly answer this question. Common suggestions included removing the commas from the year labels on the x-axis and adding unit labels to the y-axis to make clear what was actually being represented. Others wished the graphs were bigger to make interpretation easier and to have access to exact numbers when they hovered or interacted with the graph in another way so they could answer this question confidently instead of guessing based on how the graphs looked.

## Using the Results to Make Design Choices

With the results from our usability testing, we decided to focus on accessibility for our physical visualizations, as even users with no known impairments often had difficulty seeing our digital visualizations and interacting with them. We focused on designing physicalizations that users who are visually impaired or blind could use. In the analysis visualizations, users need to be able to easily compare genres with low cognitive load. For example, in our digital graph that compares movies’ revenue to budget ratios, a user can only view one genre at a time. Therefore, when asked to find the difference between two genres, they had to use the dropdown menu and remember what the previous graph looked like to tell the difference between it and the current graph. So, as seen in our sketches below, users will be able to compare the average revenue-to-budget ratio of genres based on weight and number of coins. This will allow them to hold the coins belonging to more than one genre at a time and directly compare the weights and amounts. Furthermore, during our usability testing, when asked to find the genre that produced the most films in the year 2000, one participant used their fingers to help them compare across genres and keep track of the current largest genre. We will adopt this technique to make our physicalizations more accessible because by creating 3D graphs, made with pipe cleaners, that users will be able to tacitly trace. We will also implement feedback from this visualization by making the graphs larger and mobile. So, a user will be able to move the different genres’ graphs so they can compare different genres side by side. In our persuasive visualizations, users initially compared the genres’ popularities based on the size and shade of the circles. Then, they hovered over the circles for more specific information. We can implement this in a physicalization by allowing users to feel the difference in size between genres’ circles and having labels where they can find the actual popularity score. Along with this, the interactivity between the bubble chart and stage page helps engage users. So, we will add this interactivity into our physicalizations. The addition of the auditory sense used in the stage page helps users remember the data. Therefore, we will also continue using audio to portray our information.

## Physical Prototyping Brainstorming & Sketching
### Sketches for Analysis Graphs

To create interactive and accessible visualizations of our data, we decided to represent it using eight popcorn buckets, each corresponding to a movie genre. Each bucket would correspond to a tactile line graph: the axes are outlined with raised puffy paint, the data line is represented by a pipe cleaner, and the labels are in Braille. This design allows visually impaired users to feel data trends and make comparisons across genres by tracing along the axes and pipe cleaner lines. To indicate each genre’s success rate, we added coins to each bucket representing the average revenue-to-budget ratio, with more coins signifying higher profitability. Users would be able to feel the difference in weight between buckets or hold the coins. Additionally, each bucket included a movie ticket displaying the name of the most popular movie in that genre. The buckets, line graphs, and tickets will be labeled in Braille. Through these physicalizations, users can analyze changes in the number of movies produced per genre over time, compare revenue-to-budget ratios across genres, and identify the most popular movie in each genre.

### Sketches for Persuasive Graphs

For the persuasive visualizations, we focused on making the bubble chart and stage page into interactive and tactile physicalizations so a user who is visually impaired or blind can investigate our data set. Our original visualizations are to the right of our new sketches as a reference. We planned to have 8 cylinders, one for each genre, that have a proportionally sized diameter to represent a particular genre’s average popularity. Each cylinder was to be labeled with the genre name and the popularity score. A user could pick up, hold, and stack the cylinders to compare the sizes. Then, a user could place one of these cylinders on a button inside our miniature stage model. When they press down, a noise relating to the specific genre will play. For example, if the cylinder they place is for comedy, they will hear laughter when they press the button. Due to time and supply constraints, we used Wizard of Oz prototyping to demonstrate this. When a user presses a cylinder on the button, we would play an audio clip from our computer. We obtained the audio clips relating to each genre online. If we were able to, we would use a Raspberry Pi to make the button truly play the audio clip. To ensure users with visual impairments will get the most out of our physicalization, we would also have Braille labeling. Also, the button would be raised and feel different from the rest of the stage to act as a tactile guide for users. Through this physicalization, users could compare movie genres based on popularity. The additional interactivity with the button and additional sense with the audio would ensure users remember the data.

## Physical Prototyping
### Analysis Graphs

To create our 8 tactile line graphs, we began by drawing x and y axes with puffy paint on sturdy cardstock. The raised texture of the puffy paint allows visually impaired users to feel the axes, aiding in graph analysis. Cardstock provides a durable, easily handled base for each graph. Once the paint is dry, we added the pipe cleaners. We also cut out eight cardstock movie tickets, which will receive design details and finishing touches after we receive Braille labels; their size will guide our placement. Instead of constructing individual coins, we used quarters to represent the revenue-to-budget ratio for each genre, adjusting the quantity of coins in each bucket to create a discernible weight difference for users.

### Persuasive Graphs

For our persuasive model, we transformed shoebox into a miniature stage. Red fabric served as curtains, framing each side of the stage. A tactile button, created by attaching knitted yarn to a circular cardboard base, was added to the stage, making it easy for users who are visually impaired or blind to locate by touch. It is the blue circular object in the image below. We also prepared eight cardboard circles, sized proportionally to the average popularity of each movie genre.

To get to know more about our final physical prototypes, you can view the demo video here.

## Re-Evaluation
We conducted a usability test of our physical prototype, drawing from our Human-Computer Interaction course principles of experience prototyping and user-centered design. By carefully structuring our evaluation, we aimed to gather meaningful user insights and validate our experimental approach.

Similar to the evaluation we conducted before, we invited a total of 5 participants to interact with our new physical prototype, moving beyond theoretical analysis to observe their real-world interactions. We guided participants through specific tasks and engaged them in dialogue to understand their experiences. We were given permission to use their pictures.

The usability evaluation involved testing with multiple participants across different settings, focusing on how users interacted with a physicalized data visualization about movie genres. The tests revealed several important insights about the prototype’s effectiveness and user experience.

In the persuasive evaluation, participants quickly understood the visualization’s core message. They readily identified movie genre popularity by comparing the size of circular representations. For instance, when asked about the most and least popular genres, participants immediately pointed to the largest (family) and smallest (documentary) circles. The physical design, particularly the varying circle sizes, proved intuitive for communicating popularity data.

The analysis portion of the evaluation was equally compelling. Participants demonstrated an ability to compare genre profitability using tactile cues like the weight of buckets and the number of quarters representing each genre’s revenue-to-budget ratio. One interesting observation was how participants approached ranking — some used a systematic method of comparing genres from the extremes inward, while others took a more haphazard approach like counting quarters.

A particularly valuable perspective came from a Orientation and Mobility Specialist with expertise in accessibility. The specialist praised the design’s universal approach, highlighting how the physicalization accommodates users with visual impairments. Key strengths included:

* Good color contrast
* Tactile elements like Braille labels
* Audio interactions
* Clear, bold text
* Thoughtful use of different sensory inputs

The specialist emphasized the concept of universal design — by creating an inclusive visualization for visually impaired users, the design inadvertently becomes more accessible to other groups like younger people or aging populations.

Future improvements suggested included:

* Placing Braille labels on the same side as text on the movie tickets
* Tactilely indicate the beginning of the Braille label on the movie tickets
* Potentially enlarging some text (while being mindful of field of vision limitations)
* Adding more audio elements
* Expanding Braille descriptions

From these suggestions, we were able to indicate where the Braille labels began and how the movie tickets should be oriented by adding a dot of black puffy paint to the top left corner of each label. This ensures a visually impaired or blind user knows how to hold the ticket to understand the Braille labels. If a user has low vision but uses Braille to read, they can see the black dot due to its high contrast with the color of the movie ticket. Because of time and supply constraints, we were unable to implement the other suggestions because they would require more Braille labels and rewriting other labels.

## In-Class Evaluation

We did in-class demonstrations for our peers. We showed them our original visualizations, explained our design process to make accessible physicalizations, and demonstrated how the physicalizations worked. Our peers complimented our use of Braille labels and enjoyed the sounds from our persuasive stage model. Our main point of feedback was to actually have the sounds playing from our stage button rather than using Wizard of Oz prototyping. If we had more time, we would have used Raspberry Pis to make the audio come from pushing the button. Another suggestion was to put a QR code that linked to the trailer of the genre’s most popular movie on the back of the cardboard circles. This would be more similar to our original visualization that included the most popular movie trailer on its page. Another suggestion was to have more labels on the line graphs such as titles or axes labels. We had a limited supply of Braille labels, so we decided to prioritize certain labels. If we had more supplies, we would add more Braille labels and descriptions to ensure even more usability.

## Conclusion
Overall, our physicalization project was an exciting journey of designing an inclusive, interactive data visualization about movie genres. Using usability testing and user-centered design principles, we transformed complex data into a tangible, multi-sensory experience. Our prototype successfully bridged the gap between abstract information and physical interaction, making data exploration accessible to diverse users, including those with visual impairments.

Physical prototyping allowed us to extend our ideas into a tactile product that engages multiple senses. Throughout this process, we learned invaluable lessons about designing with accessibility in mind, using materials like Braille labels, pipe cleaners, quarters, popcorn buckets, and interactive audio elements. The experience was not just educational, but genuinely innovative!

The feedback from our Orientation and Mobility Specialist as well as in-class session was particularly enlightening, reinforcing the importance of creating designs that are inherently inclusive. By focusing on accessibility, we created a visualization that potentially benefits a wide range of users, from those with visual impairments to younger learners and aging populations.