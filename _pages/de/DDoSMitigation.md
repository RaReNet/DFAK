---
layout: page
title: "DDoS Eindämmung"
author: RaReNet JC, EG, DV, TL, others
language: de
summary: ""
date: 2015-08
permalink: /de/DDoSEindammung/
redirect_from: /de/DDoSMitigation/
parent: Home
---

# DDoS Eindämmung

Eine Bedrohung, der sich zahlreiche unabhängige Journalisten, neue Websites und Blogger ausgesetzt sehen, besteht darin, dass sie durch ihre nicht mehr zugänglichen oder verunstalteten Websites "mundtot" gemacht werden. In vielen Fällen kann dies ein harmloses und frustrierendes technisches Problem sein, doch manchmal kann es sich auch um einen ‚Denial of Service (DoS)'-Angriff oder eine Website-Übernahme handeln. Dieser Abschnitt des Digitalen Erste-Hilfe-Sets führt Sie durch einige grundlegende Schritte zur Diagnose potenzieller Probleme. Wenn Ihre Website von einem Denial of Service-Angriff betroffen ist, schlagen wir einige Optionen für unverzüglich auszuführende Schritte vor.

Es ist generell wichtig zu wissen, dass es unterschiedliche Gründe dafür geben kann, warum Ihre Website nicht mehr zugänglich ist. Meistens hängt dies mit Programmierfehlern oder technischen Problemen bei dem Unternehmen zusammen, das das Hosting der Website übernimmt. Manchmal können andere Dinge wie Anfechtungsklagen einen Webhoster veranlassen, Ihre Website zu sperren. Das Problem und eventuelle Lösungen für das Problem Ihrer Website ausfindig zu machen, kann mühselig werden, wenn Sie keine Hosting-Erfahrung haben. Deshalb ist es zunächst am sinnvollsten, wenn möglich eine vertrauenswürdige Person zu kontaktieren, die Ihnen bei Ihrer Website helfen kann (Ihr Webmaster, Menschen, die Ihnen beim Aufbau Ihrer Website geholfen haben, Ihr eigenes Personal, sofern vorhanden, und das Unternehmen, das Ihre Website hostet; falls keine dieser Alternativen verfügbar ist, [suchen Sie Hilfe bei einer Organisation, der Sie vertrauen](https://github.com/CIRCL/circl.lu/blob/master/web/circl/content/pub/dfak/SecureCommunication.md#seeking-and-providing-remote-help) ).

Es empfiehlt sich, _Ihren Webmaster und den Webhoster Ihrer Website zu kontaktieren,_ nachdem Sie die nachfolgenden allgemeinen Informationen ermittelt haben! Das Problem, mit dem Sie konfrontiert sind, wurde möglicherweise nicht auf ihrer Statusseite angezeigt, ist eventuell ein vorübergehendes Problem oder der Webhoster Ihrer Website weiß noch gar nichts von dem Problem. Eine gute Beziehung zu Ihren Providern baut sich nur langsam auf – seien Sie deshalb klar und höflich und teilen Sie ihnen die Ergebnisse Ihrer Recherchen mit, indem Sie folgende Fragen nutzen, deren Antworten ihnen helfen werden, die Gründe für das Problem schnell zu finden.

## Beginnen Sie mit der Beantwortung einiger einfacher Fragen:

### Basis-Informationen

- Wer hat die Website erstellt? Können diese Leute helfen?
- Wer ist Ihr Webhoster? Das ist das Unternehmen, das den Server zur Verfügung stellt, auf dem Ihre Website läuft. Wenn Sie es nicht wissen, finden Sie auf einer Website wie http://www.whoishostingthis.com/ Hilfe.
- Haben Sie die Login-Details für Ihren Account bei diesem Webhoster?
- Wo haben Sie Ihren Domain-Namen gekauft? In einigen Fällen ist das auch Ihr Webhoster, es kann aber auch ein anderes Unternehmen sein.
- Haben Sie die Login-Details für den Domainnamen-Service? Falls nicht, ist dies der erste Schritt, um Ihre Website wiederzubekommen.
- Wer kennt diese Account-Details sonst noch oder hat Zugang zu ihnen?

### Diagnose-Informationen

Es kann unterschiedliche Gründe dafür geben, warum Ihre Website nicht mehr zugänglich ist. Dies kann vom Netzwerk über Bestimmungen von Richtlinien, Webhosting und Blockaden bis hin zu Problemen mit der Software, Verunstaltungen und der Leistung reichen. Der nachfolgende Abschnitt erklärt, worin jedes dieser Probleme besteht und wie Sie für das Problem, mit dem Sie konfrontiert sind, eine Diagnose erstellen können.

- Funktioniert Ihr Webhosting, aber Ihre Website ist nicht erreichbar? Überprüfen Sie http://www.isup.me/ – Ihre Website ist möglicherweise geöffnet, aber Sie können sie nicht sehen. Es handelt sich um ein Netzwerk-Problem. Ihre eigene Internet-Verbindung könnte Probleme haben oder Ihren Zugang zu Ihrer Website blockieren. Es könnte auch ein Zeichen dafür sein, dass Ihr Account deaktiviert wurde: Sehen Sie eine entsprechende Mitteilung von Ihrem Webhoster? Sie könnten aus Inkasso-, Rechts-, Copyright- oder anderen Gründen offline gestellt worden sein. Es handelt sich um ein Richtlinien-Problem. Stellen Sie zunächst sicher, dass Ihre Informationen über Ihre Rechnungen aktuell sind und keine Beträge für das Webhosting und den Domain-Namen offen sind. Wenn das Problem mit rechtlichen Fragen zusammenhängt, sind die von der Organisation EFF (Electronic Frontier Foundation) zur Verfügung gestellten Informationen, die sich allerdings auf das US-amerikanische Urheberrecht konzentrieren, eine gute Möglichkeit, mehr zu erfahren: https://www.eff.org/issues/bloggers/legal/liability/IP.
- Wird Ihre Website überhaupt nicht geladen? Möglicherweise hat Ihr Webhoster Probleme; in diesem Fall haben Sie es mit einem Hosting-Problem zu tun. Können Sie auf die Website Ihres Webhosters gehen? Bitte beachten Sie, dass das nicht die Admin-Ebene Ihrer eigenen Website ist, sondern die Website der Firma oder der Organisation, die Ihre Website hostet. Suchen Sie einen 'Status'-Blog (z.B. status.dreamhost.com); suchen Sie auch auf Twitter.com nach anderen Usern, die über den Ausfall bei Ihrem Webhoster diskutieren – eine simple Suche wie '(Name des Unternehmens) Absturz' zeigt oft, ob andere das gleiche Problem haben.
- Können Sie andere Websites mit ähnlichem Inhalt wie dem Ihren besuchen? Versuchen Sie, Websites zu besuchen, die ähnliche Inhalte aufweisen oder verwandte Themen behandeln. Versuchen Sie auch, Tor (https://www.torproject.org/projects/gettor.html) oder Psiphon (https://psiphon.ca/products.php) zu benutzen, um auf Ihre Website zu gelangen. Falls das hilft, haben Sie ein Blockade-Problem – Sie sind für andere Teile der Welt immer noch online, wurden jedoch in Ihrem eigenen Land zensiert.
- Sehen Sie Fehlermeldungen? Dann könnte es sich um ein Software-Problem handeln. Sie sollten darüber nachdenken, ob Sie oder Ihr Team in letzter Zeit Veränderungen vorgenommen haben und Ihren Webmaster kontaktieren. Senden Sie Ihrem Webmaster einen Screenshot, den Link zu der Seite, mit der Sie Probleme haben, sowie alle Fehlermeldungen, die Sie sehen; all das wird ihm helfen herauszufinden, was das Problem verursachen könnte. Sie könnten auch die Fehlermeldungen in eine Suchmaske kopieren, um zu sehen, ob das Problem einfach zu beheben ist.
- Sehen Sie eine Website, die nicht die Ihre ist? Erhalten Sie eine Warnmeldung von Ihrem Browser über Schadprogramme auf Ihrer eigenen Seite? Dann könnte es sich um ein Verunstaltungs-Problem handeln. Sie finden unten die weiteren auszuführenden Schritte; Sie werden mit Ihrem Webhoster zusammenarbeiten und den Bereich Account-Diebstahl überarbeiten müssen.
- Lädt Ihre Website mit Unterbrechungen oder ungewöhnlich langsam? Ihre Website könnte durch die Anzahl und die Geschwindigkeit der Seitenanfragen, die sie erhält, überlastet sein – das ist ein Leistungs-Problem. Dies könnte insofern 'gut' sein, da Ihre Website beliebter geworden ist und einfach einige Verbesserungen benötigt, um mehr Nutzer verkraften zu können – überprüfen Sie Ihre Website-Statistiken über einen längeren Zeitraum. Kontaktieren Sie Ihren Webmaster oder Webhoster, um sich beraten zu lassen. Viele beliebte Blog- und CMS-Plattformen (Joomla, Wordpress, Drupal und andere) haben Plugins, um Ihre Website lokal auf einem Cache zwischenzuspeichern und ein Content Delivery Network (CDN) zu integrieren, das die Leistung und Belastbarkeit der Website drastisch verbessern kann. Zahlreiche der unten dargestellten Lösungen können auch bei Leistungsproblemen helfen.

## Erste Schritte, um das Problem zu beheben:

### Wenn Sie es mit einem Denial of Service-Angriff zu tun haben

Wenn die oben genannten Diagnosen nicht helfen (da Sie ein gravierendes _Leistungs-Problem_ feststellen), könnte Ihre Website Opfer eines of a '_Denial of Service_'_-Angriffs_ sein, bei dem ein (oder mehrere) böswillige(r) Nutzer versuchen, die Website wiederholt und schnell (unter Verwendung automatisierter Tools) anzusehen und so legitime Besucher der Seite zu verdrängen. Manchmal versucht ein 'Angreifer' dies auf Ihrer Website, was normalerweise kein allzu großes Problem darstellt – abgesehen davon, dass es Übertragungskapazität blockiert. Häufiger ist der 'Distributed' denial of Service (DDoS), bei dem ein Angreifer tausende unter seiner Kontrolle stehende Computer benutzt, um eine Website anzugreifen.

- Schritt 1: Kontaktieren Sie eine vertrauenswürdige Person, die Ihnen mit Ihrer Website helfen kann (Ihr Webmaster, Menschen, die Ihnen beim Aufbau Ihrer Website geholfen haben, Ihr eigenes Personal, sofern vorhanden, und das Unternehmen, das Ihre Website hostet).
- Schritt 2: Arbeiten Sie mit dem Unternehmen zusammen, bei dem Sie Ihre Domain gekauft haben (etwa EasyDNS, Network Solutions, GoDaddy), und verändern Sie die 'Time to Live' oder TTL auf 1 Stunde. Dies kann Ihnen dabei helfen, Ihre Website sehr viel schneller umzuleiten, sobald sie angegriffen wird (der Standard ist 72Stunden oder drei Tage). Diese Einstellung findet sich oft unter 'erweiterte' Eigenschaften für Ihre Domain, manchmal ist sie Teil des SRV oder Service Records.
- Schritt 3: Überstellen Sie Ihre Website einem DDoS-Eindämmungs-Dienst. Eine Komplette Liste finden Sie unter https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services. Sie können es zunächst versuchen bei:
  - ca
  - Google's Project Shield
  - CloudFlare's Project Galileo

- Schritt 4: Sobald Sie die Kontrolle wiedererlangt haben, überprüfen Sie Ihren Bedarf und entschieden Sie sich, ob Sie zu einem sicheren Webhoster wechseln oder einfach mit Ihrem DDoS-Eindämmungs-Service weitermachen möchten.

### Wenn Sie von einer Website-Verunstaltung betroffen sind

- Schritt 1: Stellen Sie sicher, dass es sich tatsächlich um eine böswillige Übernahme Ihrer Website handelt. Eine unselige, aber legale Praxis stellt der Kauf von kurz zuvor abgelaufenen Domainnamen dar, um den Besucherverkehr zu 'übernehmen' und für Werbeangebote zu nutzen. Es ist sehr wichtig, mit den Zahlungen für Ihren Domainnamen nicht in Verzug zu geraten.
- Schritt 2: Wenn Ihre Website verunstaltet wurde, erlangen Sie zunächst die Kontrolle über den Login-Account Ihrer Website wieder und ändern das Passwort, weitere Hilfe finden Sie dann im Abschnitt „Account-Diebstahl".
- Schritt 3: Erstellen Sie ein Backup der verunstalteten Website, das später bei der Nachforschung nach den Urhebern der Verunstaltung hilfreich sein kann.
- Schritt 4: Stellen Sie Ihre Website vorübergehend offline – benutzen Sie dazu eine simple Landingpage oder eine 'Parkseite'.
- Schritt 5: Stellen Sie fest, wie die Website gehackt wurde. Dabei kann Ihnen womöglich Ihr Webhoster helfen. Verbreitete Probleme sind ältere Teile Ihrer Website mit benutzerdefinierten Scripts/Tools, die auf ihnen laufen, veraltete Content-Management-Systeme und benutzerdefinierte Programme mit Sicherheitslücken.
- Schritt 6: Stellen Sie Ihre Original-Website auf der Basis der Backups wieder her. Wenn weder Sie noch Ihr Webhoster über Backups verfügen, werden Sie Ihre Website von Grund auf neu aufbauen müssen! Sie sollten auch beachten, dass Angreifer, falls sich Ihre einzigen Backups bei Ihrem Webhoster befinden, möglicherweise in der Lage sind, die Backups zu löschen, wenn sie die Kontrolle Ihrer Website übernehmen!
- Schritt 7: Wechseln Sie zu einem zu einem DDoS-Eindämmungs-Service oder sicheren Webhoster. Deflect.ca kann Ihnen dabei helfen, Ihre Website gegen Angriffe aus dem Internet zu schützen. CloudFlare kann auch zahlreiche der häufigsten Angriffe abblocken. Sichere Webhoster wie VirtualRoad/Qurium bemühen sich intensiv darum, solche Angriffe aufzuspüren und zu verhindern.

## Hören Sie an dieser Stelle nicht auf! Weitere wichtige Schritte folgen

_Warten Sie nicht, bis Sie angegriffen werden!_ Alle unten aufgeführten Dienste arbeiten schnell, um Ihnen dabei zu helfen, Ihre Website während oder nach einem Angriff zu retten – doch Sie können sich selbst schützen, bevor sich ein Angriff ereignet! Dies kann Kosten reduzieren, da die Beanspruchung Ihrer Übertragungskapazität gesenkt wird, und Sie Während eines Angriffs online halten. Sobald der Angriff Sie trifft, kann das Internet bis zu drei Tagen benötigen, um Sie auf Ihrer neuen, geschützten Adresse 'wiederzufinden' – deshalb ist es in nahezu jedem Fall besser, _vorbereitet zu sein und damit jetzt gleich zu beginnen_.

1. Sichere Webhoster verlangen von Ihnen, Ihre gesamte Website auf ihre Server zu überstellen – Sie wechseln also Ihren Webhoster. Viele Anbieter können Ihnen dabei helfen. Zu den Vorteilen eines solchen Wechsels gehört unter anderem, dass die Hosting-Lösung abgesehen von der DDoS-Eindämmung zahlreiche weitere Schutzfunktionen bietet; zu den Nachteilen können höhere Kosten (das hängt davon ab, was Sie derzeit bezahlen) und weniger Kontrolle gehören – Sie müssen Ihrem Domain-Hoster vertrauen können, da er eine umfangreiche Kontrolle über Ihre Website besitzt.
  - Pro:
    - Bietet einen zentralen Service für die meisten, wenn nicht für alle Bedürfnisse Ihre Website an
    - Bietet einen Schutzservice gegen DDoS, Hacking- und Spam-Angriffe
    - Bietet oft zahlreiche zusätzliche Services und Beratung, und in einigen Fällen sogar beschränkten Rechtsschutz
    - Komplette Support-Teams stehen oft für unmittelbare Hilfe bereit

  - Contra:
    - Sie müssen Ihre Website bei diesem Service hosten
    - Sie müssen dem Service dabei vertrauen, Ihre Website zu managen und Ihre Rechte zu verteidigen
    - Diese Services sind oft sehr viel teurer (doch Sie müssen keinen anderen Webhoster/DNS-Provider mehr bezahlen!)

2. Mit DDoS-Eindämmungs-Dienste können Sie Ihre Website weiterhin bei dem Webhoster belassen, bei dem sie sich befindet; sie ändern lediglich die Art, wie andere im Internet Ihre Website finden und auf sie zugreifen können – das ist im Allgemeinen sehr viel einfacher durchzuführen. Diese Dienste verfügen über Server überall in der Welt, die vor Ihrer Website agieren und schädlichen Datenverkehr absorbieren oder ignorieren. Sie 'spiegeln' und speichern ständig aktualisierte Kopien Ihrer Website. Diese Dienste sind einfach zu installieren und Sie behalten die vollständige Kontrolle über Ihre Website und Ihre Hosting-Einstellungen. Eine Herausforderung bei der Zusammenarbeit mit beauftragten Diensten ist, dass bei sehr komplexen Websites manchmal Probleme mit nicht-Admin Nutzer-Logins und komplexen interaktiven/Javascript-Bereichen auftreten können. Bitte besprechen Sie diese Fragen mit Ihrem Webmaster und dem beauftragten Dienst, da die meisten dieser Probleme behoben werden können.
  - Pro:
    - Niedrigere Kosten (oft mit einem kostenlosen Schutzlevel)
    - Schnell und einfach zu installieren
    - Sie müssen Ihren derzeitigen Webhoster nicht wechseln
    - Sie können den Dienst jederzeit ändern oder verlassen

  - Contra:
    - Weniger Support-Optionen
    - Konzentriert sich vor allem darauf, DDoS-Angriffe lediglich einzudämmen – umfasst nicht zwingend Hilfe bei Schadprogrammen oder Spams.
    - SSL-verschlüsselter Verkehr wird vom Proxy-Server kurz entschlüsselt und wieder verschlüsselt, um ihn vom Proxy- auf Ihren Server zu leiten.

3. Wählen Sie den Anbieter gezielt aus – ganz gleich für welchen Dienst: Sie müssen mit dem Anbieter zufrieden sein. Das hat mit Vertrauen zu tun, aber auch mit dem jeweiligen Geschäftsmodell: Erfolgt die Abrechnung nach Einzelleistungen? Falls es eine Gratisversion gibt – bietet sie weniger Support als die kostenpflichtige Version? Wird der Anbieter von Regierungen unterstützt? Es ist das Beste, im Vorfeld so viele Details wie möglich zu klären, um später unliebsame Überraschungen zu vermeiden.

### Stellen Sie sich bei allen Anbietern die folgenden Fragen:

- Wie ist das Unternehmen/die Organisation strukturiert und von wem wird sie getragen? Welche Art von Kontrollen und Berichten müssen sie – wenn überhaupt – erstellen?
- Beachten Sie, in welchem Land/welchen Ländern der Anbieter eine Niederlassung unterhält und ob er verpflichtet ist, Weisungen von Vollzugsbehörden und anderen rechtlichen Bestimmungen Folge zu leisten.
- Welche Protokolle werden erstellt und für wie lange sind sie zugänglich?
- Gibt es Beschränkungen hinsichtlich der Art des Inhalts, den der Dienst hosten/weiterleiten wird, und könnten diese Auswirkungen auf Ihre Website haben?
- Gibt es Einschränkungen hinsichtlich der Länder, in denen der Dienst verfügbar ist?
- Akzeptiert der Anbieter eine Zahlungsart, die für Sie zugänglich ist? Können Sie sich den Dienst leisten?
- Sichere Kommunikation – Sie sollten sich sicher einloggen und mit dem Anbieter vertraulich kommunizieren können.
- Gibt es eine Zwei-Faktor-Authentifizierung, um die Sicherheit des Administrator-Zugangs zu erhöhen? Diese oder andere sichere Zugangsarten können dabei helfen, die Bedrohung durch andere Arten von Angriffen auf Ihre Website zu verringern.
- Welche Art von fortlaufendem Support wird für Sie zugänglich sein? Entstehen zusätzliche Kosten für Support und/oder erhalten Sie ausreichenden Support, wenn Sie eine kostenfreie Version nutzen?
- Können Sie einen 'Testlauf' Ihrer Website machen, bevor Sie über eine Staging-Website online gehen?

### Fragen an sichere Webhoster

- Bieten sie einen kompletten Support bei der Überstellung Ihrer Website auf ihren Dienst an?
- Ist der Dienst ebenso gut oder besser im Vergleich zu Ihrem derzeitigen Webhoster, zumindest hinsichtlich der Werkzeuge/Services, die Sie nutzen? Hier die wichtigsten Dinge, die Sie überprüfen sollten:
  - Management-Dashboards wie cPanel
  - E-Mail-Accounts (wie viele, Kontingente, Zugang über SMTP, IMAP)
  - Datenbanken (wie viele, welche Arten, Zugang)
  - Fernzugriff über SFTP/SSH
  - Support für die Programmiersprache (PHP, Perl, Ruby, Cgi-bin-Zugang ...) oder CMS (Drupal, Joomla, Wordpress …), die Ihre Seite benutzt.

### Fragen an DDoS-Eindämmungs-Dienste:

- Falls Sie SSL (auch bekannt unter HTTPS oder Sicherer Web-Datenverkehr) benutzen, fragen Sie, wie sie SSL verwalten. Bei gewissen Konfigurationen kann es das Einfachste sein, Ihren privaten SSL-Schlüssel zu teilen. In diesem Fall müssen Sie großes Vertrauen zu Ihrem Anbieter haben, da er Ihre Website 'imitieren' kann (das ist allerdings genau das, worum Sie ihn bitten, wenn er Ihnen einen Proxy-Server zur Verfügung stellt!).
- Fragen Sie, wie die Administrations-/Bearbeitungs-Logins verwaltet werden.
- Sprechen Sie über die interaktiven Teile Ihrer Website (Nutzer, die sich einloggen, kommentieren, Administrations-/Bearbeitungs-Anforderungen, komplexe interaktive Seiten /Javascript/Animationen) – jeder Proxy-Anbieter verwaltet diese Elemente auf seine Weise; Sie werden dies testen müssen, ehe Sie komplett umstellen.

### Besondere Eindämmungs-Dienste

Besondere Dienste sind mit ausführlichen Beschreibungen aufgelistet auf [https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services). Bitte beachten Sie, dass die dort zusammengestellte Liste keine komplette Aufstellung aller Dienste ist; es gibt noch zahlreiche weitere. Jedoch stellen diese Dienste einen guten Ausgangspunkt dar, da sie bereits von anderen Mitgliedern von unabhängigen Medien / Menschenrechtsorganisationen / Verfechtern der Meinungsfreiheit benutzt wurden. Hier einige Optionen für eine sofortige Absicherung:

-     Sichere Webhoster:
  - Qurium (früher Virtual Road)
  - Das Unternehmen Positive Internet
  - Greenhost

- DDoS-Eindämmungs-Dienste:
  - ca
  - Project Shield von Google
  - Das Projekt Galileo von CloudFlare

## Ergreifen Sie zusätzliche Vorsichtsmaßnahmen gegen Angreifer:

Auch wenn Sie noch keine Erfahrungen mit einem Denial-of-Service-Angriff gemacht haben, zeigt Ihnen dieses Handbuch einige Schritte, wie Sie sich auf einen Angriff vorbereiten können – in der Hoffnung, jede Ausfallzeit im Vorfeld zu verhindern. Gehen Sie direkt zum Abschnitt [Responding to a Denial of Service Attack](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#responding-to-a-denial-of-service-attack) und erfahren Sie mehr über gängige Lösungen, die Sie sofort anwenden können, noch bevor Sie angegriffen werden. Im Abschnitt Hilfreiche Hinweise finden Sie Anleitungen, wie Sie Ihre Website am Laufen halten können.

- Backups: Es ist immer gut, sicherzustellen, dass Sie Backups gemacht haben (die Sie an einem anderen Ort speichern als dort, wo sich Ihre Website befindet!). Viele Webhoster und Website-Plattformen bieten Backups als integrierten Teil ihres Services an, doch es ist das Beste, auch zusätzliche Offline-Kopien zu haben.
- Auf dem neuesten Stand bleiben: Wenn Sie ein Content-Management-System (CMS) wie WordPress oder Drupal benutzen, stellen Sie sicher, dass Ihre Website auf dem neuesten Stand der Software ist, besonders wenn es Sicherheits-Updates gibt. Wenn Sie eine gebräuchliche Software benutzen, denken Sie daran, zu einem CMS zu wechseln, das regelmäßige Updates erhält.
- Monitoring: Es gibt viele Dienste, die Ihre Website ständig überprüfen und Sie per E-Mail oder Textmitteilung benachrichtigen können, wenn Ihre Seite blockiert ist. Dieser Mashable-Artikel listet zehn beliebte Diensteauf. Achten Sie darauf, dass die E-Mail-Adresse oder Telefonnummer, die Sie für die Kontrolle verwenden, klar dem Management Ihrer Website zugeordnet ist.

## Recherchieren Sie

Wenn Sie Opfer eines _'Denial of Service'-_ oder _Verunstaltungs-Angriffs_ geworden sind, kann es wertvoll sein zu verstehen, warum Sie angegriffen wurden und warum gerade jetzt.

Warum wurden Sie angegriffen und warum gerade jetzt: Wer könnte Ihrer Meinung nach ein Interesse daran haben, Ihre Website oder Ihr Unternehmen ins Visier zu nehmen? Haben Sie in letzter Zeit etwas Umstrittenes gepostet oder könnte diese Bedrohung mit Ihrer Arbeit in Zusammenhang stehen oder verzeichnet Ihre Website viel Verkehr und ist Ihr Domainname abgelaufen? Warum gerade jetzt? Kann eine kürzlich auf Ihrer Website vorgenommene Veränderung sie zu einem Ziel für 'Denial of Service'- oder Verunstaltungs-Angriffe gemacht haben? Im Abschnitt Hilfreiche Hinweise finden Sie Links zu Anleitungen, die Ihnen Tipps und Tricks zeigen, wie Sie digitale Notfälle vermeiden und für Ihre digitale Sicherheit präventiv aktiv werden können.

## Hilfreiche Hinweise:

- My Website is Down: https://github.com/OpenInternet/MyWebsiteIsDown
- Keep your site alive: https://www.eff.org/keeping-your-site-alive
- Security in a Box: https://securityinabox.org/en/chapter\_7\_2
- Bedrohungsmodelle, Surveillance Self Defense Guide: https://ssd.eff.org/risk/threats
