## general notes for modding stellaris

- `on_action`
  - `bypasses` (scripts for connecting gateways/wormholes/lgates) 
    each have a "`on_action = <string>`" attribute that calls for a specific "`on_action`"-event upon entering FTL.  
    - `this = fleet`
    - `from = system jumping TO`
    - `fromfrom = system jumping FROM`
- game generates `on_building_<ship-size>` "`on-action`"-event for  ***"every station `ship-size`"*** (quote from vanilla documentation, see note)
  - `from = planet` (if it is an orbital station)
  - `this = constructor`

* note:the meaning of ***"every station `ship-size`"*** isn't specified.  
  * vanilla exerts:
    * `on_building_mining_station`
    * `on_building_research_station`
    * `on_building_outpost_station` (*no script-references exist, depricated?*)
    * `on_building_wormhole_station` (*no script-references exist, depricated?*)
    * `on_building_starbase_outpost` 
    * `on_building_observation_station`
    * `on_building_starbase_ai`
    * `on_building_starbase_ex`
    * `don_building_starbase_swarm`
    * `on_building_starbase_marauder`
  * It might apply to *every* `ship_size` and is just badly worded.
  * It might apply to specific `ship_classes` (vanilla-script includes: `shipclass_starbase`, shipclass_mining_station, shipclass_research_station shipclass_observation_station )
  * It's not "`is_space_station = yes`" as starbases have it set to "`no`". (maybe used with `OR`-trigger)
