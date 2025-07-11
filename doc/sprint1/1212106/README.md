# Building 4 #

## 1. Introduction ##
    This file documents the planning of the Building 4.

## Building Structure ##
### 1.1. Building Dimensions ### 
    Number of floors: 2
    Area: 30m x 30m = 900 m^2
    Height on floor 0: 4 meters
    Height on floor 1: 3 meters with a removable ceiling placed 2.5 meters above the floor.

### 1.2. Floor 0 ###
#### 1.2.1. Floor Layout ####
![floor_0-layout.png](images/floors_layout/floor_0_layout.png)

#### 1.2.2. Rooms ####

| Room&nbsp;Nº | Length(m) | Width(m) | Area(m^2) | Outlets |
|:------------:|:---------:|:--------:|:---------:|:-------:|
|    4.0.1     |   5,30    |   5,30   |   28,09   |    6    |
|    4.0.2     |   11,40   |  11,40   |  129,96   |   12    |
|    4.0.3     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.4     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.5     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.6     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.7     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.8     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.9     |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.10    |   7,00    |   3,50   |   24,50   |    6    |
|    4.0.11    |   7,00    |   3,50   |   24,50   |    6    |
    Room 4.0.12 is a storage area and it is not included in the measurements.
    Room 4.0.12 also does not require any network outlets. The same applies to restrooms and common areas.
### Measurements ###
![floor_0_measurements.png](images/floors_measurements/floor_0_measurements.png)

### 1.3. Floor 1 ###
#### 1.3.1. Floor Layout ####
![floor_1_layout.png](images/floors_layout/floor_1_layout.png)

#### 1.3.2. Rooms ####

| Room&nbsp;Nº  | With(m) | Length(m) | Area(m^2) | Outlets |
|:-------------:|:-------:|:---------:|:---------:|:-------:|
|     4.1.1     |  6,95   |   6,95    |   69,15   |   14    |
|     4.1.2     |  6,11   |   3,88    |   23,71   |    6    |
|     4.1.3     |  6,11   |   3,88    |   23,71   |    6    |
|     4.1.4     |  9,44   |   4,43    |   41,82   |   10    |
|     4.1.5     |  6,66   |   3,88    |   25,84   |    6    |
|     4.1.6     |  6,66   |   3,88    |   25,84   |    6    |
|     4.1.7     |  6,66   |   3,88    |   25,84   |    6    |
|     4.1.8     |  6,66   |   3,88    |   25,84   |    6    |
|     4.1.9     |  6,66   |   3,88    |   25,84   |    6    |
|    4.1.10     |  6,66   |   3,88    |   25,84   |    6    |
|    4.1.11     |  6,11   |   3,88    |   23,71   |    6    | 
|    4.1.12     |  6,11   |   3,88    |   23,71   |    6    |
|    4.1.13     |  5,56   |   3,88    |   21,57   |    6    |
|    4.1.14     |  5,56   |   3,88    |   21,57   |    6    |
|    4.1.15     |  5,56   |   3,88    |   21,57   |    6    |
|    4.1.16     |  5,56   |   3,88    |   21,57   |    6    |
|    4.1.17     |  5,56   |   3,88    |   21,57   |    6    |
|    4.1.18     |  5,56   |   3,88    |   21,57   |    6    |

    Room 4.1.19 and 4.1.20 are storage areas and are not included in the measurements.
    These rooms also don't require any network outlets.

### Measurements ###
![floor_1_measurements.png](images/floors_measurements/floor_1_measurements.png)

## 3. Outlets and  Acess Points ###
### 3.1. Outlets ###
#### 3.1.1. Overview ####
| Floor  | Outlets |
|:------:|:-------:|
| Ground |   72    |             
| First  |   120   |   

    The network outlets were placed on the walls of each room 1 meter from the ground. These
    devices were placed on strategical places of each room to minimize the cable costs related to
    its length.
    We should note that in any place of a room a network outlet is at most 3 meters away.


### 3.2. Acess Points ###
#### 3.2.1 Location ####
##### Floor 0 #####
![floor_0_ap.png](images/floors_aps/floor_0_ap.png)

##### Floor 1 #####
![floor_1_ap.png](images/floors_aps/floor_1_ap.png)


#### 3.2.2. Overview ####

| Floor  | Access Points | 
|:------:|:-------------:|
| Ground |       4       |                      
| First  |       2       |          

    The access points were placed in the ceiling of both floors. On the ground floor, 4 of them were placed covering a radious of about 6-7 meters.
    On the first floor, only 2 were needed covering a radious of 15 meters, granting full WI-FI coverage to the entire building.


## 4. Cross-Connections ##

### 4.1. Location ###

#### 4.1.1. Intermediate Cross-Connect (ICC) #### 
    Only one ICC is needed for this building.
    The intermediate cross-connect for this building is located in the room 4.0.12 (storage area in the ground floor).
    For this to be possible, the optical fiber comming from the outside the building is beeing conducted to this room via underground cable passageways.


#### 4.1.2. Horizontal Cross-Connects (HCCs) ####
    Only 2 HCCs are needed in this building, 1 per floor.
    In the ground floor it is located in the room 4.0.12 and in the first floor, it is right above in room 4.1.19.

## 5. Cables ##
### 5.1 Overview ###
    In this building we used CAT7 copper cables and optical fiber.

### 5.1.1 Caculations ###
### Floor 0 ###

![cables_tables_floor0.png](images/tables/cables_tables_floor0.png)

### Floor 1 ###
![cables_table_floor1.png](images/tables/cables_table_floor1.png)


## 6. Patch Panels ##
### 6.1 Patch Panels Overview ###
    Considering that we've opted for CAT7 cables to adhere to cable specifications, all patch panels will also be CAT7 compliant.
    In line with our selection of monomode optical fiber cables, the fiber patch panels must also be compatible with monomode fibers.
    Since the ground floor has 72 outlets we chose to use 1 patch panel of 24 ports plus a 48 ports patch panel.
    On the first floor, we have 120 outlets, so we chose to use 2 patch panels of 48 ports and one 24 ports patch panel.

| Floor  | Outlets | 24 ports Patch Panels | 48 ports Patch Panels | Switches |        Total         |
|:------:|:-------:|:---------------------:|:---------------------:|:--------:|:--------------------:|
| Ground |   72    |           1           |           1           |    2     | (2U + 2U) * 2U = 8U  |
| First  |   120   |           1           |           2           |    3     | (3U + 3U) * 2U = 12U |

    We decided to use only 24 ports CAT7 copper patch panels, each one takes 1U.
    For each corresponding switch is also added 1U, and at the end, 100% oversize must be added.

## 7. Inventory Total ##
| Floor | CAT7 COPPER CABLE(m) | OPTICAL FIBER(m) | ACCESS POINTS | OUTLETS | HCC | ICC | MCC |
|:-----:|:--------------------:|:----------------:|:-------------:|:-------:|:---:|:---:|:---:|
|   0   |       4262,47        |       3,5        |       4       |   72    |  1  |  1  |  0  |
|   1   |       7027,52        |       1,5        |       2       |   120   |  1  |  1  |  0  |