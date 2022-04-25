# Mini Serveur pour Courriel

>Technologies Internet (INF4533): Projet 2
  
## Installation
Pour tester l'ensemble des fonctionnalités de ce projet, 
il est favorable d'utiliser un deuxième ordinateur afin de bien pouvoir simuler le partage de messages entre deux ou plusieurs utilisateurs. 

En vertu de notre exemple, le premier utilisateur (ordinateur A) qui sera l'hôte de notre mini serveur, servira de destinataire aux messages envoyés, tandis que l'autre utilisateur (ordinateur B) agira comme l'expéditeur.


Pour lancer le projet, veuillez entrer dans le terminal :

```bash
  npm install
```
ensuite, afin d'activer le serveur :

```bash
  node index.js
```
Vous serez alors connecté sur le **port 3000** que vous pourrez accéder (http://localhost:3000/).
Maintenant, vous devez fournir deux informations particulières au(x) expéditeur(s) de messages.

D'abord, l'expéditeur doit se connecter au micrologiciel de votre routeur via un navigateur. N'importe quel navigateur fera l'affaire. Pour trouver l'adresse IP de votre routeur, tapez *cmd* dans la barre de recherche Windows
et appuyez sur Enter pour ouvrir le Command Prompt ou tapez *Terminal* dans Finder pour Mac. Tapez ensuite :
```bash
  ipconfig
```
Faites défiler les informations jusqu'à ce que vous voyez un paramètre pour le **IPv4 Address** sous *Ethernet adapter* ou *Wireless LAN adapter*.
C'est votre routeur, et le numéro à côté est l'adresse IP de votre routeur. 

Ensuite, dans le navigateur, vous verrez s'afficher notre page web. Notre modeste interface se divise en 3 onglets. De gauche à droite se situent respectivement l'onglet d'**Accueil** étant affichée par défaut lors du démarrage, suivi de **Carnet d'Adresse** et **Messages**. 
Vous aurez devant vous votre **clé publique** que vous devrez également partager à l'expéditeur.

En assumant que l'expéditeur ait en sa possession l'adresse IP de votre routeur ainsi que votre clé publique, il devra inscrire dans la barre d'adresse de son navigateur l'adresse IP de votre routeur suivi du numéro de port (3000) dans le format suivant :

```bash
  192.135.0.157:3000
```

L'expéditeur devrait voir s'afficher devant lui notre site web. Il devra aller sous l'onglet **Carnet d'adresse** afin de créer son premier récipient et y insérer la clé publique du destinataire.

Après avoir créer un contact, l'expéditeur devra se diriger vers l'onglet **Message** où il pourra envoyer du texte. Ceux-ci étant transmis au destinataire, seront affichés dans son navigateur, plus bas dans le même onglet sous la section Liste de Message.

## Tech Stack

- **Serveur:** Node

- **Frameworks:** Express

- **Librairies:** node-forge, body-parser



## Auteurs

- [@Jean-Pierre Masri-Clermont](https://www.github.com/JPP44)
- [@Samuel Hein](https://www.github.com/SamHein8)
- [@Patrick Patenaude](https://www.github.com/Kamaiko)
- [@Lawrence Kater](https://www.github.com/lelwrence)
- [@Marco Klayton Djouwne](https://www.github.com/)
- [@Abdel-Gany Jr Odelele](https://www.github.com/2longAGO)


