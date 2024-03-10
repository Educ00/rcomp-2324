# Building 3 #
## 1. Introduction
    This file documents the planning of the Building 1.

### 1.2. TODO: Subtitles Image ###
![Subtitles]()

## 2. Building Structure
### 2.1. Building Dimensions ### 
    Number of floors: 2
    Area: 20x20 (400 m^2)

### 2.2. Ground Floor ###

### 2.2.1. Floor Layout ###
![Floor_Ground](images/ground/floor_ground-limpo.png)

### 2.2.2. Rooms ###

| Rooms  |  Size   | Area | Outlets |
|:------:|:-------:|:----:|:-------:|
| 1.0.1  | 5,3 x 5 | 26,5 |    6    |
| 1.0.2  | 3,7 x 5 | 18,5 |    4    |
| 1.0.3  | 4,7 x 5 | 23,5 |    6    |
| 1.0.4  | 5 x 7,2 |  36  |    8    |
| 1.0.5  | 6 x 4,4 | 26,4 |    6    |
| 1.0.6  | 6 x 7,2 | 43,2 |   10    |

### 2.3. First Floor ###
#### TODO
### 2.3.1. Floor Layout ###
![Floor_First](floor_first.png)

### 2.3.2. Rooms ###

| Rooms  |   Size    | Area | Outlets |
|:------:|:---------:|:----:|:-------:|
| 3.1.1  | 5,3 x 7,8 | 31,3 |   10    |
| 3.1.2  | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.3  | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.4  | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.5  | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.6  | 8,6 x 3,3 | 17,5 |    4    |
| 3.1.7  | 8,6 x 3,3 | 17,5 |    4    |
| 3.1.8  |  2 x 6,9  | 13,8 |    4    |
| 3.1.9  | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.10 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.11 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.12 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.13 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.14 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.15 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.16 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.17 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.18 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.19 | 5,3 x 3,3 | 17,5 |    4    |
| 3.1.20 | 5,3 x 3,3 | 17,5 |    4    |


## 3. Outlets and  Acess Points ###
    We assumed that this building will be used by a large number of people, so we designed the network to support a large an equaly large number of devices simultaneously.
    The number of devices that the network support simultaneously can be increased by upgrading the model of the acess points or adding more acess points.
    In this project, we chose a model that supports up to 30 devices.
    Please note that adding more access points may change the layout and configuration of the rest.
### 3.1. Outlets ###
#### 3.1.1. Overview ####
| Floor  | Outlets | Usable Outlets |
|:------:|:-------:|----------------|
| Ground |   76    | 67             |
| First  |   86    | -              |

### 3.2. Acess Points ###
#### 3.2.1. Overview ####

| Floor  | Access Points | Max Devices (people) |
|:------:|:-------------:|:--------------------:|
| Ground |       9       |      270 (135)       |
| First  |       -       |          -           |

#### 3.2.2. Configuration ####
    All the acess points are placed in the cealing.
    The power and range of the signal is configured individually for each access point to garantee that the signals of every access point don't overlap more than 15% with each other and also to not waste signal to the outside of the building.
    The radius of every access point is configured to be around 2-3 meters to 6-7 meters.
#### 3.2.3 Location ####
##### 3.2.1. Ground Floor #####
![Acess_Points_Floor_Ground](images/ground/aps/floor_ground-aps&range.png)

##### 3.2.2. First Floor #####
![Acess_Points_Floor_Ground]()

## 4. Cross-Connections ##

### 4.1. Location ###

#### 4.1.1. Intermediate Cross-Connect (ICC) #### 
    Only one ICC is needed for this building.
    The intermidiate cross-connect for this building is located in the room 3.0.14 (storage room in the ground floor).
    For this to be possible, the optical fiber comming from the outside the building is beeing conducted to this room via underground cable passageways.

![Cross-Connections_Floor_Ground](images/ground/connectors/floor_ground-connectors&optical.png)

#### 4.1.2. Horizontal Cross-Connects (HCCs) ####
    Only 2 HCCs are needed in this building, 1 per floor.
    In the ground floor it is located in the room 3.0.14 and in the first floor, it is right above in room 3.1.18.

## 5. Cables ##
### 5.1. Layout ###
#### 5.1.1. Ground Floor ####
![Cross-Connections_Floor_Ground](images/ground/cables/floor_ground-cables&outlets&aps.png)

#### 5.1.2. First Floor ####
![Cross-Connections_Floor_First]()

### 5.2. Types ###
    Optical fiber is only used to conduct the signal from outside to the ICC.
    The rest of the cables are used to make the connection from the HCC to the outlets and the access points.
    The type of the cables was determined to be Monomode Optical Fiber and Cat7 Coper Cables.

### 5.3. Length ###
#### 5.3.1. Ground Floor ####
![img.png](images/ground/tables_length/floor_ground-table_copper_length.png)
![img_1.png](images/ground/tables_length/floor_ground-table_optical_fiber_length.png)
![img.png](images/ground/tables_length/floor_ground-table_total_length.png)


#### 5.3.2. First Floor ####