## Modding Documentation

#### Debugging
General debugging help

| Commands        		| Type           	| Notes 		|
| --------------------- | ----------------- | ------------- |
| event pog_debug.1 	| event 			| opens debugging event |
| pog_debugging  		| global_flag 		| only if turned on, allows certain options|

#### Flags
These are some some important and general flags, planet_modifiers or variables that can that are used to trigger various events:

| Commands        			 | Type          | Notes 		 |
| ---------------------		 | ------------- | ------------- |
| recent_subversive_media 	 | planet_flag	 | makes sure a planet is not bombarded with media events related to controlled media |
| recent_disaster  			 | planet_flag	 | flag that stays on for a while during and after a disaster |
| recent_drought  			 | planet_flag	 | flag that stays on for a while during and after a drought |
| parade_troubles_ahead 	 | country_flag	 | is being put on the country, if the soon-to-be parade will have some type of man-made, malicious incident |
| no_military_parade_held 	 | country_flag	 | set and stays on for a while, if a country failed or refused to have a parade |
| fleet_parade_held  		 | country_flag	 | set and stays on for a while, if a country had a successfull parade |
| grand_military_parade_held | country_flag	 | set and stays on for a while, if a country spend some extra cash to have a grand parade |
| has_insurgency_intel 		 | country_flag	 | bonus to discovering insurgents plot |
| insurgency_in_hiding		 | country_flag	 | penalty to discovering insurgents plot |

#### Custom Scripts and Triggers
These are some of the useful scripted effects and triggers that are used throughout the mod:

| Commands        				 | Type          | Notes 		 |
| ---------------------			 | ------------- | ------------- |
| is_isolationist  				 | trigger 		 | a simplified check if the country is allowed to do diplomacy, based on xenophobia or inward isolationism |
| is_murdering_monsters 		 | trigger 		 | a simplified check to see if the country will/is allowed to do diplomacy, based on murdering purifiers |
| is_artificial_planet 		     | trigger 		 | a simplified check to see if the planet is artificially created (ring worlds, habitats etc.) |
| has_disaster_resources 		 | trigger		 | checks if the country (or sector) has enough resources [for disaster aid]; scales with population |
| pay_disaster_resources 		 | effect 		 | pays the resources [for disaster aid]; scales with population |
| has_disaster_food  			 | trigger 		 | checks if the country has enough food stockpile for disaster aid; scales with population |
| pay_food_disaster_resources    | effect 		 | takes food from stockpile [for disaster aid]; scales with population |
| has_two_times_food  			 | trigger 		 | checks if the country has enough food stockpile for disaster aid; scales doubles with population; mainly used for ai decisions |
| generate_rng_10.1  			 | effect 		 | creates a random number between 1-9 and saves it as value of @ROOT.rng_value_10.1 |
| generate_rng_10.2  		 	 | effect 		 | creates a random number between 1-9 and saves it as value of @ROOT.rng_value_10.2 |
| generate_rng_100  		 	 | effect		 | creates a random number between 1-100 and saves it as value of @ROOT.rng_value_100 |
| 								 | 				 |tip: can be used to insert a number into localisation by using [@ROOT.rng_value_100.GetValue] |
| [ROOT.GetDemocraticMisconduct] | scripted_loc  | fills in a random (democratic-ish) misconduct that a government official could have committed |

-------------------------------------------------------------------------------------------------------------------------------------
#### A list of policies:

* regulation_laissez_faire
* regulation_free_markets
* regulation_heavily_regulated
* regulation_centralised_production
* regulation_gestalt_free_trade
* regulation_gestalt_no_trade
* regulation_free_trade
* regulation_mercantilism
* regulation_isolationism
* regulation_free_media
* regulation_controlled_media
* regulation_state_media
* regulation_free_assembly
* regulation_assembly_prohibited
* regulation_assembly_forced
