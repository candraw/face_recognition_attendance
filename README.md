# face_recognition_attendance
This program was made for my final project at my college, this program will detect some faces in realtime video processing on a raspberry pi device that has a webcam installed and will save it into a csv file and then send it via telegram bot

# This project consists of 4 programs

# Face_record.py
serves to capture face samples 30 times in a grayscale image and will be stored in the /dataset folder. The photos that have been collected will be used as material for making datasets. To distinguish one face from another face, id is used.

# Face_training.py
serves to create a dataset file in .yml format which will be named train.yml. This creation is sourced from the results of facial images that have been previously captured by the Face_record.py program.

# Face_attendance.py 
Serves to detect faces from the train.yml dataset file that has been created by the Face_training.py program. When a previously registered face is detected, the program will automatically add attendance data to the column in the report_attendance.csv file.

# Bot_attendanceReport.py 
function to send file report_attendance.csv via telegram.
