## Vision Text
The Vision Text (Text detector) application is designed to capture images using the device's camera and then extract text from those images using machine learning models provided by Google's ML Kit.
 
The application primarily consists of two activities: MainActivity and ScannerActivity. 
#### MainActivity: 
- This activity serves as the entry point of the application. 
- It displays a welcome message along with a brief description of the application. 
- It contains a button ("Capture Image") that directs the user to the ScannerActivity when clicked. 
#### ScannerActivity: 
- This activity handles the capturing of images and the detection of text. 
- It displays the captured image and provides buttons for image capture ("Snap") and text detection ("Detect"). 
- When the "Snap" button is clicked, the application requests camera permissions if not granted already and captures an image using the device's camera. 
- Upon successfully capturing an image, the image is displayed in an ImageView. 
- When the "Detect" button is clicked, the application processes the captured image to 
extract text using Google's ML Kit Text Recognition API. 
- Detected text is displayed in a TextView below the captured image.
#### Permissions: 
- The application requests camera permissions from the user to allow image capture.
- It also requires internet permission for ML Kit operations. 
#### ML Kit Integration: 
- The application integrates Google's ML Kit library for text recognition. 
- It uses TextRecognizer to process images and extract text from them. 
- Detected text is then displayed to the user in the ScannerActivity. 
#### UI Design: 
- The UI design of both activities is implemented using XML layout files.
- RelativeLayout is used for positioning UI elements within the activities.
- Colors are defined in a separate XML file for consistency and ease of maintenance. 
#### Gradle Configuration: 
- The project's Gradle file includes necessary dependencies for ML Kit text recognition, Firebase core, and other required libraries.

###  Screenshots :
<details>
     <summary> Click to expand </summary>
  
   Main Screen               | Functions Screen           |  Capturing Image through camera     
:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/Apoorva57/VisionText/assets/97695341/e52442ed-9b3d-4e89-8cea-8ccd222caefc)|![](https://github.com/Apoorva57/VisionText/assets/97695341/f10896f7-d491-4ebc-859d-76f1ad61b899)|![](https://github.com/Apoorva57/VisionText/assets/97695341/92c72c7a-bd1c-4870-ae74-86a4a2ae1708)|

   Confirming Image          | Image Displayed in App     |  Output    
:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/Apoorva57/VisionText/assets/97695341/216b15ee-5576-4b11-92d3-96243cec42ea)|![](https://github.com/Apoorva57/VisionText/assets/97695341/1772e858-6f8d-4d48-9188-ca6c257525ab)|![](https://github.com/Apoorva57/VisionText/assets/97695341/636b28cc-4b7f-458f-a592-d1fa443a3cf0)|
  
</details>

### Application video
https://drive.google.com/file/d/1no1gFHBkmdayGgRNGsebtzliPQDpSuPa/view

### Apk file
https://drive.google.com/file/d/1VxQqkwbQmTumElswjRrvUzw22uBOP1u_/view?usp=shari
