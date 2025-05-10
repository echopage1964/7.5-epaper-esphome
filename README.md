# 7.5-epaper-esphome
Codice per un epaper b/n da 7.5 sotto esphome
Visualizzazione dati su display e-paper con ESPHome
Progetto per ESP32 e display e-ink 7.5, con gestione avanzata del deep sleep e aggiornamento display solo in determinate fasce orarie.

Caratteristiche
Aggiornamento dati da Home Assistant via API o MQTT
Deep sleep notturno "permanente" per evitare consumi inutili
Clean completo del display al primo risveglio mattutino
Ciclo di aggiornamento personalizzabile (es: ogni 20 minuti)
Rotazione automatica delle pagine al risveglio
Hardware utilizzato
Waveshare ESP32 epaper Driver Board V3
Display e-paper Waveshare 7.5 B/N
Modulo di alimentazione senza interruzioni UPS 5V 2A 15w
Batteria Li-Po ricaricabile da 3,7 V 3000 mAh 104050
Cornice Ikea - RÖDALM 13x18
Presa usb da pannello 2 fili
File forniti
epaper-esphome.yaml : configurazione principale ESPHome
script sotto Home Assistant
automazione sotto Home Assitant
input_text input_date sotto Home assistant
Come usare questo progetto
Carica il file YAML su ESPHome.
Personalizza le impostazioni (pinnatura, WiFi, sensori, nomi delle entità).
Compila e flasha il firmware su ESP32.
Aggiungi l'integrazione su Home Assistant, se desiderato.
Configura eventuali automazioni/script per invio dati o aggiornamento.
Deep sleep intelligente
Il dispositivo:

Va in deep sleep profondo di notte (fascia configurabile)
Si risveglia al mattino e fa un "full clean" del display
Durante il giorno si aggiorna ogni 20 minuti
Licenza
MIT (vedi file LICENSE)

Credits
Creato da echopage1964
Ispirato dalla community ESPHome & HA Un sentito grazie a Madelena, Sloma, Debruina e ttuti gli altri utenti della community per il contributo, il codice originale e i vari fork da cui sono partito!
