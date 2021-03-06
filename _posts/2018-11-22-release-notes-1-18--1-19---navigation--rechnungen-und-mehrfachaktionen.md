---
title: Release Notes 1.18 / 1.19 - Navigation / Rechnungen und Mehrfachaktionen
authors:
  - roland
---

![](/uploads/desktopdekstop.png)
{: .present-before-paste}

Die Versionen 1.18 und 1.19 bringen einige gr&ouml;ssere &Auml;nderungen mit sich: So k&ouml;nnen neu f&uuml;r die Schweiz Rechnungen erstellt werden. Weiter haben wir die Navigation &uuml;berarbeitet, damit man auch auf Mobile besser navigieren kann und dank der Mehrfachselektion k&ouml;nnen f&uuml;r mehrere Personen gleichzeitig Rollen hinzugef&uuml;gt, gel&ouml;scht und verschoben werden.
{: .present-before-paste}

## Rechnungswesen

Neu k&ouml;nnen Rollen, welche die `:finance` Berechtigung haben Rechnungen erstellen. Das wichtigste in K&uuml;rze:
{: .present-before-paste}

* Jede Ebene (Verband, Kanton, Region, Lokalgruppe) hat ihre eigenen (Stamm-)Daten. Ein Kassier vom Dachverband sieht nur die Rechnungen vom Dachverband.
* Rechnungen werden von Einzelpersonen/Personenlisten oder Teilnehmerlisten erstellt. Wenn du eine Rechnung erstellen willst, navigiere zur Person und klicke auf den Button `Rechnung erstellen`. Bei Personenlisten geht die Rechnung an alle ausgew&auml;hlten Personen.

Vielen Dank an dieser Stelle der Pfadi Schweiz, Jungwacht Blauring, Insieme Schweiz und Cevi, welche die Entwicklung des Rechnungsmoduls erm&ouml;glicht haben.
{: .present-before-paste}

Es w&auml;re toll, wenn uns jemand dabei unterst&uuml;tzen k&ouml;nnte, die Anleitung hierzu oder zu anderen Teilen von hitobito auszuarbeiten. Melde dich doch bei [roland@hitobito.com](roland@hitobito.com)
{: .present-before-paste}

## Navigation

![](/uploads/mobilemobile.png)
{: .present-before-paste}

Die Navigation funktioniert jetzt auch gut auf dem Handy. Daf&uuml;r haben wir die Navigation oben und links kombiniert.
{: .present-before-paste}

## Mehrfachaktionen

![](/uploads/multi-actions.gif)
{: .present-before-paste}

Mehrere Personen k&ouml;nnen jetzt ausgew&auml;hlt werden, um deren Rollen zu &auml;ndern (hinzuf&uuml;gen, l&ouml;schen, verschieben). Auch kann man so mehrere ausgew&auml;hlte Personen zu einem Anlass oder Kurs hinzuf&uuml;gen.
{: .present-before-paste}

Hat man Personen ausgew&auml;hlt, werden auch nur diese exportiert und es werden nur zu den ausgew&auml;hlten Personen Rechnung gestellt.
{: .present-before-paste}

## Haushalte zusammenfassen

![](https://content.screencast.com/users/RolandStuder/folders/hitobito/media/ad6850c1-6a3e-48ca-818b-23575421a501/00000036.png)
{: .present-before-paste}

Personen, die in einem Haushalt zusammenwohnen, k&ouml;nnen jetzt verkn&uuml;pft werden. Beim Export kannst du dann w&auml;hlen, ob du auf einer Zeile die Person oder den Haushalt haben m&ouml;chtest.
{: .present-before-paste}

## Mailchimp Integration

Sch&ouml;n formatierte Newslettervers&auml;nde k&ouml;nnen jetzt mit [Mailchimp](https://mailchimp.com/) realisiert werden, du kannst jetzt per Knopfdruck ein Abo mit Mailchimp abgleichen. Zu beachten:
{: .present-before-paste}

* Die MailChimp-Liste wird durch den Export &uuml;berschrieben
* Die MailChimp-Liste wird auf Knopfdruck exportiert, nicht periodisch

Mehr Informationen findest du in der [Dokumentation](https://hitobito.readthedocs.io/de/latest/mailing_lists_mailchimp_export.html).
{: .present-before-paste}

## Weitere &Auml;nderungen

* Alle Personenfilter sind zusammengefasst und lassen sich abspeichern, so k&ouml;nnen auch Rollen- und Qualifikationsfilter jetzt kombiniert werden.
* Personenfilter erlauben den G&uuml;ltigzeitszeitraum einer Rolle einzuschr&auml;nken. Zu beachten: Aufgrund des Berechtigungssystems habt ihr in den meisten F&auml;llen auf Personen mit abgelaufenen Rollen keinen Zugriff mehr.
* Es gibt eine neue Berechtigung `:impersonation`, mit dieser kann man sich als eine andere Person einloggen, praktisch zum Testen und f&uuml;r Support-Personen.
* Bei Mailinglisten kann man w&auml;hlen, an welche E-Mail Adressen einer Person diese verschickt werden soll (basierend auf den vergebenen E-Mail Labels.
* ICAL Kalender Export f&uuml;r Anl&auml;sse
* PDF-Export f&uuml;r Personen
* Grosse Exports werden im Hintergrund heruntergeladen.
* In Teilnehmerlisten kann man jetzt direkt nach bestimmten Personen suchen.
* Anl&auml;sse, welche externe Anmeldung zulassen, k&ouml;nnen jetzt ohne Login angeschaut werden (mit dem direkten Link).
* M&ouml;glichkeit Service API Tokens zu erstellen.
* Technische Information: Ab Version 1.18.9 ben&ouml;tigt die Applikation mindestens Ruby 2.2