# Color Detection model

- This Python script allows you to detect the name of a color in an image by clicking on a specific pixel. The model uses the OpenCV library and a pre-defined dataset of color names to accurately identify the color.

## Steps
-- The script loads the necessary libraries, including pandas for data manipulation and OpenCV (cv2) for image processing.   
-- Set the path to the image you want to analyze by assigning the imageUrl variable.   
-- The color names dataset is loaded from a CSV file using pandas.    
-- The dataset contains information about various colors, including their RGB values.   
-- The image specified in imageUrl is read using the cv2.imread() function and stored in the image variable.   
-- The getColorName() function is defined, which takes RGB values as input and returns the closest matching color name from the dataset.   
-- The draw_function() function is defined to handle mouse events. When a double-click event occurs, it retrieves the RGB values of the clicked pixel and assigns them to the respective variables.   
-- The main loop starts, where the script waits for a mouse event to occur. Once a double-click event is detected, it draws a rectangle on the image with the color of the clicked pixel.    
-- The script calls the getColorName() function to determine the name of the selected color and displays it on the image.   
-- The script checks the brightness of the color and adjusts the text color accordingly for better visibility.   
-- The image with the color name is displayed using cv2.imshow(), and the loop continues until the user presses the 'esc' key.   
-- When the loop is exited, all windows are closed using cv2.destroyAllWindows().  

## How to Run the Code
Ensure that you have Python installed on your system.   
Install the required libraries by running the following command:   
Copy code   
pip install pandas opencv-python   
Save the code in a Python file, for example, color_detection.py.   
Set the imageUrl variable to the path of the image you want to analyze.   
Open a terminal or command prompt and navigate to the directory where the Python file is saved.   
Run the script using the following command:   
Copy code   
python color_detection.py   
Click on a pixel in the displayed image to detect the corresponding color name.   
Press the 'esc' key to exit the program.   
How to Use the Model   
Run the script as described above.   
An image window will appear displaying the selected image.   
Double-click on any pixel in the image to detect the color name of that pixel.   
The color name will be displayed on the image.   
Repeat the process by double-clicking on different pixels to identify their colors.   
To exit the program, press the 'esc' key.  

## Uses of this Model   
Color identification: This model can be used to identify colors in images, which can be beneficial for tasks like image processing, object recognition, and computer vision applications.   
Design and branding: Designers and marketers can utilize this model to extract color information from images and use it for creating appealing visuals, choosing color schemes, or analyzing color trends.   
Educational purposes: This model can serve as a useful tool for teaching color theory, computer vision, and image processing concepts.   
Accessibility: The color detection feature can assist individuals with color vision deficiencies in identifying colors accurately.   

## Technology Used 
#### Python: 
The programming language used to develop the color detection model. Python is widely used for its simplicity, versatility, and extensive libraries for various applications.   
#### OpenCV (cv2): 
OpenCV is a powerful open-source computer vision library that provides a wide range of functions and algorithms for image and video processing. In this model, OpenCV is utilized for reading images, handling mouse events, drawing rectangles, and displaying images.
#### Pandas: 
Pandas is a popular data manipulation library in Python that provides data structures and functions for efficient data analysis. In this model, Pandas is employed to load the color names dataset from a CSV file, manipulate the data, and retrieve the closest matching color name based on RGB values.
## Conclusion
The color detection model presented here is a simple yet effective solution for identifying colors in images. By leveraging the power of Python, OpenCV, and Pandas, the model allows users to interactively select a pixel in an image and obtain the corresponding color name. Whether for practical applications like image processing or for educational purposes, this model provides a useful tool for color analysis. Feel free to use and modify the code according to your needs, and enjoy exploring the world of colors with this color detection model.
