# Update notes
This page lists the updates we've made to DorsetExplorer and any changes you should be aware of. The [technical release notes can be found on GitHub](https://github.com/Dorset-Council-UK/GIFramework-Maps/releases).
## Version 1.7.0
- Added an option for including a simple [scale bar](./exporting-and-printing.md#scale-bar) on your prints
- Some layers will now have disclaimers when you first click them to inform you of any important data quality or licencing information
- Fixed a few bugs and improved some behind the scenes tech to make things quicker

## Version 1.6.0
- Added option for including a [north pointer](./exporting-and-printing.md#north-pointer) on your prints
- Added a 'Collapse all' button to the layer control, to collapse all open folders in one click
- Fixed a bug where coordinates copied from two seperate cells in a spreadsheet would not be recognised

## Version 1.5.0
- Added a new scale bar style - click on the scale bar to toggle it between two styles
- Added a link to further information about a layer when you click on a feature on the map

## Version 1.4.0
- Made [measurements configurable](./measuring.md#configuring-your-measurements)
- Added more font options to the [text annotations tool](./drawing.md#add-text)
- Added a [version switcher](./versions.md)
- Share panel - 'Embed the map in your own page' has been removed

## Version 1.3.0
- Added Dark Mode - Click the sun icon :octicons-sun-16: to switch to a dark theme or use whatever your system uses. The map itself will not become dark, but there is a basemap option available which has a dark colour pallete. 
- Added [Buffer annotations](./drawing.md#draw-a-circular-buffer)
- Map projection is now in British National Grid - This improves the quality of our basemaps and prevents warping caused by reprojection. This does mean that you are restricted to Great Britain now.
- Added attribution information to the [metadata](./layers.md#metadata) dialogs

## Version 1.2.0
- Added new point icons and border options in [annotations](./drawing.md)
- Opacity and Saturation sliders now have labels

## Version 1.1.0
- Improved handling of [metadata](./layers.md#metadata)
- Added [legends to prints](./exporting-and-printing.md)
- Made sidebar headers 'sticky'

## Version 1.0.0
- Added [GPS tracker](./geolocation.md) functionality
- Allowed [multiple search result pins](./searching.md#advanced-customising-your-search) on the map at once
- Added [Short Links](./sharing-your-map.md#short-links) feature to Share tool
- Added [Bookmarks](./bookmarks.md) feature (logged in users only)

## Changes from DorsetExplorer 3
We've made a number of changes to DorsetExplorer from our old version. 

### Major changes

- ⭐ A new and refreshed style! We've refreshed the design to be more modern and touch friendly. We've tried to maintain consistency with the old version so it should still feel familiar, but there have been some minor changes, such as the Search Bar now being in the top left, your coordinates being in the bottom left, and annotation and measurement tools being on the left hand side
- 🖍 Saturation controls for all layers. You can now control the saturation of the basemaps and layers, meaning you can choose to turn a basemap or layer greyscale or just tone down the colours as and when you like
- 🗺 A new set of basemaps. We now make use of the base maps provided to us by Ordnance Survey which are higher quality and consistent across all zoom levels. They also come in a couple of different styles which you can choose from in the basemaps panel
- ✨ A redesigned layer control. The layer control is probably the most important part of DorsetExplorer, so we've given it a fresh lick of paint and added some additional functionality.
    - You can now choose to sort the folders alphabetically rather than by their default
    - The search is a bit friendlier and allows for basic spelling mistakes
    - Layers now have metadata available (via the 'i' button next to the name), so you can learn more about what a layer is and where it comes from
    - You can choose different styles for certain compatible layers
- 📍 Add your own layers to the map. You can now add a GPX, KML, GeoJSON or IGC file simply by dragging and dropping it on to the map. You can also add layers from a number of external web services to further enhance your map
- ✏ Editable annotations. You can now edit your annotations geometry and style after drawing them, and there are a bunch more styling options for them as well. The annotations toolbar is now on the left, instead of in its own panel on the right

### Improvements
- Features you click will be highlighted on the map, showing exactly what it was that you clicked
- Measurements can now be edited, and the measurement buttons are always available on the left, rather than being hidden behind the right click menu
- Polygon and Buffer feature searches are now always available on the left, rather than being hidden behind the right click menu
- You can now rotate the map. Just hold down <kbd>Alt</kbd> and <kbd>Shift</kbd> and drag the map to rotate the map, or use two fingers and rotate the map on a touch screen
- Legends now show how many features there are of that type in the window you are currently looking at. Some layers from external services do not have this option and will display as usual
- The link that is generated by the share tool now includes any transparency or saturation settings for your layers and the search result pin you have on the map. The URL in your browsers address bar also updates as you move around. Note that you cannot currently share measurements, annotations or custom layers
- You can copy a locations' coordinates to your clipboard by right clicking on the map and choosing 'Copy coordinates to clipboard'
- You can search for What3Words and Plus Code locations in the search bar, as well as all the usual searches
- You can also search for coordinates in Degrees/Minutes/Seconds format. This currently requires quite specific formatting, and some formats may not work, so for the avoidance of doubt, try to search for these coordinates using this format - 50° 48′ 49.2″ N 2° 28′ 29.3″ W
- Printing should be a bit quicker and slicker than before

### Minor changes
- Google Street View imagery will now open straight into Google Maps rather than in a popup bubble on the map
- Only one 'search result' pin will be shown on the map at once by default. You can change this back to the previous behaviour by going into the search preferences dialog (the cog next to the search box) and checking 'Allow multiple search results on map at once'

### Removed features
- The Coordinate Translator has been removed. It was under utilised and there are better alternatives out there for converting coordinates.
- Print to Scale has not been included. We may add this back in at some point, but no immediate plans. If you need something properly printed to a measurable scale, you should probably be using professional GIS software such as QGIS
