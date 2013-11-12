---
layout: post
title: JavaBar prezentációk
date: 2013-11-12 16:42u
tags:
   - javabar
   - prezi 
---

Miközben mi már Antwerpenben készülünk a holnap induló Devoxxra (pontosabban University rész már két napja megy, holnap a konferencia kezdődik), szeretettel ajánljuk mindenki figyelmébe, hogy az eddigi JavaBar minden prezentációja elérhető a [meetup][javabar]os oldalról. (Kicsit el van dugva, a *Discussions* alatt van egy *Konzerv anyagok* szekció, ahol megtalálhatóak a linkek.) Például Varga Patrik legutolsó JavaEE7/Java8 [fóliái][patrik] is letölthetőek. Kíváncsian várjuk, hogy holnap délelőtt Mark Reinhold tud-e a Patrik után valami újat mondani a Java 8-ról ;-)

A prezentációk egyébként a legkülönbözőbb rendszerekkel készültek (impress.js, reveal, prezi, LibreOffice, ...). Az aktuális módszer a PDF konverzióra, hogy az egzotikusabb prezentációkból screenshotokat készítünk, és azt rakjuk be egy PDF-be. Emiatt kicsit pixeles lehet némelyik PDF, valamit a mérete is 20-30 Mbyte, viszont legalább PDF-ben terjeszthető. A screenshotokat linux alól készítjük, a ```watch -n 5``` parancs öt másodpercenként meghív egy scriptet, amiben a ```scrot``` készít egy screenshotot a ```beep``` pedig pittyen egyet jelezve, hogy lehet tovább lapozni. A kész képeket, pedig imagemagick-el méretezzük át és fűzzük össze PDF-be. Nem túl elegáns, de praktikus megoldás, ami például a prezi saját PDF exportjánál is hatékonyabbnak bizonyult...

[patrik]: http://dpc.hu/javabar/varga_patrik_javabar_java8_javaee7.pdf
[javabar]: http://www.meetup.com/bpjavabar/messages/boards/thread/282675421
