# MyFit: Real-Time Automated Assistance for Personalized Fitness and Nutrition

## Overview:

In the evolving landscape of fitness, virtual fitness assistance has gained popularity as a guiding force for individuals on their health and wellness journeys. However, these conventional virtual fitness assistants lack personalization and real-time progress tracking, hampering effectiveness and interactivity. Going beyond conventional approaches, our platform provides users with tailored exercise routines and nutritional guidance, considering their unique fitness history, current levels, and health objectives ensuring that workout plans are aligned with each user's capabilities, creating a more effective and engaging fitness journey. Further, our system leverages Mediapipe for real-time posture monitoring during workouts allowing proper guidance and posture correction thereby minimizing the risk of injury due to poor posture during exercise. Furthermore, our system dynamically adjusts exercise and diet recommendations based on user performance and nutrient consumption. This personalized approach ensures evolving guidance that reflects user progress and adapts to changing fitness needs. Integrated robust progress tracking tools contribute to user motivation, offering transparent insights into metrics like weight, fitness level, and exercise performance. By offering personalized guidance, real-time feedback, and robust progress tracking, our platform becomes an integral part of users' holistic well-being journeys, facilitating continuous steps toward their health and fitness goals.

## Objectives:

1. Provide user specific exercise plans
2. Provide diet plan recommendation
3. Provide pose detection and correction
4. Perform adaptive progress tracking

## Mind Map:
![MyFit Flow](https://github.com/Hardik20042002/MyFit/assets/102477681/1039589d-9e53-4c2b-b203-eb18be779e57)

## System Design:
![MyFit High Level Design](https://github.com/Hardik20042002/MyFit/assets/102477681/a2d1146f-a476-47ab-9835-29f7f64d08d8)

## Novelty:

1. Leverages users’ health to tailor diet plans, ensuring proper nutrition recommendations for overall wellness.
2. We assess user fitness levels and track exercise progress to provide adaptive workout routines.
3. During workouts, we offer interactive monitoring, ensuring users maintain correct exercise poses, reducing the potential for injuries, and enhancing posture.
4. Our platform offers a holistic, one-stop solution for users' overall wellness.
   
## Implementation:

### Modules:

1. **Diet Recommendation System:**
   - **Running Command:** `python dietRecommender.py`
   - **Description:** This module is a diet plan recommendation system that, based on the user's current fitness levels, nutritional requirements, and goals, provides a daily diet plan.
   - **Flow Chart:** ![Diet Plan Recommendation System Working](https://github.com/Hardik20042002/MyFit/assets/102477681/3524092d-bdeb-46f5-a183-965dad6d1c2b)
   - **Demo:** ![Diet Plan Recommendation System Demo](https://github.com/Hardik20042002/MyFit/assets/102477681/339f1171-6a43-464c-ad0b-43348fae5c34)

2. **Exercise Plan Recommendation System:**
   - **Running Command:** `python exerciseRecommender.py`
   - **Description:** This module is an exercise plan recommendation system that provides the user with a weekly exercise plan based on the user's goals, historic exercise sessions performed on the platform, and current fitness level.
   - **Flow Chart:** ![Exercise Plan Recommendation System Working](https://github.com/Hardik20042002/MyFit/assets/102477681/056558be-e5dd-4a9c-9802-c462cc22a53f)
   - **Demo:** ![Exercise Plan Recommendation System Demo](https://github.com/Hardik20042002/MyFit/assets/102477681/3666a1af-f256-4a17-98bd-1f54c92d552a)

3. **Exercise Monitoring System:**
   - **Running Command:** `cd MonitoringSystem`
                          `python monitoringTest.py`
   - **Description:** This module utilizes Mediapipe for real-time monitoring of the user during exercise sessions, including error detection in the pose. Additionally, it estimates the user's current fitness level during monitoring, enabling dynamic adjustments to the user's exercise and diet recommendations based on feedback from the session.
   - **Flow Chart:** ![Exercise Monitoring System Working](https://github.com/Hardik20042002/MyFit/assets/102477681/78d0fb8d-bf18-40f8-be0d-30c27fef511a)
   - **Demo:** [Exercise Monitoring System Demo](https://github.com/Hardik20042002/MyFit/assets/102477681/e9807944-c3a9-4d87-9391-f8584ba7a37f)

4. **Calorie Counter:**
   - **Running Command:** `python calorieCntr.py`
   - **Description:** This module is used to provide the calorie count for a dish. This module was used as a sub-module in diet plan recommendation module.

5. **Image Generator:**
   - **Running Command:** `python imageGenerator.py`
   - **Description:** This module is used to generate images of food items by using the name of the item. We used this module in our front end design to display images of food items recommended by our system to the user.

### Folders:

1. **Analysis:** This folder contains the user base created for testing of our system along with the python codes that we used to test the accuracy of our system.
2. **Datasets:** The folder contains various datasets that we used for the development of MyFit.
3. **Files:** This folder contains various documentations about our system along with the output files containing some sample outputs of our recommendation systems
4. **FrontEnd:** This folder contains the front end design of our web application 

### Conclusion: 

Our system serves as an indispensable companion in the daily journey of our users, seamlessly integrating into every facet of their health and wellness routine. From the moment they embark on their day by making mindful choices about their nutrition to engaging in workout sessions, our platform is designed to enhance and support every step of their journey. By offering personalized guidance, real-time feedback, and robust progress tracking, our platform becomes an integral part of the user's holistic well-being journey, ensuring that each day is a step forward toward their health and fitness goals.

![A User's Day With MyFit](https://github.com/Hardik20042002/MyFit/assets/102477681/718b2744-3d0e-4271-bdda-71e57678b397)