:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/PhysicsTestMotionParameters3D.xml.

.. _class_PhysicsTestMotionParameters3D:

PhysicsTestMotionParameters3D
=============================

**Inherits:** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Parameters to be sent to a 3D body motion test.

.. rst-class:: classref-introduction-group

Description
-----------

This class contains parameters used in :ref:`PhysicsServer3D.body_test_motion<class_PhysicsServer3D_method_body_test_motion>`.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`collide_separation_ray<class_PhysicsTestMotionParameters3D_property_collide_separation_ray>` | ``false``                                           |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`RID[]<class_RID>`               | :ref:`exclude_bodies<class_PhysicsTestMotionParameters3D_property_exclude_bodies>`                 | ``[]``                                              |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`int[]<class_int>`               | :ref:`exclude_objects<class_PhysicsTestMotionParameters3D_property_exclude_objects>`               | ``[]``                                              |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`from<class_PhysicsTestMotionParameters3D_property_from>`                                     | ``Transform3D(1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0)`` |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`float<class_float>`             | :ref:`margin<class_PhysicsTestMotionParameters3D_property_margin>`                                 | ``0.001``                                           |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`int<class_int>`                 | :ref:`max_collisions<class_PhysicsTestMotionParameters3D_property_max_collisions>`                 | ``1``                                               |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`motion<class_PhysicsTestMotionParameters3D_property_motion>`                                 | ``Vector3(0, 0, 0)``                                |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`recovery_as_collision<class_PhysicsTestMotionParameters3D_property_recovery_as_collision>`   | ``false``                                           |
   +---------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_PhysicsTestMotionParameters3D_property_collide_separation_ray:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **collide_separation_ray** = ``false``

.. rst-class:: classref-property-setget

- void **set_collide_separation_ray_enabled** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_collide_separation_ray_enabled** **(** **)**

If set to ``true``, shapes of type :ref:`PhysicsServer3D.SHAPE_SEPARATION_RAY<class_PhysicsServer3D_constant_SHAPE_SEPARATION_RAY>` are used to detect collisions and can stop the motion. Can be useful when snapping to the ground.

If set to ``false``, shapes of type :ref:`PhysicsServer3D.SHAPE_SEPARATION_RAY<class_PhysicsServer3D_constant_SHAPE_SEPARATION_RAY>` are only used for separation when overlapping with other bodies. That's the main use for separation ray shapes.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_exclude_bodies:

.. rst-class:: classref-property

:ref:`RID[]<class_RID>` **exclude_bodies** = ``[]``

.. rst-class:: classref-property-setget

- void **set_exclude_bodies** **(** :ref:`RID[]<class_RID>` value **)**
- :ref:`RID[]<class_RID>` **get_exclude_bodies** **(** **)**

Optional array of body :ref:`RID<class_RID>` to exclude from collision. Use :ref:`CollisionObject3D.get_rid<class_CollisionObject3D_method_get_rid>` to get the :ref:`RID<class_RID>` associated with a :ref:`CollisionObject3D<class_CollisionObject3D>`-derived node.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_exclude_objects:

.. rst-class:: classref-property

:ref:`int[]<class_int>` **exclude_objects** = ``[]``

.. rst-class:: classref-property-setget

- void **set_exclude_objects** **(** :ref:`int[]<class_int>` value **)**
- :ref:`int[]<class_int>` **get_exclude_objects** **(** **)**

Optional array of object unique instance ID to exclude from collision. See :ref:`Object.get_instance_id<class_Object_method_get_instance_id>`.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_from:

.. rst-class:: classref-property

:ref:`Transform3D<class_Transform3D>` **from** = ``Transform3D(1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0)``

.. rst-class:: classref-property-setget

- void **set_from** **(** :ref:`Transform3D<class_Transform3D>` value **)**
- :ref:`Transform3D<class_Transform3D>` **get_from** **(** **)**

Transform in global space where the motion should start. Usually set to :ref:`Node3D.global_transform<class_Node3D_property_global_transform>` for the current body's transform.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_margin:

.. rst-class:: classref-property

:ref:`float<class_float>` **margin** = ``0.001``

.. rst-class:: classref-property-setget

- void **set_margin** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_margin** **(** **)**

Increases the size of the shapes involved in the collision detection.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_max_collisions:

.. rst-class:: classref-property

:ref:`int<class_int>` **max_collisions** = ``1``

.. rst-class:: classref-property-setget

- void **set_max_collisions** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_max_collisions** **(** **)**

Maximum number of returned collisions, between ``1`` and ``32``. Always returns the deepest detected collisions.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_motion:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **motion** = ``Vector3(0, 0, 0)``

.. rst-class:: classref-property-setget

- void **set_motion** **(** :ref:`Vector3<class_Vector3>` value **)**
- :ref:`Vector3<class_Vector3>` **get_motion** **(** **)**

Motion vector to define the length and direction of the motion to test.

.. rst-class:: classref-item-separator

----

.. _class_PhysicsTestMotionParameters3D_property_recovery_as_collision:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **recovery_as_collision** = ``false``

.. rst-class:: classref-property-setget

- void **set_recovery_as_collision_enabled** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_recovery_as_collision_enabled** **(** **)**

If set to ``true``, any depenetration from the recovery phase is reported as a collision; this is used e.g. by :ref:`CharacterBody3D<class_CharacterBody3D>` for improving floor detection during floor snapping.

If set to ``false``, only collisions resulting from the motion are reported, which is generally the desired behavior.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
