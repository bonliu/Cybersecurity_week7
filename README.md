# Cybersecurity_week7
<br />
<b>Task:</b> Exploat vulnerability of old version WordPress.<br />

<b>Vulnerability 1</b><br />
[!] Title: WordPress <= 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS)<br />
    Reference: https://wpvulndb.com/vulnerabilities/7945<br />
    Reference: http://klikki.fi/adv/wordpress2.html<br />
    Reference: http://packetstormsecurity.com/files/131644/<br />
    Reference: https://www.exploit-db.com/exploits/36844/<br />
[i] Fixed in: 4.2.1<br />
<br />
  >Steps:<br />
  >  - login to http://wpdistillery.vm/ as admin with credential provided in config.yml<br />
  >  - Install and activate theme TwentyFifteen<br />
  >  - Install and activate Genericon'd Plugin<br />
  >  - Go to content/themes/twentyfifteen/genericons/example.html<br />
  >  - modify url to <br />
  >    http://wpdistillery.vm/wp-content/themes/twentyfifteen/genericons/example.html#1<img/ src=1 onerror=alert("HACKED")>sdf<br />

<b>GIF walkthrough:</b><br />
![genericonxss](https://user-images.githubusercontent.com/31838335/38178052-70db0200-35d8-11e8-9df4-840ce02b2451.gif)
