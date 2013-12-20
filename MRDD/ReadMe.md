Minecraft resource density detector.

Right now it is not very sophisticated, but as a proof of concept it works.

The program accepts an image consisting of transparent blocks representing undesirable blocks and desirable blocks that colored to a heightmap.

The way that I know how to do this is via [Cartograph-G](http://www.minecraftforum.net/topic/153066-cartograph-g-map-your-world-minecraft-14/). The tool is a little out of date, so you might need [this supplementary file](http://www.minecraftforum.net/topic/153066-cartograph-g-map-your-world-minecraft-14/page__st__1220#entry26583172) for newer resources, which is included in the repository.

Generate the map by choosing "overhead", heightmap (color), show only 52. The program will create a png image in the Cartograph-G directory.

You can load your map by dragging and dropping the image into the file input field, or navigating to the file.  Press load once you are ready.  This will be resource intensive.

Drawbacks: Y-stacked blocks will not be detected.

// TODO: Custom search radius, height difference.
// TODO: Custom heightmap color importing.
// TODO: high/max Y item included could serve as a coordinates marker to compute from (Please be careful getting down from it!)
// TODO: I am fairly sure the location algorithm could be better. Maybe quadtree if accuracy isn't a huge issue (Example: flowers).
