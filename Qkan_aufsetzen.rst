QKan - Step by Step Installation
================================

Willkommen beim Step by Step Tutorial zur Installation von QKan. 
Um QKan auf einem Computer neu einzurichten sind einige Arbeitsschritte notwendig, welche Ihnen im Folgenden vorgestellt werden:

Schritt 1: QGIS Installieren
----------------------------

Da QKan auf der Grundlage des Opensourcprogramms QGIS basiert wird ebendieses Programm im Vorraus benötigt.
Die Aktuelle Version von QGIS finden Sie hier: QGIS_ oder falls dieser Link nicht funktioniert könne Sie manuell www.QGIS.org aufrufen. 

.. _QGIS: http://www.QGIS.org/de/site/forusers/download.html

Die aktuelle Version von QGIS ist Version 2.18.3 (stand Februar 2017). Durch das klicken des "Jetzt herunterladen"-Buttons auf der Startseite werden Sie sofort
zur Downloadseite weitergeleitet. Gehen Sie Vorher sicher, dass Ihnen genügend freier Speicherplatz zur Verfügung steht, da die QGIS-Installation etwa 1,5 GB 
Speicherplatz einnehmen wird. Wählen Sie in Abhänigkeit von Ihrem Betriebssystem und Ihrer Version einen Downloadlink aus. In diesem Beispiel verwenden wir die
unter dem Punkt "Für Windows herunterladen" zu findende Version "Eigenständige QGIS-Installation Version 2.18 (64bit)":

.. image:: .\QKan_Bilder\QGIS_herunterladen.png

Wählen Sie ein entsprechendes Verzeichnis zum Speichern der Installationsdatei und führen Sie diese anschließend aus. Bestätigen Sie die Installation,
aktzeptieren Sie das Lizenzabkommen und wählen anschießend das Verzeichnis in dem QGIS installiert werden soll. Sie können auch einfach auf den Weiter-Button
drücken um es im Standartverzeichnis "C:\\Programme\\QGIS 2.18" zu installieren. Als letzes wird QGIS Sie nach den zusätzlichen Komponenten, wie zum Beispiel
dem North Carolina Data Set fragen:

.. image:: .\QKan_Bilder\QGIS_komponenten.png

Für die Nutzung von QKan wird keine dieser zusätzlichen Komponenten benötigt, sollte QGIS jedoch noch für andere Zwecke genutzt werden, können diese Komponenten
noch Verwendung finden. Beachten Sie, dass sich der benötgte Speicherplatz entsprechend erhöht wenn Sie sich dazu entscheiden die zusätzlichen Komponenten zu 
installieren. Klicken Sie anschließend auf "Installieren" um die Installation zu starten. Diese Installation kann einige Minuten in Anspruch nehmen.

| Wenn Sie alles richtig gemacht haben, sollten Sie folgende Nachricht erhalten:

.. image:: .\QKan_Bilder\QGIS_fertigstellen.png

Herzlichen Glückwunsch, Sie haben nun erfolgreich QGIS installiert! Auf Ihrem Desktop sollte nun ein Verzeichnis mit dem Namen "QGIS 2.18" erstellt worden sein,
in welchem sich mehrere Verknüpfungen befinden. Die, für die Nutzung von QKan verwendete, Verknüpfung heißt "QGIS Desktop 2.18.3 with GRASS 7.2.0". Dabei handelt
es sich um die momentan aktuelle Version. Sollten Sie die Installation zu einem späteren Zeitpunkt durchführen, kann die Versionsnummer abweichen. Um zu testen,
ob QGIS korrekt Installiert wurde, können Sie die vorhin gegannte Anwendung einmal öffnen. Wenn Sich das Programm ganz normal öffnen lässt, hat alles
funktioniert. Doch bevor es mit QGIS weiter geht, wird eine Firebird Datenbank benötigt. Hierzu geht es jetzt weiter mit Schitt 2: Firebird Installieren.

Schritt 2: Firebird Installieren
--------------------------------

Um die Funktionen von QKan verwenden zu können, wird außerdem eine Firebird 2.5.6 Datenbank benötigt. Diese Firebird Datenbank dient zur Bereitsellung, 
Verwaltung und Nutzung von Daten. Einen Link zur Downloadrubrik der Firebirdseite finden sie hier: Firebird_ oder Sie besuchen www.firebirdsql.org und 
wählen dort unter dem Reiter "Downloads" den Punkt Firebird 2.5 aus.

.. _firebird: http://www.firebirdsql.org/en/firebird-2-5-6/
 
Auf der Seite befinden sich änhlich, wie bei der QGIS Installation, wieder mehrere Downloadlinks. Benötigt wird der "installer for Superclassic/Classic or 
Superserver". Wählen Sie auch hier wieder den für Ihr Betriebssystem und Version passenden Link aus. In diesem Beispiel verwenden wir den "Windows executable 
installer for full Superclassic/Classic or Superserver, recommended for first-time users" für Windows 64-bit: 

.. image:: .\QKan_Bilder\firebird_herunterladen.png

Über diesen Link werden Sie zu einem Downloadportal names sourceforge.net weitergeleitet, wo nach wenigen Sekunden der Download starten sollte. Sollte es 
Probleme mit dem Download geben, beachten Sie bitte die Hinweise auf der Seite. Anschließend starten Sie die heruntergeladene Setup.exe. Aktzeptieren Sie auch
hier wieder die Lizenzvereinbarungen. Wählen Sie ein Verzeichnis um Firebird zu speichern oder verwenden Sie das Standartverzeichnis 
"C:\\Program Files\\Firebird\\Firebird_2_5". Gehen Sie nun sicher, dass Sie bei der Installation der Komponenten den Punkt "Super Server Binärdateien" ausgewählt
haben.

.. image:: .\QKan_Bilder\firebird_komponenten.png

Als nächstes wird Firebird einen Startmenü-Ordner anlegen. Dieser wird nicht unbedingt benötigt und kann durch die Checkbox "Keinen Order im Startmenü erstellen"
verhindert werden. Anschließend wird eine Abfrage über die zusätzlichen Aufgaben von Firebird erscheinen. Gehen Sie sicher, dass Ihre Auswahl wie folgt aussieht:

.. image:: .\QKan_Bilder\firebird_aufgaben_anwendung.png

Bevor die Installation fertiggestellt werden kann, werden noch zwei Checkboxen erscheinen:

.. image:: .\QKan_Bilder\firebird_fertigstellen.png

Wenn sie QKan sofort Verwenden möchten können Sie "Firebird jetzt starten?" auswählen. Sie können Firebird aber auch zu einem späteren Zeitpunkt manuell staten.
Der Punkt "After installation - What Next?" bringt Sie zurück auf die Firebirdseite und bietet weitere Informationen zur Nutzung von Firebird. Die zur Nutzung 
von QKan benötigten Informationen bekommen Sie jedoch hier. Um zu testen ob der Firebirdserver auch richitg auf Ihrem System läuft, öffnen Sie den Taskmanager
mit der Tastenkombination strg+shift+esc (bei Windows) und schauen Sie unter dem Reiter Prozesse nach "fbserver.exe". 

Sie haben nun erfolgreich den Firebirdserver auf Ihrem System installiert, um jedoch seine Funktionalitäten nutzen zu können benötigen Sie ein weiters Modul 
für Firebird names "pyfirebirdsql". Dieses Modul wurde von Hajime Nakagami erstellt und steht auf seinem github Verzeichnis zur Verfügung. Einen Link dazu finden
Sie hier: pyfirebirdsql_ oder besuchen Sie www.gihub.com/nakagami/pyfirebirdsql.

.. _pyfirebirdsql: https://github.com/nakagami/pyfirebirdsql    

Dieses Modul wird benötigt, damit die Pythonplugins in QGIS auf die Firebird Datenbank zugreifen können. Sie sollten sich nun auf der folgenden Seite befinden:
 
.. image:: .\QKan_Bilder\pyfirebird_herunterladen.png

Wenn Sie die Seite manuell öffnen achten Sie unbedingt darauf, dass Sie das richtige Modul auswählen. Wenn Sie auf der weiter oben angegebenen Seite angekommen
sind, können Sie durch den "clone or download"-Button die Datei herunterladen. Drücken Sie erst auf "clone or download" und anschließend auf "Dowload ZIP". Dann
führen Sie den Download entsprechend ihrem Browser durch.    

.. image:: .\QKan_Bilder\pyfirebird_dwn.png

Sie erhalten nun eine .zip Datei mit dem Namen "pyfirebirdsql-master" der darin enthaltene Ordner kann jetzt entpackt und anschließend in ein beliebiges
Verzeichnis verschoben werden. Um das Modul zu installieren müssen Sie die "OSGeo4W Shell", eine Art eingebaute Konsole von QGIS, als Administrator ausführen.
Diese finden Sie entweder auf Ihrem Desktop oder im Startmenü Ordner von QGIS.

.. warning:: Achten Sie unbedingt darauf, die "OSGeo4W Shell" als Administrator auszuführen! Da sonst kein Zugirff möglich ist.

.. image:: .\QKan_Bilder\OSGeo4Wexe.png

Geöffnet sieht sie dann etwa so aus:

.. image:: .\QKan_Bilder\OSGeo4Wshell.png

Geben Sie nun mit Hilfe des Befehls "cd" den Pfad zu Ihrem "pyfirebirdsql-master" Ordner an. In diese Beispiel nutzen wir
"C:\\Users\\Christian\\Desktop\\QKan\\install\\pyfirebirdsql-master". Anschließend geben Sie den Befehl "python setup.py install" ein.

.. image:: .\QKan_Bilder\OSGeo4Wshellcd.png

Nachdem QGIS und Firebird erfolgreich auf Ihrem System installiert wurden, können nun die QKan spezifischen Erweiterungen für QGIS geladen werden. 

Schritt 3: QKan Plugins für QGIS
--------------------------------

Als nächstes benötigen Sie die QKan spezifischen Plugins für QGIS. Diese erhalten Sie auf dem github Verzeichnis von Professor Jörg Höttges. Einen Link dazu
finden Sie hier: Höttges_ oder auf github.com/hoettges. Dort finden Sie aktuell vier Plugins (stand  Feburuar 2017) und die extra für die Nutzung optimierten
Eingabemasken. Laden Sie alle Dateien herrunter, welche mit der Bezeichnung "QKan" beginnen. Vorerst widmen wir uns allerdings nur den Plugins: 

.. _Höttges: https://github.com/hoettges

.. image:: .\QKan_Bilder\hoettges.png

Auch diese Ordner erhalten Sie wieder in einem .zip Archiv, welches Sie zuerst entpacken müssen. Um die QKan Plugins in QGIS nutzen zu können müssen diese
erstmal in das Pluginverzeichnis von QGIS verschoben und anschließend in QGIS geladen werden. Die Verzeichnisstruktur von QGIS wird sich automatisch nach
dem ersten Start der Anwendung erstellen, sollten Sie dies in Schritt 1 also noch nicht ausprobiert haben, müssen Sie dies jetzt nachholen. Das Automatisch,
erzeugte Verzeichnis "C:\\Benutzer\\Benutzername\\.qgis2\\python" sollte nun vorhanden sein. In diesem Verzeichnis können nun alle Plugins in einem
Unterverzeichhnis mit dem Namen "plugins" eingefügt werden. Zu diesem Zeitpunkt sollte dieses "plugin" Unterverzeichhnis noch nicht erstellt worden sein. 
Erstellen Sie also ein neues Verzeichnis mit dem Namen "plugins" und legen Sie die vier Plugin Ordner welche Sie von Github heruntergeladen haben dort ab.

.. image:: .\QKan_Bilder\QKan_plugin.png

Das Beispiel findet an Hand der vier ersten QKan Plugins statt: 

.. image:: .\QKan_Bilder\QKan_plugins.png

Anschließend öffnen Sie QGIS mit Hilfe der "QGIS Desktop 2.18.3 with GRASS 7.2.0" Verknüpfung, welche sich im QGIS Ordner auf Ihrem Desktop befinden sollte. 
Wenn Sie QGIS gestartet haben, wählen Sie in der Hauptmenüleiste unter dem Menüpunkt "Erweiterungen" den Unterpunkt 
"Erweiterungen verwalten und installieren..." aus um folgendes Fenster zu öffnen:

.. image:: .\QKan_Bilder\Qgis_erweiterungen.png

Wählen Sie an der linken Seite den Reiter "Installiert" und gehen Sie sicher das an allen neu geladenen Plugins außer "Qkan_Database" das Kästchen ausgewählt ist.
Nun sollten diese drei Plugins in ihrer QGIS Menüleiste zur verfügung stehen.

.. image:: .\QKan_Bilder\Qgis_menue.png

Herzlichen Glückwunsch Sie haben QKan erfolgreich auf Ihren Computer installiert!

(Schritt 4: QKan Eingabemasken für QGIS) - Baustelle


.. _Startseite: index.html	
	
Zurück zur Startseite_.
