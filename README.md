# Local_IoT_Cloud_Server
Here I created a Local IoT Cloud Server using Flask(Python) which provides Read_API_Key and Write_API_Key for storing and retrieving data in real time. This project also provides an interface for every user to view the updates of their data in real time.

# How to run the project?
Download all files and folders of this project and place them to your desired folder. Open terminal and change your directory to that specific folder from terminal. Run the command: <b>python app.py</b> <br>
If you see something like below, It means the local IoT cloud server is running on the Localhost and available to your local network through the 2nd ip:port (http://192.168.0.100:5000). If it shows any error, install the libraries or dependencies by reading the message provided through your terminal. Then, run the same command again.  

<img width="678" alt="image" src="https://github.com/user-attachments/assets/f3fd1390-12d8-4571-8224-5f6005f8669e">

Now if you hit to the url <b>(http://192.168.0.100:5000/register)</b>, you will be navigated to the register page. Give a unique username, password, senosr count, sensor names and click Register button. You will get message whether your registration is successfull or not. 
