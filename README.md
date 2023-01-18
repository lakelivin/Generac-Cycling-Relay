# Generac-Cycling-Relay
A Hardware solution to cycle Generac generator running during an extended power outage to conserve fuel.

On Jan-12-2023 tornadic storms across Alabama caused wide-spread power outages. My house lost power from 1/12/23 13:45 to 1/13/23 11:15. This was a 21.5 hour power interuption.

I have a Generac Guardian 22kw air-cooled wholehouse back-up generator with an Evolution 2.0 generator controller and a 200 amp automatic transfer switch. My generator was manufactured in 11/2021. I have a dedicated 250 gallon buried propane tank, with nothing else connected to it. The tank was filled to 80% capacity 2 weeks before the storm.

Weather during this event was 57degF at sundown falling to 47degF overnight, with an average windspeed of 10mph. We are on a lake and have no protection from the wind. We have a large home with (2) electric heatpumps for heating/cooling, and (2) refigerator/freezers. The heatpumps cycled frequently throughout the night because of the weather. We had made no changes to our normal thermostat settings.

The generator ran continuously through the night.  I checked my propane tank level in the morning, and observed it had dropped to 40%. This is 100 gallons of propane useage. I shut the generator off to conserve remaining propane. Power was restored about 1 hr later (yay!). 

The generator had run 20.56 hrs according to the Generac MobileLink app. This is a fuel consumption rate of 4.86 gal/hr. Upon refilling, the full delivered price of propane was $3.18/gallon, so the generator operation had cost $318 for 20.5 hours of power production.

I thought that that was an excessive consumption rate. I called Generac Support to get their opinion. They said the generator is rated to consume 3.9 gal/hr at full load, and thought that 4.86 gal/hr was not unreasonable. They advised me that it appeared the generator was operating normally.

Ideally a propane tank operates between 80% and 20% full, giving you 60% to consume. A 250 gallon tank provides 150 gallons of reliable propane consumption. You can go lower, but this is preferred range. At 5 gal/hr, that provides only 30 hours of operation. (I called to request propane refill Friday morning, and the delivery was not made until Tuesday, 96 hrs later.)

It seemed that a reasonable solution would be to operate the generator on a cycle for 20 minutes, then have the generator cycle off for 2 hours, then repeat the cycle. Then to sustain this cycling rate during the duration of the power outage. This would allow the heat pumps to provide heating or cooling to restore temperature setpoints and for the refrigerator/freezers (2) to maintain proper temperatures. This cycle rate should result in a fuel consumption rate of 12.5% of the full time rate. At this rate my 250/150-useable gallon propane tank would provide 240 hours of cyclic backup power.

There is not a programable feature for this in the Generac Evolution 2.0 generator controller. I did not want to have to go outside twice every 2 hours and cycle the generator manually myself.

This project identifies how to add a Cyclic Timer Relay to a Generac generator and utilize the equipment protection features of the Evolution controller to prevent causing damage to the generator or household.
