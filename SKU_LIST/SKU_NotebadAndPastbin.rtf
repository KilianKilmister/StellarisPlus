#SKU_LIST = {
#	event_target:SKU_LIST_CONTROLLER = {
#		switch = {
#			#scope
#			trigger = has_country_flag
#			SKU_LIST_list:last = {
#			}
#			SKU_LIST_list:new = {
#				#SKU_CREATE_LIST = yes
#			}
#			#	$identifier$_$list$ = { }				#saved event target list
#			SKU_LIST_list:get_list = {
#			}
#			SKU_LIST_list:$list$ = {
#				event_target:$list$ = {
#					save_event_target_as = SKU_CURRENT_LIST
#				}
#			}
#		}
#		#list_$num$
#		switch = {
#			#actions
#			trigger = $action|overwrite$
#			add_object = {
#			}			#add this object to the list
#			clear_objects = {
#			}			#clear every item
#			clear_objects_$attribute$ = {
#			}			#clear every item
#			copy_to = {
#			}			#copy to target list
#			delete_list = {
#			}			#delete scoped list
#			get_$attribute$ = {
#			}			#e.g. get_ID_<list id>
#			get_content = {
#			}			#get every list item
#			get_content_$attribute$ = {
#			}			#get every list item with $attribute$
#			set_flag = {
#			}			#sets flag
#		}
#		#	SKU_PRINT = yes
#	}
#}
#
#

| = = Structure of scripted_variables for SKU:
||==========================================================================================||
|| [@typeError:SKU_ExceededListLimit] ====> @[type] [ Error ] : [SKU] _ [ExceededListLimit] ||
|| _ _	_ _ _ _ _ _ _ _ _ _  _ _ _ _ _ _ 	  <type> <Subtype>   <MOD>   <   name  /  id   >||
||  <CASE - FORMAT>      : < key >  =>	 < key-description >							 	||
||-(U=UPPER, s=lower)----: ---------=>------------------------------------------------------||
|| 					  :    @     => Vanilla-designatior for scripted_variable 	 		 	||
||(ssssss) !-all-lower-! : < type > => the type of the variable 							||
||(UsssUss) !FirstOfWord!: < SubT > => the sub-type of the variable 						||
||  		    		  :  " : "   =>   (formatting) seperator [ types : naming ]			||
|| (UUU)   !-ALL-UPPER-! : < MOD >  => MOD-tag 										     	||
|| 		   		  	  :  "_"     =>   (formatting) seperator [MOD-tag _ variable name] 	 	||
||(UsssUss)!FirstOfWord! : < name > => name/ID of the variable 							 	||
||.o.p.t.i.o.n.a.l...o.p.t.i.o.n.a.l...o.p.t.i.o.n.a.l...o.p.t.i.o.n.a.l...o.p.t.i.o.n.a.l..||
|| 		   		  	  :  "_"     =>   (formatting) seperator [MOD-tag _ variable name] 	 	||
||(UsssUss) !FirstOfWord!:<name1..n>=> potential to add additional last segmenst 			||
||-----------------------:------------------------------------------------------------------||
 ==Variable Type
  (VTypes dictate the use of the variable, so Code can be easily navigated without much forehand knowlege of the project)
  -type 		=>			(Used to mimik Enum)
  -limit		=>  		(Used to globally limit values)
  -value		=> 			(Used to globally set costs or modifier values)

		 ==Variable Subtypes:
		  (Subtype is named after what kind or groupe of object/modifiers/etc. the variable dictates)
		 	-for VType: -type	=>		[(property-)Type]					=>	(can be used to check for a specific type of an Object category.
		 																			e.g: associated with leaders "@typeLeader:SKU_[leader Type]" or countrys @typeCountry:SKU_[country- /ethic- /authority-type]
		 	-for VType: -limit => 		[(trigger-)Property-to-limit] 		=> (if we want to limit the amount of caravans existing simultaniously, we could have @limitCaravans:SKU_[limit we want])
		 	-for VType: -value => 		[Property/Value/Modifier/Factor]	=> (can for examle be used to set a Ship_section-price for a new shipclass, rather selfexplanatory)

				 ==Variable Name/ID:
				  (final property giving the Variable a unique name/ID and shows a specific use)
					for: Vtype: -type 	=> 		-SubType: type 					 	=> 	here we ascociate the variable with a specific property of our SubType.
				 																 			e.g: @typeLeaderclass:SKU_General/Scientist/ModdedClassXYZ
				 	for: VType: -limit 	=> 		-SubType: [property-to-limit] 	 	=> 	here we can specify how something should be limited
																							e.g: @limitPlanetpop:SKU_[max/min/range/value/]
				 	for: VType: -value 	=> 		-SubType: [Property/Value/etc.]	 	=> 	here we can say what value this variable sets compared to other variables that would fit this property.
				 																			e.g: @valueShipupkeep:SKU_[High/Medium/low/Efficient/<TriggerXYZ>]

						 ==Defining Value
						 (Lastly there is the actual numeric Value to add to the Variable)
						 	this is selfexplanatory for VType limit/value	=> 	two Vanilla-variables written in our format:
																					(for -limit:	VANILLA: @tier1materialmin = 100	=> 		@limitMaterialreward:SKU_tier1_min = 100
						 															(for -value:	VANILLA: @tier1materialreward = 6	=>  	@valueMaterialreward:SKU_tier1 = 6
						 																													-now we start to see the difference in readability.
						 																													-our format also has way higher Mod-compatability due to the more complex structure
						 																													-BUT THIS DOES NOT MEAN that it takes noticably more effort/time to write and maintain our variables



												-here it becomes interesting:
						 							For VType: -type 	=> 	let's write Variables for all the leader classes like we did before and assign them each a different number,
						 								we get what is basically an Enum. (Placed on the left)
	PSEUDO_ENUMS									   -Now these Scripted_Variables are not connected in the script to what they represent,
	<CONSTANT = LeaderClass>				<value>	 	but don't need to be constantly linked, and when we want to give some value over to vanill things, it only has to be connected for an instant
	@typeLeaderClass:SKU_Leader 	= 			0	 	In the mean time we can perform all the logic we want with this enum savely away from Vanilla and other mods. and with a complex naming convention,
	@typeLeaderClass:SKU_Governeur 	= 			1	 	these values (and the connected) logic are well protected from accidental interfierence but can be very easily
	@typeLeaderClass:SKU_Scientist 	= 			2	 	accessed and used by people who want to. With a clear format, people will be able to work with theses files with little additional information.
	@typeLeaderClass:SKU_Admiral 	= 			3 	 	this makes working together or making Compatability-Patches much faster and less frustrating.
	@typeLeaderClass:SKU_General 	= 			4		on a final note: we can add non-Vanilla represented entries to this list and if we want to create new mechanics,
														for example a new attribute for Leaders called "LeaderPersonality", if we create another Enum for that,
														all the logic can be done without even having to touch an actual in-Game leader. (example also on the left)
														We would just have to setup some effects/events/modifiers that pass what is relevant and the
Same with non_Vanilla properties						resulting code would be multiple times more stable to outside influences like other mods and Vanilla-Weirdness
<CONSTANT = LeaderPersonality>			   <value>
@typeLeaderPersonality:SKU_Leader 		= 		0
@typeLeaderPersonality:SKU_Governeur 	= 		1
@typeLeaderPersonality:SKU_Scientist 	= 		2
@typeLeaderPersonality:SKU_Admiral 		= 		3
@typeLeaderPersonality:SKU_General 		= 		4
@typeLeaderPersonality:SKU_Leader 		= 		5
@typeLeaderPersonality:SKU_Governeur 	= 		6
@typeLeaderPersonality:SKU_Scientist 	= 		7
@typeLeaderPersonality:SKU_Admiral 		= 		8
@typeLeaderPersonality:SKU_General 		= 		9
@typeLeaderPersonality:SKU_Leader 		= 		10
@typeLeaderPersonality:SKU_Governeur 	= 		11
@typeLeaderPersonality:SKU_Scientist 	= 		12
@typeLeaderPersonality:SKU_Admiral 		= 		13
@typeLeaderPersonality:SKU_General 		= 		14

-------------------------------------------------------------------------------------------------



set_country_flag = <key>
set_planet_flag = <key>
set_fleet_flag = <key>
set_ship_flag = <key>
has_pop_flag =
global
star
relation
leader
ambient_object
species
megastructure
pop_faction

flag types
	country
	planet
	fleet
	ship
	pop
	star
	relation
	leader
	ambient_object
	species
	megastructure
	pop_faction



				buttonType = {
				name = "button_topbar_help"
				quadTextureSprite = "GFX_button_60_29"
				position = { x = @expand_x_pos y = -105  } #no direct anchoring to expand_button. uses scripted variable @expand_x_pos
				orientation = lower_right
				shortcut="alt+b"
			}


	spriteType = {
		name = "GFX_ship_class_small"
		textureFile = "gfx/interface/icons/ship_classes.dds"
		noOfFrames = 30											#system icon like primitive/megastructure usw
	}


	containerWindowType = {
		name = "station_icon_entry"
		size = { width = 28 height = 30 }

		iconType = {
			name = "type_bg2"
			position = { x = 4 y = 2 }
			quadTextureSprite = "GFX_typt_bg"
		}
		iconType = {
			name ="type"
			spriteType = "GFX_ship_class_small"
			position = { x = 4 y = 2 }
			alwaysTransparent = yes
			#scale = 0.75
		}
		iconType = {
			name = "type_bg"
			position = { x = 0 y = 0 }
			quadTextureSprite = "GFX_type_frame"
		}
	}


######################################
#	#NOTE:
#		use archeological sites with different leaders and scnenarios e.g: general to fight unrest
#
######################################

run file from script