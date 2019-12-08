### **36B Finch West - Finch Station**

Colab file to generate graphs: https://colab.research.google.com/drive/1w1z60YoJOD_x4EVJp-liVCIrGLfHF6qq


Data set: 'https://raw.githubusercontent.com/diluisi/Toronto36B/master/36B_FW_FS.csv'

**Start Date:** 2018-03-19

**Finish Date:** 2018-06-23

**Source:** AVL Data, GTFS File

### **Metadata**:

* **'Date_Key'** - day of collection *type:Date*

* **'Peak'** - 6:30-10:00 (AM peak) and 3:00-7:00 (PM peak) *type:string*

* **'StopSequence'** - Sequential number of each bus stop *type:int*

* **'DepartureStop'** - Name of the bus stop *type:string*

* **'DepartureStopNumber'** - bus stop ID AVL file

* **'ActualTime_DepartureStop'** - AAAA-MM-DD HH:MM:SS Actual Departure Time *type:int*

* **'ScheduledTime_DepartureStop'** - AAAA-MM-DD HH:MM:SS Schedule Departure Time  *type:DateTime*

* **'ScheduleAdherenceDeparture'** - ('ActualTime_DepartureStop' - 'ScheduledTime_DepartureStop') *type:int*

* **'ArrivalStop'** - Name of the bus stop *type:string*

* **'ArrivalStopNumber'** - bus stop ID AVL file *type:int*

* **'ActualTime_ArrivalStop'** - AAAA-MM-DD HH:MM:SS Actual Arrival Time *type:DateTime*

* **'ScheduledTime_ArrivalStop'** - AAAA-MM-DD HH:MM:SS Schedule Arrival Time *type:DateTime*

* **'ScheduleAdherenceArrival'** - ('ActualTime_ArrivalStop' - 'ScheduledTime_ArrivalStop') *type:int*

* **'ShapeDistance'** - Distance (km) from stop to stop *type:int*

* **'ShapeDistance_CC'** - Accumulated distance *type:float*

* **'link_id'** - FROM # bus stop TO # bus stop *type:int*

* **'ltt'** - link travel time *type:float*

* **'dayweek'** - 0 monday, 1 tuesday, 2 wednesday, 3 thursday, 4 friday, 5 saturday, 6 sunday *type:int*

* **'travel_id'** - trip sequence of the day *type:int*

* **'speed'** - 'ShapeDistance' / 'ltt' *type:float*

* **'seq'** - trip sequence (incremental) *type:int*

* **'hplanSchedule'** - 279s AM peak and 317s PM Peak. Based on TTC schedule from Finch West *type:int*

* **'headway'** - Difference between 'ActualTime_ArrivalStop' of two consecutive buses *type:float*

* **'bunch'** - binary if headway <= 0.5 headway scheduled *type:int*
