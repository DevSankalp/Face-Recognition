<h1 align=center> Face Recognition Login System </h1>
<hr/>
<h4 align="center"> :camera: A facial recognition based login system using Python,HTML,CSS and Bootstrap 
</h4>
<hr/>
<h2> Tools & Libraries Used </h2>
<hr/>
<ul>
  <b>
<li> Python - https://www.python.org/ </li>  
<li> XAMPP - https://www.apachefriends.org/download.html </li>
<li> Tailwind CSS - https://tailwindcss.com/ </li>
<li> Daisy UI - https://daisyui.com/ </li>    
<li> CGI </li>
    
  </b>
</ul>
<strong> Note </strong>  - These files must be hosted on XAMPP Apache server or other server, else login.py will not work.

<hr/>
<h2> Working </h2>

- Install Python
- Install XAMPP
- Navigate to `htdocs` folder and clone this project.
- Open `login.py` and make sure to replace the top comment `#! C:\Python39\python.exe` with your python path.
- Navigate to `htdocs/Face-Recognition` and execute the following command `pip install -r requirements.txt`
- Navigate to `xampp/apache/config` and modify the `httpd.conf` file by adding

```conf
Options Indexes FollowSymLinks Includes ExecCGI
AddHandler cgi-script .py .cgi .pl .asp
```

at the end of the file. Then save & exit
- Then run XAMPP & go to `localhost/Face-Recognition/index.html`
 <img src='Preview/n2.png'><br>
<hr/>

<h2> Making it work for Windows </h2>
<p>
Go to the python's installed location and right click on the 
python39 folder and go to security tab and give "Full Control" permission to users
</p>
</br/>
<p>
And then go the scripts folder in python's installed path
(C:\Python39\Scripts)
</p>
and run the below commands in that folder 
<br/>

Command 1 : `C:\python39\python.exe -m pip install --upgrade pip --user`

In the above command replace the exe path with your path

Comand 2 : `pip install cmake --ignore-installed`

Command 3 : `pip install dlib --ignore-installed`

Command 4 : `pip install face_recognition --ignore-installed`

Then try to restart the XAMPP Server it should work.

If it did not work, try installing below tools on windows
- CMAKE
- Visual Studio with CMAKE Build tools installed

Also to for debugging, ensure to check Apache Error Logs
![image](https://user-images.githubusercontent.com/36433104/155829373-9b1482f4-f657-4f85-ae76-ff20bcccb2eb.png)
