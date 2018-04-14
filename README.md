# gpkg-arna
Augmented Reality Navigation Assistance Using GeoPackage


__Release Notes__

# How to Use
 - You can change some settings by clicking on the wrench in the bottom left of the screen.
 - The heading on the top center of the screen represents the direction the phone is currently oriented towards (as you look through the camera)
 - When you begin a route, the distance to the next waypoint is shown under the heading indicator.
 - Select a GeoPackage file and route from the "SELECT ROUTE" button on the top right of the screen
 - The white line from the bottom middle of the screen points you to the next waypoint in the route line
 - The white/black marker identifies the next Critical Navigation Point (CNP) in the route. The CNP closest to the waypoint in the route will be displayed
 - If there is an related image for the CNP in the GeoPackage, using the Related Tables Extension, it will appear in the bottom right of the screen
 - The 'pause' button near the bottom middle of the screen will switch to manual navigation mode. In this mode, you select the next waypoint with the forward button and the previous waypoint is selected with the rewind button.
 - Pressing the 'play' button while in manual navigation mode will switch back to automatic navigation mode.
 - In automatic navigation mode, the route line will point to the next waypoint on the route. If you wander too far from the route, the line will point towards the nearest heading to intercept and return to the route. The distance you must be to be considered off route is 25 meters by default, and is configurable in the settings dialog.
 - In automatic mode, once you are a certain distance from the next waypoint (10 meters by default, configurable through the settings screen), the waypoint will automatically be advanced to the next on the route.
 - The pink markers are Points of Interest (POIs) for the selected route

# Known Issues
  - Group Overlapping CNP Markers has not been implemented yet, so if there are many markers in the same part of the screen, the text may overlap.
  - AOI features have not been implemented

# Building
See the INSTALL.md file.

__DEADLINE: APRIL 15TH__

# Requirements for the app:

 - **Software builds and installs according to supplied instructions** <a href="#note1" id="note1ref"><sup>1</sup></a>
 - **Route highlighted as overlay on live device camera image** <a href="#note1" id="note1ref"><sup>1</sup></a>
 - **Markers displayed for Critical Navigation Points (CNPs)** <a href="#note1" id="note1ref"><sup>1</sup></a>
 - **Accurate location of live AR navigation aids** <a href="#note1" id="note1ref"><sup>1</sup></a>
 - Photos stored in Related Tables Extension media table displayed at CNPs
 - User able to select from pre-defined routes available in the GeoPackage
 - Distance-to-CNP and other navigation hints (visual and/or audible)
 - Look-ahead option (see next CNP and the one after that)
 - Use POIs to highlight landmarks for route confidence/verification
 - Cross-platform operation, e.g. browser-based solution
 - Utilize proposed RTE “features” relation type linking routes and their CNPs & POIs
 - Additional functionality & UI/UX features addressing ease of use in high-stress scenarios.

 <a id="note1" href="#note1ref"><sup>1</sup></a>Top priority functionality required for prize award)

# Mockup of main screen
<img src="/docs/main_screen_mockup.png"/>

# Mockup of settings screen
<img src="/docs/settings.png"/>
