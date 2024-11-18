# CS781-Formal Methods ML Project - Safe Reinforcement Learning

Team Name

Tipu Sultan (23V0010) 

How to change inputs

We can give visibility frequencies in the jupyter file (PlayGround.iypnb) for random instances when Shield is unable to see the environment.

Files to run

1. Launch jupyter notebook by launching the command inside the docker: pip install -e ./notebooks/environments/Minigrid && jupyter lab --ip=0.0.0.0 --allow-root --notebook-dir=./notebooks --no-browser
2. Keep utils.py, sbutils.py files
3. Run "Playground.iypnb" jupyter notebook.
  
How to run codes:

1. Run the Experiments: Check with visibility frequency = 1 (safe RL as discussed in class);
2. Vary visibility frequency from 0.1 to 1 to observe how the Shield works in Partially Observable Environment (utils.py: inside default_action_mask = all possible actions (safe + unsafe all );
3. Next allow the shield synthesis by performing no action whenever shield misses to visualize environmental actions.

Result Interpretation:

1. Get all the results; observe how shield behaves with full observability, partial observability with all actions possible allowed actions and partial observability with no action when environment is invisible.
2. Plots are generated for each visibility frequency demonstrating how quickly and how much rewards (achieved_goal) agent is accumulating.
3. Results also suggest how episode length (successful goll acheieved steps) are being achieved with timesteps. Episode length and mean values are expected to reduce faster with safe RL.
   
