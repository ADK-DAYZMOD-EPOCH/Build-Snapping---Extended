Installation instructions:
 
1. Download and extract Snapping_v1.6.zip
 
2. unpbo MPMissions\YOURMISSIONNAME.pbo
 
3. Copy custom folder from the extracted Snapping_v1.6 to MPMissions\YOURMISSIONNAME\
 
4. Open MPMissions\YOURMISSIONNAME\init.sqf

Find this line:

	call compile preprocessFileLineNumbers "\z\addons\dayz_code\init\compiles.sqf";
	
and add this line RIGHT BELOW it:

	call compile preprocessFileLineNumbers "custom\snap_build\compiles.sqf";
	
so it will look like:

	call compile preprocessFileLineNumbers "\z\addons\dayz_code\init\compiles.sqf";
	call compile preprocessFileLineNumbers "custom\snap_build\compiles.sqf";

5. Open MPMissions\YOURMISSIONNAME\description.ext

Add this line to the VERY BOTTOM of it! (Yeah this means AFTER the last closing bracket!)
It has to be the VERY LAST LINE of the File!

	#include "custom\snap_build\points.hpp"
	
6. repbo MPMissions\YOURMISSIONNAME\

 - upaload - reload - snap - smile!
 
 
I hope I could clarify the !IMPORTANCE! that you copy the lines I mentioned to the VERY BOTTOM!
Else:
No Snap - No Smile - unneeded questions
 
 
 
Have fun with it,
Otter
aka Bob der Baumeister