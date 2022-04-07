# Bau des Mikroskops


Der folgende Text soll als verbesserte Bauanleitung für zukünftige Mikroskop-Bauten fungieren. Die nachfolgend aufgeführten Schritte spiegeln unsere Durchführung des Projekts wider. Sie sollen als Orientierung dienen, können je nach Bedarf verändert werden.

## Antriebselemente

Für jede der drei Achsen des Mikroskops gibt es je ein Antriebselement, die am jeweiligen Fuß eine Kennzeichnung für die betroffene Achse besitzen. Die X- und Y-Elemente ermöglichen eine Verschiebung der Probe in die jeweilige Richtung, während das Z-Element eine genaue Fokussierung auf das Objekt ermöglicht. Für diesen Schritt werden das Hauptgehäuseteil (HGT (*main body*)), die großen Zahnräder, die Sechskant-Schrauben, die O-Ringe, die Messing-Muttern, sechs Unterlegscheiben und die gedruckten Werkzeuge für die Antriebselemente benötigt.

Zunächst wird in die entsprechenden Schlitze am HGT mit dem Mutternwerkzeug je eine Mutter eingeführt. Hier muss darauf geachtet werden, dass die Muttern passgenau am Werkzeug anliegen, damit sie richtig eingeführt werden können.

Danach werden die Sechskant-Schrauben in die großen Zahnräder gesteckt, sodass die Schraubenköpfe in die Sechskant-Aussparungen der Zahnräder liegen. Die Schrauben mit den Zahnrädern werden (mit je zwei Unterlegscheiben dazwischen) in die entsprechenden Schraubenlöcher am HGT gedreht und die Muttern mit dem Werkzeug festgehalten, bis die Schrauben festgedreht sind.

Als nächstes werden die Füße für den Anbau vorbereitet. Am HGT an den jeweiligen Stellen können noch dünne Querstreben vorhanden sein, diese müssen mit einem Messer entfernt werden.

Um die Fußelemente am HGT zu befestigen, wird mit dem Gummiband-Werkzeug jeweils ein O-Ring in ein Fußelement eingebracht. Dies ist in Abbildung \ref{pic: no01} zu sehen.

Die so präparierten Füße werden nun an den jeweiligen Stellen befestigt. Dazu wird der jeweilige Fuß am HGT aufgesetzt und das Gummiband-Werkzeug hineingedrückt, bis es zweimal (einmal pro Seite) klickt. Das Werkzeug wird dann herausgezogen und die Prozedur für die anderen Achsen wiederholt.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.3\textwidth]{Bilder/band_insertion_through_foot_1.jpg}
%\caption{Montage der Füße an das Mikroskop ($\ast$)}
\captionof{figure}[Montage der Füße an das Mikroskop]{Montage der Füße an das Mikroskop\footnote{} \label{pic: no01}}
%\label{pic: no01}
\end{figure}

\footnotetext{\textbf{Quelle:} \href{https://build.openflexure.org/openflexure-microscope/v6.1.5/docs/\#/1\_actuator\_assembly}{https://build.openflexure.org/openflexure-microscope/v6.1.5/docs/\#/1\_actuator\_assembly} (abgerufen am 28.02.2022)}

Der Fuß für die Z-Achse unterscheidet sich in Größe und Auflageform von den anderen und muss in der Mitte platziert werden. Bei den anderen Füßen bleibt es einem prinzipiell selbst überlassen, an welcher Stelle diese eingesetzt werden. Baut man die motorisierte Variante des Mikroskops, wie bei diesem Projekt, muss jedoch später darauf geachtet werden, die Schrittmotoren richtig zu verkabeln.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.45\textwidth]{Bilder/aktuatoren.jpg}
\caption{HGT mit angebauten Füßen}
\label{pic: no02}
\end{figure}

## Optikmodul (Hochauflösend)

Für das Optikmodul werden das entsprechende gedruckte Teil, das Linsen-Werkzeug, die achromatische Linse, das Mikroskop-Objektiv, die Raspberry Pi-Kamera, die M3x10- und zwei M2x6-Zylinderkopfschrauben und die Edelstahl-Mutter benötigt.

Generell wird empfohlen, das gedruckte Optikmodul von Staub und eventuell quer durchhängenden Filamentfäden zu befreien. Danach wird zunächst die Mutter in den vorhandenen Schlitz an der Seite des Moduls eingeführt und die große Zylinderkopfschraube eingeschraubt. Diese dient dazu, das Optikmodul in das Mikroskop einzubauen, daher muss sie im weiteren Verlauf noch festgezogen werden.

Als nächstes wird die achromatische Linse auf das Linsen-Werkzeug gesetzt, sodass die konvexe (nach außen gewölbte) Seite unten auf dem Werkzeug aufliegt. Das Optikmodul wird so von oben auf die plane Seite der Linse aufgedrückt, dass die Linse im Modul festgeklemmt wird. Auf der gleichen Seite wird dann das Mikroskopobjektiv in das große Gewinde geschraubt, sodass dieses auch festsitzt. Das feine Gewinde bietet dabei Raum für fehlerhafte Montage, weshalb hier vorsichtig vorgegangen werden muss.

Nun muss die Linse von der Raspberry Pi-Kamera entfernt werden. Dazu wird zunächst die Schutzfolie von der Linse entfernt und danach mit Hilfe eines speziellen (und normalerweise mitgelieferten) Werkzeugs die Linse selbst. Das Kameramodul wird dann so auf die andere Seite des Moduls gelegt, dass deren Schraubenlöcher genau übereinander liegen und die Kamera so mit den verbleibenden Schrauben befestigt werden kann.


## Beleuchtung (Durchlicht)

Für die Durchlichtbeleuchtung wird nun die Kondenserlinse, deren Halterung, das Schwalben-schwanz-Bauteil, die LED, Litzenkabel (am besten Jumperkabel mit mindestens einem Kupp-lungs-Kontakt) und etwas Schrumpfschlauch benötigt.

Zu Beginn werden die Kontakte der LED gekürzt und an der Anode der Festwiderstand angelötet. Anschließend werden ein rotes und ein schwarzes Jumperkabel mit jeweils einer Kupplung am anderen Ende an den Widerstand (rotes Kabel) und die Kathode (schwarzes Kabel) gelötet und die Lötstellen sicherheitshalber mit Schrumpfschlauch ummantelt. Zusätzlich können die Kabel für zusätzliche Stabilität verzwirbelt werden.

Als nächstes wird die Kondenserlinse in ihre Halterung eingesetzt. Dazu wird das bereits beim Optikmodul benutzte Linsen-Werkzeug eingesetzt. Auch hier muss die konvexe Seite nach unten aufgelegt werden. Auf der anderen Seite der Halterung wird die LED eingesetzt. Das fertige Modul ist in Abbildung \ref{pic: no021} zu sehen.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/beleuchtungsmodul2.jpg}
\caption{Beleuchtungsmodul mit eingesetzter LED}
\label{pic: no021}
\end{figure}

## Objekthalterung

Zunächst wird das Doppelkabel für die LED über entsprechende Verlängerungskabel auf die entsprechenden Kontakte des Raspberry Pi gesteckt - das rote Kabel auf einen 5V-Anschluss (Pin 4), das schwarze Kabel auf Masse (Pin 6). Die Pins 4 und 6 befinden sich an zweiter und dritter Stelle von der Ecke an der Außenseite. Im Zweifelsfall ist unter \href{https://pi4j.com/1.2/pins/model-2b-rev1.html}{https://pi4j.com/1.2/pins/model-2b-rev1.html} eine detaillierte Darstellung der Pins zu finden. Der Raspberry Pi selbst kann mit zwei diagonal zueinander angeordneten Schrauben in den Mikroskopsockel geschraubt werden.

Danach wird das Kameramodul mit dem Raspberry Pi verbunden - das Flackbandkabel wird in die Schnittstelle nahe dem Ethernet-Anschluss gesteckt.
Auf der Objektseite des HGTs wird aufgrund der Objektivlänge der Objektheber angeschraubt. Da die Stabilität von selbstgedrehten Gewinden im Filament häufig zu wünschen übrig lässt, wird empfohlen, dass die Schraubenlöcher auf dem HGT vollständig durchbohrt und der Objektheber mit längeren Schrauben und Muttern auf dem HGT fixiert wird. Auf die gleiche Art und Weise werden die Objektklemmen auf der Kombination aus HGT und Objektheber befestigt.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/bohrlöcher.png}
\caption{Zu verändernde Bohrlöcher am HGT}
\label{pic: no0221}
\end{figure}



% https://www.okdo.com/de/wp-content/uploads/sites/7/2019/03/2358-05.jpg?w=734

Nun wird zusätzlich der Schwalbenschwanz für das Beleuchtungsmodul angeschraubt. Am HGT sind bei den Schraubenlöchern seitlich Aussparungen für Muttern eingebracht, um eine mechanisch stabile Beleuchtung zu gewährleisten.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/aussparungen_beleuchtung.png}
\caption{Aussparungen für die Beleuchtungsmontage}
\label{pic: no023}
\end{figure}

Das Beleuchtungsmodul wird anschließend auf den Schwalbenschwanz gesetzt.

## Aufsetzen des Raspberry Pi mit Raspbian OpenFlexure

1. *Raspberry Pi* Betriebssystem-Image herunterladen \\(\href{https://openflexure.org/projects/microscope/install}{https://openflexure.org/projects/microscope/install})

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/raspberry_install2.png}
\caption{Download des Betriebssystem-Images}
\label{pic: no03}
\end{figure}

2. Installieren des *Raspberry Pi*-Betriebssystems auf der microSD-Karte

  * *Raspberry Pi Imager](https://www.raspberrypi.com/software/}{https://www.raspberrypi.com/software/)* herunterladen. Die Bedienoberfläche sollte nach erfolgreicher Installation wie in Abbildung \ref{pic: no04} aussehen.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/raspberry_imager.png}
\caption{Benutzeroberfläche des Installationsprogramms}
\label{pic: no04}
\end{figure}

  * microSD-Karte in Computer mittels entsprechendem Schlitz oder Adapter einstecken
  * Raspberry Pi Imager starten und mittels **OS wählen** die in Schritt 1 heruntergeladene Datei auswählen
  * Mittels **SD-Karte wählen** die microSD-Karte auswählen, die beschrieben werden soll
  * Einstellungen überprüfen und auf **Schreiben** klicken. Das Betriebssystem wird nun auf die microSD-Karte geschrieben.
  * microSD-Karte in *Raspberry Pi* einsetzen


3. *Raspberry Pi* einrichten (erstes Hochfahren)
  * Bildschirm, Maus und Tastatur an *Raspberry Pi* anschließen
  * Der *Raspberry Pi* fährt hoch, sobald er mit einer Spannungsquelle angeschlossen wird
  * Den Setup-Anweisungen folgen
  * Neues Passwort einrichten. Die Standard-Anmeldedaten sind:\\
      Benutzername:\hspace{1em}  \emph{pi} \\
      Passwort: \hspace{3em} \emph{openflexure}



## Schrittmotoren

Für die Ansteuerung der Schrittmotoren stehen verschiedene Möglichkeiten zur Auswahl. Zum einen kann das sogenannte \emph{Sangaboard} aus einer selbst hergestellten Platine und SMD-Bauteilen selbst zusammengebaut, zum anderen kann ein Mikrocontroller, wie zum Beispiel der \emph{Arduino nano}, genutzt werden, um die Motoren anzusteuern. Da die Arduino-Variante keine Nachteile gegenüber dem Sangaboard hat und für das Sangaboard zahlreiche verschiedene Einzelteile nötig wären, die (zum Zeitpunkt des hier beschriebenen Baus) nicht in der Hochschule vorrätig waren und deren Bestellung nur in größeren Mengen sinnvoll wären, wird hier nur die Konstruktion für die Ansteuerung per Arduino beschrieben.

### Vorbereitung der Motorsteuerung mittels *Arduino nano*

1. [Arduino IDE herunterladen](https://www.arduino.cc/en/software}{https://www.arduino.cc/en/software) und installieren
2. Den Code für die Motorsteuerung als [ZIP-komprimierten Ordner herunterladen](https://gitlab.com/bath\_open\_instrumentation\_group/sangaboard/-/tree/master/arduino\_code/sangaboard) siehe Abbildung \ref{pic: no05}) oder direkt aus diesem Ornder hier XXX herunterladen\\ 

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/gitlab_sangaboard.png}
\caption{GitLab-Seite mit den Programmdateien für die Motorensteuerung}
\label{pic: no05}
\end{figure}

3. ZIP-komprimierten Ordner entpacken
4. *Arduino nano* per USB an Computer anschließen
5. In der Arduino IDE über \emph{Datei~>~Öffnen...} die Datei *sangaboard.ino* (im entpackten Ordner unter \emph{sangaboard-master\textbackslash arduino\_code\textbackslash sangaboard}) öffnen
6. In der Arduino IDE über \emph{Werkzeuge~>~Port} überprüfen, ob ein COM-Port mit dem Arduino verbunden ist. Die beiden Bedienflächen *Überprüfen*(Häkchen) und *Hochladen* (Pfeil nach rechts) nacheinander betätigen, der Code **Sangaboard** wird nach dem Kompilieren auf den Arduino geschrieben.
7. Der Arduino kann anschließend mit den Motortreiberplatinen der drei Motoren verbunden werden. Per USB wird der Arduino vor dem Hochfahren mit dem Raspberry Pi verbunden. Beim Hochfahren wird der Arduino durch den Raspberry Pi erkannt und kann anschließend angesteuert werden.


### Montage der Schrittmotoren und die Verkabelung der Elektronik

In Abbildung \ref{pic: no06} ist schematisch dargestellt, wie die Schrittmotoren und ihre Treiberplatinen mit dem Mikrocontroller verbunden werden.

%\begin{figure}[!htbp]
%\centering
%\includegraphics[width=0.6\textwidth]{Bilder/motor_verkabelung.png}
%\caption{Schaubild für die Verkabelung der Schrittmotoren mit dem Arduino}
%\label{pic: no06}
%\end{figure}

Zunächst sollte die Funktionstüchtigkeit der Schrittmotoren überprüft werden. Dazu kann der Arduino auf einer Steckplatine gesteckt und über Jumperkabel mit den Treiberplatinen und den daran angeschlossenen Motoren verbunden werden. Für die Stromversorgung empfiehlt sich vorerst die Verwendung eines Labornetzteils.

Wenn die Schrittmotoren einwandfrei funktionieren können diese nun fest verlötet werden. Als Basis empfiehlt sich eine Lochrasterplatine, auf welche der Arduino problemlos aufgesteckt werden kann. An den entsprechenden Stellen können Bohrlöcher zur Befestigung der Platine eingebracht werden (siehe Abbildung \ref{pic: no062}).

Für die Stromversorgung kann zum Beispiel eine USB-C-Buchse neben dem Mini-USB-Anschluss auf die Platine befestigt werden. Die Versorgungs- und Massekontakte der Treiberplatinen werden in diesem Fall mit den jeweiligen Kontakten auf der Buchse verlötet.

Weil hier eine möglichst hohe Stabilität notwendig ist, ist es ratsam, die Buchse über Drähte an die Lochrasterplatine zu löten.  Hierfür werden zwei Drähte jeweils in einem Bogen über die Buchse gespannt und auf beiden Seiten auf der Unterseite der Platine verlötet und auf der Oberseite mit dem Außenkontakt der Buchse per Lötnaht befestigt (siehe Abbildung \ref{pic: no066}).


\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/motor_verkabelung.png}
\captionof{figure}[Schaubild für die Verkabelung der Schrittmotoren mit dem Arduino]{Schaubild für die Verkabelung der Schrittmotoren mit dem Arduino\footnote{} \label{pic: no06}}
\end{figure}

\footnotetext{\textbf{Quelle:} \href{https://build.openflexure.org/openflexure-microscope/v6.1.5/docs/\#/6\_motor\_controllers}{https://build.openflexure.org/openflexure-microscope/v6.1.5/docs/\#/6\_motor\_controllers} (abgerufen am 28.02.2022)}

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/testverkabelung_motoren.jpg}
\caption{Testweise Verkabelung der Schrittmotoren mit dem Arduino}
\label{pic: no061}
\end{figure}

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/platine_arduino.jpg}
\caption{Zugeschnittene Lochrasterplatine mit Bohrlöchern und dem aufgesteckten Arduino}
\label{pic: no062}
\end{figure}

%\clearpage

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/rasterplatine_versorgung.jpg}
\caption{Zusammengelötete Versorgungsleitungen für die Schrittmotoren}
\label{pic: no063}
\end{figure}

Neben der Stromversorgung werden auch die Steuerungsleitungen mit den entsprechenden Kontakten des Arduino verlötet. Die Treiberplatinen können auf die Lochrasterplatine geklebt werden.


\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/verkabelte_platine_roh.jpg}
\caption{Vollständig mit dem Arduino verkabelte Treiberplatinen samt Stromversorgung}
\label{pic: no064}
\end{figure}

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/usb_c_buchse.jpg}
\caption{Neu befestigte USB-C-Buchse}
\label{pic: no066}
\end{figure}

Nach einem erfolgreichen Funktionstest mit der vollständig zusammengelöteten Platine können nun die Motoren auf dem HGT fixiert werden. Dazu sind neben den Motoren selbst die kleinen Zahnräder und die Linsenkopfschrauben notwendig. Die Zahnräder werden auf die Motorenachsen gesteckt und die Motoren auf den Schraubenlöchern bei den größeren Zahnrädern befestigt.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.8\textwidth]{Bilder/mikroskop_weiss.jpg}
\caption{Vollständiger Grundaufbau des Mikroskops}
\label{pic: no065}
\end{figure}

%\begin{figure}[!htbp]
%\centering
%\includegraphics[scale=1]{Bilder/Download.jpg}
%\caption{Spulenelektrode des \emph{thermatur 200}}
%\label{pic: no06}
%\end{figure}



## 3D-Teile modifizieren

Die Teile in der OpenFlexure-Bibliothek sind unveränderliche STL-Dateien. Für das Umsetzen eigener Ideen kann es notwendig sein, diese zu verändern, beziehungsweise für eigene Funktionen anzupassen. Dies ist durch folgende Vorgehensweise möglich:

1. Beschaffung einer Studierendenlizenz bei *Autodesk Inc.*. Diese kann kostenlos mittels aktueller Studienbescheinigung unter der [Autodesk-Website](https://www.autodesk.de/education/home) freigeschaltet werden.
2. Die Programme *3ds Max* und *Inventor* herunterladen und installieren.
3. In *3ds Max* die zu verändernde STL-Datei über *File~>~Open* importieren. Beim Import die Einstellungen aus Abbildung \ref{pic: no07} übernehmen.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.3\textwidth]{Bilder/import_stl.png}
\caption{Import-Einstellungen für STL-Dateien in \emph{3ds Max}}
\label{pic: no07}
\end{figure}

4. Das importierte Teil in der 3D-Ansicht anklicken, sodass es farbig umrandet wird
5. Datei unter \emph{File~>~Export~>~Export selected} als DWG-Datei exportieren (unter \emph{Save as type} die Option \emph{AutoCAD (*.dwg)} wählen und auf das Ablageverzeichnis achten!)

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/dwg_export.png}
\caption{Die zu verändernde STL-Datei muss für die weitere Bearbeitung in Inventor in das DWG-Dateiformat konvertiert werden}
\label{pic: no08}
\end{figure}

6. Bei Export die Einstellungen in Abbildung \ref{pic: no09} beachten

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.3\textwidth]{Bilder/dwg_export_einstellungen.png}
\caption{Export-Einstellungen für zu verändernde Dateien}
\label{pic: no09}
\end{figure}

7. \emph{Inventor} öffnen
8. Unter \emph{Datei~>~Öffnen~>~DWG importieren} die zuvor gespeicherte DWG-Datei öffnen
\item Nun öffnet sich der \emph{DWG-/DXF-Dateiassistent}. Hier muss \emph{Inhalt lesen aus AutoCAD- oder AutoCAD Mechanical-Datei} ausgewählt werden. Mit einem Klick auf \emph{Weiter} wird die Dateivorschau geöffnet. Mit einem erneuten Klick auf \emph{Weiter} öffnen sich die \emph{Importoptionen} für die ausgewählte Datei.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.65\textwidth]{Bilder/import_bauteil2.png}
\caption{Import-Einstellungen in \emph{Inventor} für die zu verändernde Datei}
\label{pic: no10}
\end{figure}

\item In \emph{Importoptionen für Ziel} müssen die in Abbildung \ref{pic: no10} gezeigten Einstellungen ausgewählt werden. Insbesondere die rot umrandete Einstellung \emph{Neues Bauteil} ist wichtig.
\item Auf \emph{Fertig stellen} klicken und warten, bis das Modell vollständig geladen ist. Dieses wird als Mesh dargestellt.
\item Mit der Maus ein Rechteck über das Teil ziehen, sodass alle Kanten markiert sind und loslassen. Das gesamte Modell sollte nun eingefärbt sein.
\item Im Reiter \emph{3D-Modell} im Bereich \emph{Oberfläche} auf \emph{Heften} klicken.
\item Im Fenster, das sich öffnet, auf \emph{Anwenden} klicken
\item Das Teil kann nun in \emph{Inventor} bearbeitet werden und als STL-, STEP- oder OBJ-Datei exportiert werden.

\end{enumerate}

Während dieses Projekts wurde der Mikroskop-Sockel (\emph{microscope\_stand\_30-BS.stl}) modifiziert. An der Seitenwand links von der Öffnung in der Grundfläche wurden zwei rechteckige und eine kreisförmige Öffnung eingearbeitet. Diese sind in Abbildung \ref{pic: no11} zu sehen.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.6\textwidth]{Bilder/microscope_stand_mod.png}
\caption{Modifizierte Stelle am Mikroskopsockel}
\label{pic: no11}
\end{figure}

Diese Aussparungen sind für ein Potentiometer und zwei Schiebeschalter vorgesehen. Mit einem Schalter soll die Stromversorgung ein- und ausgeschaltet werden können, während der andere Schalter die Möglichkeit bieten soll, zwischen zwei LEDs umzuschalten (in dieser Konfiguration zwischen der weißen Standard-LED und einer ultrahellen grünen LED mit einer Lichtwellenlänge von 525 nm). Mit dem Potentiometer soll die jeweilige LED gedimmt werden können. Die Aussparungen in der Lochraserplatine wurden mit einer Laubsäge erstellt und die Durchkontaktierungslöcher zur Orientierung genutzt. Beide Aussparungen sind sechs Löcher (ca. 20 mm) ,,hoch``. Die Aussparung für das Potentiometer ist drei Löcher (ca. 10 mm) ,,breit``, bei der Aussparung für die Schalter sind es vier (ca. 13 mm). Um die Schalter an die Platine schrauben zu können musste lediglich ein Durchkontaktierungsloch auf jeder Seite für jeden Schalter vergrößert werden. Die vorbereitete Platine ohne Bauteile sowie die bestückte Platine sind jeweils in Abbildung \ref{pic: no12} zu sehen.

\begin{figure}[!htbp]
\centering
\subfloat{\includegraphics[width=0.4\textwidth]{Bilder/schalterplatine_form.jpg}} \\
\subfloat{\includegraphics[width=0.4\textwidth]{Bilder/schalterplatine_front.jpg}} \,
\subfloat{\includegraphics[width=0.4\textwidth]{Bilder/schalterplatine_back.jpg}}
\caption{Oben: Rohplatine für die Steuerung mit Aussparungen\\ Unten: Bestückte Steuerplatine für die Mikroskop-Beleuchtung von vorne (links) und von hinten (rechts)}
\label{pic: no12}
\end{figure}

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.75\textwidth]{Bilder/maße_mod.png}
\caption{Bemaßungen der Modifikationen in Millimetern}
\label{pic: no13}
\end{figure}

Um die Platine befestigen zu können, wurden in den Sockel an passenden Stellen von Hand zwei Löcher für M2.5-Gewindeschrauben gebohrt. Die Platine wurde eingesetzt, dort die passenden Bohrlöcher mit einem Stift markiert und diese danach ebenfalls hineingebohrt. Die Befestigung erfolgte durch M2.5-Gewindeschrauben und M2.5-Muttern.

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.75\textwidth]{Bilder/befest_platine.jpg}
\caption{Befestigte Steuerplatine von außen}
\label{pic: no14}
\end{figure}

Damit der Raspberry Pi noch Platz im Sockel hat, mussten für die Schalter möglichst kurze Schrauben gewählt werden. 
