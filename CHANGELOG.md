# CHANGELOG

## Version 2.1.3

- Fixed bug with the search menu in the demo app
- Added API call to retrieve universes for an organization, MWZMapView.setUniverseForVenue can now take a MWZUniverse 
- Deprecated onMapLoad method, even if still fired for now; Use onMapLoaded instead 
- Added getBounds method for geometries

## Version 2.1.2

- Added get methods to MWZSearchable
- Added search bar example in demo app

## Version 2.1.1

- Added API methods to get venues, places and placeLists
- Added geometry and other parameters to MWZVenue

## Version 2.1.0

- showdirection is deprecated. Use MWZApi.getDirections and MWZMapView.startDirections methods instead.
- MWZLatLon and MWZLatLonBounds are replaced by MWZCoordinate and MWZBounds.
- MWZPosition has been removed. MWZPlace, MWZPlaceList and MWZCoordinate now implement the MWZDirectionPoint interface.
- Introduced MWZApi, a wrapper to easily retrieve Mapwize data. All API methods that were previously linked to the map have been moved to MWZApi.
- Introduced MWZAccountManager to share API Key between MWZApi and MWZMapView
- The MWZPlace object now includes the geometry
- MWZPlaceStyle has been renamed in MWZStyle

## Version 1.7.2

- Fixed bug related to measurement parsing and directions
- Added proguard rules

## Version 1.7.1

- Improved location service. Requires bluetooth et bluetooth_admin permissions to use iBeacons.
- Introduced startLocation and stopLocation methods in MWZMapView.
- onMapLoad only then the map is fully loaded.
- Added minZoom and maxBounds map options.

## Version 1.6.0

- Added completionHandlers to all methods which can fail
- Added support for multilingual venues
- General improvements and bugfix

## Version 1.5.0

- Added locationEnabled and beaconsEnables in MapOptions
- Added placeList support with api methods and directions to a list

## Version 1.4.1

- Added method to stop showing directions.
- Added method to set user position with accuracy.
- Added methods to set top and bottom margins.
- Added the possibility to display user heading. See code in example app.
- Added methods to query venues and places on id, name and alias.
- Added caching to limit network traffic and resist to loss of connection. Call refresh on the map to force the update of the data.
