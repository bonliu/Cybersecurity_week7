# Cybersecurity_week7
<br />
<b>Task:</b> Exploat vulnerability of old version WordPress.
<br /><br />
<b>Vulnerability 1</b><br />
![genericonxss](https://user-images.githubusercontent.com/31838335/38178297-a4c3e9ce-35dd-11e8-9155-3505d0a9950b.PNG)
<br />
  Steps:<br />
    - login to http://wpdistillery.vm/ as admin with credential provided in config.yml<br />
    - Install and activate theme TwentyFifteen<br />
    - Install and activate Genericon'd Plugin<br />
    - Go to content/themes/twentyfifteen/genericons/example.html<br />
    - modify url to <br />
      http://wpdistillery.vm/wp-content/themes/twentyfifteen/genericons/example.html#1<img/ src=1 onerror=alert("HACKED")>sdf<br />

<b>GIF walkthrough:</b><br />
![genericonxss](https://user-images.githubusercontent.com/31838335/38178052-70db0200-35d8-11e8-9df4-840ce02b2451.gif)

<br />
<b>Vulnerability 2</b><br />
![xss1](https://user-images.githubusercontent.com/31838335/38178301-b8ecc164-35dd-11e8-9162-f4b539fa6093.PNG)
<br />
  Steps:<br />
    - Go to http://wpdistillery.vm/ as admin <br />
    - Go to one of the post and put crafted malicious code in the comment <br />
    - post comment <br />

<b>GIF walkthrough:</b><br />
![xss1](https://user-images.githubusercontent.com/31838335/38178228-33f0004e-35dc-11e8-9764-6d91a88c7902.gif)



