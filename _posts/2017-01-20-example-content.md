---
layout: post
title: How to install LAMP on Debian

tags:
  - lamp
  - linux
description: >
  LAMP Linux, Apache, MySQL, and PHP Apache Web Server,MySQL Data management system,PHP object-oriented scripting language
hero: https://images.unsplash.com/photo-1518432031352-d6fc5c10da5a
overlay: green
published: true
---

quis ipsa consequuntur iure atque! Necessitatibus quam quidem illum, corrupti molestiae, maxime neque, consequuntur quia alias, modi commodi.Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cupiditate rem ducimus dolores repellat itaque perferendis corporis ex dicta doloremque optio harum excepturi, ut, praesentium asperiores! Voluptatum amet perspiciatis iusto, fugiat!Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum, libero quia placeat necessitatibus culpa mollitia, illum, quam sed ratione ad eaque suscipit consectetur itaque quasi aperiam. Quaerat, nihil voluptas tenetur?Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos unde quam autem fugit, aliquam perspiciatis, accusamus numquam, pariatur impedit excepturi debitis repellendus consectetur laboriosam voluptatem temporibus su

(/assets/img/lamp1.png)

apt-get update

ေနာက္တစ္ဆင့္မွာက်ေနာ္တို့ apache web server ကို install လုပ္ေပးပါမယ္။

apt-get install apache2

(/assets/img/lamp2.png)

MySQL database ကို install လုပ္ပါမည္။

apt-get install mysql-server

(/assets/img/lamp3.png)

mysql server install လုပ္ေနခ်ိန္တြင္ mysql password ေပးခိုင္းပါလိမ့္မည္။မိမိတို့ အသံုးျပုမည့္ password ထည့္ေပးလိုက္ပါ။

(/assets/img/lamp4.png)

က်ေနာ္တို့အသံုးျပုမည့္ MySQL ပိုမိုလံုျခံုေစရန္ secure installation လုပ္ေပးရန္လိုပါသည္။command line မွရိုက္ေပးလိုက္ပါ။

mysql_secure_installation

(/assets/img/lamp5.png)

Change the root password? [Y/n] n
 Remove anonymous users? [Y/n] Y
 Disallow root login remotely? [Y/n] Y
 Remove test database and access to it? [Y/n] Y
 Reload privilege tables now? [Y/n] Y

အေပါ္ကအဆင့္ေတြအတိုင္းေရြးေပးလိုက္ပါ။password ေတာင္းရင္က်ေနာ္တို့အေပါ္မွာေပးခဲ့တဲ့ mysql password ကိုျပန္ရိုက္ေပး လိုက္ပါ။

က်ေနာ္တို့ apache,mysql သြင္းျပီးသြားရင္ php ကိုက်ေနာ္ဆက္လက္ install ျပုလုပ္ပါမည္။php5 ကိုပဲ က်ေနာ္ install လုပ္ျပသြားပါမည္။

apt-get install php5 php-pear php5-mysql

(/assets/img/lamp6.png)

က်ေနာ္တို့ apache,mysql,php စတာေတြကိုအကုန္ install လုပ္ျပီးသြားပါျပီ။Server မွာ apache service ေတြအလုပ္မလုပ္သိဖို့အတြက္ apache ကို restart ခ်ျကည့္လိုက္ပါ။command line ကေန run ေပးပါ။

service apache2 restart
browser ကေန မိမိရဲ့ vps ip သို့မဟုတ္ local မွာ install လုပ္တာဆိုရင္ localhost စသည္ျဖင့္ ေခါ္ျပီးျကည့္နိုင္ပါသည္။

(/assets/img/lamp7.png)


LAMP သြင္းရာတြင္အခက္အခဲမ်ားရွိပါက က်ေနာ္ ရဲ့ Facebook Page ကေနတစ္ဆင့္ဆက္သြယ္ေမးျမန္းနိုင္ပါသည္။
