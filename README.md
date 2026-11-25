# flobb's turnbinds
# Turnbinds mit anpassbaren Drehgeschwindigkeiten für CS2/CSGO

Diese Config nutzt einen Workaround, um die alten Konsolenvariablen `cl_yawspeed` und `cl_pitchspeed` aus ***Counter-Strike: Source*** in das neueste Spiel der Reihe, ***Counter-Strike 2***, sowie in dessen Vorgänger ***Counter-Strike: Global Offensive*** zu bringen – <ins>ausschließlich mit Konsolenbefehlen</ins>. Außerdem bietet sie eine Vielzahl verschiedener <ins>Binds und Anpassungsmöglichkeiten</ins>, mit denen sich diese längst verloren geglaubten, aber nicht vergessenen Konsolenbefehle voll ausschöpfen lassen.

## Features
### cl_yawspeed
Diese Config ermöglicht es, den **Yawspeed zu ändern**, indem du `cl_yawspeed_[value]` in die Entwicklerkonsole eingibst oder `.cfg`-Dateien ausführst.
>[!IMPORTANT]
>`cl_yawspeed` wird in **Grad pro Sekunde** gemessen und kann auf einen beliebigen ganzzahligen Wert von `1` bis `300` gesetzt werden.

### cl_pitchspeed
Diese Config ermöglicht es, den **Pitchspeed zu ändern**, indem du `cl_pitchspeed_[value]` in die Entwicklerkonsole eingibst oder `.cfg`-Dateien ausführst.
>[!IMPORTANT]
>`cl_pitchspeed` wird in **Grad pro Sekunde** gemessen und kann auf einen beliebigen ganzzahligen Wert von `1` bis `45` gesetzt werden.

### Fixed Binds
**Belege** beliebig viele **Tasten mit verschiedenen** `cl_yawspeed`-/`cl_pitchspeed`-**Befehlen**!  

`bind "[key]" "cl_yawspeed_[value]"`  
`bind "[key]" "cl_pitchspeed_[value]"`

### Toggle/Cycle Binds
- **Wechsle** mit **einer einzigen Taste** zwischen zwei, drei oder vier **verschiedenen** `cl_yawspeed`-**Einstellungen**!
- **Wechsle** mit **einer einzigen Taste** zwischen zwei oder drei **verschiedenen** `cl_pitchspeed`-**Einstellungen**!
- **Kombiniere** Fixed Binds mit Toggle/Cycle Binds, sodass die Fixed Binds **auch den Zyklus-Alias beeinflussen**!
- Setze den `cl_yawspeed`-**Zyklus-Alias** optional **automatisch zurück**, **sobald** du deine **Stage oder deinen Run neu startest**!

### Hold-to-Activate Binds
Hold-to-Activate Binds **müssen gedrückt gehalten werden**, um die `cl_yawspeed`-Einstellung zu ändern.  
**Solange keiner dieser Binds gehalten wird**, ist eine anpassbare Standard-`cl_yawspeed`-Einstellung aktiv.  
Diese Config unterstützt bis zu drei Hold-to-Activate Binds, die zusammen mit der Standardeinstellung bis zu vier verschiedene Geschwindigkeitseinstellungen ergeben.  

>[!IMPORTANT]
>Hold-to-Activate Binds **lassen sich nicht mit** Fixed Binds oder Toggle/Cycle Binds **kombinieren**!

### Visuelles Feedback
- Farbwechsel des **HUDs**
- Farbwechsel des **Fadenkreuzes**
- Farbwechsel von **HUD und Fadenkreuz gleichzeitig**
- 10 verschiedene Farben für alle oben genannten Optionen

>[!NOTE]
>Damit der **Fadenkreuz-Farbwechsel** in ***Counter-Strike: Global Offensive*** funktioniert, musst du die **Datei** `turnbinds\setup\setup.cfg` **bearbeiten**.   
>Weitere Anweisungen findest du in dieser Datei.

### Soundeffekte
- Füge deinen Binds **Soundeffekte** hinzu!
- Wähle aus **21 verschiedenen** Sounds!

>[!NOTE]
>**Jede** Sounddatei aus den Spieldateien von CS2/CS:GO, einschließlich Musik-Kits, **kann** über die Datei `turnbinds\setup\setup.cfg` als Soundeffekt **hinzugefügt werden**.
>Weitere Informationen findest du in dieser Datei.

### Volle Lesbarkeit
**Ich verheimliche hier nichts**. Jede einzelne Config-Datei hat einen eigenen Header, der ihren Zweck erklärt, und ich habe mein Bestes gegeben, damit alles **leicht zu lesen und zu verstehen** ist.

### Volle Anpassbarkeit
In der enthaltenen Datei `turnbinds\settings.cfg` habe ich **viele Anpassungsmöglichkeiten** bereitgestellt, damit du daraus **deine ganz eigene** Config machen kannst. 
Wenn du schon einmal an Counter-Strike-Configs getüftelt hast und selbst weitere Features hinzufügen möchtest, empfehle ich dir außerdem einen Blick in die Datei `turnbinds\setup\setup.cfg`.

## Anleitung
1. Lade die `.zip`-Datei mit den Config-Dateien unter „Releases“ herunter.
2. Entpacke alle Dateien aus dem `.zip`-Archiv.
3. Wähle deine bevorzugte Sprache für die Config-Dateien und öffne den entsprechenden Ordner.
4. Darin findest du den Ordner `turnbinds`. Kopiere diesen Ordner samt seinem gesamten Inhalt nach  
   `[Laufwerk]:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg`
5. Richte die Config über die Datei `settings.cfg` im Ordner `turnbinds` ein.
6. Um die Config auszuführen, gib `exec turnbinds\exec.cfg` in die Entwicklerkonsole ein. Der Screenshot zeigt, wie es danach aussehen sollte.
7. Der Einfachheit halber empfehle ich, den exec-Befehl auf eine Taste zu legen: `bind "[key]" "exec turnbinds\exec.cfg"`
8. Du kannst `exec turnbinds\exec.cfg` auch in deine `autoexec.cfg`-Datei einfügen.

<img width="2160" height="1440" alt="preview_screenshot" src="https://github.com/user-attachments/assets/86c1bc19-dbad-441e-8e74-61ae4351ca24" />

>[!NOTE]
>Deine Konsole **zeigt** beim Start den Bestätigungstext **nicht an**, **wenn du** die autoexec-Methode **verwendest**.

## Warum sollte ich diese Config statt externer Turnbind-Software verwenden?
### Die Vorteile
- Deutlich mehr Möglichkeiten beim Erstellen von Binds
- Visuelles Feedback
- Soundeffekte
- Verwendet ausschließlich Konsolenbefehle
- Einstellungen lassen sich im Spiel über die Entwicklerkonsole ändern

### Der Nachteil
Da `cl_yawspeed` und `cl_pitchspeed` im Spiel nicht tatsächlich als Convars existieren, „emuliert“ diese Config sie, indem sie die Befehle `turnleft`/`turnright` und `turnup`/`turndown` verändert. Der Nachteil ist, dass du die Drehgeschwindigkeit nicht ändern kannst, während du dich drehst. Damit eine Änderung der Drehgeschwindigkeit wirksam wird, musst du die Drehung kurz unterbrechen und danach neu beginnen.

## Besonderer Dank
- an INSPECTRO von Cybershoke

## Cybershoke
<img width="4100" height="475" alt="banner_cybershoke_anthrazit" src="https://github.com/user-attachments/assets/01df9424-7de2-40b0-8295-f4221597aebe" />
Wenn du in CS2 surfen möchtest, empfehle ich dir Cybershoke. Die Server bieten viele Features, die Maps werden gründlich getestet und die Bestenlisten sind hart umkämpft.
