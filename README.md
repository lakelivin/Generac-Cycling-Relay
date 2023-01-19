# Generac-Cycling-Relay
A Hardware solution to cycle Generac generator running during an extended power outage to conserve fuel.

This project identifies how to add a Cyclic Timer Relay [alt search terms: cycling relay, cycle timer, timer relay] to a Generac generator and utilize the equipment protection features of the Evolution controller to prevent causing damage to the generator or household, while automatically stopping and starting the generator to extend fuel availability.

A Generac 22kw Guardian air cooled backup generator is rated to consume 3.8 gal/hr of propane running at full load. In real-world conditions my Generac 22kw generator actually consumed 4.9 gal/hr during a 20 hour period of continuous running. This rate of fuel consumption would exceed my tank capacity and propane suppliers refill delivery timing for a multi-day extended power outage. It is also very expensive to run continuously for 24 hr/day, costing $375/day in propane usage.

It was desired to be able to command the generator to shut off and pause for a selectable period of time then restart and run for a selectable period of time, and for this to occur repeatedly without the user having to go outside to the generator, other than the initial selection of cyclic operation.

There is not a programable feature for this in the Generac Evolution 2.0 generator controller. 

Two concerns about manually shutting off a generator under load, and for restarting a generator are to 1.) Remove the load before stopping or starting the generator; and 2.) to provide a cool-down period after shut down and a warm-up period before applying the load.

The Evolution controller is a very good controller and specifically provides these two features, as well as control of the Automatic Transfer Switch.

The Evolution 1.0 and Evolution 2.0 controllers have a legacy feature that is disabled by factory default. A feature called "2-wire start" exists from prior generations of generators. 

It is possible to re-enable the "2-wire start" feature from the Dealer Set-up menu, although it is password protected. The controller has two unused contacts in the two I/O molex connectors of the Evolution controller that are dedicated to this feature. You can purchase a Generac accessory kit that contains 2 or 3 wires with terminal ends that fit into the existing molex connectors and allow utilization of the 2-wire start feature. You will not find this kit by search, you have to know the part number. It is not unique by generator model, but rather a standard pin terminal.

When the two connectors are closed together by relay or switch the generator will start. The Evolution controller will monitor conditions, allow a brief warm-up and then command the Automatic Transfer Switch to close to generator power, providing power to the house. When the two connectors are opened by relay or switch the Evolution controller will open the Automatic Transfer Switch, which disconnects the house load from the generator, allow the generator engine to run briefly to cool down, then shut off the generator engine. 

BACKGROUND
On Jan-12-2023 tornadic storms across Alabama caused wide-spread power outages. My house lost power from 1/12/23 13:45 to 1/13/23 11:15. This was a 21.5 hour power interuption.

I have a Generac Guardian 22kw air-cooled wholehouse back-up generator with an Evolution 2.0 generator controller and a 200 amp automatic transfer switch. My generator was manufactured in 11/2021. I have a dedicated 250 gallon buried propane tank, with nothing else connected to it. The tank was filled to 80% capacity 2 weeks before the storm.

Weather during this event was 57degF at sundown falling to 47degF overnight, with an average windspeed of 10mph. We are on a lake and have no protection from the wind. We have a large home with (2) electric heatpumps for heating/cooling, and (2) refigerator/freezers. The heatpumps cycled frequently throughout the night because of the weather. We had made no changes to our normal thermostat settings.

The generator ran continuously through the night.  I checked my propane tank level in the morning, and observed it had dropped to 40%. This is 100 gallons of propane useage. I shut the generator off to conserve remaining propane. Power was restored about 1 hr later (yay!). 

The generator had run 20.56 hrs according to the Generac MobileLink app. This is a fuel consumption rate of 4.86 gal/hr. Upon refilling, the full delivered price of propane was $3.18/gallon, so the generator operation had cost $318 for 20.5 hours of power production.

I thought that that was an excessive consumption rate. I called Generac Support to get their opinion. They said the generator is rated to consume 3.9 gal/hr at full load, and thought that 4.86 gal/hr was not unreasonable. They advised me that it appeared the generator was operating normally.

Ideally a propane tank operates between 80% and 20% full, giving you 60% to consume. A 250 gallon tank provides 150 gallons of reliable propane consumption. You can go lower, but this is preferred range. At 5 gal/hr, that provides only 30 hours of operation. (I called to request propane refill Friday morning, and the delivery was not made until Tuesday, 96 hrs later.)

It seemed that a reasonable solution would be to operate the generator on a cycle for 20 minutes, then have the generator cycle off for 2 hours, then repeat the cycle. Then to sustain this cycling rate during the duration of the power outage. This would allow the heat pumps to provide heating or cooling to restore temperature setpoints and for the refrigerator/freezers (2) to maintain proper temperatures. This cycle rate should result in a fuel consumption rate of 12.5% of the full time rate. At this rate my 250/150-useable gallon propane tank would provide 240 hours of cyclic backup power.

There is not a programable feature for this in the Generac Evolution 2.0 generator controller. I did not want to have to go outside twice every 2 hours and cycle the generator manually myself.


