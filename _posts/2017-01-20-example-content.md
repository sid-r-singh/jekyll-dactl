---
layout: post
title: How to install LAMP on Debian

tags:
  - lamp
  - linux
description: >
  LAMP ဆိုတာကေတာ့ Linux, Apache, MySQL, and PHP ပဲျဖစ္ပါတယ္။ LAMP ကေတာ့ open source web development platform အတြက္ျဖစ္ျပီးေတာ့ Linux Operation system ေပါ္မွာ Apache Web Server,MySQL Data management system,PHP object-oriented scripting language ေပါင္းစည္းျပီးအသံုးျပုထားတာပဲျဖစ္ပါတယ္။တစ္ခါတေလမွာ Perl or Python တို့ကိုလည္းအသံုးျပုတက္ျကပါသည္
hero: https://images.unsplash.com/photo-1518432031352-d6fc5c10da5a
overlay: green
published: true
---

LAMP ဆိုတာကေတာ့ Linux, Apache, MySQL, and PHP ပဲျဖစ္ပါတယ္။ LAMP ကေတာ့ open source web development platform အတြက္ျဖစ္ျပီးေတာ့ Linux Operation system ေပါ္မွာ Apache Web Server,MySQL Data management system,PHP object-oriented scripting language ေပါင္းစည္းျပီးအသံုးျပုထားတာပဲျဖစ္ပါတယ္။တစ္ခါတေလမွာ Perl or Python တို့ကိုလည္းအသံုးျပုတက္ျကပါသည္

က်ေနာ္တို့Linux မွာမ်ုိးကဲြေတြအမ်ားျကီးရွိပါတယ္။အကုန္လံုးမွာတင္နည္းကို က်ေနာ္ေျပာျပေနရင္ ျကာသြားမွာဆိုးလို့ လူသံုးမ်ားတဲ့ Debian OS ေပါ္ပဲမူတည္ျပီးေျပာျပေပးပါ့မယ္။

ဒီနည္းအတိုင္းတျခား Debian အနြယ္၀င္ေတြျဖစ္တဲ့ Kali Linux,Ubuntu,Linux mint,backbox,etc.. အစ ရွိသည္ေတြမွာသြင္းနိုင္ပါသည္။အခုသြင္းမယ့္နည္းေတြအကုန္လံုးက command line ကေနပဲသြင္းသြားမွာပါ။

အရင္ဆံုးက်ေနာ္တို့ရဲ့စက္ကို update တစ္ခ်က္လုပ္ေပးပါ။

(/assets/lamp1.png)

apt-get update

ေနာက္တစ္ဆင့္မွာက်ေနာ္တို့ apache web server ကို install လုပ္ေပးပါမယ္။

apt-get install apache2

MySQL database ကို install လုပ္ပါမည္။

apt-get install mysql-server

mysql server install လုပ္ေနခ်ိန္တြင္ mysql password ေပးခိုင္းပါလိမ့္မည္။မိမိတို့ အသံုးျပုမည့္ password ထည့္ေပးလိုက္ပါ။


က်ေနာ္တို့အသံုးျပုမည့္ MySQL ပိုမိုလံုျခံုေစရန္ secure installation လုပ္ေပးရန္လိုပါသည္။command line မွရိုက္ေပးလိုက္ပါ။

mysql_secure_installation

Change the root password? [Y/n] n
 Remove anonymous users? [Y/n] Y
 Disallow root login remotely? [Y/n] Y
 Remove test database and access to it? [Y/n] Y
 Reload privilege tables now? [Y/n] Y

အေပါ္ကအဆင့္ေတြအတိုင္းေရြးေပးလိုက္ပါ။password ေတာင္းရင္က်ေနာ္တို့အေပါ္မွာေပးခဲ့တဲ့ mysql password ကိုျပန္ရိုက္ေပး လိုက္ပါ။

က်ေနာ္တို့ apache,mysql သြင္းျပီးသြားရင္ php ကိုက်ေနာ္ဆက္လက္ install ျပုလုပ္ပါမည္။php5 ကိုပဲ က်ေနာ္ install လုပ္ျပသြားပါမည္။

apt-get install php5 php-pear php5-mysql

က်ေနာ္တို့ apache,mysql,php စတာေတြကိုအကုန္ install လုပ္ျပီးသြားပါျပီ။Server မွာ apache service ေတြအလုပ္မလုပ္သိဖို့အတြက္ apache ကို restart ခ်ျကည့္လိုက္ပါ။command line ကေန run ေပးပါ။

service apache2 restart
browser ကေန မိမိရဲ့ vps ip သို့မဟုတ္ local မွာ install လုပ္တာဆိုရင္ localhost စသည္ျဖင့္ ေခါ္ျပီးျကည့္နိုင္ပါသည္။


LAMP သြင္းရာတြင္အခက္အခဲမ်ားရွိပါက က်ေနာ္ ရဲ့ Facebook Page ကေနတစ္ဆင့္ဆက္သြယ္ေမးျမန္းနိုင္ပါသည္။
