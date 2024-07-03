**Step 1) Install the apache2 package**
```
sudo apt-get update\
sudo apt-get install apache2 -y 

```

**Step 2) Make sure the service is active by running the command** 
```
systemctl status apache2.service

```

**Output:-**

aws\@aws:\~$ **systemctl status apache2.service** 

● apache2.service - The Apache HTTP Server

     Loaded: loaded (/lib/systemd/system/apache2.service; enabled; vendor preset: enabled)

     Active: active (running) since Wed 2024-07-03 15:05:58 IST; 19s ago

       Docs: https\://httpd.apache.org/docs/2.4/

   Main PID: 23988 (apache2)

      Tasks: 55 (limit: 9282)

     Memory: 5.4M

        CPU: 38ms

     CGroup: /system.slice/apache2.service

             ├─23988 /usr/sbin/apache2 -k start

             ├─23989 /usr/sbin/apache2 -k start

             └─23991 /usr/sbin/apache2 -k start

Jul 03 15:05:58 aws systemd\[1]: Starting The Apache HTTP Server...

Jul 03 15:05:58 aws apachectl\[23987]: AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 1>

Jul 03 15:05:58 aws systemd\[1]: Started The Apache HTTP Server.

**Step 3) Checked the port on which apache2 running with below command** 

**Output:-**

aws\@aws:\~$ **netstat -tulnp | grep 80**

tcp6       0      0 :::80                   :::\*                    LISTEN      -  

**Check with the command apache2 running fine or not**
```
curl -l localhost:80

```

**To check the default url enter it into your browser’s address bar**

http\://localhost:80![](https://lh7-us.googleusercontent.com/docsz/AD_4nXf84dvmNPv19nsFx10FXsUb07uOgzt2TNpFU-qcoVwyhCjOs4DCG8d_AiFX98M_v3cuQOoNq1e8ZNVDK-kSevQDTH_RoXqENadyxOVKlsRCokZA5TpLGg92pmv4-fFcpxv8xjjLUiMnPWgt2mTySS-TuXPJ?key=DvDc7us21QKZqg3Pu5lL6A)

