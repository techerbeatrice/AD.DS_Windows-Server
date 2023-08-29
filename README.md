# Active Directory sur windows server

**Les étapes :**   

**Installation du rôle AD DS**    

**Création du domaine "wilders.lan"**    

___

Donner le rôle **AD DS** à windows Server, pour cela aller dans Gérer --> Ajouter des rôles et fonctionnalités --> Dans Type d'installation, sélectionner Installation basée sur un rôle ou une fonctionnalité --> Dans sélection du serveur --> Sélectionner un serveur du pool de serveurs --> Sélectionnner le serveur de destination --> Dans la liste des rôles, cocher **AD DS** ---> suivre l'assistant Ajout de rôles et de fonctionnalités

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/ed997ce7-46da-42fb-b344-a86b0c14d632)


Après avoir coché **AD DS**, faire 3 fois Suivant > Dans Confirmation, cliquer Installer

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/6f1e6a6a-87d5-4c54-855d-7b84f833ee64)

___

Arrivé dans Résultats, cliquer sur "**Promouvoir ce serveur en contrôleur de domaine**"

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/165e2c64-1c06-4833-b6c6-02d8ef1dc8bb)

La fenêtre **Assistant Configuration des services de domaines Active Directory** s'ouvre dans **Configuration de déploiement** ---> Sélectionner **Ajouter une nouvelle forêt** ---> Renseigner la partie **Nom de domaine racine**, dans notre cas **wilders.lan** 

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/74bb1564-542b-4255-85ae-9d4fa0b74bc2)
