
<h2 align="center">Activité pratique N° 4 : Sécurité des micro services avec Keycloak</h2><br><br>

<!-- sommaire -->
<details>
<summary>📖 Sommaire</summary>

la partie 1 : [Présentation de Keycloak](#partie-1--présentation-de-keycloak)
<br>
1. Télécharger Keycloak 19
<br>
2. Démarrer Keycloak
<br>
3. Créer un compte Admin
<br>
4. Créer une Realm
<br>
5. Créer un client à sécuriser
<br>
6. Créer des utilisateurs
<br>
7. Créer des rôles
<br>
8. Affecter les rôles aux utilisateurs
<br>
9. Avec PostMan :
<br>
    9.1.  Tester l'authentification avec le mot de passe
<br>
    9.2.  Analyser les contenus des deux JWT Access Token et Refresh TokenP
<br>
    9.3.  Tester l'authentification avec le Refresh Token
<br>
    9.4.  Tester l'authentification avec Client ID et Client Secret
<br>
    9.5.  Changer les paramètres des Tokens Access Token et Refresh Token

</details>


## la partie de Keycloak:
<p>
        <h3>1. Télécharger Keycloak 19</h3>
        <p>https://www.keycloak.org/downloads.html</p>
        <img src="./Images/Screenshot_1.png" alt="Screenshot_1" width="700">
        <h3>2. Démarrer Keycloak</h3>
        <p>cd keycloak-19.0.2/bin</p>
        <p>./kc.bat start-dev</p>
        <img src="./Images/Screenshot_2.png" alt="Screenshot_2" width="700">
        <h3>3. Créer un compte admin</h3>
        <p>http://localhost:8888</p>
        <img src="./Images/Screenshot_3.png" alt="Screenshot_3" width="700">
        <img src="./Images/Screenshot_4.png" alt="Screenshot_4" width="700">
        <h3>4. Créer une realm</h3>
        <img src="./Images/Screenshot_5.png" alt="Screenshot_5" width="700">
        <img src="./Images/Screenshot_6.png" alt="Screenshot_6" width="700">
        <img src="./Images/Screenshot_7.png" alt="Screenshot_7" width="700">
        <h3>5. Créer un client à sécuriser</h3>
        <img src="./Images/Screenshot_8.png" alt="Screenshot_8" width="700">
        <img src="./Images/Screenshot_9.png" alt="Screenshot_9" width="700">
        <img src="./Images/Screenshot_10.png" alt="Screenshot_10" width="700">
        <img src="./Images/Screenshot_11.png" alt="Screenshot_11" width="700">
        <img src="./Images/Screenshot_12.png" alt="Screenshot_12" width="700">
        <h3>6.utilisateur</h3>
        <img src="./Images/Screenshot_14.png" alt="Screenshot_14" width="700">
        <h3>7. Créer des rôles</h3>
        <img src="./Images/Screenshot_16.png" alt="Screenshot_16" width="700">
        <h3>8. Affecter les rôles aux utilisateurs</h3>
        <img src="./Images/Screenshot_17.png" alt="Screenshot_17" width="700">
        <img src="./Images/Screenshot_18.png" alt="Screenshot_18" width="700">
        <h3>9. Tester l'authentification avec postman</h3>
        <h5>9.1. Tester l'authentification avec le mot de passe</h5>
        <img src="./Images/Screenshot_19.png" alt="Screenshot_19" width="700">
        <img src="./Images/Screenshot_20.png" alt="Screenshot_20" width="700">
        <img src="./Images/Screenshot_21.png" alt="Screenshot_20" width="700">
        <img src="./Images/Screenshot_22.png" alt="Screenshot_21" width="700">
        <h5>9.2. Analyser les contenus des deux JWT Access Token et Refresh Token</h5>
        <img src="./Images/Screenshot_24.png" alt="Screenshot_24" width="700">
        <h5>9.3. Tester l'authentification avec le Refresh Token</h5>
        <img src="./Images/Screenshot_25.png" alt="Screenshot_25" width="700">
        <img src="./Images/Screenshot_26.png" alt="Screenshot_26" width="700">
        <h5>9.4. Tester l'authentification avec Client ID et Client Secret</h5>
        <img src="./Images/Screenshot_27.png" alt="Screenshot_27" width="700">
        <img src="./Images/Screenshot_28.png" alt="Screenshot_28" width="700">
        <img src="./Images/Screenshot_29.png" alt="Screenshot_29" width="700">
        <img src="./Images/Screenshot_30.png" alt="Screenshot_30" width="700">
        <h5>9.5. Changer les paramètres des Tokens Access Token et Refresh Token</h5>
        <img src="./Images/Screenshot_31.png" alt="Screenshot_31" width="700">
    </p>

## la partie 2 : Sécuriser un micro service avec Keycloak

<p>
    <p>Sécuriser L'architecture Micro services du projet Customer-service, Inventory-service et Order-service</p>
        <h1>Customer-service </h1>
            <p>
            <h5>1. Ajouter les dépendances</h5>
            <img src="./Images/Screenshot_32.png" alt="Screenshot_32" width="700">
            <h5>2. Modifier le fichier de configuration</h5>
            <img src="./Images/Screenshot_33.png" alt="Screenshot_33" width="700">
            <img src="./Images/Screenshot_34.png" alt="Screenshot_34" width="700">
            <h5>3. Creation des fichiers de configuration</h5>
            <img src="./Images/Screenshot_35.png" alt="Screenshot_35" width="700">
            <img src="./Images/Screenshot_36.png" alt="Screenshot_36" width="700">
            <h5>4. Test accés h2-console</h5>
            <img src="./Images/Screenshot_37.png" alt="Screenshot_37" width="700">
            <img src="./Images/Screenshot_38.png" alt="Screenshot_38" width="700">
            <h5>5. Test accés à la ressource</h5>
            <img src="./Images/Screenshot_39.png" alt="Screenshot_39" width="700">
            <img src="./Images/Screenshot_40.png" alt="Screenshot_40" width="700">
            </p>
        <h1>Inventory-service </h1>
            <p>
            <h5>1. Ajouter les dépendances</h5>
            <img src="./Images/Screenshot_41.png" alt="Screenshot_41" width="700">
            <h5>2. Creation des fichiers de configuration</h5>
            <img src="./Images/Screenshot_42.png" alt="Screenshot_42" width="700">
            <img src="./Images/Screenshot_43.png" alt="Screenshot_43" width="700">
            <h5>3. Test accés /products</h5>
            <img src="./Images/Screenshot_44.png" alt="Screenshot_44" width="700">
            <img src="./Images/Screenshot_47.png" alt="Screenshot_47" width="700">
            <img src="./Images/Screenshot_48.png" alt="Screenshot_48" width="700">
            </p>
        <h1>Order-service </h1>
            <p>
            <h5>1. Ajouter les dépendances</h5>
            <img src="./Images/Screenshot_49.png" alt="Screenshot_49" width="700">
            <h5>2. Creation des fichiers de configuration</h5>
            <img src="./Images/Screenshot_50.png" alt="Screenshot_50" width="700">
            <img src="./Images/Screenshot_51.png" alt="Screenshot_51" width="700">
            <h5>3. Test accés /orders</h5>
            <img src="./Images/Screenshot_52.png" alt="Screenshot_52" width="700">
            <img src="./Images/Screenshot_53.png" alt="Screenshot_53" width="700">
            </p>
