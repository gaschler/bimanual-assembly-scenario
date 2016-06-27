Bimanual Assembly Scenario
=======

This is a benchmark scenario for integrated task and motion planning.
It is motivated by [industrial assembly](http://www.smerobotics.org/demonstrations/d1.html) and
was first solved in a [thesis by A. Gaschler](http://www6.in.tum.de/Main/Publications/GaschlerPhd.pdf#page=115) (see Section 6.2.3).

Unlike pure path planning, there are interesting symbolic preconditions and effects.
The scenario is not an extreme benchmark case, but rather one of practical relevance.

Definition
-----------

For a first overview, you can watch a [video how the scenario is solved by task-level programming](https://youtu.be/B1Qu8Mt3WtQ?t=14s).

Then, you can find the scenario definition in this [thesis on page 115](http://www6.in.tum.de/Main/Publications/GaschlerPhd.pdf#page=115).

The problem is to find a sequence of actions and a collision-free path to assemble a gearbox component.


Evaluation
-----------

Contrary to pure path planning, integrated task and motion planning allows for several evaluation criteria.

Core criteria
 * The sequence of actions solves the scenario.
 * The motion paths are collision-free. (Collision checks succeed for a resolution of at most 1 degree in the configuration space.)
 
Extended criteria
 * The planner is likely to solve for any random placement of objects (for instance by using different grasping angles for the cylindrical objects).
 * The planner will theoretically solve if a solution exists.
 * The planner is likely to solve in the presence of additional objects.
 * The planner can easily be adapted to other scenarios.
 * Planning is fast.
 * Execution is fast.
 * Motion paths are collision-free in any resolution.
 * Paths are smooth.


License
-----------

Most geometric shapes are conversions of the STEP files provided by the respective manufacturers.

 * Robot:  http://www.comau.com/Download/robot/six-6-14/cad-files/EN_3dstep_six614.zip (VRML conversion from https://github.com/roboticslibrary/rl-examples/archive/0.6.2.tar.gz)
 * Parallel gripper: https://www.weiss-robotics.com/en/produkte/gripping-systems/performance-line-en/wsg-50-en/#tab-downloads_tab


