# Campo Volo Mini

Simulatore 3D nel browser per allenarsi a pilotare un DJI Mini 2.
Il drone si comporta come un DJI in modalità GPS: gli stick chiedono una velocità e, quando li lasci, il drone frena e resta fermo in hovering.

Non è un prodotto DJI e non è affiliato a DJI. La fisica è approssimata: serve per fare pratica con gli stick, non come replica esatta del drone.

## Come si usa

Apri `index.html` in Chrome (o in un altro browser moderno), oppure usa la versione online su GitHub Pages.
Serve una connessione internet al primo avvio, per scaricare il motore 3D (Three.js) e i caratteri.

## Funzioni

- Modalità Cine, Normal e Sport con le velocità del Mini 2 (6, 10 e 16 m/s)
- Mode 2 (predefinito DJI) o Mode 1
- Decollo, atterraggio e ritorno a casa automatici
- Avvio manuale dei motori con gli stick in basso (CSC)
- Vento con raffiche, batteria simulata, collisioni
- Tre viste: dietro al drone, camera del drone, dal pilota
- Percorso di allenamento: cerchio di coni, slalom di pali, porta

## Comandi

| Azione | Controller / Steam Deck | Tastiera |
|---|---|---|
| Gas e rotazione | Stick sinistro | W S · A D |
| Avanti e laterale | Stick destro | Frecce |
| Decollo / atterraggio | A | T |
| Ritorno a casa | Y | H |
| Annulla automatismo | B | B |
| Cambia vista | X | C |
| Modalità di volo | LB · RB | 1 2 3 · M |
| Gimbal | LT · RT | Q · E |
| Riparti | Start | R |
| Impostazioni | View / Select | P · Esc |

## Steam Deck

Apri la pagina in Chrome avviato dalla modalità Gioco, con layout controller "Gamepad".
Se il browser non vede il controller, da Konsole in modalità Desktop:

```
flatpak --user override --filesystem=/run/udev:ro com.google.Chrome
```

## Tecnologia

Un solo file HTML con JavaScript, grafica 3D con [Three.js](https://threejs.org) r128.

## Licenza

Rilasciato con licenza [MIT](LICENSE).
