---
layout: post
title:  "Introducere în C++ pentru GIS"
subtitle: "<a href='http://www.geo-spatial.org/osgeo'>Seminariile geo-spațial.org, București</a>"
categories: seminar
permalink: cpp
---

Pregătirea mediului de lucru
===========
Pentru utilizatorii de Linux:
   Instalați [gcc][gcc_url] și [Geany][geany_url] din depozite.
   
Pentru utilizatorii de Windows: vom folosi programele menționate sub 
[x/cygwin][xcyg_url]. Pentru aceasta, descărcați [installer-ul cygwin][cyginst_url] și instalați-l cu opțiunile implicite, **în afară de**:
   
   + selectarea unui sit _mirror_: alegeți un sit dintr-o țară apropiată (de exemplu Germania - se alege după extensia .de a adresei);
   
   ![](/assets/ps_cysetup_mirrorsel.png)
   
   + selectarea pachetelor: alegeți pentru instalare `gcc-core`, `gcc-g++`, `xorg-server`, `xinit` și `geany`. Dacă întîmpinați dificultăți, urmăriți instrucțiunile detaliate de [aici][cyginst_tutor].
   
   ![](/assets/ps_cysetup_packsel.png)
   
După instalare, lansați `XWin Server` din meniul de start. 

![](/assets/ps_xwinserver_start.png)

După lansare, în _taskbar_ sînt vizibile două pictograme noi. Faceți clic pe cea cu titlul `X Applications Menu on :0` și selectați `Programming >> Geany`.

![](/assets/ps_xappmenu.png)

Din acest punct instrucțiunile sînt comune pentru toți utilizatorii.

Aplicația 0: "Hello World!"
=============
Aproape toate tutorialele de programare încep cu un prim program denumit `HelloWorld`. Vom proceda la fel, deoarece acest program vă permite să testați instalarea mediului de lucru. Pentru moment, doar executați pașii de mai jos. De-a lungul seminarului vom avea ocazia să discutăm toate detaliile din cod, și multe altele.

   + În Geany creați un fișier text nou, pe care îl salvalți cu denumirea `HelloWorld.cpp` (calea este relativă la `C:\cygwin64\home`).
   + În acest fișier introduceți următorele linii de cod:
{% highlight c %}
#include <iostream>

int main void(){
   std::cout << "Hello world!";
   
   return 0;
}
{% endhighlight %}

   + Salvați fișierul și executați, din _toolbar_-ul Geany, `Build` și `Execute`.
   ![](/assets/ps_geany_compile-build-execute.png)
   + După execuție, apariția mesajului "Hello world!" ca în fereastra de mai jos indică faptul că totul este pregătit pentru restul aplicațiilor din acest seminar.
   
   ![](/assets/ps_geany_execute-output.png)
    


[gcc_url]:        https://en.wikipedia.org/wiki/GNU_Compiler_Collection
[geany_url]:      https://en.wikipedia.org/wiki/Geany
[xcyg_url]:       http://x.cygwin.com/  
[cyginst_url]:    http://cygwin.com/setup-x86_64.exe
[cyginst_tutor]:  http://x.cygwin.com/docs/ug/setup.html#setup-cygwin-x-installing
