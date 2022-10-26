# Lab06 - Reaction Diffusion
Let's play with the parameters and setup of the reaction-diffusion equation to create cool effects. You may work with a partner for this lab. **Please choose 3 of the following 5 puzzles/tasks to complete this lab.** Additional puzzles/task may be completed for extra credit.

# Setup
Download and open Houdini with the ReactionDiffusionPlayground.hipc file found in this repository.

# Puzzle 1
Modify the **feed rate** to create a cell mitosis (cellular division) affect.

The other parameters will be as follows:

D_A = 1

D_B = 0.5

kill_rate = 0.0608

delta_time = 1


![image](https://user-images.githubusercontent.com/60444726/197622415-ca9b9623-d01b-4e54-9b1a-b79109248cab.png)

# Answer:
feed_rate = 0.0275

![9ad5c19a8ddd43d24dbec91864d94cde](https://user-images.githubusercontent.com/65415823/198054638-3bf8c634-e435-4a88-bc93-f65253fd3cc2.gif)

<img width="638" alt="image" src="https://user-images.githubusercontent.com/65415823/198054850-2da372dc-5e28-430e-9436-0d918c0413f4.png">

# Puzzle 2
Modify the **kill rate** to create an simulation that reaches equilibrium very quickly. The rings should be approximately where the starting seeds were, and there should be little change between the 5th and the 100th frame.

The other parameters will be as follows:

D_A = 1

D_B = 0.5

feed_rate = 0.055

delta_time = 1



![image](https://user-images.githubusercontent.com/60444726/197624737-58ab1aca-accb-4b4a-9654-cdc5fe84e723.png)

Frame 5


![image](https://user-images.githubusercontent.com/60444726/197624645-e5b13798-ae74-4e18-84dc-955a9919021c.png)

Frame 100

# Answer
kill_rate = 0.0654

Frame 5

<img width="589" alt="image" src="https://user-images.githubusercontent.com/65415823/198061726-6887c14b-90db-4964-9724-4bade8b4788b.png">

Frame 100

<img width="562" alt="image" src="https://user-images.githubusercontent.com/65415823/198061826-e191ac1a-dac8-4de5-9f1a-aebd090960c4.png">

# Puzzle 3
Modify the diffusion rate of chemical B (D_B) to create a simulation that still demonstrates where the seeds were at the start of the algorithm. There should be parts of concentric circles surrounding each seed location. To see if you're on the right track, run the simulation and then check (or have a friend check) and see if you can idenitfy where all the seeds were at the start of the algorithm!

The other parameters will be as follows:

D_A = 1

feed_rate = 0.055

kill_rate = 0.062

delta_time = 1

![image](https://user-images.githubusercontent.com/60444726/197626261-1e4fa5d4-d9d8-4563-8b92-c2b2a20038f7.png)
Seed Placement

![image](https://user-images.githubusercontent.com/60444726/197626365-9a91a0d6-1e6f-4b0f-838b-7047c153d860.png)
Frame 100

# Answer

D_B = 0.205

<img width="573" alt="image" src="https://user-images.githubusercontent.com/65415823/198059713-15f5ae8b-b6fc-4fdf-835f-d876997d69fa.png">

# Task 1
Modify the shape, size, or placement of the seeds in the playground to create an interesting effect. Which node might you need to adjust? How can you change the exisitng VEX to create something interesting?

# Task 2
Modify some of the parameters to create a cool effect. This effect can be displayed with a video or image, depending on whether you want to showcase the animated effect or the algorithm's result.

# Cool Effects
D_A = 0.7
D_B = 0.12
feed_rate = 0.050
kill_rate = 0.06

![ca0f92547827d71081141d5beacaf09e](https://user-images.githubusercontent.com/65415823/198064122-f00b5de3-421d-40d6-a5e3-753598ba286e.gif)

# Submission
- Create a pull request to this repository
- In the README, include the names of both of your team members
- In the README, include a description of the task or puzzle you completed, screenshots/images (or videos!) of your results, AND the values for all the parameters you changed
- There is no need to upload a Houdini File. Screenshots of your results and images (or written values) of the parameters will be sufficient!
