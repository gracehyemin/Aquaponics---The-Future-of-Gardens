

==============
[Aquaponics – The Future of Gardens]
==============

[In aquaponics, maintaining the levels of several variables are necessary to ensure ideal plant yield. This project will focus on the hydroponics subsystem. Future additions may include the aquaculture part of the system.]

Personas
========

Personas are a tool used to contextualize user and acceptance stories and aid
in the communication of product requirements.

[Gia]
--------------

[The Gardener]

Details
^^^^^^^

[Spends free time tending to garden with a less than satisfactory yield. Interested in creating an aquaponics system where one is able to gauge various conditions. Wants to automate system to increase efficiency and decrease need for constant adjustment in water levels, temperature, sunlight, pH, percentage of oxygen reaching roots, rate of water flow, etc.]

Goals
^^^^^

[Regular and precise measurements of conditions will ensure better quality crop yield in minimal space. Timed readings will allow him to know what to adjust and the system will also make needed adjustments.]

Problem Scenarios
=================

Problem scenarios are in-depth descriptions of situations particular
`Personas`_ would like to to improve. Effective problem scenarios describe the
problem at hand, the current alternatives or workarounds the user may employ
and the related value proposition.

[Insufficient Data Collection]
-----------------------

[Gia does not have regularly recorded readings of various conditions that she can access to figure out the cause of low plant yield.]

Current Alternatives
^^^^^^^^^^^^^^^^^^^^

[She records data by hand in the various conditions on a somewhat irregular basis. Without enough data, Bill finds it difficult to known exactly when to adjust variables ideally.]

Value Proposition
^^^^^^^^^^^^^^^^^

[Attaching sensors to measure the data and gathering recording in one place. Any irregularities will be notified to Gia through a text. In case of immediate attention required, the code will have a section to adjust levels accordingly. For example, a pH out of the required range for the soil will trigger an immediate response to decrease the water flow, until Gia approves further necessary adjustments.]

User Stories
============

A user story is a structured way of capturing a functional requirement from the
perspective of a specific user. User stories provide the context, intention,
and business case for each newly developed feature.

[Create equilibrium]
------------

As Gia the Gardener, I want to access regularly recorded data to know when and what is not within normal levels for several variables that directly influence the plants’ health so that necessary changes can be made immediately.

Acceptance Stories
==============

[Scenario 01: Water Excess]
```````````````````````
Given that it is time for another flooding of the growbed,
And there are no clogs in the valves,
When water begins to flow through input valve,
Then the water level will rise to 100 mm
And the water will be diverted into a separate valve back into the fish tank using a bypass ball valve.
This bypass ball valve will remain open until next scheduled flooding in fill-flood cycle.



[Scenario 02: Roots drowning in water]
```````````````````````
When there is a clog or other error causing the water level to remain high for too long,
And the roots are drowning,
A motorized ball valve will be used, which allows for gravity feed pressures and more precise control over water cycles.
When there is an error with the mechanical bell siphon, this motorized ball will be used as an alternative.
All water will be automatically drained and fill-flood watering cycle will be paused, until I manually turn it back on. An Arduino Uno microcontroller will be used to have precise control of cycle times. I will use this microcontroller to optimized growth environment of plants.



[Scenario 3: Moisture and temperature Control]
```````````````````````
When water is entering the grow bed, there will be a moisture analog probe, 
And the DS18B20 temperature probe will be used.
When there is a large quantity of water that is not meeting standards of proper filtration or biotreatment, there will be a master system kill relay. 
To prevent the soil moisture, humidity, and temperature from further irregularities, a water drain will open to detect several things.
Maximum will be kept in the fish tank. This will ensure higher oxygen levels for fish while growbed issue is detected and addressed.
Detect current data on Soil moisture, humidity, and temperature.
And detect if there is a slower rate of flow in a specific output drain.
This would indicate a possible clog from rocks, roots or other media.
