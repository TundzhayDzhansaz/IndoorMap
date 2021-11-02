# IndoorMap
Interview question

#Building Maps (Any modifications you’d make to the building map)
Usually, buildings have not only one flat. We can create maps for each flat (mostly flat designs are the same each other. Possibly we'll need some little changes after designing the first flat.). Another option is to create 3D Building maps in the AR scene. That will be more effective than 2D for end-user.

#Algorithms (Any algorithms, third party libraries or frameworks you might use)
We can use it to draw the roads PollyLine third-party library. (https://github.com/raphaelmor/Polyline). If we can adapt our building roads to Dijkstra's algorithm it will be an awesome solution for us. Technically that is possible for example in the mall. Malls have most different paths to arrive from the first shop to the second shop. Some shops staying mid of the building and those shops have 2 side entertainment. Furthermore, if we think 3D, we should add the fire stairs and lift. Sum of these, if we can design the map very detailed, we'll have developed a difficult node(shops) network.

#Searching
I search route drawing algorithm on Stackoverflow and I found Eigen algorithm. https://stackoverflow.com/questions/11716268/point-in-polygon-algorithm/43896965#43896965


#Approach the problem (A clear explanation of how you’d approach this problem.)
I approached this problem with multiple solution styles. Because it was dependent on the indoor projects. 
1) We can solve this problem with access pointers. (for Indoor projects, we can use wifi access points and rooms access points to create. Example for shop mall: customer access point and brand access point.)
2) We can create/design/module detailed paths for our indoor area and we find the best path to our rotation.

----- I tried to draw a road with basic information. I think I didn't use effectively the hallway points. Normally before drawing the road we should set these hallway points as our road. Basically, without setting custom road points MapKit library is using the normal street path.

#Indoor navigation service https://github.com/dmsl/anyplace