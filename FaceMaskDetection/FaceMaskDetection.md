In covid, mask is required in office. So to monitor wether persons are wearing the mas or not this project is developed.

In FaceMask_Detection_Video.ipynb:

detector function uses the Haar Cascade classifier, loaded from the "haarcascade_frontalface_default.xml" file, to detect faces in an input gray scale image (gray_image). 

Once faces are detected, the function draws rectangles around the detected faces and adds corresponding text based on whether the detected face is wearing a mask or not. 
                      
                      "faces = face_classifier.detectMultiScale(gray_scale, scaleFactor, minNeighbors)"

Choose a smaller scaleFactor (e.g., 1.05) to detect smaller faces or use the default value (1.1) for a balanced approach. Use larger values (e.g., 1.5) for faster processing but might miss smaller faces.

The minNeighbors parameter controls the quality of detected faces. Higher values (e.g., 3-6) result in fewer but higher-quality detections. For this case, minNeighbors=5 worked well for the image used.
