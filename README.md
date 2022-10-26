# Submission

## Puzzle 1

feed_rate = 0.028

![image](https://user-images.githubusercontent.com/3106877/198052585-ca97f0b7-4a29-47a4-a4ba-ef79adec607c.png)

## Puzzle 2

kill_rate = 0.065

![image](https://user-images.githubusercontent.com/3106877/198052970-e004c88b-bafa-4528-80d1-7b34827667b9.png)

## Puzzle 3

D_B = 0.25

![image](https://user-images.githubusercontent.com/3106877/198053692-9c3cc042-0c0d-4cc7-a201-52c06f32d8a1.png)

## Task 1

D_A = 1.19  
D_B = 0.35  
feed_rate = 0.053  
kill_rate = 0.0596  

The initial conditions were set using a noise function in the `set_seeds` node.

https://user-images.githubusercontent.com/3106877/198058103-a82495dd-89c6-4ba7-96a5-e653ed8bdcda.mp4

There is some strange behavior where it becomes striped:

![image](https://user-images.githubusercontent.com/3106877/198058748-98949cd5-6136-4ae4-b77a-2a094578c700.png)

I don't know what causes this but it's cool so it's fine with me.

## Task 2

D_A = 1  
D_B = 0.5  
feed_rate = 0.07  
kill_rate = 0.062  

I use the same noise-based seed as the previous task, but this time I added a moving circle to "erase" the chemicals.

https://user-images.githubusercontent.com/3106877/198063830-d3ebeff4-4981-4b08-a039-fcae412a7bb7.mp4

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

# Task 1
Modify the shape, size, or placement of the seeds in the playground to create an interesting effect. Which node might you need to adjust? How can you change the exisitng VEX to create something interesting?

# Task 2
Modify some of the parameters to create a cool effect. This effect can be displayed with a video or image, depending on whether you want to showcase the animated effect or the algorithm's result.

# Submission
- Create a pull request to this repository
- In the README, include the names of both of your team members
- In the README, include a description of the task or puzzle you completed, screenshots/images (or videos!) of your results, AND the values for all the parameters you changed
- There is no need to upload a Houdini File. Screenshots of your results and images (or written values) of the parameters will be sufficient!
