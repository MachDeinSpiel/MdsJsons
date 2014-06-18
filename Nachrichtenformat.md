###Login
**Spieler einloggen**  
```{"mode":"login", "username":"Alice", "password":"s3cur3P4ssw0rd"}```


###Globale Lobby
**Verfügbare Spiele anfordern**  
```{"mode":"gametemplates"}```

**Laufende Spiele anfordern**  
```{"mode":"activegames"}```

**Spiel joinen**  
```{"mode":"join","id":0,"name":"Jason"}```

**Spiel erstellen (Initialspieler)**  
```{"mode":"create","id":0,"name":"Jason", "maxplayers":2}```

###Spiele Lobby
 
**Liste der Spieler anfordern**  
```{"mode":"gamelobby", "action":"players"}```

**Spieler Liste**  
```{"mode":"gamelobby", "action":"players", "players": [ {"name":"Jason", "id":0}, {"name":"Eva", "id":1}]}```

**Spiel starten**  
```{"mode":"gamelobby", "action":"start"}```

**Spieler Eva kicken**  
```{"mode":"gamelobby", "action":"kick", "player":1}```

**Spiel Lobby verlassen**  
```{"mode":"gamelobby", "action":"leave"}```

###Monitoring Tool  

**Monitoring Tool mit Namen "Monitor1" in laufendes Spiel 0 einhängen**  
```{"mode":"monitor", "id":0, "name":"Monitor1"}```


###Fehler Nachrichten  
```{"mode":"error", "message":"This is an error."}```
