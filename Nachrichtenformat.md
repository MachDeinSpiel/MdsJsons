###Login
**Spieler einloggen**  
```{"mode":"login", "username":"Alice", "password":"md5-Passwort"}```


###Globale Lobby
**Verfügbare Spiele anfordern**  
```{"mode":"gametemplates"}```

**Laufende Spiele anfordern**  
```{"mode":"activegames"}```

**Spiel joinen (nur nach Login)**  
```{"mode":"join","id":0,"name":"Jason"}```

**Spiel erstellen (nur nach Login)**  
```{"mode":"create","id":0,"name":"Jason", "maxplayers":2}```

###Spiele Lobby
 
**Liste der Spieler anfordern**  
```{"mode":"gamelobby", "action":"players"}```

**Spieler Liste ohne Teams**  
```{"mode":"gamelobby","action":"players","isteamgame":false,"players":[{"name":"Jason","id":0},{"name":"Eva","id":1}]}```

**Spieler Liste mit Teams**  
```{"mode":"gamelobby","action":"players","isteamgame":true,"players":[{"name":"Team A","players":[{"name":"Jason","id":0},{"name":"Eva","id":1}]}]}```

**Spiel starten**  
```{"mode":"gamelobby", "action":"start"}```

**Spieler Eva kicken**  
```{"mode":"gamelobby", "action":"kick", "player":1}```

**Spiel Lobby verlassen**  
```{"mode":"gamelobby", "action":"leave"}```

**Team wechseln**  
```{"mode":"gamelobby", "action":"changeteam", "team":"Team A"}```


###Monitoring Tool  

**Monitoring Tool mit Namen "Monitor1" in laufendes Spiel 0 einhängen**  
```{"mode":"monitor", "id":0, "name":"Monitor1"}```


###Fehler Nachrichten  
```{"mode":"error", "message":"This is an error."}```
