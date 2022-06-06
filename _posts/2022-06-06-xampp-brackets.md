---
layout: post
title: Comment installer XAMPP et Brackets
date: 2022-06-06
Description: This post describes a step by step method to install XAMPP and Brackets.
tag: writing 
---

## Installation de XAMPP sur Windows

Allez sur https://www.apachefriends.org/fr/index.html et cliquez sur **XAMPP pour Windows** 

![1](https://user-images.githubusercontent.com/17012616/172158564-a73ee1fc-5b48-4d38-9520-90e0dbaf0749.PNG)

Attendez que le fichier soit téléchargé. Après le téléchargement, faites un clic droit sur le fichier téléchargé et sélectionnez "Exécuter en tant qu'administrateur". Dans la boîte de dialogue qui apparaît vous demandant de désactiver votre contrôle de compte d'utilisateur, cliquez sur "OK".

Suivez l'assistant d'installation et cliquez sur "Suivant" pour continuer lorsque vous y êtes invité. Lorsque vous êtes invité à sélectionner un dossier d'installation, assurez-vous que **C://xampp** est sélectionné comme emplacement d'installation. Continuez à cliquer sur **Suivant** jusqu'à ce que l'installation commence. Une fois l'installation terminée, cliquez sur le bouton **Terminer**.

Accédez au dossier **C://xampp** et double-cliquez sur le fichier **xampp-control.exe**

![2](https://user-images.githubusercontent.com/17012616/172151759-e767f594-8d62-4565-9820-b0493bd065bd.PNG)

Pour démarrer n'importe quel module, cliquez sur le bouton Démarrer(Start) à côté du module. Pour l'arrêter, cliquez sur le bouton Arrêter(Stop). 

![6](https://user-images.githubusercontent.com/17012616/172158373-cfe2a254-a42d-402e-9875-5088ee81588f.PNG)


## Installation de Brackets 

Pour installer Brackets, rendez-vous sur http://brackets.io/ et cliquez sur le bouton « Download Brackets » pour télécharger l'application.

Une fois téléchargé, double-cliquez sur le fichier téléchargé pour lancer l'installation.

Sous Windows, continuez à cliquer sur "Suivant" pour terminer l'installation. Une fois l'installation terminée, cliquez sur le bouton "Terminer".

### Création et exécution d'un fichier PHP

Ouvrez Brackets et créez un nouveau fichier (Fichier > Nouveau). Tapez le code suivant dans le fichier: 

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ma première page PHP</title>
</head>
<body>
    <h1>Ma première page PHP</h1>
    <?php   
        echo "Hello World!";
    ?>
</body>
</html>
```

Enregistrez le fichier sous **hello.php** dans votre dossier **htdocs**

Sous Windows, le dossier htdocs se trouve dans votre répertoire d'installation XAMPP (c'est-à-dire, **C:\xampp**).

Pour exécuter le fichier, ouvrez le panneau de configuration XAMPP et assurez-vous qu'Apache est en cours d'exécution.

Sous Windows, tapez **http://localhost/hello.php** dans la barre d'adresse de votre navigateur. (Remarque : si Apache s'exécute sur un port différent, vous devez également ajouter le numéro de port à l'URL. Par exemple, saisissez **http://localhost:8089/hello.php** si vous utilisez le port 8089...)

Vous devriez voir l'output suivant:
![4](https://user-images.githubusercontent.com/17012616/172157812-af8bb00d-5f5b-49ca-9d2d-350e77a38190.PNG)


