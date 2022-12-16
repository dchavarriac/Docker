# Webmin Docker
Webmin is a web-based interface for system administration for Unix. Using any modern web browser, you can setup user accounts, Apache, DNS, file sharing and much more. Webmin removes the need to manually edit Unix configuration files like /etc/passwd, and lets you manage a system from the console or remotely.
![header](https://user-images.githubusercontent.com/52936025/208161556-1e882dd9-b640-47d6-b6d8-c9fb13b01cbd.png)
# Docker Compose
<pre><font color="#33C7DE"><b>version</b></font><font color="#FFD7D7">:</font> <font color="#C061CB">&apos;3&apos;</font>
<font color="#33C7DE"><b>services</b></font><font color="#FFD7D7">:</font>
  <font color="#33C7DE"><b>webmin</b></font><font color="#FFD7D7">:</font>
    <font color="#33C7DE"><b>image</b></font><font color="#FFD7D7">:</font> dchavarriac/webmin
    <font color="#33C7DE"><b>container_name</b></font><font color="#FFD7D7">:</font> Webmin
    <font color="#33C7DE"><b>volumes</b></font><font color="#FFD7D7">:</font>
      <font color="#E9AD0C">- </font>webmin-vol:/media/storage
      <font color="#E9AD0C">- </font>webmin-vol:/data

    <font color="#33C7DE"><b>ports</b></font><font color="#FFD7D7">:</font>
      <font color="#E9AD0C">- </font><font color="#C061CB">&quot;10000:10000&quot;</font>
<font color="#33C7DE"><b>volumes</b></font><font color="#FFD7D7">:</font>
  <font color="#33C7DE"><b>webmin-vol</b></font><font color="#FFD7D7">:</font>
</pre>

#  Accessing the Web GUI Interface
<p>The container publsihes Webmin on all available IP addresses using port 10000</p>

<p>Browse to https://[Switch or Host IP Address&gt;]:10000 to get to the Web GUI interface.<br />
If you browse to the HTTP address it will re-direct you<br />
Default username and password are:<br />
Username: root<br />
Password: password</p>

# Versions
<ul>
	<li>Webmin&nbsp;2.010 released</li>
</ul>







      
                            

