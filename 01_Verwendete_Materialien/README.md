# Verwendete Materialien 

## Gedruckte Mikroskop- und Zubehörteile

Alle Teile werden auf einem \emph{Prusa i3 MK3S} 3D-Drucker gedruckt. Als Filament wird \emph{Prusament PLA} in \emph{Galaxy Silver} und \emph{Vanilla White} verwendet.
Im Prusa-Slicer wurden folgende Druck-Parameter eingestellt:
* Schichtdicke: 0,2 mm (SPEED)
* Infill: 20\%
* Stützen: Keine (alle Teile sind so konstruiert, dass keine Stützstrukturen notwendig sind)

    <p align="left">
    <img src="01_Bilder/Tabelle_Druckzeiten.PNG" width="550">
    <em><br />3D-gedruckte Teile und ihre Druckzeiten</em>
    </p>



## Elektronische Bauteile

Nachfolgend !!! (noch einfügen) befindet sich eine vollständige Kostenübersicht der verwendeten, nicht druckbaren Bauteile. Bei den unter [Sonstige Kleinteile](Sonstige Kleinteile) aufgeführten Positionen (insbesondere den O-Ringen) empfiehlt es sich, einige Teile in Reserve zu haben und je nach Bedarf z.~B. mit unterschiedlichen Schraubenlängen zu experimentieren.

* LED (weiß, \emph{Nichia 500D})
    * Durchmesser: 5 mm
    * Sockel: T-1 3/4
    * Spannung: 3,2 V
    * Betrachtungswinkel: 15\textdegree
    * Lichtstärke: 10 cd

* LED (grün, 525 nm, \emph{LuminousLED ultrahell})
    * Durchmesser: 5 mm
    * Sockel: T-1 3/4
    * Spannung: 3,0 - 3,4 V
    * Betrachtungswinkel: 15\textdegree
\item Lichtstärke: 22 cd
\end{itemize}

\item Ohmsche Widerstände
\begin{itemize}
\item 2x 60 $\Omega$ Festwiderstände
\item Potentiometer mit bis zu 10 k$\Omega$
\end{itemize} 

\item Raspberry Pi 4 Model B + Kameramodul
\begin{itemize}
\item Arbeitsspeicher (RAM): 2 GB
\item Prozessor: ARM Cortex-A72 (4x1,5 GHz)
\item Anschlüsse:
\begin{itemize}
\item Ethernet/LAN (10/100/1000 Mbit)
\item 2x USB 2.0
\item 2x USB 3.0
\item 2x HDMI
\item microSD
\item 3,5 mm-Klinke
\item USB-C ($\to$ Stromversorgung)
\end{itemize}
\item Ausgangsspannung: 5 V
\item Ausgangsstrom: 3 A
\end{itemize}

\item Mikroschritt-Motoren \emph{28BYJ-48} + Treiberplatinen
\begin{itemize}
\item Getriebeübersetzung: 1/64
\item Schrittwinkel: 5625 $\ast$ 1/64
\end{itemize}

\item Mikrocontroller \emph{Arduino nano}
\begin{itemize}
\item Arbeitsspeicher (RAM): 2 GB
\item EPROM: 1 KB
\item Taktrate: 16 MHz
\end{itemize}

\item USB-C-Buchse
