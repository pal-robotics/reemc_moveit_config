^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package reemc_moveit_config
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.3.5 (2020-10-02)
------------------
* Merge branch 'hey5_marker' into 'dubnium-devel'
  Add hand links in the hand groups
  See merge request robots/reemc_moveit_config!4
* Add hand links in the hand groups
* Contributors: Adria Roig, victor

0.3.4 (2020-10-01)
------------------

0.3.3 (2019-08-01)
------------------
* Merge branch 'hand_collisions' into 'dubnium-devel'
  Disable some collisions of the hand
  See merge request robots/reemc_moveit_config!3
* Disable more hand collisions
* Disable some collisions of the hand
* Disable some collisions of the hand
* Contributors: Adria Roig, Victor Lopez

0.3.2 (2019-03-18)
------------------
* Merge branch 'realsense' into 'dubnium-devel'
  Remove collision between camera_link and head2_link (realsense)
  See merge request robots/reemc_moveit_config!2
* Remove collision between camera_link and head2_link (realsense)
* Contributors: Adria Roig, Victor Lopez

0.3.1 (2018-03-29)
------------------
* Merge branch 'add_missing_collisions' into 'dubnium-devel'
  Add missing collisions
  See merge request robots/reemc_moveit_config!1
* Added missing collisions
* Contributors: Hilario Tome, Jordan Palacios

0.3.0 (2016-04-05)
------------------

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
