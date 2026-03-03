# Hexesoft Bridge Bticino

## Descrizione del Sistema
**Hexesoft Bridge Bticino** è un'applicazione per interfacciarsi con il sistema domotico **BTicino MyHome (bus SCS)**. 
Il software funge da ponte (bridge) tra il gateway fisico Bticino e **Home Assistant**, 
utilizzando il protocollo **MQTT** per la comunicazione.

### Funzionalità Principali
* **Sincronizzazione Automatica**: All'avvio, il sistema pubblica tutti i dispositivi configurati e rimuove automaticamente da Home Assistant quelli eliminati dal file di configurazione.
* **Monitoraggio Real-Time**: Intercetta istantaneamente ogni variazione di stato sul bus SCS e aggiorna Home Assistant tramite MQTT.
* **Controllo Bidirezionale**: Traduce i comandi MQTT in pacchetti **OpenWebNet** per azionare luci, tapparelle e termostati.
* **Monitoraggio Energetico**: Interroga ciclicamente i moduli F520 per riportare potenza istantanea (W) ed energia totale (kWh).
* **Termostati**: Gestione dei termostati diretta senza centrale 99 zone. Possibilità di impostare caldo e freddo per ogni singolo termostato.
* **Pompe e Valvole** Gestione dell'apertura delle valvole comandate dai termostati e della relativa pompa collegata. 

## System Description
**Hexesoft Bridge Bticino** is an application designed to interface with the **BTicino MyHome (SCS bus)** home automation system.
The software acts as a bridge between the physical Bticino gateway and **Home Assistant**,
using the **MQTT** protocol for communication.

### Main Features
* **Automatic Synchronization: On startup, the system publishes all configured devices and automatically removes from Home Assistant those deleted from the configuration file.
* **Real-Time Monitoring: Instantly intercepts every state change on the SCS bus and updates Home Assistant via MQTT.
* **Bidirectional Control: Translates MQTT commands into OpenWebNet packets to operate lights, shutters, and thermostats.
* **Energy Monitoring: Cyclically polls F520 modules to report instantaneous power (W) and total energy (kWh).
* **Thermostats: Direct thermostat management without a 99-zone central unit. Ability to set heating and cooling for each individual thermostat.
* **Pumps and Valves: Management of the opening of valves controlled by thermostats and the related connected pump.