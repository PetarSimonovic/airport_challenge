Airport Challenge
=================

```
        ______
        _\____\___
=  = ==(____MA____)
          \_____\___________________,-~~~~~~~`-.._
          /     o o o o o o o o o o o o o o o o  |\_
          `~-.__       __..----..__                  )
                `---~~\___________/------------`````
                =  ===(_________)

```

This software controls the flow of planes at an airport.

The planes can land and take off if the weather is sunny.

Planes can't land or take off if the weather is stormy.

Planes can't land if the runway is full.

```
--- GETTING STARTED ----

Load 'airport.rb' to begin

```

--- AIRPORT ---

The airport controls the flow of planes.

It grants planes permission to take off and land.

Planes are stored on the RUNWAY

The runway has a default capacity of 20.

To change the capacity use 'Airport.new(X)'.

Methods:

- Airport.land_plane(plane)
  - Adds a plane to the runway if the aircraft has permission to land and the runway is not full.

- Airport.take_off(plane)
  - Allows plane to land if the aircraft is flying.

- Airport.weather?
  - Checks that weather conditions are safe enough for take_off and land_plane

- Airport.storm
  - Generates a random number between 1 and 10. Any value above 7 creates a storm.

```

--- PLANE ---

Planes keep track of their status: they can either be on the runway or in the air.

The Airport can ask the plane whether it's flying or not.

All planes start on the runway.

Methods:

- Plane.landed
  - Sets the plane's status to on_runway (in_air is false, on_runway is true)

- Plane.in_air
  - Sets the plane's status to flying (on_runway is false, in_air is true)

- Plane.flying?
  - True if plane is in the air; false if it's on the runway

- Plane.on_runway?
  - True if plane is on the runway; false if it's in the air
