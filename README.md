DayZCommunityOfflineMode

-mission=.\Missions\DayZCommunityOfflineMode.ChernarusPlus -scrAllowFileWrite

L3DT

	making a fantasy island can all be created using L3DT. If you haven't already I'd suggest following jakerods Atlas tutorial on getting started with terrain builder first. If you have already done that then read on.

	For a basic mask and sat image you don't even need photoshop as L3DT does all the work for you.

	heres a base guide for a simple quick and easy terrain done in two stages.



Stage 1:


	Open L3dT and click new map, then follow the wizard.

 

	or


	File/new/Designable Map

 

	click next. 

Heightfield size:

	this is where you decide on how big you want your map. To begin with I'd recommend going smallish. 512x512 (use the sliders to do this)
	then adjust your horizantal scale. This will give you the meter per pixel differentiate. set that to 10 and you have a map just over 5x5 Km, or 26sq Km overall.

	Click next twice and you come to a window showing you map parameters.

Design Map:
	Here you can set you land features, more water, less water, rolling hills or mountains and valleys.
	Use the sliders to choose what you want more or less of and then choose what type of climate you want.

Climate choice;

	When choosing your climate you need to be mindful that when you come to generating your layers in terrain builder you may not be so lucky in having all 18 or so ground textures that L3DT gives you.
	Terrain builder use 4,5 or 6 ground textures per grid. You can find more info on that here: http://forums.bistudio.com/showthread.php?186855-Is-this-really-what-our-mask-should-look-like&p=2843467&viewfull=1#post2843467

	if you wanted to use a temperate climate in L3DT you WOULD need to use Photoshop or similar program to alter the mask colours to fit in with the 4,5,6 rule.

However: demo-grass-rock gives you just 3 textures and it is as basic as can be for your first random generated map. and fits within the 4,5,6 rule.

	Select demo-grass-rock-sand from the list in the dropdown box, you'll find that at the bottom. Then click next.

Calculation queue:
	Here you can select all your maps in one go to get generated in L3DT. Check off all the boxes and then click next again.

	The following 2 boxes you can just click next through Attributes map.

Attributes map:
	The Attributes map is the map you can use for your mask. Check off the box that is "Make High-res attributes map" then click next.

Normals map;
	Normal mapping: this one generates a normals map you can use if you want to. Terrain builder will allow you to have 5 textures on your map using this map. Check off the high res normals box again and click next.

	Light mapping.
	the next two windows are for lighting effects. my advice would be not to mess around with the values much as it will screw things up on your map when you look at it in 3D mode (More on that later). click past the first window then when you are at the second lighting window you only need to select "Make High res light map. You have already applied the bump mapping. click next and next again on Light/water effects.

Texture map:
	Texture settings again click on next and save the project under something you can recognise and put it in a folder you can easily locate.

	(when you save your project a number of folders will be created and you also will get a project file. When you close and reopen L3DT you only need the project file to load,not the files within the newly created folders. )

	Once saved, L3DT will go through the motions of creating a map based on your own parameters you set in the wizard. Using a small map of 512x512 you should get a map within 20-30 seconds showing on your screen.

Stage 2:

	You should now see a number of tabs across your screen starting with Design map through to TN-Tangent. you can click on any one of the tabs and once that map loads you can see your map in various different ways.

	Once you do, click on the 3D button at the top and you should see all your hard work (cough L3DTcough) work in 3D format.

	Navigating your way around the map is quite easy. ,W,A,S,D for the usual, then you have E for height up and R for height down. Rotate and select are the mouse and LMB. If you press H you get your heightmap tools so you can actually alter the map however you like if you are not fully with L3DT's result. by Pressing Esc you go back to your map tabs.

	heightmap editing is quite extensive so looking at the L3DT tutorials would be best for that.

	Once you have your map and are happy with it, there are 3 maps you need to use from your project. Heightmap, Attributes and textures. You can export each of them into your Pdrive; work folder for your Arma map. then at least you will be able to figure out where those 3 files go too. It would be in any case, Pdrive/Yourtag/projectname/source.

	Once you are ready to export the maps from L3DT to get them in terrain builder, start with the Heightmap.

Exporting the maps:

Heightfield map:
	Click the heightfield tab in L3DT, let it loadup if you are looking at another map, then put your cursor on the tab and rightclick. then Export layer. The wizard appears again, drop down the file format box and select x.y.z or ASC, then click options and double click on true, it shoudl change to false, then click ok.

	In the filename box click the three dots, and navigate to your source folder for your project in terrain builder. Name your map "heightmap" and then save.

Attributes map:
	Now go to your attributes map and do the same thing, except you don't need to go with x.y.z its just a simple BMP image you can save it as. If you are not entirley happy with the why L3DT has produce textures you can optionally edit it in photoshop or similar. Again navigate to your source folder and save it as "mask_lco". Without quotations marks of course.

	Now when you export this map, L3DT also exports two other files for you. an HTML file containing the RGB colourings and their values, it also gives you a text file doing the same except it is just text. Unless you don't like the L3DT colours and you changed them in Photoshop you can use these values for the layers file so terrain builder can cross reference the information.

texture map:
	As you did with the attributes map you do the same with the texture map. Navigate and save it as a bmp image again in your source folder but name it "sat_lco".

	Thats pretty much it for generating a basic L3DT "fantasy island/map. the rest of the work is done using terrain builder. If you have gone through Jakerods tutorial then you should be having a wail of a time figuring out what works and what doesn't in TB but for the most part you are as you have seen on armaholic able to generate a full blown map to play on.



PMC Terrain Builder Mini Tutorial

ArmA 3 Terrain Builder Mini Tutorial by PMC

Updated for DayZ / terrain builder v1.31.0.139381

	Settings: tools - settings
		User settings
		Data directory: c:\zen0bit
		Project directory: C:\zen0bit\GrandeTerra
	Buldozer:
		.exe file path: D:\Steam\steamapps\common\DayZ\DayZ_x64.exe
		launch parameters: -buldozer -window -nopause -mod= -profiles=<path_to_work_folder-drive>\Buldozer -name=Buldozer
		data directory: C:\zen0bit
		
how to...

    mapframes › add mapframe, click ok
    type in project name to properties › name
    type in project root dir to properties › output root folder. (this would be P:\prefix\tag_projectname)
    click create subfolders button, click ok
    copy your data ground texture rvmat's and paa's into <project>\data\ directory
    copy your layers.cfg and maplegend.png files into <project>\source\ directory
    set easting to 200000 and northing to 0
    switch to samplers tab, setup properties according to your terrain (make sure texture layer is at least 2x your cell size)
    switch to processing tab, use “…” button to browse into your source\layers.cfg file
    click rebuild terrain button, click yes
    click OK in bottom of mapframe properties dialog
    save your project to Source\TerrainBuilder\ directory
    file › import › terrains (xyz file)
    file › import › satellite images (you can choose bmp or png)
    file › import › satellite mask images (you can choose bmp or png)
    layers manager do on all layers, click RMB › Terrain Coordinates & Properties, easting: 200000, northing: 0, also Size width/height
    mapframes window › your project name › click RMB › properties (or double LMB click)
    switch to processing tab, click rebuild terrain button, click yes
    tick export satellite texture and surface mask (make sure 4 materials per cell is selected)
    click generate layers button and wait until its done
    click OK and save your project
    convert layers\*.png to *.paa

Now your terrain is ready for viewing using terrain builder buldozer.
Object Placement

Adding P3D objects into a template

    library manager › template libraries › RMB › create library
    give it a name
    tick create new library from directory
    source directory point to › P:\a3\plants_f\Tree
    click ok, all done

Single Object

    create object template
    select object from library manager › template libraries › whatever-template
    click add object icon from main menu (icon: side ways box and plus sign)
    LMB click anywhere on the map, object is placed

Forests

    turn on view shapes icon in main menu
    click layers manager › shapes tab
    click add new layer button icon, give it some name
    click add polygon icon from main menu (icon: box and plus sign)
    now LMB click points to create a polygon, once youre done double LMB click to close the polygon
    click layer manager › objects tab
    click add new layer button icon, give it some name
    unselect “add polygon” button
    click to select any of your polygons in terrain, RMB › Fill (add new objects)
    select objects (trees for a forest)
    properties › preset name: add some name like forest 1 etc
    other settings are up to you what you use, object density 60, click
    click ok and objects are placed inside your selected polygon

Export / Import Objects

Export

    file › export › objects
    click document to export all objects in your project
    click available templates select all button
    use whatever format suits you, custom is compatible with the old arma2 formats
    select destination file, click OK to export

Import

    select which layer you want to import objects
    file› import › objects
    select file to import with the “…” browse button on destination file
    click OK to import

Export heightmap from terrain builder for l3dt
to *.xyz