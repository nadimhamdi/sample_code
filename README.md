# sample_code

**Call_Center_Redirection_Frensh.Tar.Gz**

You will find in this file two python files ;the first that will be activate is the server.py to activate the app in your local machine and the second will be called by the first one to convert the speech into text.
then to test the app you need to send this :

curl -X POST -H "Content-Type: application/json" \ -d '{"voc":"path to the wave file","id":"abc","res":""}' \http://0.0.0.0:5080/  

*********************************************************

**Calling_An_Agent_Frensh_Arabic.Tar.Gz**

This file contain a speech recognition systeme, to activate the app you need to insert the command bellow
python SPEECH_comm.py
this app is based on GTTS and speech_recognition  library



*********************************************************

**Hand_Raiser_Recog.Tar.Gz**

to activate the app you run this command: python main.py
Note: you need to change cap = cv.VideoCapture(1) in line 32 in utils.py if you want to used your local camera (0) 

*********************************************************

**Qrcode.Tar.Gz**

it's an attendance system with facial recognition and QRcode scanner to activate run:
pythonguiQR4.py

you need to install pyzbar

first click on yes for chosing the camera and then start if you want to test it with your image the code is based on a simple DLIB for face recognition you must add this:

your_image = face_recognition.load_image_file("your_name.jpg")
your_face_encoding = face_recognition.face_encodings(your_image)[0]

and

known_face_encodings = [
                        meriam_face_encoding,
                        
                        your_face_encoding,

                        
                        
                        
                        ]
known_face_names = [
                    
                    "nadim_hamdi",
                    "your_name",
                    
                    
                    
                    ]

and

cap = cv2.VideoCapture(1) line 48 change it if you're using the local camera

