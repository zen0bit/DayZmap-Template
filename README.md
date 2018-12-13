DayZCommunityOfflineMode

-mission=.\Missions\DayZCommunityOfflineMode.ChernarusPlus -scrAllowFileWrite

L3DT



PMC Terrain Builder Mini Tutorial

ArmA 3 Terrain Builder Mini Tutorial by PMC

Updated for DayZ / terrain builder v1.31.0.139381

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