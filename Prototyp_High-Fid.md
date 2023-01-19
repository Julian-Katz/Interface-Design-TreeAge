[<- Übersicht](README.md)

# Prototyp 

High-Fid Prototyp Code: [TreeAgeBot Code](https://github.com/Julian-Katz/tree-age)


High-Fid Prototyp Website: [TreeAgeBot Website](https://julian-katz.github.io/tree-age/) **Achtung funktioniert nicht in Safari und mobilen IOS Browsern**
<br>Weitere Infos auf https://caniuse.com/web-bluetooth

## Erkenntnisse aus Low-Fid Prototyp und Evaluation

Beim entwickeln des Telegram Bots auf dem ESP32 kam ich schnell an Grenzen, da die entsprechende Telegram Library einige Telegram Bot Features nicht unterstützt und einige Erkenntnisse aus der Evaluation dadurch schwer umzusetzen waren. Deshalb habe ich nach andern Möglichkeiten für ein Conversational Interface gesucht. 

Hierbei bin ich auf Bluetooth Low Energy (BLE) in einigen Browsern kann auf diese Schnittstelle zurückgegriffen werden, das ermöglicht eine Datenübertragung zwischen ESP32 und Browser welche auch Unabhängig von einer Internet Verbindung funktioniert. Diese Methode hat den Vorteil das ich im Browser quasi keine Grenzen hinsichtlich der Gestaltung und Interaktion gesetzt sind. Der Nachteil ist natürlich das ich nur wenig auf den bereits bestehenden Prototyp aufbauen kann.

In der Umsetzung hat sich vor allem die Browser BLE Schnittstelle als herausfordern erwiesen da sie relativ neu ist und es wenig Dokumentation und Beispiele gibt. Deshalb war am Ende nicht mehr besonders viel Zeit das Conversational Interface welches mit Vue.js umgesetzt wurde bis ins Detail zu gestalten und alle Ergebnisse der Evaluation umzusetzen. Allerdings ist allein durch die Umstellung auf BLE die Nutzung wesentlich einfacher geworden und der Prototyp ausgereifter.    


