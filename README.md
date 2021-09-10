# Interactive Map 
#### UofT Group Project: The Geographic Information System Mapping App
### Visiualization and Extracting Data from OSM
#### Autocomplete & Street Suggestion
This feature allows the user to input letter by letter and it autocompletes when there are enough characters.

![autocomplete](https://user-images.githubusercontent.com/61924332/132877398-3cd10a4c-e675-4fed-aff4-c39c9013a398.gif)

#### Find POI Tool
The use can set a pin as reference point, search a POI name, zoom into a feature, and remove a pin. 

![POI](https://user-images.githubusercontent.com/61924332/132878087-61c0faf3-c2e9-4b5e-9568-9c6438a6b061.gif)

#### Filter Tool
This feature Reduces clutter in dense locations and shows one or more types of point of interest at a time. It also utilizes familiar icons to improve readability for the user. 

![filter](https://user-images.githubusercontent.com/61924332/132878651-cfd3e531-ae7b-4aa6-89e9-955072831f95.gif)

### Advanced Features 

#### Auto Zoom
This feature prevents information overload which requires less attention from the user! Allows the user to find the closest POI relative to their selected position. 

![nearest](https://user-images.githubusercontent.com/61924332/132879973-5884ad8c-8a77-45e4-9f62-500fddc12106.gif)

#### Direction Finder
Get detailed travel directions and path finding visiualization. Use interchangebly between searching for an intersection and clicking on an intersection. 

![direction](https://user-images.githubusercontent.com/61924332/132880947-14c6e659-4708-4bac-bcdb-36c8dbb56ed8.gif)

#### The multi-dijkstra algorithm to solve the travelling courier problem



https://user-images.githubusercontent.com/61924332/132925209-9a6acd69-c748-4076-b5ca-397c1054a392.mp4

#### How our team tackled the Traveling Courier Problem. 

Given dropoffs, pickups and depot locations, we were tasked to find the fastest delivery path to deliever packages. 

We want to stay true to our goal of maintaining efficiency but also balance accuracy, so, we used multi-destination dijkstra's algorithm and multithreading to speed up the process.

Let’s start with multi-destination dijkstra. How does it save time? Well, we like to imagine a single source, single destination dikjstra’s algorithm, like a rock as a source, falling into a pond.

In the video for example, the destination is on top, but part of the wave goes below too. Keep in mind that this wave costs resources, for a rock, its energy, and for path-finding, this is time to search. 

Multi-destination dikjstra takes this opportunity, to look at all destinations whenever you send out a wave from a single source. Some could be to the left, maybe some to the right, but we are conserving resource this way by using the same wave.

We can lower the time down to 5.7 seconds by multithreading. This involves dividing the work up between the cores of the processor, and we can save the remaining time for the most important part: optimization!


