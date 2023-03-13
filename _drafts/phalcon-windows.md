---
layout: post
title: Installation de phalcon sur Windows 10 (PHP 7.4 et plus)
Description: Installation de phalcon sur Windows 10 (PHP 7.4 et plus) avec XAMPP 
tags: writing
---

## 1 Checks à faire
Vérifiez votre version PHP, votre architecture et votre extension php sur localhost en utilisant phpinfo(); 

Les miens sont (voir figure) : 
    PHP Version 7.4.29
    x64
    TS, vc15
![1](https://user-images.githubusercontent.com/17012616/224748879-66223ca0-ff11-4926-865e-086021dba4be.JPG)

## 2 Allez sur le site Web de phalcon et téléchargez le fichier dll approprié

![2](https://user-images.githubusercontent.com/17012616/224749777-5f29b0e4-e848-4012-8df8-d9885f05c888.JPG)

![3](https://user-images.githubusercontent.com/17012616/224750440-cc8d56bb-77bd-4cd8-ba04-0dcd748139b9.JPG)

![4](https://user-images.githubusercontent.com/17012616/224750656-0d3369e6-f18e-4ed7-85ae-66de495a61db.JPG)

Ouvrez dans un autre onglet le lien en cliquant sur here come sur l'image.

![5](https://user-images.githubusercontent.com/17012616/224751002-9676ad00-76a8-4d87-a63a-f384b14bab96.JPG)

![6](https://user-images.githubusercontent.com/17012616/224751715-42e4ee41-2f28-41b3-8db9-e783b93948dd.JPG)

Faites défiler vers le bas et sélectionnez la version qui correspond à votre version php, architecture et constructeur d'extension php. En cliquant, le téléchargement du fichier zip sera lancé

![7](https://user-images.githubusercontent.com/17012616/224752187-677865d8-e4e9-43e3-a5a4-4fc34833c677.JPG)

Extraction de dll vers xampp>php>ext

![9](https://user-images.githubusercontent.com/17012616/224756575-9869c323-8c5c-4d56-8137-b862fb6c56e6.JPG)

Étant donné que Phalcon est faiblement couplé, il expose les fonctionnalités sans avoir besoin d'extensions supplémentaires. Cependant, certains composants s'appuient sur des extensions supplémentaires pour fonctionner. Lorsque vous avez besoin de connectivité et d'accès à la base de données, vous devrez installer l'extension php_pdo. Si votre SGBDR est MySQL/MariaDB ou Aurora, vous aurez également besoin de l'extension php_mysqlnd. De même, l'utilisation d'une base de données PostgreSql avec Phalcon nécessite l'extension php_pgsql. 

Placez "extension=php_phalcon.dll" après les pdo comme sur l'image. Verifiez la correspondance du nom de l'extention avec le dll que vous avez telecharger, cela peut être diffrent de "php_phalcon" ainsi vous changerez en fonction. 

![10](https://user-images.githubusercontent.com/17012616/224758191-0e890ed2-eeb3-40fc-a50b-2036ea43de69.JPG)

## Restart your web server 

Recherchez phalcon dans votre phpinfo(). Si c'est le cas, l'installation est réussie. 

![11](https://user-images.githubusercontent.com/17012616/224759067-780d4773-4b31-4910-918f-a348237fbb5e.JPG)


## Recherchez PSR pour Windows et obtenez la dernière version stable

Retour à la page d'accueil de phalcon et allez dans get phalcon

![8](https://user-images.githubusercontent.com/17012616/224753749-15c45815-ed1d-4f66-847a-fc55deffe419.JPG)

## Installation de Dev-tools

Allez sur https://github.com/phalcon/phalcon-devtools

![12](https://user-images.githubusercontent.com/17012616/224764845-df50ba98-ec6f-4cee-9b04-b52d8cda9e08.JPG)

## Download the repository as a zip file

![13](https://user-images.githubusercontent.com/17012616/224765133-ad119cb8-2343-455c-a0e0-292dd4adbeff.JPG)

## Extraire vers C:\\ et renonmmer le dossier "phalcon" pour plus de flexibilité.

![14](https://user-images.githubusercontent.com/17012616/224766336-f4a467ca-c7b1-48ea-bbba-8b19f55aa75c.JPG)

## Ajoutez php et phalcon dans les variables d'environnements 

Ouvrez les paramètres avancées du système  

![image](https://user-images.githubusercontent.com/17012616/224767663-5073bae5-b39a-4f12-973a-2bdf9f37c335.png)

Dans les variables system, modifiez Path 

![16](https://user-images.githubusercontent.com/17012616/224768030-3d0c8b8f-06e5-4987-9a71-2252a432f2e9.JPG)

![17](https://user-images.githubusercontent.com/17012616/224768577-3ea1b95f-ecd0-42dc-b79c-0085a3ed7f53.JPG)

Enregistrez et re-ouvrir l'invite de commande. 

## Download and install composer 

![18](https://user-images.githubusercontent.com/17012616/224770700-556db207-9ee5-4dfe-b2c6-36e935bb92fa.JPG)

![19](https://user-images.githubusercontent.com/17012616/224770732-18979635-882a-4010-928d-230c5e377e3a.JPG)

![20](https://user-images.githubusercontent.com/17012616/224772937-9c93971b-4d93-48b5-81f2-cc136ca9ea32.JPG)









