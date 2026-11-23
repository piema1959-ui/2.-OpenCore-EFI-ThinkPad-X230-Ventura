# EFI OpenCore per Lenovo ThinkPad X230 - macOS Ventura 13.7.4

Cartella EFI testata e funzionante per eseguire **macOS Ventura 13.7.4** su **Lenovo ThinkPad X230** utilizzando OpenCore.

## Specifiche Hardware Testate
- **Modello:** Lenovo ThinkPad X230
- **Processore:** Intel Core i5-3320M @ 2.60 GHz (Dual-Core, Ivy Bridge)
- **Grafica:** Intel HD Graphics 4000 (1536 MB)
- **Memoria RAM:** 8 GB 1600 MHz DDR3
- **Audio:** Integrato (Input/Output funzionanti)
- **Rete:** Ethernet e Wi-Fi (AirPort) funzionanti
- **SMBIOS configurato:** `MacBookPro14,1` (MacBook Pro 13", 2017, Two Thunderbolt 3 ports)
- **Sistema Operativo:** macOS Ventura 13.7.4

## Stato delle Funzionalità

### Cosa funziona
- [x] **Accelerazione grafica** completa (Intel HD Graphics 4000 1536 MB)
- [x] **Audio** (altoparlanti interni e microfono integrato)
- [x] **Connettività di rete** (Ethernet e Wi-Fi)
- [x] **Input** (Tastiera, TrackPoint e Touchpad)
- [x] **Porte USB**

### Problemi noti / Da verificare
- [ ] **Bluetooth:** Non testato / non funzionante su questa macchina (probabile guasto hardware del modulo Bluetooth sul computer di test).
- [ ] **Stop / Riattivazione (Sleep/Wake):** Non testato a fondo (sul sistema viene utilizzata l'app *Caffeine* per mantenere il computer sempre attivo ed evitare lo stop automatico).

## Note importanti prima dell'uso
1. **Genera i tuoi numeri seriali:** Prima di avviare macOS con questa EFI, apri `EFI/OC/config.plist` con *OpenCore Configurator* o *ProperTree* e genera nuovi valori univoci nella sezione `PlatformInfo -> Generic` (`SystemSerialNumber`, `MLB`, `SystemUUID`, `ROM`) mantenendo lo SMBIOS **MacBookPro14,1**.
2. **Backup:** Effettua sempre una copia di sicurezza della tua cartella EFI funzionante su una chiavetta USB avviabile prima di applicare modifiche.

