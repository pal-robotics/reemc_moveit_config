^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package reemc_moveit_config
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Forthcoming
-----------

0.2.4 (2015-06-12)
------------------
* Add missing runtime dependency
* Contributors: Adolfo Rodriguez Tsouroukdissian

0.2.3 (2015-06-09)
------------------
* Allow collisions between same hand links
* config defaults to true now
* Roslaunch 'robot' arg: default to 'full_ft_hey5'
  Previous default was 'full'.
* Add reemc-ft-hey5 stuff and argument passing for launching it
* Contributors: Adolfo Rodriguez Tsouroukdissian, Bence Magyar

0.2.2 (2015-04-08)
------------------
* Remove gazebo_dependency.
  Getting urdf using xacro from reemc_description.
* Contributors: Luca Marchionni

0.2.1 (2015-04-08)
------------------
* Merge pull request #3 from pal-robotics/fix-ik-spec
  Remove KDL IK solvers for non-chain groups.
* Merge pull request #2 from pal-robotics/joint-limits
  Update joint limits specification.
* Update joint limits specification.
  - Explicitly specify acceleration limits
* Remove KDL IK solvers for non-chain groups.
  Upcoming MoveIt! changes will start to complain that these groups are not chains,
  and that the KDL IK plugin can't be instantiated for them.
* Merge pull request #1 from bmagyar/fix_finger_collisions
  Removed "disable collision" with fingers for several links where it was ...
* Removed "disable collision" with fingers for several links where it was dangerous.
* Remove unused planner config params.
  - The defaults for the longest_valid_segment_fraction are good enough.
  I played with custom fixed values to see if I could improve plan quality,
  but only increased computation times, and a marginal quality improvement.
  - Removing the projection_evaluator makes moveit default to RRT-connect, which
  is faster and yields better plans than Kpiece .I still need to understand
  how default planners are chosen.
* Update joint_limits.yaml
* Added default config for rviz with MoveIt plugin
* Update README.md
* Initial public reemc_moveit_config release
* Initial commit
* Contributors: Adolfo Rodriguez Tsouroukdissian, Bence Magyar, Sammy Pfeiffer
