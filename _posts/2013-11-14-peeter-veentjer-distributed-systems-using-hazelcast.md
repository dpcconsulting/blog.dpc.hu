---
layout: post
title: "Peeter Veentjer: Distributed Systems using Hazelcast"
date: 2013-11-14 10:53
tags: 
   - devoxx
   - hazelcast
   - nosql
---
	
Egyszer indítani fogok egy olyan sorozatot, ahol a szépen megmunkált Java librarykról fogok írni. Mindig öröm olyan alkalmazással találkozni, amin látszik a gondos kezek munkája. A Hazelcast, amit szintén régóta kerülgetek már, pont ilyen. Kicsi, egyetlen Jar file, egyszerű api, okos defaultok, és jól lehet hangolni nagyon sok részletét. Mintha olyan fejlesztők gondoznák akik használják is.

Maga a Hazelcast a NoSQL világ datagrid osztályához tartozik, ahol pl. a Gigaspaces vagy a Coherence is versenyez. Csak ez Open Source és ingyenes (support elérhető). Aki nem látott még ilyet az leginkább egy nagyon elosztott ConcurrentHashMap-re kell, hogy gondoljon. Meg persze emellett még BlockingQueue-ra, Topic/Subscriber-re, valamint bármilyen saját adatszerkezetre (ugye szépen kiterjeszthető). 

<a href="http://www.flickr.com/photos/108542198@N03/10852431703/" title="Untitled by dpcconsultingltd, on Flickr"><img src="http://farm3.staticflickr.com/2882/10852431703_bfb1c56b88.jpg" width="500" height="375" alt="Untitled"></a>

Mindez nagyon sok ügyes extrával:

* Lehet állítani a backupok számát. 
* Lehet kérni külső rendszerbe való perzisztálást. 
* Hangolható, hogy egy művelethez szükséges adatok egy helyen legyenek. 
* Lecserélhető a szerializáció (Protobuf, Kryo, bármi),
* Lehet futtatni kódot a megfelelő node-okon. (Ahelyett, hogy kiszedjük az adatot, műveletet végzünk, vissza tesszük, a művelet kódját küldjök az adathoz.)
* Multicast és TCP autodiscovery.

Nem véletlen, hogy sok Open Source pojekt használja a felszín alatt.

<a href="http://www.flickr.com/photos/108542198@N03/10852250294/" title="Untitled by dpcconsultingltd, on Flickr"><img src="http://farm6.staticflickr.com/5548/10852250294_14ca3ae1e9.jpg" width="500" height="375" alt="Untitled"></a>

