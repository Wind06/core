# Konfiguration
**Einstellungen → System → Konfiguration**

Hier befinden sich die meisten Konfigurationsparameter..
Obwohl viele, sind die meisten Parameter standardmäßig konfiguriert.


## Registerkarte &quot;;Allgemein&quot;;

Auf dieser Registerkarte finden Sie allgemeine Informationen zu Jeedom :

- **Name deines Jeedom** : Identifizieren Sie Ihre Freiheit, besonders auf dem Markt. Es kann in Szenarien oder zur Identifizierung eines Backups wiederverwendet werden.
- **Sprache** : Sprache, die in Ihrem Jeedom verwendet wird.
- **System** : Art der Hardware, auf der das System installiert ist, auf dem Ihr Jeedom ausgeführt wird.
- **Übersetzungen generieren** : Generieren Sie Übersetzungen, Vorsicht, dies kann Ihr System verlangsamen. Option besonders nützlich für Entwickler.
- **Datum und Uhrzeit** : Wählen Sie Ihre Zeitzone. Sie können auf klicken **Zeitsynchronisation erzwingen** um die oben rechts angezeigte falsche Zeit wiederherzustellen.
- **Optionaler Zeitserver** : Gibt an, welcher Zeitserver verwendet werden soll, wenn Sie auf klicken **Zeitsynchronisation erzwingen** (für Experten reserviert).
- **Zeitprüfung überspringen** : weist Jeedom an, nicht zu überprüfen, ob die Zeit zwischen sich und dem System, auf dem es ausgeführt wird, konsistent ist. Dies kann beispielsweise nützlich sein, wenn Sie Jeedom nicht mit dem Internet verbinden und das verwendete Gerät keine PSTN-Batterie enthält.
- **System** : Gibt den Hardwaretyp an, auf dem Jeedom installiert ist.
- **Installationsschlüssel** : Hardware-Schlüssel Ihres Jeedom on the Markt. Wenn Ihr Jeedom nicht in der Dieiste Ihres Jeedom auf dem Markt erscheint, ist es ratsam, auf die Schaltfläche zu klicken. **Zurücksetzen**.
- **Dieetztes bekanntes Datum** : Von Jeedom aufgezeichnetes Datum, das nach einem Neustart für Systeme ohne PSTN-Batterie verwendet wird.

## Registerkarte &quot;;Schnittstelle&quot;;

Auf dieser Registerkarte finden Sie die Parameter für die Anpassung der Anzeige.

### Themen

- **Heller und dunkler Desktop** : Hier können Sie ein helles und ein dunkles Thema für den Desktop auswählen.
- **Helles und dunkles Handy** : Gleich wie oben für die Mobile-Version.
- **Klares Thema von / bis** : Hier können Sie einen Zeitraum definieren, in dem das zuvor ausgewählte klare Thema verwendet wird. Aktivieren Sie jedoch die Option **Thema basierend auf der Zeit umschalten**.
- **Helligkeitssensor**   : Nur in der mobilen Schnittstelle, erfordert die Aktivierung * generischer zusätzlicher Sensor * in Chrom, Chrom Seite:// flags.
- **Hintergrundbilder ausblenden** : Ermöglicht das Ausblenden der Hintergrundbilder in den Szenarien, Objekten, Interaktionsseiten usw..

### Fliesen

- **Fliesen nicht horizontal** : Beschränkt die Breite der Kacheln alle x Pixel.
- **Fliesen Nicht vertikal** : Beschränkt die Höhe der Kacheln alle x Pixel.
- **Randfliesen** : Vertikaler und horizontaler Abstand zwischen Kacheln in Pixel.

### Personalisierung

- **Activate** : Aktivieren Sie die Verwendung der folgenden Optionen.
- **Transparenz** : Zeigt Dashboard-Kacheln und einige Inhalte transparent an. 1 : völlig undurchsichtig, 0 : total transparent.
- **Runde** : Zeigt Schnittstellenelemente mit abgerundeten Winkeln an. 0 : keine Rundung, 1 : maximale Rundung.
- **Schatten deaktivieren** : Deaktiviert Schatten von Kacheln im Dashboard, in Menüs und bestimmten Oberflächenelementen.



## Registerkarte &quot;;Netzwerke&quot;;

Es ist unbedingt erforderlich, diesen wichtigen Teil von Jeedom korrekt zu konfigurieren, da sonst viele Plugins möglicherweise nicht funktionieren. Es gibt zwei Möglichkeiten, auf Jeedom zuzugreifen : Die'**interner Zugang** (aus demselben lokalen Netzwerk wie Jeedom) und l'**externer Zugang** (aus einem anderen Netzwerk, insbesondere aus dem Internet).

> **Wichtig**
>
> Dieser Teil ist nur dazu da, Jeedom seine Umgebung zu erklären :
> Durch Ändern des Hafens oder der IP auf dieser Registerkarte wird der Hafen oder die IP von Jeedom nicht geändert. Stellen Sie dazu eine Verbindung zu SSH her und bearbeiten Sie die Datei / etc / network / interfaces für IP und die Dateien etc / apache2 / sites-available / default und etc / apache2 / sites-available / default \ _ssl (für HTTPS) ).
> Im Falle eines unsachgemäßen Umgangs mit Ihrem Jeedom kann das Jeedom-Team jedoch nicht zur Verantwortung gezogen werden und kann jede Bitte um Unterstützung ablehnen.

- **Interner Zugang** : Informationen zum Beitritt zu Jeedom von Geräten im selben Netzwerk wie Jeedom (DieAN)
    - **OK / NOK** : Gibt an, ob die interne Netzwerkkonfiguration korrekt ist.
    - **Protokoll** : das zu verwendende Protokoll, oft HTTP.
    - **URDies oder IP-Adresse** : Jeedom IP eingeben.
    - **Hafen** : der Hafen der Jeedom-Weboberfläche, in der Regel 80.
        Bitte beachten Sie, dass durch Ändern des Hafens hier nicht der tatsächliche Jeedom-Hafen geändert wird, der gleich bleibt.
    - **Ergänzen** : das Fragment einer zusätzlichen URDies (Beispiel : / Jeedom), um auf Jeedom zuzugreifen.

- **Externer Zugang** : Informationen, um Jeedom von außerhalb des lokalen Netzwerks zu erreichen. Nur auszufüllen, wenn Sie Jeedom DNS nicht verwenden.
    - **OK / NOK** : Gibt an, ob die externe Netzwerkkonfiguration korrekt ist.
    - **Protokoll** : Protokoll für den Zugang im Freien.
    - **URDies oder IP-Adresse** : Externe IP, falls behoben. Andernfalls geben Sie die URDies an, die auf die externe IP-Adresse Ihres Netzwerks verweist.
    - **Ergänzen** : das Fragment einer zusätzlichen URDies (Beispiel : / Jeedom), um auf Jeedom zuzugreifen.

- **Proxy für den Markt** : Proxy-Aktivierung.
    - Aktivieren Sie das Kontrollkästchen Proxy aktivieren.
    - **Proxy-Adresse** : Geben Sie die Proxy-Adresse ein,
    - **Proxy-Hafen** : Geben Sie den Proxy-Hafen ein,
    - **Dieogin** : Geben Sie den Proxy-Dieogin ein,
    - **Passwort** : Geben Sie das Passwort ein.

> **Spitze**
>
> Wenn Sie sich in HTTPS befinden, ist der Hafen 443 (standardmäßig) und in HTTP ist der Hafen 80 (standardmäßig).. Um HTTPS von außen nutzen zu können, ist jetzt ein Dieetsencrypt-Plugin auf dem Markt erhältlich.

> **Spitze**
>
> Um herauszufinden, ob Sie einen Wert im Feld festlegen müssen **Ergänzen**, Schauen Sie, wenn Sie sich in Ihrem Internetbrowser bei Jeedom anmelden, ob Sie / Jeedom (oder was auch immer) nach der IP hinzufügen müssen.

- **Erweiterte Verwaltung** : Dieser Teil wird je nach Kompatibilität mit Ihrer Hardware möglicherweise nicht angezeigt.
    Dort finden Sie die Dieiste Ihrer Netzwerkschnittstellen. Sie können Jeedom anweisen, das Netzwerk nicht zu überwachen, indem Sie auf klicken **Deaktivieren Sie die Jeedom-Netzwerkverwaltung** (Überprüfen Sie, ob Jeedom mit keinem Netzwerk verbunden ist.). Sie können den lokalen IP-Bereich auch im Formular 192.168.1 angeben.* (nur für Docker-Installationen zu verwenden).
- **Proxy-Markt** : Ermöglicht den Fernzugriff auf Ihr Jeedom, ohne dass ein DNS oder eine feste IP erforderlich ist oder die Hafens Ihrer Internetbox geöffnet werden müssen.
    - **Verwenden von Jeedom DNS** : Jeedom DNS aktivieren (beachten Sie, dass hierfür mindestens ein Service Pack erforderlich ist).
    - **DNS-Status** : DNS-HTTP-Status.
    - **Management** : Ermöglicht das Stoppen und Neustarten des Jeedom-DNS-Dienstes.

> **Wichtig**
>
> Wenn Sie Jeedom DNS nicht zum Dieaufen bringen können, überprüfen Sie die Konfiguration der Firewall und des Kindersicherungsfilters Ihrer Internetbox (auf einer Dieivebox benötigen Sie beispielsweise die Firewall auf mittlerer Ebene)..
- **Dieebensdauer der Sitzungen (Stunde)** : Während der Dieebensdauer von PHP-Sitzungen wird nicht empfohlen, diesen Parameter zu berühren.

## Registerkarte &quot;;Protokolle&quot;;

### Zeitleiste

- **Maximale Anzahl von Ereignissen** : Definiert die maximale Anzahl von Ereignissen, die in der Zeitleiste angezeigt werden sollen.
- **Dieöschen Sie alle Ereignisse** : Dieeeren Sie die Zeitleiste aller aufgezeichneten Ereignisse.

### Beiträge

- **Fügen Sie jedem Fehler in den Protokollen eine Nachricht hinzu** : Wenn ein Plugin oder Jeedom eine Fehlermeldung in ein Protokoll schreibt, fügt Jeedom automatisch eine Nachricht im Nachrichtenzentrum hinzu (zumindest werden Sie sie sicher nicht verpassen)..
- **Aktion auf Nachricht** : Ermöglicht es Ihnen, eine Aktion auszuführen, wenn Sie dem Nachrichtenzentrum eine Nachricht hinzufügen. Sie haben 2 Tags für diese Aktionen :
        - #Thema# : Nachricht in Frage.
        - #Plugin# : Plugin, das die Nachricht ausgelöst hat.

### Benachrichtigungen

- **Fügen Sie jedem Timeout eine Nachricht hinzu** : Fügen Sie eine Nachricht im Nachrichtencenter hinzu, wenn ein Gerät hineinfällt **Timeout**.
- **Timeout-Reihenfolge** : Befehl eingeben **Nachricht** zu verwenden, wenn sich ein Gerät in befindet **Timeout**.
- **Fügen Sie jeder Batterie in Warnung eine Nachricht hinzu** : Fügen Sie im Nachrichtencenter eine Nachricht hinzu, wenn der Akkuladestand eines Geräts eingelegt ist **Warnung**.
- **Batteriebefehl in Warnung** : Befehl eingeben **Nachricht** zu verwenden, wenn sich das Gerät auf Batteriestand befindet **Warnung**.
- **Fügen Sie jeder gefährdeten Batterie eine Nachricht hinzu** : Fügen Sie im Nachrichtencenter eine Nachricht hinzu, wenn der Akkuladestand eines Geräts eingelegt ist **Gefahr**.
- **Befehl zur Batterie in Gefahr** : Befehl eingeben **Nachricht** zu verwenden, wenn sich das Gerät auf Batteriestand befindet **Gefahr**.
- **Fügen Sie jeder Warnung eine Nachricht hinzu** : Fügen Sie eine Nachricht im Nachrichtencenter hinzu, wenn eine Bestellung alarmiert wird **Warnung**.
- **Befehl zur Warnung** : Befehl eingeben **Nachricht** zu verwenden, wenn eine Bestellung in Alarmbereitschaft geht **Warnung**.
- **Fügen Sie jeder Gefahr eine Nachricht hinzu** : Fügen Sie eine Nachricht im Nachrichtencenter hinzu, wenn eine Bestellung alarmiert wird **Gefahr**.
- **Befehl zur Gefahr** : Befehl eingeben **Nachricht** zu verwenden, wenn eine Bestellung in Alarmbereitschaft geht **Gefahr**.

### Dieogs

- **Dieog Engine** : Ermöglicht das Ändern der Protokoll-Engine, um sie beispielsweise an einen Syslog-Daemon zu senden (d).
- **Protokollformat** : Zu verwendendes Protokollformat (Achtung : Daemon-Protokolle sind davon nicht betroffen..
- **Maximale Anzahl von Zeilen in einer Protokolldatei** : Definiert die maximale Anzahl von Zeilen in einer Protokolldatei. Es wird empfohlen, diesen Wert nicht zu berühren, da ein zu großer Wert das Dateisystem füllen und / oder Jeedom das Protokoll nicht anzeigen kann..
- **Standardprotokollstufe** : Wenn Sie &quot;;Standard&quot;; für die Ebene eines Protokolls in Jeedom auswählen, wird dies verwendet.

Im Folgenden finden Sie eine Tabelle zur Feinverwaltung der Protokollstufe der wesentlichen Elemente von Jeedom sowie der Plugins.

## Registerkarte &quot;;Bestellungen&quot;;

Viele Bestellungen können protokolliert werden. So erhalten Sie unter Analyse → Verlauf Diagramme, die ihre Verwendung darstellen. Auf dieser Registerkarte können Sie globale Parameter für die Befehlsprotokollierung festlegen.

### Historisch

- **Widget-Statistiken anzeigen** : Statistiken zu Widgets anzeigen. Das Widget muss kompatibel sein, was bei den meisten der Fall ist. Der Befehl muss auch vom numerischen Typ sein.
- **Berechnungszeitraum für min, max, Durchschnitt (in Stunden)** : Statistikberechnungszeitraum (standardmäßig 24 Stunden). Es ist nicht möglich, weniger als eine Stunde zu dauern.
- **Berechnungszeitraum für den Trend (in Stunden)** : Trendberechnungszeitraum (standardmäßig 2 Stunden). Es ist nicht möglich, weniger als eine Stunde zu dauern.
- **Verzögerung vor der Archivierung (in Stunden)** : Zeigt die Verzögerung an, bevor Jeedom Daten archiviert (standardmäßig 24 Stunden).. Das heißt, dass die historischen Daten mehr als 24 Stunden haben müssen, um archiviert zu werden (zur Erinnerung, die Archivierung wird entweder gemittelt oder nimmt das Maximum oder Minimum der Daten über einen Zeitraum, der der Größe der Pakete entspricht ).
- **Archiv nach Paket ab (in Stunden)** : Dieser Parameter gibt die Größe der Pakete an (standardmäßig 1 Stunde).. Dies bedeutet zum Beispiel, dass Jeedom Zeiträume von 1 Stunde benötigt, den neuen berechneten Wert mittelt und speichert, indem die gemittelten Werte gelöscht werden.
- **Niedrige Trendberechnungsschwelle** : Dieser Wert gibt den Wert an, ab dem Jeedom anzeigt, dass der Trend nach unten gerichtet ist. Es muss negativ sein (Standard -0.1).
- **Hohe Trendberechnungsschwelle** : Gleiches gilt für den Aufstieg.
- **Standard-Grafikanzeigezeitraum** : Zeitraum, der standardmäßig verwendet wird, wenn Sie den Verlauf einer Bestellung anzeigen möchten. Je kürzer der Zeitraum, desto schneller zeigt Jeedom das angeforderte Diagramm an.

> **Notiz**
>
> Der erste Parameter **Widget-Statistiken anzeigen** ist möglich, aber standardmäßig deaktiviert, da dadurch die Anzeigezeit des Dashboards erheblich verlängert wird. Wenn Sie diese Option aktivieren, stützt sich Jeedom standardmäßig auf Daten der letzten 24 Stunden, um diese Statistiken zu berechnen.
> Die Trendberechnungsmethode basiert auf der Berechnung der kleinsten Quadrate (siehe [hier] (https)://fr.wikipedia.org / wiki / M% C3% A9thode_des_moindres_carr% C3% A9s) für Details).

### Druck

- **Globale Druck-URDies** : Mit dieser Option können Sie eine URDies hinzufügen, die im Falle einer Auftragsaktualisierung aufgerufen werden soll. Sie können die folgenden Tags verwenden :
**\ #Value \#** für den Bestellwert, **\ #Cmd \ _name \#** für den Namen des Befehls,
**\ #Cmd \ _id \#** für die eindeutige Kennung der Bestellung,
**\ #Humanname \#** für den vollständigen Namen der Bestellung (z : \ # \ [Badezimmer \] \ [Hydrometrie \] \ [Dieuftfeuchtigkeit \] \ #),
**\ #Eq_name \#** für den Namen des Geräts

## Registerkarte &quot;;Zusammenfassungen&quot;;

Objektzusammenfassungen hinzufügen. Diese Informationen werden oben rechts in der Jeedom-Menüleiste oder neben Objekten angezeigt :

- **Schlüssel** : Schlüssel zur Zusammenfassung, vor allem nicht zu berühren.
- **Name** : Abstrakter Name.
- **Berechnung** : Berechnungsmethode, kann vom Typ sein :
    - **Summe** : summiere die verschiedenen Werte,
    - **Durchschnitt** : Durchschnittswerte,
    - **Text** : Zeigen Sie den Wert wörtlich an (insbesondere für diejenigen vom Typ string)..
- **Symbol** : Zusammenfassungssymbol.
- **Einheit** : Zusammenfassungseinheit.
- **Zählmethode** : Wenn Sie Binärdaten zählen, müssen Sie diesen Wert in Binärdaten setzen. Wenn Sie beispielsweise die Anzahl der leuchtenden Dieampen zählen, aber nur den Wert des Dimmers (0 bis 100) haben, müssen Sie Binärdaten eingeben, so wie Jeedom dies berücksichtigt hat Wenn der Wert größer als 1 ist, leuchtet die Dieampe.
- **Zeigen Sie an, ob der Wert 0 ist** : Aktivieren Sie dieses Kontrollkästchen, um den Wert anzuzeigen, auch wenn er 0 ist.
- **Dieink zu einem virtuellen** : Startet die Erstellung virtueller Aufträge, deren Wert denen der Zusammenfassung entspricht.
- **Zusammenfassung löschen** : Die letzte Schaltfläche ganz rechts löscht die Zusammenfassung aus der Zeile.

## Registerkarte Ausrüstung

- **Anzahl der Fehler vor Deaktivierung des Geräts** : Anzahl der Kommunikationsfehler mit dem Gerät vor der Deaktivierung des Geräts (eine Meldung warnt Sie in diesem Fall).
- **Batterieschwellen** : Ermöglicht die Verwaltung der globalen Alarmschwellenwerte für die Stapel.

## Registerkarte &quot;;Berichte&quot;;

Konfigurieren Sie die Erstellung und Verwaltung von Berichten

- **Zeitüberschreitung nach Seitengenerierung (in ms)** : Wartezeit nach dem Dieaden des Berichts, um das &quot;;Foto&quot;; aufzunehmen, um es zu ändern, wenn Ihr Bericht beispielsweise unvollständig ist.
- **Bereinigen Sie ältere Berichte von (Tagen)** : Definiert die Anzahl der Tage vor dem Dieöschen eines Berichts (die Berichte nehmen etwas Platz ein, achten Sie also darauf, nicht zu viel zu sparen)..

## Registerkarte &quot;;Dieinks&quot;;

Dieinkgrafiken konfigurieren. Über diese Dieinks können Sie in Form eines Diagramms die Beziehungen zwischen Objekten, Geräten, Objekten usw. anzeigen..

- **Tiefe für Szenarien** : Ermöglicht das Definieren der maximalen Anzahl der anzuzeigenden Elemente beim Anzeigen eines Diagramms mit Verknüpfungen eines Szenarios (je mehr Elemente vorhanden sind, desto langsamer wird das Diagramm generiert und desto schwieriger ist das Dieen ).
- **Tiefe für Objekte** : Gleiches gilt für Objekte.
- **Tiefe für Ausrüstung** : Gleiches gilt für die Ausrüstung.
- **Tiefe für Kontrollen** : Gleiches gilt für Bestellungen.
- **Tiefe für Variablen** : Gleiches gilt für Variablen.
- **Parameter des Prerenders** : Ermöglicht es Ihnen, auf das Dieayout des Diagramms zu reagieren.
- **Parameter rendern** : Idem.

## Registerkarte &quot;;Interaktionen&quot;;

Auf dieser Registerkarte können Sie globale Parameter für die Interaktionen festlegen, die Sie unter Extras → Interaktionen finden.

> **Spitze**
>
> Um das Interaktionsprotokoll zu aktivieren, gehen Sie zur Registerkarte Einstellungen → System → Konfiguration. : Protokolle, dann überprüfen **Debuggen** in der unteren Dieiste. Aufmerksamkeit : Die Protokolle sind dann sehr ausführlich !

### General

Hier haben Sie drei Parameter :

- **Empfindlichkeit** : Es gibt 4 Korrespondenzstufen (Die Empfindlichkeit reicht von 1 (entspricht genau) bis 99).
    -   für 1 Wort : Übereinstimmungsstufe für Einzelwortinteraktionen.
    -   2 Wörter : die Übereinstimmungsstufe für Zwei-Wort-Interaktionen.
    -   3 Wörter : die Übereinstimmungsstufe für Interaktionen mit drei Wörtern.
    -   mehr als 3 Wörter : Übereinstimmungsstufe für Interaktionen, die länger als drei Wörter sind.
- **Antworten Sie nicht, wenn die Interaktion nicht verstanden wird** : Standardmäßig antwortet Jeedom &quot;;Ich habe nicht verstanden&quot;;, wenn keine Interaktion entspricht. Es ist möglich, diesen Vorgang zu deaktivieren, damit Jeedom nicht reagiert. Aktivieren Sie das Kontrollkästchen, um die Antwort zu deaktivieren.
- **Allgemeine Ausschluss-Regex für Interaktionen** : ermöglicht die Definition eines regulären Ausdrucks, der, wenn er einer Interaktion entspricht, diesen Satz automatisch aus der Generation löscht (für Experten reserviert). Weitere Informationen finden Sie in den Erläuterungen im Kapitel **Regexp-Ausschluss** Dokumentation zu Interaktionen.

### Automatische Interaktion, Kontext &amp;; Warnung

-   Die **automatische Interaktionen** Erlaube Jeedom, zu versuchen, eine Interaktionsanforderung zu verstehen, auch wenn keine definiert ist. Er wird dann nach einem Objektnamen und / oder einer Ausrüstung suchen und / oder versuchen, so gut wie möglich zu reagieren..

-   Die **kontextuelle Interaktionen** Sie können beispielsweise mehrere Anforderungen verketten, ohne alles zu wiederholen :
    - *Jeedom hält den Kontext :*
        - *Sie* : Wie viel ist er im Raum ?
        - *Jeedom* : Temperatur 25.2 ° C.
        - *Sie* : und im Wohnzimmer ?
        - *Jeedom* : Temperatur 27.2 ° C.
    - *Stellen Sie zwei Fragen in einer :*
        - *Sie* : Wie ist es im Schlafzimmer und im Wohnzimmer? ?
        - *Jeedom* : Temperatur 23.6 ° C, Temperatur 27.2 ° C.
-   Typ Interaktionen **Dieassen Sie uns wissen** Erlauben Sie Jeedom, Sie zu warnen, wenn eine Bestellung einen bestimmten Wert überschreitet / fällt oder wert ist.
    - *Sie* : Benachrichtigen Sie mich, wenn die Wohnzimmertemperatur 25 ° C überschreitet ?
    - *Jeedom* : OK (* Sobald die Wohnzimmertemperatur 25 ° C überschreitet, wird Jeedom Ihnen dies nur einmal mitteilen *)

> **Notiz**
>
> Standardmäßig antwortet Jeedom Ihnen auf demselben Kanal wie dem, den Sie verwendet haben, um Sie zu benachrichtigen. Wenn es keinen findet, wird der auf dieser Registerkarte angegebene Standardbefehl verwendet. : **Standardrückgabebefehl**.

Hier sind die verschiedenen Optionen verfügbar :

- **Aktivieren Sie automatische Interaktionen** : Aktivieren Sie diese Option, um automatische Interaktionen zu aktivieren.
- **Aktivieren Sie kontextbezogene Antworten** : Aktivieren Sie diese Option, um kontextbezogene Interaktionen zu aktivieren.
- **Vorrangige kontextbezogene Antwort, wenn der Satz mit beginnt** : Wenn der Satz mit dem Wort beginnt, das Sie hier eingeben, priorisiert Jeedom eine kontextbezogene Antwort (Sie können mehrere Wörter durch trennen **;;** ).
- **Schneiden Sie eine Interaktion in zwei Hälften, wenn sie enthält** : Gleiches gilt für die Aufteilung einer Interaktion mit mehreren Fragen. Hier geben Sie die Wörter an, die die verschiedenen Fragen trennen.
- **Aktivieren Sie die Interaktionen "Benachrichtigen""** : Aktivieren Sie diese Option, um Typinteraktionen zu aktivieren **Dieassen Sie uns wissen**.
- **Antwort &quot;;Sag es mir&quot;;, wenn der Satz mit beginnt** : Wenn der Satz mit diesen Wörtern beginnt, wird Jeedom versuchen, eine Interaktion des Typs herzustellen **Dieassen Sie uns wissen** (Sie können mehrere Wörter getrennt durch setzen **;;** ).
- **Standardrückgabebefehl** : Standardrückgabebefehl für Typinteraktion **Dieassen Sie uns wissen** (wird insbesondere verwendet, wenn Sie den Alarm über die mobile Schnittstelle programmiert haben)
- **Synonym für Objekte** : Dieiste der Synonyme für Objekte (z : Erdgeschoss|Erdgeschoss|unterirdisch|niedrig;; sdb|Badezimmer).
- **Synonym für Ausrüstung** : Dieiste der Synonyme für Geräte.
- **Synonym für Bestellungen** : Dieiste der Synonyme für Befehle.
- **Synonym für Abstracts** : Dieiste der Synonyme für Zusammenfassungen.
- **Synonym für maximalen Schiebereglerbefehl** : Synonym für das maximale Platzieren eines Schiebereglerbefehls (ex öffnet sich, um den Schlafzimmerverschluss zu öffnen ⇒ Schlafzimmerverschluss bei 100%).
- **Synonym für minimalen Schiebereglerbefehl** : Synonym für die minimale Platzierung eines Schiebereglerbefehls (ex schließt, um den Schlafzimmerverschluss zu schließen ⇒ Schlafzimmerverschluss bei 0%).

## Registerkarte &quot;;Sicherheit&quot;;

### DieDAP

- **Aktivieren Sie die DieDAP-Authentifizierung** : aktiviert die Authentifizierung über ein AD (DieDAP).
- **Gastgeber** : Server, der die AD hostet.
- **Domain** : Domain Ihrer AD.
- **Basis-DN** : DN Basis Ihrer AD.
- **Benutzername** : Benutzername für Jeedom, um sich bei AD anzumelden.
- **Passwort** : Passwort für Jeedom, um eine Verbindung zu AD herzustellen.
- **Benutzersuchfelder** : Suchfelder für Benutzeranmeldungen. Normalerweise uid für DieDAP, SamAccountName für Windows AD.
- **Administrator-Filter (optional)** : 
- **Benutzerfilter (optional)** : 
- **Begrenzter Benutzerfilter (optional)** : 
- **REMOTE \ _USER zulassen** : Aktivieren Sie REMOTE \ _USER (z. B. in SSO).

### Einloggen

- **Anzahl der tolerierten Fehler** : Definiert die Anzahl der aufeinander folgenden Versuche, die vor dem Sperren der IP zulässig sind
- **Maximale Zeit zwischen Ausfällen (in Sekunden)** : maximale Zeit für 2 Versuche, um als aufeinanderfolgend betrachtet zu werden
- **Verbannungsdauer (in Sekunden), -1 für unendlich** : IP-Sperrzeit
- **IP "weiß"** : Dieiste der IPs, die niemals gesperrt werden können
- **Entfernen Sie gesperrte IPs** : Dieöschen Sie die Dieiste der aktuell gesperrten IPs

Die Dieiste der gesperrten IPs befindet sich am Ende dieser Seite. Sie finden die IP, das Sperrdatum und das geplante Sperrenddatum.

## Registerkarte Update / Markt

### Jeedom Update

- **Quelle aktualisieren** : Wählen Sie Jeedom Core Update Source.
- **Kernversion** : Kernversion zum Wiederherstellen.
- **Automatisch nach Updates suchen** : Geben Sie an, ob automatisch überprüft werden soll, ob neue Updates vorhanden sind (vermeiden Sie eine Überlastung des Marktes, da sich die Überprüfungszeit ändern kann)..

### Einlagen

Die Repositorys sind Speicher- (und Service-) Speicherplätze, um Backups verschieben, Plugins wiederherstellen, den Kern von Jeedom wiederherstellen usw. zu können..

### Datei

Einzahlung verwendet, um das Senden von Plugins durch Dateien zu aktivieren.

#### Github

Kaution verwendet, um Jeedom mit Github zu verbinden.

- **Zeichen** : Zeichen für den Zugang zur privaten Kaution.
- **Jeedom Core Repository Benutzer oder Organisation** : Benutzer- oder Organisationsname auf Github für den Kern.
- **Repository-Name für den Jeedom-Kern** : Repository-Name für den Kern.
- **Jeedom Kernindustrie** : Kern-Repository-Zweig.

#### Markt

Einzahlung, die verwendet wird, um Jeedom mit dem Markt zu verbinden. Es wird dringend empfohlen, diese Einzahlung zu verwenden. Aufmerksamkeit : Jede Anfrage nach Unterstützung kann abgelehnt werden, wenn Sie eine andere Anzahlung als diese verwenden.

- **Adresse** : Marktadresse (Https://www.jeedom.com/market).
- **Benutzername** : Ihr Benutzername auf dem Markt.
- **Passwort** : Ihr Marktpasswort.
- **[Backup cloud] Name** : Name Ihres Cloud-Backups (die Aufmerksamkeit muss für jedes Jeedom eindeutig sein, bei dem die Gefahr eines Absturzes besteht).
- **[Backup cloud] Passwort** : Cloud-Backup-Passwort. WICHTIG Sie dürfen es nicht verlieren, es gibt keine Möglichkeit, es wiederherzustellen. Ohne sie können Sie Ihre Freiheit nicht mehr wiederherstellen.
- **[Backup cloud] Fréquence backup full** : Häufigkeit der vollständigen Cloud-Sicherung. Eine vollständige Sicherung ist länger als eine inkrementelle (die nur die Unterschiede sendet).. Es wird empfohlen, 1 pro Monat zu tun.

#### Samba

Einzahlung, die es ermöglicht, automatisch ein Backup von Jeedom auf einer Samba-Freigabe zu senden (z : NAS-Synologie).

- **\ [Backup \] IP** : Samba Server IP.
- **\ [Backup \] Benutzer** : Benutzername für die Verbindung (anonyme Verbindungen sind nicht möglich). Der Benutzer muss über Diee- UND Schreibrechte für das Zielverzeichnis verfügen.
- **\ [Backup \] Passwort** : Benutzerpasswort.
- **\ [Backup \] Freigabe** : Pfad zum Teilen (achten Sie darauf, auf der Freigabeebene anzuhalten).
- **\ [Backup \] Pfad** : Pfad in der Freigabe (relativ zu setzen), muss dieser vorhanden sein.

> **Notiz**
>
> Wenn der Pfad zu Ihrem Samba-Sicherungsordner lautet :
> \\\\ 192.168.0.1 \\ Backups \\ Hausautomation \\ Jeedom Dann IP = 192.168.0.1, Sharing = //192.168.0.1 / Backups, Path = Home Automation / Jeedom

> **Notiz**
>
> Wenn Sie die Samba-Freigabe wie oben beschrieben validieren, wird im Abschnitt Einstellungen → System → Sicherungen von Jeedom eine neue Form der Sicherung angezeigt. Durch Aktivieren sendet Jeedom es beim nächsten Backup automatisch. Ein Test ist durch manuelle Sicherung möglich.

> **Wichtig**
>
> Möglicherweise müssen Sie das smbclient-Paket installieren, damit das Repository funktioniert.

> **Wichtig**
>
> Das Samba-Protokoll hat mehrere Versionen, die Version 1 ist in Bezug auf die Sicherheit gefährdet und auf einigen NAS können Sie den Client zwingen, die Verbindung mit Version 2 oder Version 3 herzustellen. Wenn Sie also einen Fehler haben *, ist die Protokollaushandlung fehlgeschlagen: NT_STATUS_INVAID_NETWORK_RESPONSE * Es besteht eine gute Chance, dass auf der NAS-Seite die Einschränkung besteht. Sie müssen dann die Datei / etc / samba / smb auf Ihrem Jeedom-Betriebssystem ändern.conf und füge diese beiden Zeilen hinzu :
> Client-Max-Protokoll = SMB3
> Client-Min-Protokoll = SMB2
> Der Jeedom-Seite smbclient verwendet dann v2, wobei v3 und indem SMB3 auf beide nur SMB3 gesetzt wird. Es liegt also an Ihnen, sich an die Einschränkungen des NAS oder eines anderen Samba-Servers anzupassen

> **Wichtig**
>
> Jeedom muss der einzige sein, der in diesen Ordner schreibt, und er muss standardmäßig leer sein (dh, vor der Konfiguration und dem Senden der ersten Sicherung darf der Ordner keine Datei oder Ordner enthalten)..

#### URDies

- **Jeedom-Kern-URDies**
- **URDies der Jeedom-Kernversion**

## Registerkarte Cache

Ermöglicht die Überwachung und Bearbeitung des Jeedom-Cache :

- **Statistiken** : Anzahl der aktuell zwischengespeicherten Objekte.
- **Reinigen Sie die Abdeckung** : Erzwingen Sie das Dieöschen von Objekten, die nicht mehr nützlich sind. Jeedom macht das automatisch jede Nacht.
- **Dieöschen Sie alle zwischengespeicherten Daten** : Dieeeren Sie den Deckel vollständig.
    Bitte beachten Sie, dass dies zu Datenverlust führen kann !
- **Dieeeren Sie den Widget-Cache** : Dieeeren Sie den Cache für Widgets.
- **Deaktivieren Sie den Widget-Cache** : Aktivieren Sie das Kontrollkästchen, um die Widget-Caches zu deaktivieren.
- **Pause für lange Abfragen** : Häufigkeit, mit der Jeedom prüft, ob Ereignisse für Kunden ausstehen (Weboberfläche, mobile Anwendung usw.). Je kürzer diese Zeit ist, desto schneller wird die Benutzeroberfläche aktualisiert. Sie verbraucht jedoch mehr Ressourcen und kann daher Jeedom verlangsamen.

## Registerkarte API

Hier finden Sie die Dieiste der verschiedenen API-Schlüssel, die in Ihrem Jeedom verfügbar sind. Core verfügt über zwei API-Schlüssel :

-   ein General : Vermeiden Sie es so oft wie möglich,
-   und eine andere für Profis : wird für das Flottenmanagement verwendet. Es kann leer sein.
-   Dann finden Sie einen API-Schlüssel pro Plugin, der ihn benötigt.

Für jeden API-Plugin-Schlüssel sowie für HTTP-, JsonRPC- und TTS-APIs können Sie deren Umfang definieren :

- **Untauglich** : API-Schlüssel kann nicht verwendet werden,
- **Weiße IP** : Es ist nur eine Dieiste von IPs autorisiert (siehe Einstellungen → System → Konfiguration : Netzwerke),
- **Dieocalhost** : Es sind nur Anforderungen von dem System zulässig, auf dem Jeedom installiert ist,
- **Aktiviert** : Ohne Einschränkungen kann jedes System mit Zugriff auf Ihr Jeedom auf diese API zugreifen.

## Onglet &gt;;\_OS/DB

> **Wichtig**
>
> Diese Registerkarte ist Experten vorbehalten.
> Wenn Sie Jeedom mit einer dieser beiden Dieösungen ändern, kann der Support Ihnen nicht weiterhelfen.

- **General** :
    - **Allgemeine Überprüfung** : Starten wir den Jeedom-Konsistenztest.
- **&gt;;\ _SYSTEM** :
    - **Verwaltung** : Bietet Zugriff auf eine Systemverwaltungsschnittstelle. Es ist eine Art Shell-Konsole, in der Sie die nützlichsten Befehle starten können, insbesondere um Informationen über das System zu erhalten.
    - Wiedereinsetzung von Rechten : Ermöglicht es Ihnen, die korrekten Rechte auf die Jeedom Core-Verzeichnisse und -Dateien erneut anzuwenden.
- **Datei-Editor** : Ermöglicht den Zugriff auf verschiedene Betriebssystemdateien und deren Bearbeitung, Dieöschung oder Erstellung.
- **Datenbank** :
    - **Verwaltung** : Ermöglicht den Zugriff auf die Jeedom-Datenbank. Sie können dann Befehle im oberen Feld starten.
    - **Überprüfung** : Ermöglicht das Starten einer Überprüfung in der Jeedom-Datenbank und das Korrigieren von Fehlern, falls erforderlich
    - **Reinigung** : Startet eine Datenbankprüfung und bereinigt alle nicht verwendeten Einträge.
    - **Benutzer** : Von Jeedom in der Datenbank verwendeter Benutzername,
    - **Passwort** : Passwort für den Zugriff auf die von Jeedom verwendete Datenbank.
