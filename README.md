Title: Supersense - Comparison between experienced and non experienced users
GROUP: AC
================
Description of contents:
PROJECT_AC - Our 3 pages long report and code at the end
Project.Rmd - Rmarkdown file that contains the code we used during our research
================
To reproduce our dataset:
1. Download "supersense_with_session_time" from Google Drive link https://drive.google.com/drive/u/1/folders/0APVXBpxX-CJqUk9PVA
2. Open Project.Rmd code file
3. Change line 89 (read.csv) path to the path where the data file is
4. Change line 114 to the path where the data is
5. Run all chunks in Project.Rmd
================
Link to github repository: https://github.com/avielbst/adv_programming_project/
================
# SISE2601 Project data description
================
Here we can see information about all columns that we used during our analysis (Not in the final model)
  * **event_date** - `char`Date in which the event happened (in our dataset we only have 2021-01-31).
  * **event_timestamp** - `dbl`Counts the micro seconds passed from 1970-01-01 to the event.
  * **event_name** - `char`Defines the specific action used (session_start, explore, explore_end, select_object_event, detection_success, speech_recognition, speech_event, find_useful)
  * **user_pseudo_id** - `dbl`Unique id of the user.
  * **mobile_brand_name** - `char`Mobile brand used to run Supersense application
  * **language** - `char`Language user used to control the application and the region he was in
  * **continent** - `char`Continent in which the user has been while activating the application
  * **country** - `char`Country in which the user has been while activating the application
  * **sub_continent** - `char`Sub-Continent in which the user has been while activating the application
  * **object** - `char`What object did the application try to find (from detection)
  * **answer** - `char`Users' answer ("Yes"/"No"/"No idea") to the question "Was the search useful"
  * **firebase_screen_class** - `char`Type of activity used by the user
  * **object_name** - `char`What object the application managed to find (result from detection)
  * **session_id** - `char`Unique id for every session (from when the app starts running until it closes)
  * **transcript** - `char`Vocal input that describes what the user is trying to find
  * **time.form.zero** - `dbl`Variable we created that holds timestamp-min(timestamp)
  * **experienced** - `char`User type. experienced if used 20 or more sessions
  * **session_length** - `dbl`Seconds passed from session start until it ended
  * **speak** - `char`The language the user is speaking (only 2 first letters of language column)