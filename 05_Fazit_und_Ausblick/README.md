# Fazit und Ausblick

## Fazit

Das openflexure-Mikroskop zu bauen, war eine Projektarbeit, die sehr vielseitig war. Durch die unterschiedlichen Fertigungsschritte, die Einrichtung auf elektronischer Seite sowie das Einbringen von Erweiterung konnten verschiedene Themenbereiche kennengelernt werden. 

Der zeitliche Umfang von drei Semestern war gut für dieses Projekt geeignet. Aufgrund von Lieferzeiten der Teile, Druckdauer der Teile und anderen Faktoren konnten manche Prozesse erst über einen längeren Zeitraum abgeschlossen werden. Der zeitliche Rahmen gibt die Möglichkeiten, iterativ Veränderungen vorzunehmen. Die Notwendigkeit für Anpassungen ergibt sich oft erst im Laufe des Projekts durch Funktionstests oder Überprüfung der Benutzerfreundlichkeit. Auch bietet eine Bearbeitung über mehrere Semester die Möglichkeit, tief in die Themen einzusteigen und sich intensiv damit zu beschäftigen. 

Der Vorteil an der Bearbeitung eines open source-Projekts ist, dass es viele Möglichkeiten zum Austausch gibt und Fragen, Feedback und Änderungen online geteilt werden können. Auch sind Codes und 3D-Modelle frei zugänglich und bieten damit ein Gerüst, das je nach Anwendung verändert werden kann. 

Der Bau eines kostengünstigen Mikroskops erfordert im Gegenzug viel Arbeitszeit, viele technische Gegebenheiten (3D-Drucker, Lötplatz, Computer) und Kreativität. Die Gesamtsumme der Ausgaben beträgt (bezogen auf die jeweils benötigte Stückzahl der Teile) ca. 350 €. Die tatsächlich investierte Summe kann davon abweichen, da ggf. manche Teile bereits vorrätig sind. Auch können manche Teile nur in größerer Stückzahl als benötigt bestellt werden und Versandkosten können ebenfalls anfallen, wodurch sich die Kosten erhöhen können. Für den vollständigen Aufbau eines Mikroskop-Arbeitsplatzes sind zusätzlich eine Maus, eine Tastatur und ein Bildschirm notwendig. Müssen diese ebenfalls neu gekauft werden, fallen nochmals zusätzliche Kosten von mindestens ca. 50 € an. Im Anhang befindet sich eine Kostenübersicht und Bestelllinks zu den wichtigen Teilen. Diese Liste ist nicht vollständig, da Schrauben, Kabel und Widerstände nicht aufgelistet sind. 

Mit einer Gesamtsumme von ca. 350 € (Stand März 2022) ist das Mikroskop deutlich günstiger als vergleichbare kommerzielle Mikroskope von mindestens 3500 €. Es ist allerdings zu bedenken, dass kommerzielle Mikroskope meist über mehrere Objektive verfügen und oft trinocular aufgebaut sind (es kann sowohl eine Kamera angeschlossen werden als auch direkt auf die Probe geschaut werden). Der Vorteil des selbst gebauten Mikroskops ist die einfache Wartbarkeit und die Möglichkeit, selbst Veränderungen durchzuführen.
Das Mikroskop bietet in jedem Fall eine günstigere Alternative mit guten Ergebnissen und einem geringen Gewicht. Es ist gut transportabel und kann an jedem beliebigen Arbeitsplatz, an dem ein Bildschirm, eine Maus und eine Tastatur vorhanden sind, eingesetzt werden. 

Nach drei Semestern konnte das Mikroskop mit allen geplanten Konfigurationen fertiggestellt werden, sodass es beispielsweise für den Einsatz in einem Praktikum geeignet ist. 

## Ausblick

Das Mikroskop bietet in vielerlei Hinsicht Potential, weiterentwickelt und verbessert zu werden. 

Das Dimmen der LEDs (momentan über ein Potentiometer geregelt) könnte mittels einer Pulsweitenmodulation (PWM)-Ansteuerung über den Raspberry Pi realisiert werden. Mit dieser Lösung könnte die Helligkeit feiner eingestellt werden. Eine softwareseitige Implementierung (z.b. auf der GUI des Mikroskops) kann die Wiederholbarkeit bestimmter Einstellungen gewährleisten. Andernfalls könnte nach wie vor das Potentiometer genutzt werden, um die PWM einzustellen. 

Eine andere Erweiterung besteht darin, die Fluoreszenz für verschiedene Wellenlängen zu ermöglichen. Dazu sind jeweils eine LED mit definierter Wellenlänge und ein dazu passender Filter notwendig, der das Anregungslicht herausfiltert und nur das emittierte Licht hindurchlässt. Das Anschließen anderer LEDs lässt sich einfach implementieren, indem diese mit Jumper-Kabeln verbunden werden, die einfach an den Platz der vorherigen LEDs angesteckt werden können. 
 
Umfangreiche Anpassungen und Verbesserung sind auch auf der grafischen Benutzeroberfläche des openflexure-Programms auf dem Raspberry Pi möglich. Eine mögliche Funktion ist z.B. das oben beschriebene Dimmen der LEDs. Auch das Erstellen einer übersichtlichen Datenbank für mehrere Aufnahmen und das einfache Speichern könnte zusätzlich implementiert werden. 

Die Erweiterung zu super resolution könnte ebenfalls softwareseitig gelöst werden. Hier kann eine Lösung mit dem Einsatz eines trainierten Netzwerks angewendet werden, wie sie Mario Baars in seiner [Bachelorarbeit](https://www.github.com/aazang/srgan-for-microscopy) vorgestellt hat. Ein Beispiel, wie die Bildverbesserung aussehen könnte, ist in Abbildung \ref{pic: no15} anhand einer Blutzellenaufnahme zu sehen. Das linke Bild dient als Referenzbild, das mittige zeigt das Bild als herunterskalierte Version und rechts ist die Verbesserung des mittleren Bildes mittels eines Super-Resoltion-Generative-Adversarial-Network (SRGAN) zu sehen. Erste Versuche mit Aufnahmen aus dem Mikroskop funktionierten noch nicht so zuverlässig wie in diesem Beispiel. 

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/SRGAN-Image.png}
\caption{Bildverbesserung mittels SRGAN am Beispiel von Blutzellen}
\label{pic: no15}
\end{figure}



Die Möglichkeit der Merkmalsextraktion bzw. der Segmentierung könnten mit einer Bildverarbeitungs-Software ebenfalls realisiert werden. Über diese Aufzählung hinaus gibt es sicherlich noch viel mehr Möglichkeiten, an diesem Projekt anzuknüpfen.
