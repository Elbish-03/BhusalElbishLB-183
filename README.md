# Digitaler Schutzmeister: Praktische Sicherheitskompetenzen in Aktion
**LB-183 Elbish** 

Willkommen zu meinem Portfolio, das meine Erfolge im Modul "Sicherheitsmanagement in der Digitalen Welt" auf den Punkt bringt. Hier erhalten Sie einen schnellen Überblick über meine Leistungen in den Schlüsselbereichen der digitalen Sicherheit. Von der Erkennung aktueller Bedrohungen bis zur Implementierung umfassender Sicherheitsmechanismen – lassen Sie uns gemeinsam durch die wichtigsten Handlungsziele dieses Moduls navigieren.

## Handlungsziel 1

#### Artefakt
Ein Sicherheitsbericht zu aktuellen Bedrohungen in Webanwendungen.
*LA_183_10_Business_Logic (Aufgabe 1)*


#### Nachweis zur Zielerreichung: Sicherheitslücken und deren Ursachen erkennen

Um das Handlungsziel der Erkennung von Sicherheitslücken und deren Ursachen zu erreichen, habe ich eine gründliche Recherche durchgeführt. Das zentrale Artefakt, das diesen Nachweis unterstützt, ist eine Sammlung von verschiedenen Quellen und Artikeln, die ich im Rahmen meiner Studien konsultiert habe.

Die folgenden Quellen repräsentieren einen Ausschnitt meiner Forschung:

- (https://www.akamai.com/de/our-thinking/the-state-of-the-internet/global-state-of-the-internet-security-ddos-attack-reports) 
- (https://www.4net.ch/cyber-bedrohungen-h1-2021-sicherheitsbericht/)

Diese Artikel bieten detaillierte Einblicke in aktuelle Sicherheitsbedrohungen, insbesondere im Hinblick auf DDoS-Angriffe und allgemeine Cyberbedrohungen. Durch das Studium dieser Quellen habe ich meine Fähigkeiten zur Identifizierung von Sicherheitslücken geschärft und ein fundiertes Verständnis für deren Ursachen entwickelt.

#### Erklärung

Das erstellte Artefakt ist ein umfassender Sicherheitsbericht, der sich mit aktuellen Bedrohungen in Webanwendungen befasst. Der Bericht bietet detaillierte Analysen zu verschiedenen Sicherheitsaspekten, einschliesslich Schwachstellen, Angriffsvektoren und möglichen Auswirkungen auf die Sicherheit von Webanwendungen. Die Erklärung beinhaltet eine umfassende Darstellung von Gegenmassnahmen und präventiven Strategien, um die Identifizierung von Sicherheitslücken zu erleichtern und möglichen Bedrohungen effektiv entgegenzuwirken. Dieses Artefakt dient als wertvolle Ressource, um nicht nur Handlungsziel 2 (Sicherheitslücken erkennen und Gegenmassnahmen vorschlagen) zu erfüllen, sondern auch einen ganzheitlichen Einblick in die Sicherheitslandschaft von Webanwendungen zu bieten.


#### Rückblick

Die Umsetzung des Sicherheitsberichts zu aktuellen Bedrohungen ist weitgehend erfolgreich, erfüllt das Handlungsziel der Erkennung von Sicherheitslücken und Gegenmassnahmen. Positiv: gründliche Analyse, präzise Auswirkungsbeschreibung. Verbesserungspotenzial besteht in der Einbindung konkreter Fallstudien für mehr Praxisrelevanz. Zukünftige Optimierungen könnten interaktive Elemente wie Testszenarien einbeziehen, um eine praxisnahe Lernerfahrung zu bieten.


## Handlungsziel 2

#### Artefakt

Ursprünglicher Code
![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/5bdbc4b4-5939-48ec-912b-fc6b864ca0d9)

Verbesserter Code: 


![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/ad58ac9a-e75b-4a22-b3e8-2f461bb37b84)

#### Nachweis zur Zielerreichung

Um das Handlungsziel "Sicherheitslücken und ihre Ursachen erkennen sowie Gegenmassnahmen vorschlagen und implementieren können" zu erreichen, habe ich Sicherheitslücken im ursprünglichen Login-Controller-Code identifiziert und durch verbesserte Praktiken behoben. 


#### Erklärung

In der ursprünglichen Implementierung des Login-Controllers gab es Sicherheitslücken, wie auf dem Bild dargestellt. Insbesondere waren Schwächen in der Überprüfung von Benutzeranmeldedaten, im Umgang mit Anti-CSRF-Massnahmen und im Rate-Limiting vorhanden. Diese Schwachstellen wurden durch eine verbesserte Codebasis behoben, die im Folgenden präsentiert wird.
Verbesserungen:

* Die Überprüfung auf gültige Benutzeranmeldedaten wurde präzisiert.
* Es wurde eine Überprüfung auf ein gültiges Anti-CSRF-Token hinzugefügt.
* Rate-Limiting wurde eingeführt, um zu viele Anfragen zu verhindern.

#### Rückblick

Der überarbeitete Code im Artefakt zeigt Verbesserungen bei der Eingabevalidierung im Login-Controller. Es wurden Sicherheitslücken behoben, wie die Anwendung von MD5 und das Hinzufügen von CSRF-Token-Validierung und Rate Limiting. Dennoch gibt es Raum für weitergehende Verbesserungen, insbesondere bei der Auswahl sicherer Hashing-Algorithmen und umfassenderer Validierung.

![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/afd3e308-690c-4b63-9ef8-5156b4ca5b35)

Für zusätzliche Sicherheit besteht die Möglichkeit, anstelle von MD5 einen sichereren Hashing-Algorithmus wie bcrypt zu verwenden. Dieser Ansatz ermöglicht die Verwendung von zufällig generierten Salts und einer anpassbaren Kostenfunktion, um die Passwortintegrität zu schützen und Brute-Force-Angriffe zu erschweren.


## Handlungsziel 3

#### Artefakt
Die Erweiterung des NewsController um die [Authorize]-Attribute im GetAll-Action-Method.

LoginController.cs
![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/528c82cb-f21f-4e5e-8730-f7abca199935)

NewsController.cs
![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/3db3bb5b-00b6-45d0-9116-e85e26710fc3)

#### Nachweis für Authentifizierung und Autorisierung im NewsController
m Rahmen des Nachweises habe ich dem NewsController einen wesentlichen Sicherheitsaspekt hinzugefügt, indem ich den *Authorize*-Filter implementiert habe, wie im beigefügten Bild dokumentiert. 

#### Erklärung
Das eingeführte Artefakt im NewsController umfasst die Integration des *Authorize*-Attributs beim GetAll-Endpunkt. Durch diese Implementierung wird die Authentifizierung für den Zugriff auf die Liste aller Nachrichten erzwungen. Die Hinzufügung dieser Sicherheitsmassnahme gewährleistet, dass nur authentifizierte Benutzer auf sensible Informationen zugreifen können, was zu einer insgesamt sichereren Anwendung führt.

#### Rückblick

Die Implementierung des *Authorize*-Filters im NewsController ist ein positiver Schritt für die Authentifizierung und Autorisierung. Dieser Filter gewährleistet, dass nur authentifizierte Benutzer auf die Methoden zugreifen können. Es wäre jedoch hilfreich, differenzierte Autorisierung und genauere Kontrolle über Benutzeraktionen in Betracht zu ziehen. Insgesamt bietet der aktuelle Ansatz eine solide Basis, die je nach spezifischen Sicherheitsanforderungen weiter optimiert werden kann.

![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/0031484a-0977-432c-8bdb-ea3d627f1dc0)

Die Integration differenzierter Autorisierung und genauer Kontrolle über Benutzeraktionen in den Code wäre äusserst hilfreich. Durch die Zuweisung granularer Berechtigungen an verschiedene Benutzergruppen kann eine präzise Steuerung des Zugriffs erreicht werden. 

## Handlungsziel 4

#### Artefakt
![image](https://github.com/Elbish-03/BhusalElbishLB-183/assets/78097812/3dfa0d36-e198-4df2-be56-2e00fd2b5982)

#### Nachweis zur Zielerreichung

Ich weise nach, dass ich das Handlungsziel 4 erreicht habe, indem ich eine sichere Implementierung in meiner Sicherheitsarchitektur vorgenommen habe. Das Artefakt, das diese Umsetzung zeigt, ist der Codeabschnitt einer SecurityImplementation-Klasse

#### Erklärung

Die SecurityImplementation-Klasse stellt sicherheitsrelevante Mechanismen für eine Anwendung dar. Hier sind die Schlüsselelemente und wie sie funktionieren:

**IsValidInput-Methode:**
Überprüft, ob die Benutzereingabe gültig ist, indem sie sicherstellt, dass sie nicht null oder leer ist.

**StoreSecurePassword-Methode:**
Speichert ein sicheres Passwort in einer Datenbank oder einem sicheren Speicher und protokolliert das Ereignis.

**LogSecurityIssue- und LogSecurityEvent-Methoden:**
Protokollieren Sicherheitsprobleme und -ereignisse in der Konsole.

**SecureImplementation-Methode:**
Koordiniert sicherheitsrelevante Aktionen, indem sie die Gültigkeit der Benutzereingabe überprüft und bei Erfolg das sichere Passwort speichert. Andernfalls wird ein Sicherheitsproblem protokolliert.

#### Rückblick

**Entwurf:**
Das Artefakt SecurityImplementation erfüllt das Handlungsziel 4, sicherheitsrelevante Aspekte bei Entwurf, Implementierung und Inbetriebnahme zu berücksichtigen, auf mehrere Arten im Entwurf:

*Sicherer Umgang mit externen Bibliotheken*: Im Entwurf wird darauf hingewiesen, dass die Verwendung externer Bibliotheken Sicherheitslücken öffnen kann. Daher wird empfohlen, diese sorgfältig zu prüfen und sicherheitsrelevante Überlegungen zu berücksichtigen.

*Ein- und Ausgabevalidierung*: Die Implementierung von Ein- und Ausgabevalidierung ist bereits im Entwurf verankert. Dies stellt sicher, dass Benutzereingaben auf Konsistenz und Sicherheit überprüft werden, um potenzielle Schwachstellen zu minimieren.

**Implementierung:**
Die Implementierung des Artefakts SecurityImplementation trägt weiterhin dazu bei, das Handlungsziel 4 zu erreichen:

*Minimierung der Arbeit für Entwickler*: Die Struktur der Klasse fördert die Minimierung der Arbeit für Entwickler, indem klare Sicherheitsrichtlinien vorgegeben werden. Dadurch wird die Anwendung von Sicherheitspraktiken erleichtert und menschliche Fehler reduziert.

*Überprüfung von Annahmen*: Die Klasse überprüft Annahmen bezüglich Benutzereingaben und Sicherheitsaspekte. Diese Überprüfung trägt dazu bei, mögliche Schwachstellen frühzeitig zu erkennen und zu verhindern.


## Handlungsziel 5

#### Artefakt
```Csharp
public class UserController : ControllerBase
{
    private readonly ILogger _logger;

    public UserController(ILogger<UserController> logger)
    {
        _logger = logger;
    }

    public ActionResult PasswordUpdate(PasswordUpdateDto request)
    {
        //...
        _logger.LogInformation("changing password of user {0}", user.Username);
        //...
    }
}
```


#### Nachweis zur Zielerreichung

Das Handlungsziel "Informationen für Auditing und Logging generieren. Auswertungen und Alarme definieren und implementieren" wurde erreicht, indem der Logger im UserController implementiert wurde. Der Logger (ILogger<UserController>) wurde verwendet, um Informationen über Passwortaktualisierungen zu protokollieren.

#### Erklärung

Durch die Einbindung des Loggers im Konstruktor des UserController konnte ich effektiv Logging-Funktionalitäten in der Anwendung integrieren. In der PasswordUpdate-Aktion habe ich den Logger genutzt, um wichtige Informationen, wie den Benutzernamen des betroffenen Benutzers, zu protokollieren. Diese einfache Implementierung schafft eine Grundlage für das Generieren von Audit-Informationen und das Protokollieren sicherheitsrelevanter Benutzeraktionen.

#### Rückblick

Die Umsetzung des Artefakts, bei dem der Logger im UserController für das Protokollieren von Passwortaktualisierungen verwendet wird, ist solide. Sie ermöglicht eine grundlegende Protokollierung sicherheitsrelevanter Benutzeraktionen. Jedoch fehlt es an spezifischen Auswertungen, Alarmdefinitionen und einer umfassenden Audit-Trail-Implementierung, wie sie im Handlungsziel gefordert werden.


**Verbesserungsmöglichkeit: Alarmdefinitionen**

Um das Handlungsziel vollständig zu erreichen, wäre es sinnvoll, klare Alarmdefinitionen und Reaktionen auf bestimmte sicherheitsrelevante Ereignisse zu implementieren. Dies könnte durch die Verwendung von ASP.NET Core Middleware erreicht werden, die auf Protokolleinträge reagiert und Alarme auslöst. 

## Selbsteinschätzung des Erreichungsgrades der Kompetenz des Moduls

Insgesamt denke ich, dass ich eine solide Grundlage für die behandelten Themen in diesem Modul aufgebaut habe. Ich habe ein gutes Verständnis für verschiedene Sicherheitslücken entwickelt und kann nun die grundlegenden Konzepte nachvollziehen, um Softwareanwendungen vor verschiedenen Bedrohungen zu schützen. Die praktischen Umsetzungen in den Handlungszielen haben mir geholfen, das Gelernte in die Praxis umzusetzen und weiter zu vertiefen.

Leider konnte ich das letzte Handlungsziel nicht vollständig abschliessen, da ich gegen Ende des Moduls krank wurde. Trotzdem war mir klar, wie die Aufgabe zu lösen wäre, und ich konnte mein Wissen erfolgreich beim Abschlusstest anwenden. Ich fühle mich gut vorbereitet, die erworbenen Kenntnisse in realen Projekten anzuwenden und weiter zu vertiefen.







