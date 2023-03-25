RCOMP 2021-2022 Project - Sprint 1 - Member 1191831 folder
===========================================

***Disclaimer:** To calculate how many outlets we have for each room, we used the structured cabling standards that specify a minimum of two outlets per work area, and also a ratio of two outlets for each 10 square meters of area.*

<hr>

<h2> Building 2 - Floor 0 </h2>

<h3>Structured Cabling</h3>

![](https://raw.githubusercontent.com/rui-goncalo/rcomp/main/1191831/assets/building2_floor0.png)

<h4>Room 2.0.1</h4>

in this room we’ll have an Intermediate Cross-Connect(IC) and a Horizontal Cross-Connect (HC) with 24 connectors. The IC receive optical fibre from the Main Cross-Connect (MCC) and will send the optical fibre to the HC. From HC, we’ll pass copper cable to outlets in the floor. The room - with 9.79m2 - will have 2 outlets.

<h4>Room 2.0.2</h4>

This room has 24.8 m2. With that, we use 6 outlets based in the logic described in the beginning of this document. In this room, like any other one, we have an outlet everywhere less than 3 meters.

<h4>Room 2.0.3</h4>

This room has an area of 83.5 m2 and because of that, we’ll use 18 outlets. In this room we'll also have an Access Point (AP) and a consolidation point with 24 connectors.

<h4>Room 2.0.4 / 2.0.5 / 2.0.6</h4>

These rooms are the same size - 28.3m2 -, and have 6 outles in each room. The room 2.0.6 also have a consolidation point with 24 connectors.

<h3> Inventory - Floor 0 </h3>

- 1 Intermediate cross-connect
- 1 Horizontal cross-connect:
    - 1 Patch Panels (Optical Fibre) with 24 ports each
- 2 Consolidation Point
    - 2 Patch Panels (Copper) with 24 ports each
- 2 Access Points
- Optical Fibre Cable: 2 meters
- Copper Cable: 907.49m ≈ 908 meters
- 44 outlets
- 44 Patch Cords

<hr>

<h2>Building 2- Floor 1</h2>

<h3>Structured Cabling</h3>

![](https://raw.githubusercontent.com/rui-goncalo/rcomp/main/1191831/assets/building2_floor1.png)

<h4>Room 2.1.1</h4>

With a total area of 6.29 m2 we can implement here 2 outlets. We also have a HC that receives optical fibre from the IC.

<h4>Room 2.1.2 / 2.1.3 / 2.1.4 / 2.1.5 / 2.1.6</h4>

In these rooms we have an area of 8.50 m2 in each one, which means that we will have 4 outlets as well**.**

<h4>Room 2.1.7 / 2.1.8</h4>

These rooms have the same area of 11.66 m2 and both will have an Access Point.

<h4>Room 2.1.9 / 2.1.10 / 2.1.11 / 2.1.12</h4>

In those we have an area of 8.29 m2 and 8 outlets at all. The room 2.1.12 will have a Consolidation Point.

<h3> Inventory - Floor 1 </h3>

- 1 Horizontal cross-connect:
    - 1 Patch Panel (Optical Fibre) with 24 ports each
- 1 Consolidation Point
    - 1 Patch Panel (Copper) with 24 ports each
- 2 Access Points
- Optical Fibre Cable: 2m (+ 2.5m of building height) = 4.5m ≈ 5 meters
- Copper Cable: 942.61m ≈ 943 meters
- 28 Outlets
- 28 Patch Cords

<hr>

<h2>Dimensions</h2>

| Room | Length | Width | Area (m2) | Outlets |
| ----------- | ----------- | ----------- | ----------- | ----------- |
| <strong>2.0.1</strong> | 3.5 | 2.8 | 9.8 | 2 |
| <strong>2.0.2</strong> | 4.3 | 5.8 | 24.8 | 6 |
| <strong>2.0.3</strong> | 8.5 | 9.8 | 83.5 | 18 |
| <strong>2.0.4/5/6</strong> | 8.5 | 9.8 | 83.5 | 18 |
| <strong>2.1.1</strong> | 1.7 | 2.0 | 6.3 | 2 |
| <strong>2.1.2/3/4/5/6</strong> | 2.7 | 1.7 | 8.5 | 2 |
| <strong>2.1.7/8</strong> | 3.3 | 3.5 | 11.6 | 6 |
| <strong>2.1.9/10/11/12</strong> | 1.6 | 2.8 | 8.3 | 4 |


<hr>

<h2>-> Intermediate Cross-Connect</h2>

The IC receives the optical fibre cable from the Main Cross-Connect. Usually exists one per building and make the connection to all the HCs.

<hr>

<h2>-> Horizontal Cross-Connect</h2>

The area of this building is approximately 400 m2, so no needed more than one per floor.

<hr>

<h2>-> Consolidation Point</h2>

Consolidation Points give the utility of regenerate the signal to make possible reach outlets that may possible be too far away or in zones with a big amount of outlets. We implemented 2 in floor 0 and 1 in floor 1.

<hr>

<h2>-> Copper Cable</h2>

To connect our HCs to the outlets we will use CAT7 cables. When compared to CAT6a, the use is justified, since despite having the same maximum speed, the frequency is doubled. That said, the signal will be able to pass through CAT7 cable twice as many times as it will pass through CAT6a.