I seguenti script hanno entrambi lo stesso obiettivo, ovvero quello di verificare se si è Root.Nel primo caso si confronta l'$UID dell'utente che sta eseguendo lo script nella shell e il $ROOT_UID 
printando nel caso la condizione -eq sia vera "You are root".Nel secondo script lo scopo è il medesimo, con la differenza che invece di paragonare gli $UID confronta $ROOTUSER_NAME con $username.
