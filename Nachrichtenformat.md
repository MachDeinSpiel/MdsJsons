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
