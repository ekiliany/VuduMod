NOTE: Currently using the Bacon Specter glass material as a placeholder, but the default ARTII glass works fine as well. There will be a new glass material before the final version, and at some point the original glass objects in the model could probably be redone as well. Same situation applies with the crosshair, but from the the 3.5-10x scope.

List of major changes to be made:

o	Actual Vudu reticle needs to be added as eluded to above. The optic functionally is in a great spot, and textures are wip, so this has become a high priority. SR1 is the classic, but a modified SR4 or SR5 might work better in practice.

o Model-specific glass material needs to be set up as mentioned above. Have plans for this already

o	Colliders need to be added. Just got too deep in tweaking functionality and left this behind momentarily. This has already been done for the Vortex scope, so will be easy to complete ASAP.

o	Textures needs more metalness or something. I like the current texture but it looks so much different from the other scopes and weapon assets, and my evaluation is it looks less metal? Update: Oboe helping here since this is too important for the look of the scope in game, and apparently for avoiding the HDR bug

o	Parallax effects and potentially the PiP settings need to be tweaked to make moving while ADS to feel a bit more real.

o	Eventual transition to using the Bacon illuminated PiP scope object. IRL the reticle is illuminated and it looks awesome, so this will be important for both fidelity + cool factor. Not important at all in the short-run.

Previous issues now solved:

o	!!!SOLVED (sorta)!!! Brightness shoots up whenever aiming down sights. This is the #1 issue that needs solved before the scope is truly usable. Have solutions in mind to test soon. Solution note: This was due to my manual override of the textures making them darker to try and make the scope look better. Turns out that ends up triggering an HDR bug that is apparently caused by the game measuring the % of "dark pixels" on the screen. Lightening up the textures got rid of the sudden brightness, and the PiP layer in the blender model was also bumped back towards the eye a bit so there is less dark material 

o	!!!SOLVED!!!! Scope PiP and 2D now match decently, but now the scope is effectively zooming out a bit at 1x as opposed to matching 1:1 with unscoped world scale. This is issue #2 right behind the brightness stuff. Need to figure out how to balance all of this out so 2D and PiP are both true 1x. Solution note: cominbation of tweaking eye relief and effective FOV was the primary solution that will stay for now. Might need further tweaking but need to test under conditions where focus isn't auto enabled when ADSing like it is in the workbench environment for some reason
