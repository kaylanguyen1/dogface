# **Finding a Person's Dog Breed Program**



## **Overview**

### **Project Objectives:**

- Using a live camera stream to compare a person's face with different dog breeds, ultimately matching them to the most similar face
- Compare by measuring and identifying different facial features like face height-to-width ratio, eye distance, nose height-to-width ratio, eye color, and skin color (fur color for a dog)



### **Tools and Technologies Used:**

- Written in Python on VSCode
- Uses a conda environment to ensure minimal interaction with user's previously installed libraries
- Python libraries: os, opencv, mediapipe



### **Things to Note Before/While Running:**

- Create the conda environment and install all of the Python libraries
- Ensure the device you're using has a webcam or other camera
- Ensure camera has ability to be accessed (can turn permission on while running cell 2)
- run each cell individually in order to ensure everything is working
- You can run each cell infividually by clicking the play button to the left of the cell or doing shift+enter on keyboard
- This program currently only detects one face at a time



## **How to Run:**

- Download or clone repository

    ```bash
    git clone https://github.com/kaylanguyen1/dogface.git
    ```

- Open in folder VSCode (or another application, although I've only ran it in VSCode)
- Open Command Line in application and navigate to root directory of main.ipynb
- Create conda environment

    ```bash
    conda create --dogs myenv
    ```

- Activate conda environment

    ```bash
    conda activate dogs
    ```

- Select the correct kernel by running the first cell to show you your current location vs. what you should be running
- Once using the correct kernel, install the additional Python libraries in the terminal

    ```bash
    pip install numpy==1.26.4 opencv-python==4.7.0.72 mediapipe==0.10.21
    ```


- Run cell 2 to ensure camera functionality and allow access to the camera if not already done
- Run cell 3 to fill the dog dictionary
- Run cell 4 to get the live camera stream comparing each face to a dog's face
- You can view the output in the command line of your application



### **Current Limitations:**

- Only a select few amount of dog breeds have been verified 
- Requires good/bright lighting since skin and eye color are analyzed for similarity



