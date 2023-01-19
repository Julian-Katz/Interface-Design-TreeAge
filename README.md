# Interface Design
Alter von Bäumen bestimmen durch Telegram Bot mithilfe eines Conversational User Interface über den Durchmesser und die Baumart. Dieser soll auf einem ESP32 laufen mit dessen Hilfe soll über einen rotary Encoder der Durchmesser gemessen werden.
## Inhalt
1. Übersicht (diese Seite)
2. [Prototyp](Prototyp.md)
3. [Evaluation Low-Fid Prototyp](Evaluation.md)
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

### Messen des Durchmessers mit ESP32
Der Esp32 soll mit einem Messrad den Umfang des Baumes bestimmen. Hierzu gibt es folgendes [Beispiel](https://www.circuitschools.com/diy-measuring-wheel-using-arduino-and-rotary-encoder/).


