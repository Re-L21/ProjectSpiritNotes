Character State

- Idle : grounded, locomotion
	- Walk (movement input <= .5 and movement input > 0)
	- Run ( movement input > .5)
	- Jump (jump input pressed)
	- Dash (dash input pressed and can dash)
	- Fall (not grounded (ground gone) )
	- Crouch (crouch input held)
- Walk : grounded, locomotion
	- Idle (movement input <= 0 )
	- Run ( movement input > .5)
	- Jump (jump input pressed)
	- Dash (dash input pressed and can dash)
	- Sprint ( sprint input held )
	- Fall (not grounded)
	- Crouch ( crouch input held )  

- Run : grounded, locomotion
	- Idle (movement input <= 0 )
	- Walk (movement input <= .5 and movement input > 0)
	- Jump (jump input pressed)
	- Dash (dash input pressed)
	- Sprint ( sprint input held )
	- Fall (not grounded)
	- Slide ( crouch input pressed )  

- Sprint : grounded, locomotion
	- Idle (movement input <= 0 )
	- Walk (sprint button not held and movement input <= .5 and movement input > 0)
	- Run ( sprint button not held and movement input > .5)
	- Jump (jump input pressed)
	- Dash (dash input pressed and can dash)
	- Fall (not grounded)
	- Slide ( crouch input pressed )
  

- Crouch : grounded, locomotion	
	- Slide (slide input pressed)
	- Idle (crouch input not held and has room)
	- Fall (not grounded)  

- Slide : grounded, locomotion, combat
	- Fall (not grounded)
	- Idle (slide ended and (crouch input not held and has room) )
	- Crouch ( slide ended and (crouch input held or has no room) )  

- Jump : in-air, locomotion
	- fall (not grounded and jump ended)
	- Dart (dart input pressed)  

- Fall : in-air, locomotion
	- Idle ( ground detected )
	- Jump (jump input pressed and can double jump)
	- Wall slide ( touching wall )
	- Glide ( jump input held )
	- Dart (dart input pressed)
	- Ledge hang ( ledge detected )  

- Dash : grounded, locomotion
	- Idle (dash ended)
	- Fall (not grounded)  

- Dart : in-air, locomotion
	- Fall (dart ended)  0

- Glide : in-air, locomotion
	- Idle ( ground detected )
	- Fall ( jump is not held )
	- Dart ( dart input pressed)
	- Wall slide ( touching wall )
	- Ledge hang ( ledge detected )  

- Wall Slide : touching wall, locomotion
	- Idle ( ground detected )
	- Wall jump ( jump input pressed )
	- Falling ( not touching wall )  

- Wall Jump : touching wall, locomotion
	- Fall (wall jump ended)  

- Ledge Hang : touching wall, locomotion
- Ledge climb : touching wall, locomotion
- Ceiling grab ? : 
- Special Actions <!> : ?
- Deflecting : combat
- Ultimate : combat, grounded
- Attack : grounded, in-air, combat

- Attack 
	- Aerial Attack 
	- Attack while moving