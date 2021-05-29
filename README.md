# FaceRecognitionBasedAttendanceSystem


  Blockdiagram:
  



  
![Capture](https://user-images.githubusercontent.com/55623365/120057860-37c74180-c064-11eb-9946-333f9126652f.JPG)

  
  
  
  
  
  
	Figure: Proposed system  
The block diagram in figure describes the proposed system for Face Recognition based Classroom attendance system. The system requires a camera installed in the classroom at a position where it could capture all the students in the classroom and thus capture their images effectively. This image is processed to get the desired results. The working is explained in brief below:
• Capturing Camera: Camera is installed in a classroom to capture the face of the student. The camera has to be places such that it captures the face of all the 
students effectively. This camera has to be interfaced to computer system for further processing either through a wired or a wireless network. In our prototype we use the in-built camera of the laptop.
 • Image Processing: Facial recognition algorithm is applied on the captured image. The image is cropped and stored for processing. The module recognizes the images of the students face which have been registered manually with their names and ID codes in the database. The whole process requires the following steps:
 a) Train Database: Initially we take facial image of the enrolled students. In our system we have taken three images each. This data is used later used in the facial recognition algorithm. All the cropped image of the face is resized. 
b) Face Detection and cropping: The captured image of the classroom is initially scanned to detect faces. The detected faces are cropped and resized , same as the train database.
 c) Face Recognition: For recognition the feature locations are refined and the face is normalized with eyes and month in fixed locations. Images from the face tracker are used to train a frontal Eigen space, and the leading three eigenvectors are retained. Since the face images have been warped into frontal views a single eigen space is enough. Face recognition 
is then performed using the Eigen face approach with additional temporal information added. The projection coefficients of all images of each person are modelled as a Gaussian distribution and the face is classified based on the probability of match.
 d) Attendance Recording: We use Excel spreadsheet to store the recorded attendance for easy-to-use output format, which is also the software which is familiar to majority of the institution staffs. This is done using Spreadsheet Link EX toolbox. If a student is recognized, the corresponding cell is updated with ‘1’, else a ‘0’. Using the formatting in the Excel, we can effectively retrieve the information effectively.

