- [`small_artifact_reward` (Line 7)](#small_artifact_reward-line-7)
- [`medium_artifact_reward` (Line 25), `large_artifact_reward` (Line 43), `great_artifact_reward` (Line 61):](#medium_artifact_reward-line-25-large_artifact_reward-line-43-great_artifact_reward-line-61)
- [`create_grand_herald`](#create_grand_herald)
 
 
 ### `small_artifact_reward` (Line 7)
(scripted effect, often called by archaeological-stage-comletion-events, *[scopes](#notes_1): `this = fleet`, `from = archaeological_site`*)  
  * custome_tooltip calls for loc.: `"$minor_artifacts$ Found:"` [*1](#notes_1)  
  * The assosiated loc. calls for a string-variable: `$minor_artifacts$`.
    but note [`$minor_artifacts$` [*2]](#notes_1) does not have a value set yet.  
  * The scripded_effect is called once the stage-event-option is triggered by the player.
    so using `random_list` the Event-Window would close before the outcome is decided.
    but using [`locked_random_list` [*3]](#notes_1) we can determin the outcome before we execute the effect. and thus we can get a [proper tooltip [*4]](#notes_1):  
    > Minor Artifacts Found:  
    >`£minor artifact£` [amount] 
  * proper effect-tooltips are important in archeological-events as they are printet in the log **as is**.
    

 #### notes_1<!-- omit in toc -->
  * valid scopes: `fleet, ship, planet, pop, leader, army, megastructure, sector, starbase`
  * 1: `minor_artefacts` itself has associated locs.:  
    > `minor_artifacts:0 "Minor Artifacts"`  
    > `minor_artifacts_desc:0 "Minor artifacts ( £minor_artifacts£ ) [ ... continued]"`
  * 2: *investigate: different values for `string-variable`*
  * 3: outcome of `locked_random_list` is chosen **once** per event-scope
        (probably through some seed that is generated for each event-scope)
  * 4:  tooltip usin "random_list":  
    > Minor Artifacts Found:  
    > 33% chance of: `£minor artifact£` 1  
    > 33% chance of: `£minor artifact£` 3  
    > 33% chance of: `£minor artifact£` 5  


### `medium_artifact_reward` (Line 25), `large_artifact_reward` (Line 43), `great_artifact_reward` (Line 61):  
* same as `small_artifact_reward` (Line 7) with different amounts.  

### `create_grand_herald`
* *todo*