# Interface Design - TreeAge
Prototyping eines Chat Bots, um das Alter von Bäumen mithilfe eines Messgerätes auf ESP32 Basis zu bestimmen.

Hier wurde zu Beginn der Ansatz mithilfe eines Telegram Bots gewählt, welcher die Erstellung eines Conversational User Interface erlaubt. Im ersten Ansatz sollte noch die Baumart bestimmt werden. Der Telegram Bot sollte auf einem ESP32 laufen, welcher mit einem rotary encoder Distanz messen soll nach dem Prinzip eines Messrads. Dieser Ansatz wurde beim Low-Fid Prototyp umgesetzt. Beim High-Fid Prototyp gab es noch einige Änderungen.
## Inhalt
1. Übersicht / Ideation (diese Seite)
2. [Prototyp Low-Fid](Prototyp_Low-Fid.md)
3. [Evaluation Low-Fid Prototyp](Evaluation.md)
3. [High-Fid Prototyp](Prototyp_High-Fid.md)
3. [Abschlusspräsentation](https://hsfurtwangende-my.sharepoint.com/:b:/g/personal/julian_david_katz_associate_hs-furtwangen_de/EW8K70f1q8lAo-66Be6UyC4BUQEnLtXCKLpMbrXhbpkbnw?e=rUHhwz)

## Ideation Präsentation

[Präsentationsfolien](https://hsfurtwangende-my.sharepoint.com/:b:/g/personal/julian_david_katz_associate_hs-furtwangen_de/EXZ7ShHWZUJMny61jhGVloQBIIyUjjwOPEB6EzLmJWw9Bg?e=6nlKwi)

Persona: Thomas Thiele

## Baumart bestimmen

Die Baumart zu bestimmen ist relativ komplex, da man entsprechende Daten über jeden Baum braucht und diese dann mithilfe eines Abfrageschemas durchgehen muss um den passenden zu finden. Deshalb werde ich erst mal an der Altersbestimmung arbeiten und wenn später zeitlich noch möglich die Bestimmung der Baumart einbauen. 

## Alter bestimmen

Zu beachtende Parameter: Baumart und Durchmesser

### Faktoren für gängige Baumarten:

**Durchmesser in  cm * <br>**
Eichen und Linden **0,8** <br>
Eiben und Kastanien **0,7** <br>
Buchen, Ahorne (nicht Feldahorn), Tannen, und Ulmen **0,6** <br>
Eschen, Erlen, Fichten, Lärchen, Pappeln, Robinien und Walnussbäumen **0,3** bis **0,5** <br>
Platanen und Esskastanien **0.4**<br>
**= Alter in Jahren**




