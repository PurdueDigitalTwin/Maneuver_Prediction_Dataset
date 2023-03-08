# Maneuver Labeling Instructions
General Instructions:

- This dataset contains videos recorded in two views (in-cabin and front-facing) simultaneously.
- Each video file in the dataset is one minute long, except for a few shorter ones.
- Please assign the same video ID to the two videos recorded simultaneously (the file names are different).
- The maneuver can be labeled by watching the front-facing view only. Use the timestamp in that video to determine the start/end time.
- The recording times are available at the bottom of each video.
- If there are no predefined maneuvers presented in the video, put all video names (both views) into the 'REXING_Lexus_ignored' spreadsheet. For example, if the ego-vehicle does not move for the whole video.
- It is recommended to sort the file names before starting labeling to avoid any confusion.
- Do not add annotations to time windows that do not belong to the 5 predefined maneuvers.
- None of the predefined maneuvers include moving reversely.
- In case of a roundabout, please ignore it for now and do not label it (treat it as not defined time window).

**Several videos have already been labeled as examples.**

Goal: 300 labeled videos by the end of March.

--- 

The links are:

[REXING_Lexus_anno](https://docs.google.com/spreadsheets/d/12g0dBMUhm32yTdb6MrWoJemRPFTceEK4Z6uQIpUcy1w/edit?usp=sharing)
, [REXING_Lexus_ignored](https://docs.google.com/spreadsheets/d/1YJWXQ2VK6FuBlz6XrVM6R3Roq4FHtAmtJ6EByZqRHxQ/edit?usp=sharing), [Videos](https://purdue0-my.sharepoint.com/:f:/g/personal/yunsheng_purdue_edu/EoucJS393QFIvna7avg2u5YBOJgGr98rA3aouQc4uBb3Cw?email=chloe.2018.lgccccpc%40gmail.com&e=IzVTdf)

## Label Definitions
### List of maneuvers
0: Go Straight
1: Left Lane Change
2: Right Lane Change
3: Left Turn
4: Right Turn

### List of camera views
A: Forward-facing
B: In-cabin

## Annotation File Fields Definitions
- Video ID: An incremental 5-digit number that starts from 00000.
- Video file name (without .MP4).
- Camera View: A or B as defined in the List of Camera Views.
- Start Time (in seconds, >= 0): The start time of a lane change and turn is defined as the point at which the wheel touches the lane marking or the vehicle yaw at the intersection, respectively. The start time of going straight is defined as the point at which the vehicle starts moving.
- End Time (in seconds, <= 60): The end time of a lane change and turn is defined as the point at which the vehicle resumes going straight. The end time of going straight is defined as the point at which the lane change or turning starts or the vehicle stops.
- Maneuver Label: An integer label of the maneuver defined in the List of Maneuvers.
- Day/Night (Day or Night): Whether it is recorded during the day or night (can be told by whether the in-cabin camera is in infrared mode).

**If you have any questions, please send me an email. Thank you.**
