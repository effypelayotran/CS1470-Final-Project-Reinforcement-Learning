# Model Tuning Bookkeeping
- run_policy_3 —> attempt to put the d_star in the state.obs by modifying the get_obs function to return that data in the obs dictionary as well. 
- run_policy_4 —> put the v_xy in the obs space.Has both v_xy and goal.
- run_policy_5 —> changed to velocity[1:3]
- run_policy_6 —> hip reward 
- run_policy_7 —> only v_xy + humanoid_fixed
- run_policy_8 —> only v_xy + humanoid_fixed + changed healthy z-range to 0.5 to 2.0