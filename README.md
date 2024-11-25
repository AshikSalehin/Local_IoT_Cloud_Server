# Local_IoT_Cloud_Server
Here I created a Local IoT Cloud Server using Flask(Python) which provides Read_API_Key and Write_API_Key for storing and retrieving data in real time. This project also provides an interface for every user to view the updates of their data in real time.

# How to run the project?
Download all files and folders of this project and place them to your desired folder. Open terminal and change your directory to that specific folder from terminal. Run the command: <b>python app.py</b> <br>
If you see something like below, It means the local IoT cloud server is running on the Localhost and available to your local network through the 2nd ip:port (http://192.168.0.100:5000). If it shows any error, install the libraries or dependencies by reading the message provided through your terminal. Then, run the same command again.  

<img width="678" alt="image" src="https://github.com/user-attachments/assets/f3fd1390-12d8-4571-8224-5f6005f8669e">


Now if you hit to the url <b>(http://192.168.0.100:5000/register)</b>, you will be navigated to the register page. Give a unique username, password, senosr count, sensor names and click Register button [N.B: Replace the ip with your local ip shown in the terminal]. You will get message whether your registration is successfull or not. 

<img width="1414" alt="image" src="https://github.com/user-attachments/assets/211717ca-1813-4eba-a9bc-6f1cddc6a64c">


After Registration, navigate to Login page (http://192.168.0.100:5000/login). Login with your username and password. 

<img width="1423" alt="image" src="https://github.com/user-attachments/assets/7fbf5bef-8c47-4148-ad0b-5cacb82e122b">


After login, you will be navigated to your profile page. Here, you will find read and write API keys. 


<img width="1055" alt="image" src="https://github.com/user-attachments/assets/c00dab33-f3f3-4ef5-9dce-5bcd351b7c6d">


Send HTTP GET request through the write API key modifying the values of argument part of the API key and pasting it to the url field of your browser. For example:  .......:5000?S1=<YOUR_DESIRED_VALUE>&S2=<YOUR_DESIRED_VALUE>&S3=<YOUR_DESIRED_VALUE>. 

<img width="1420" alt="image" src="https://github.com/user-attachments/assets/9f7e7635-2b58-40b4-b205-318843e80d8b">


You will be able to see the updated of data in real time from your profile page. In this way, you can feed data to the server using the write API key. You also can send HTTP GET request to the write API key from any other device and any other programming languate to feed data from the same network. 

<br><br>
Now, if you want to read data from other devices connected to the same network, you have to copy the read API key from your profile page and specify how many recent enteries you want to read by changing the value of <b>n</b> at the end of the API key: <br>


<img width="1427" alt="image" src="https://github.com/user-attachments/assets/58eadd60-e2d8-48da-b8e3-a9604222f75c">
<br>
<img width="1435" alt="image" src="https://github.com/user-attachments/assets/16246dfa-aa52-4fe9-bd2b-1af9be1cd5e8">
<br>
<img width="1512" alt="image" src="https://github.com/user-attachments/assets/224ed7a5-44de-4256-a223-343fcd2f05f1">
<br><br>
# Features of this Project: <br>
&nbsp; 1. Using a Text file (.txt) to store username and password.<br>
&nbsp; 2. Using an excel file to store the sensor values.<br>
&nbsp; 3. When a user registers, a new tab is created to the excel file with the same title as username. Given sensor names ared added to that particular tab as columns. <br>
&nbsp; 4. Usernames must have to be unique.<br>
&nbsp; 5. When someone hits Write API key, data are feed to the particular tab of that user and stored to the columns titled by the sensor names to the excel file. <br>


# Conclusion:
For any further information, contact me through <b>ashiqussalehin0001@bdu.ac.bd</b>.


