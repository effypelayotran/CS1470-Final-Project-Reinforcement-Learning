# CS1470 - Deep Learning Final Project 

**Team** :
C++_Undergrad_Neural_Trainers


**Paper** : DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills (Peng et al., SIGGRAPH 2018)

**Final Results of our Implementation**
See ```good_walk_.mp4``` and ```good_walk_2.mp4``` to see our final DeepMimic Policy in Action!

**Implementation Outline**
1. Load and parse the humanoid XML into a Gym Env class that is comptabile with Stable Baselines 3
2. Expose the State Space: joint quaternions, velocities, COM, phase variable
3. Expose the Action Space: target joint-angle setpoints for PD controllers
4. Parse the Mocap Joints Rotations per Frame per Clip per Action (Walk, Run, Jump, Etc.)
5. Implement Motion Imitation Reward and Task Reward, according to the DeepMimic Paper's equations. Implement this in the Humanoid Env's step() function.
6. Train, Render, and Tune Learned Policies!
7. Add Arena Obstacles and Generate HeightMap using CNNs that will be fed into PPO networks, if time permits. This allows Humanoid to learn how to generalize running through new arena obstacles. 




**GitHub Main Repo**
- https://github.com/your-username/C++_Undergrad_Neural_Trainers. 
- Our entire implementation is in the ```with_hip_rotation_render_script.ipynb``` notebook in this repo!

**Our Other Resources Repo**
- Our custom modified humanoid models: https://github.com/effypelayotran/mujoco_resources/tree/main/humanoid_CMU_folder 
- Mujoco's models: https://github.com/google-deepmind/mujoco_menagerie/tree/main 
