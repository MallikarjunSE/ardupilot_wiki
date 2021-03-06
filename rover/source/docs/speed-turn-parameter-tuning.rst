.. _speed-turn-parameter-tuning:

===========================
Speed Turn Parameter Tuning
===========================

The speed-scaling parameters are used to set the percentage reduction in
throttle when turning around a waypoint and the distance before a target
when the Rover will start to slow down.

The two parameters are listed below:

* :ref:`rover:SPEED_TURN_GAIN <SPEED_TURN_GAIN>` 

  * Range 0-100 Units: percent Increment 1 (50)
  * The percentage to reduce the throttle while turning. 
    If this is 100% then the target speed is not reduced while turning. 
    If this is 50% then the target speed is reduced in proportion to the turn rate, 
    with a reduction of 50% when the steering is maximally deflected.  

* :ref:`rover:SPEED_TURN_DIST <SPEED_TURN_DIST>` 

  * Range 0-100 Units: meters Increment .1 (50)
  * The distance to the next turn at which the rover reduces its target 
    speed by the SPEED_TURN_GAIN.                                                                                                                                                                          |


The parameters are set in the *Mission Planner* **CONFIG/TUNING \| Basic
Tuning** page:

.. figure:: ../images/MissionPlanner_Rover_Basic_Tuning.png
   :target: ../_images/MissionPlanner_Rover_Basic_Tuning.png

   Mission Planner: Rover BasicTuning

.. note::

   All parameters may be adjusted in the "Advanced Parameter List" in
   Mission Planner). All the Rover user settable parameters are listed in
   :doc:`APMrover2 Parameters <parameters>`.
