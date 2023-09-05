# Active Directory sur windows server
___

Installe et configure Active Directory server en reprenant la machine virtuelle que tu as utilisé pour faire les quêtes sur le DNS et DHCP   
•	Installer le rôle AD DS sur Windows Serveur 2012 R2    
•	Créer un domaine wilders.lan    
•	Explique la procédure que tu as utilisée dans une documentation qui permet de reproduire ton installation et que tu posteras comme solution à cette quête    
•	La procédure permet effectivement de mettre en place un contrôleur de domaine    
•	Les explications sont claires et adaptées à un administrateur·rice débutant·e   

____

**Les étapes :**   

**Installation du rôle AD DS**    

**Création du domaine "wilders.lan"**    

___

Donner le rôle **AD DS** à windows Server, pour cela aller dans Gérer --> Ajouter des rôles et fonctionnalités --> Dans Type d'installation, sélectionner Installation basée sur un rôle ou une fonctionnalité --> Dans sélection du serveur --> Sélectionner un serveur du pool de serveurs --> Sélectionnner le serveur de destination --> Dans la liste des rôles, cocher **Services AD DS** ---> suivre l'assistant Ajout de rôles et de fonctionnalités

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/ed997ce7-46da-42fb-b344-a86b0c14d632)


Après avoir coché **Services AD DS**, faire 3 fois Suivant > Dans Confirmation, cliquer Installer

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/6f1e6a6a-87d5-4c54-855d-7b84f833ee64)

___

Arrivé dans Résultats, cliquer sur "**Promouvoir ce serveur en contrôleur de domaine**"

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/165e2c64-1c06-4833-b6c6-02d8ef1dc8bb)

La fenêtre **Assistant Configuration des services de domaines Active Directory** s'ouvre dans **Configuration de déploiement** ---> Sélectionner **Ajouter une nouvelle forêt** ---> Renseigner la partie **Nom de domaine racine**, dans notre cas **wilders.lan** 

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/74bb1564-542b-4255-85ae-9d4fa0b74bc2)


Dans **Options du contrôleur de domaine**, renseigner le **mot de passe** de votre accès machine ---> Suivant

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/21c732d0-6565-4d39-bfcf-aa337faa8281)

Dans options DNS, un message d’erreur en jaune vient alerter de la délégation du serveur DNS. Il n’y a rien à faire à ce stade, cliquer simplement sur Suivant pour continuer.    

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/73f195d9-f779-4751-bf02-a79a6eecc8ad)

____

Indiquer l’équivalent NetBIOS. Par exemple, pour « domaine.local » on pourra choisir le NetBIOS « DOMAINE » . Dans notre cas, pour "wilders.lan" on met "WILDERS" ---> Suivant ---> Dans Chemin d'accès, laisser par défaut ---> Suivant 

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/16d2494a-cbfc-42c7-8668-87bf412714aa)
![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/9b4fcfcb-5f3c-4bbb-b8c4-a6abeb4f2f28)
![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/d6833ef4-0986-489f-b452-53bb11b41999)

Une dernière vérification est effectuée, des notifications sont affichées mais cliquer sur Installer pour démarrer le processus.

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/841fef86-5ebd-4eed-ab2a-415b9fdff4f5)

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/cdbbff38-8e2b-472e-9561-033c1739a1d9)

Après l'installation, windows server redémarre.
On retombe sur le tableau de bord avec AD DS et les autres rôles

![image](https://github.com/techerbeatrice/AD.DS_Windows-Server/assets/138071140/69677c06-acdc-4332-9551-ab00ffa21e9a)

