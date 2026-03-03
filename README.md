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

