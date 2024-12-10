---
layout: post
title: "Design for Another World"
author: "Ally Smith"
categories: journal
tags: [documentation,sample]
image: spools.jpg
---

We created a VR skydiving experience where the user skydives above Davidson’s campus, deploys their own parachute, and lands on Chambers Lawn. We gathered data about our target users through a survey and coded the experience using A-Frame and Blender.

---

Our Skydiving VR project takes a shared dream — experiencing the thrill of freefall from thousands of feet in the air — and brings it to life, right here on Davidson’s campus. Together, our team sought to create a VR experience that would let users feel the excitement and awe of skydiving in a familiar, accessible setting. From the start, we envisioned an experience that captures the sensory rush of an actual dive, complete with realistic sounds, breathtaking views, and interactive elements that mimic the thrill of the fall. Setting our virtual descent above Davidson allowed us to infuse this project with personal meaning, grounding an extraordinary experience in the campus we know and love. Although we faced challenges and time limitations, our Skydiving VR experience serves as a testament to VR’s potential to make exciting adventures — whether typically inaccessible or daunting — feel not only possible but exhilaratingly real.

## Brainstorming and Planning
In planning what we would be creating, we started with sketching many different potential ideas. We wanted to think of exciting experiences that people may not be able to easily do in real life. We decided to utilize A-Frame in the actual coding and creation of this experience, as A-Frame proved to be easiest to learn and the most simple given our time constraints. Our steps of development included deciding our objectives, sketching different ideas, sending a survey for user input, then moving onto how we would design and implement it.

## Ideas and Sketches

Throughout the brainstorming process, we landed on four main ideas: walking on a high rope, seeing the view from different places in the world, riding a roller coaster, and going skydiving. These ideas gave users an experience they may be unable to do in real life for many reasons, such as financial, age, or disabilities.

### Tightrope

When the user is in VR, they can look down to see their avatar walking on a tightrope, high above the ground. The scene could be a cityscape or natural, such as a canyon or mountain. For example, we could create an environment where users walk between buildings in New York City or at the level of Burj Khalifa. Users could also walk across the Grand Canyon or the Swiss Alps. The purpose of this experience would be to elicit fear safely, as many people are afraid of heights. Also, users could see different places in the world from a unique perspective.

### Views of the World

We could create different scenes from around the world. For example, users could stand on top of the Eiffel Tower or Mt. Everest looking at the surrounding world. Similar to the tightrope idea, we could create cities and natural environments for users to experience. Users who cannot travel to these places can still be immersed in them through VR. The sketch is of Singapore, where the user looks at the city from a boat.

### Rollercoaster

We also came up with the idea of having the user ride a roller coaster in VR. So, the user will see the front of the coaster cart, the track, and the surrounding area. We could create different roller coasters to choose from or make scenes for each of the roller coasters at a particular amusement park, such as Carowinds. Some people may be too scared of roller coasters or cannot go on them for health reasons, so they could use VR to experience the thrill.

### Skydiving

Our final idea was to replicate skydiving. When the user is in VR, they see the surrounding world from a bird’s-eye view and the ground gets closer to them. At a certain point, the user’s parachute will deploy either automatically or from user interaction. Similar to the previous ideas, we could create multiple scenes where a user skydives into different places. In VR, users can land in areas they cannot in real life. So, we could have them land on Mt. Everest or a skyscraper.

To create the most unique VR scene we could, we decided to move forward with the skydiving idea. We wanted to make an exhilarating experience for people who do not want to go or cannot go skydiving in real life.

## Survey

We made a survey to understand our users better. We sent this survey to about 70 Davidson College students. Even though this is not a very diverse group to survey, it was the best way to get quick responses so that we could move forward with our design process. Our goal was to identify if people are interested in skydiving but are too scared to go or are not interested in it. We also wanted to choose a location to model in VR.

In this survey, we asked:

1. Are you scared of skydiving? Why or why not?
2. Are you interested in going skydiving? Why or why not?
3. Where would you like to skydive? What would you see while skydiving there?

Our results show that 91.3% of our respondents are scared of skydiving. Most reasoning is fear of heights, the parachute malfunctioning, and death. 8.7% of respondents who are not scared have been skydiving before.

What is fascinating is that 65.2% of respondents said they are possibly interested in skydiving, while 30.4% said they are interested. Only one person, 4.3%, said they are not interested in it at all. The general reasoning behind their responses is that skydiving would be an incredible life experience if their safety was guaranteed. However, the fear of heights and death outweighs their desire for a thrill. Therefore, most respondents do not think they will go skydiving, even though it piques their interest.

Our final question was open-ended, allowing respondents to explain where they would skydive and what they would see. Because we sent the survey to Davidson students, most responses were about Davidson’s campus. One person suggested landing on the football field in the middle of a game; another suggested landing at Doug Hicks’ house. The most popular landing spot was Chambers Lawn. Many responses mentioned seeing Lake Norman and the town of Davidson during the descent as well.

From the survey results, we chose to have our user skydive above Davidson’s campus and land on Chambers Lawn. When the user begins their descent, they will see mostly the academic side of campus, including Richardson Stadium, Union, the library, Wall, multiple dorms, Chambers, and Sloan. As they fall, the user will approach Chambers to land. Due to time constraints, we could not include Lake Norman and more of the Davidson area because modeling those areas is difficult.

## Target Users

The survey results are intriguing because most people are interested in skydiving but are scared of it. The respondents think it is an incredible life experience, but they will not commit to it. Therefore, our virtual reality could help users decide to execute skydiving in real life. Through a thrilling experience of falling through the sky, seeing Davidson’s campus below, and landing on Chambers lawn, users can get a taste of what it would be like to be flying. Therefore, we can provide users with a cheaper and lower-stakes option before they sign up for the next skydiving adventure.

Another group of users we can accommodate are people who cannot skydive for reasons such as financial, health, age, and more. Our VR experience will require low physical and cognitive effort that many people can use. As a result, users who do not have the option of skydiving in real life can still feel what it would be like.

Finally, VR skydiving could be used to train instructors. Replicating parachute malfunctions and other mistakes in the real world is too dangerous. However, instructors need experience with issues to act quickly and correctly while guiding their participants to safety. People training to become instructors could use VR to practice their responses to these situations and be more prepared if they occur in real skydiving adventures.

## Building

Our primary objective for this project was to deliver an exhilarating experience while eliminating the real dangers or intense fear often associated with skydiving. We planned on making the design as immersive as possible, attempting to integrate sensory cues such as the rush of wind as users begin their descent, the distinct sound of the parachute opening, and the gradual quieting of wind as the parachute deploys. The visual sensation of the ground coming closer was also a crucial part of capturing the thrill of free fall in a safe, controlled virtual environment.

To enhance user interactivity, we wanted to implement intuitive input mechanisms that enable the deployment of the parachute. Users should be able to look down at a wrist button where a simulated “rope/button/harness” control is located. By focusing on this spot for a few moments until a circular timer fills, users can activate the parachute, creating a sense of agency in the descent. For added guidance, we considered implementing a countdown or audio cue prompting users to deploy the parachute, enhancing realism and user engagement.

With these elements in mind, we developed a structured plan to execute our vision. The process began with setting up a 3D scene using A-Frame, establishing the falling motion, and finally incorporating interactive features like the parachute deployment. Each of these steps was designed to maximize immersion and accessibility, bringing our idea of virtual skydiving closer to reality.

The A-Frame creation process was a completely new workflow for us, since we had never built a VR experience before, let alone one in a web environment. Nevertheless, the process of building our basic scene wasn’t too grueling. The first step involved creating the 3D model in Blender using as few polygons as possible to optimize performance.

After that was created, we needed to learn how to import the model into A-Frame. We set up a sample project in VS Code and then used A-Frame’s documentation to learn how to render models in the environment. We then implemented the falling mechanics, including an exponentially increasing rate of falling (with a cap) and stopping at ground level. We initially had a great deal of visual errors (such as Z-fighting) in the environment, so some time was taken to correct these errors to the best of our ability. Finally, we needed to work on the interaction. Although we worked extensively on how to implement look-based interaction in our environment, A-Frame’s look-based raycaster didn’t play nicely (as in at all) with our 3D models, so after multiple hours of work, we decided to just have the user press the spacebar to pull their skydiving parachute.

With all of this implemented, we put in final touches like fog and editing the sky color, and the experience was complete!

## Final Result

Our final result can be viewed and interacted with here. Our demonstration video can be viewed here.

Short description of the VR experience for the user:

1. The experience starts the player high in the sky.
2. It counts down from 5 seconds before dropping.
3. The hands follow the player character to give a sense of connection with the character. We recognize that the skin color chosen here is white and not necessarily representative of everyone. If we had more time, we would include more skin colors.
4. The player is dropped at an exponentially increasing speed.
5. If the player presses space to deploy their parachute, we have the parachute appear above them and slow their descent. If they don’t, they maintain speed towards the ground.
6. Regardless of what they choose, the player stops at the ground and can look at the campus around them.

## Limitations and Future Directions
While our project accomplished much of what we set out to achieve, some elements of our original vision could not be realized within the time constraints. We were unable to successfully figure out the VR eye-tracking feature of interactivity for deploying the parachute, although it works using the spacebar. Given more development time, we would have also loved to add features like the ability for users to control their movement in freefall, offering a more dynamic sense of “flying” through the sky. Expanding the surrounding environment with additional settings and visual details would have further enhanced the realism, immersing users even more fully in the experience.

We also identified opportunities to enrich the auditory aspects of the simulation. The demo video includes wind sounds along with the sound of the deploying parachute, which greatly adds to the immersion in this experience. We were intending to implement this in our actual VR simulation, but the timing did not work out with adding this feature in the end. More audio cues — like a countdown timer to deploy the parachute — could also deepen user engagement and improve guidance through the experience. Another potential improvement would be including visual cues for the parachute mechanism, such as deploying straps or parts of the parachute in response to user actions, to reinforce interactivity.

Ideally, we envisioned the experience beginning inside a plane, allowing users to make the jump and gradually transition into the free fall. Despite these limitations, we successfully implemented the core experience of descent and a 360-degree view, enabling users to take in chambers as they fall, pass through clouds, and activate the parachute. Though some planned details are missing, the project effectively conveys the thrill of skydiving, offering a taste of adventure in a familiar setting.

## Class Feedback 10/30
In class on 10/30, we were able to showcase this design to classmates. We created an even more immersive experience by bringing in a small fan. When the user started their descent, one of our members turned the fan on high. As soon as they hit the spacebar to deploy the parachute, we turned the fan to low to show the change in wind. Classmates truly enjoyed this experience, and commented on how exciting it was to feel like they were truly falling.

The only two points of feedback we received were that they wished it was a bigger space to view when falling, and they wish the fall lasted longer. We were not able to incorporate these changes due to time constraints, as the development of the landing space took a significant amount of time. Along with this, we couldn’t develop a higher jump due to A-Frame height limitations. If we had more time to improve this experience, we would be sure to add more to the surroundings (or more of Davidson’s campus) to make it more immersive and realistic. Overall, classmates really enjoyed the experience and most voted it their favorite simulation out of the bunch.

## Conclusion
Our Skydiving VR project demonstrates the vast potential of virtual reality to transform the imagination into immersive experiences. By allowing users to experience the thrill of skydiving, we’ve opened up this exhilarating activity to those who may never be able to experience it otherwise, whether due to fears, health concerns, financial limitations, or accessibility needs. With Davidson’s campus as our setting, we prioritized sensory details — from the immersive 360-degree fall to the attempted interactive parachute deployment — to create a realistic yet safe experience. Although there were limitations to what we could implement in this initial iteration, our project exemplifies VR’s unique capacity to broaden access to awe-inspiring experiences, providing users a memorable glimpse into the thrill of skydiving while maintaining accessibility and safety. Through future iterations, we hope to expand on this foundation to bring even more dynamic and lifelike elements to our virtual skydiving world.