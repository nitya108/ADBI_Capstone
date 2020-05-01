# ADBI_Capstone

The following is the repo to solve a variation of Capacitative Vehicle Routing problem in a school cus routing scenario.


To run the given Graph Routing Open AI Gym environment for the Vehicle Routing Problem, please follow the below steps.

1. Install Open AI Gym : pip install gym.

2. Manually copy and paste the contents of this classic control folder ( this has all the files related to graph routing env) to the originally
   install folder of classic_control of the Gym library.

3. Edit the __init__.py of gym/envs folder.
   Add a new registration
   
   register(
    id='vrp-v0',
    entry_point='gym.envs.classic_control:VrpEnv',
    )
 
 4. Edit the __init__.py of gym/envs/classic_control.
    Add the following import.
    
    from gym.envs.classic_control.vrp_env import VrpEnv
    
 5. Setup is done. With classic_control as working directory. You can play with our Graph Routing environement.
     
 6. To make the env, do
    import gym
    env = gym.make('vrp-v0')
