# FACIAL RECOGNITION BASED AUTHENTICATION AND ATTENDANCE SYSTEM

Face recognition is one of the mostly used biometrics. It can be used for security, authentication, identification, and has many more advantages. Face recognition systems can be used for taking attendance in schools, colleges, offices, etc. In the base paper we chose, the author has created a facial recognition-based attendance system where a student’s face coordinates are stored in a database and the image in the ID card is scanned for attendance. If his/her coordinates match with the ones stored in the database, then the attendance list gets updated. Although this reduces the chances of proxy attendance, this does not completely eliminate the proxy factor as a student might show another student’s ID card and the face recognised in the ID might match the coordinates in the database and the attendance can get updated. So, we enhance the system by doing an authentication where we scan the face and if the coordinates match the ones in the database, the attendance list gets updated, else it is discarded. So, there is no possibility of someone else trying to give attendance to another individual. This completely eliminates the possibility of proxy and enhances the system reliability.


## Experimental Setup

### Software:
• OpenCV
• Dlib
• Numpy

### Hardware:
• Web camera

## Methodology

For face detection, it is essential that the faces are identified by the system based on certain criteria. The criteria followed by humans for identification is not the same as the one used by computers. Therefore, setting up the criteria is another important feature to be included. And then based on the set criteria the face must be identified with the images already stored in the system. To include all of these features, different algorithms have been used which are explained below.

### Histogram of Oriented Gradients
HOG is a feature descriptor which helps in object detection in image processing. In the project, the image is converted into black and white and each and every pixel and the surrounding pixels are analyzed. The darkness of the pixel is figured out and an arrow is used to represent the direction of increase of darkness. Performing this process for each and every pixel, gives us gradients. The image is then analyzed based on the direction of the gradient turning the image into a simpler representation of the face. The pattern created is known as HOG pattern and it helps us compare an image with it and find the most similar one.

### Face Landmark Estimation
Face Landmark Estimation helps in identifying key points on the face, such as tip of the nose, center of the eye etc. In the project, the landmarks on the face are identified. Then a machine learning algorithm is used to identify these landmarks in all the faces. It allows the image to be rotated in any direction and still be identified.

