##Nachrichten an den Server  
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

##Nachrichten vom Server  

###Liste aktiver Spiele  
```{"games":[{"id":0,"serverurl":"https://raw.githubusercontent.com/MachDeinSpiel/MdsJsons/master/KeyQuest_Server.json","author":"MDS Team","maxplayers":2,"players":"Alice","name":"KeyQuest","isteamgame":false,"activeplayers":1,"clienturl":"https://raw.githubusercontent.com/MachDeinSpiel/MdsJsons/master/KeyQuest_Client.json","apptheme":"light","version":0.1}],"mode":"activegames"}```  

###Liste verfügbarer Spiele  
```{"games":[{"id":0,"author":"MDS Team","teams":0,"serverurl":"https://raw.githubusercontent.com/MachDeinSpiel/MdsJsons/master/KeyQuest_Server.json","maxplayers":2,"name":"KeyQuest","isteamgame":false,"clienturl":"https://raw.githubusercontent.com/MachDeinSpiel/MdsJsons/master/KeyQuest_Client.json","apptheme":"light","version":0.1}],"mode":"gametemplates"}```

###Spiele Lobby

**Spieler Liste ohne Teams**  
```{"mode":"gamelobby","action":"players","isteamgame":false,"players":[{"name":"Jason"},{"name":"Eva"}]}```

**Spieler Liste mit Teams**  
```{"mode":"gamelobby","action":"players","isteamgame":true,"players":[{"name":"Team A","players":[{"name":"Jason"},{"name":"Eva"}]}]}```

###Fehler Nachrichten  
Z.B. bei Login-Fehler, JSON-Exceptions und wenn der Server beendet wird.  
```{"mode":"error", "message":"This is an error."}```  

