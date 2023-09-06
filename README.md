# Users-and-Groups-Management
| Chapter | Description |
|-----:|-----------|
|     1| Create a User Account |
|     2| Rename a User Account |
|     3| Delete a User |
|     4| Change Your Passsword |
|     5| Change a User's Password |
|     6| Lock and Unlock User Accounts |

## 1 Create a User Account
1. Créer un utilisateur.
   
   a. Depuis la barre des favoris, sélectionnez Terminal.
   
   b. Tapez **useradd -c "Paul Denunzio" pdenunzio**, puis appuyez sur Entrée pour créer l'utilisateur et définir le commentaire en une seule commande.
   
3. Créez un mot de passe pour le nouvel utilisateur.

   a. Tapez **passwd pdenunzio** et appuyez sur Entrée.
   
   b. Tapez **eye8cereal** comme mot de passe, puis appuyez sur Entrée.
   
   c. Retapez **eye8cereal** comme mot de passe, puis appuyez sur Entrée.
   
4. Consultez le fichier passwd et répondez à la question.
   
   Tapez **cat /etc/passwd** et appuyez sur Entrée pour vérifier que le compte a été créé.

![](https://imgur.com/PsXVATF.png)

## 2 Rename a UserAccount

a. Depuis la barre des favoris, sélectionnez Terminal.

b. tapez **usermod -c "Brenda Palmer" -d /home/bpalmer -m -l bpalmer bcassini**, puis appuyez sur Entrée.

c. Tapez **cat /etc/passwd** et appuyez sur Entrée.

d. Tapez **ls /home** et appuyez sur Entrée pour vérifier que le compte a été modifié.

![](https://imgur.com/k0LdjG2.png)


## 3 Delete a User 

Tapez **userdel -r thaslam**, puis appuyez sur Entrée pour supprimer le compte utilisateur et le répertoire personnel.

Tapez **cat /etc/passwd** et appuyez sur Entrée.

Tapez **ls /home** et appuyez sur Entrée pour vérifier que le compte a été supprimé.

![](https://imgur.com/Ep8pqq2.png)

## 4 Change Your Passsword

a- Depuis la barre des favoris, sélectionnez Terminal.

b- Tapez **passwd**, puis appuyez sur Entrée.

c- Lorsqu'on vous le demande, saisissez **7hevn9jan** comme mot de passe actuel, puis appuyez sur Entrée.

Vous ne verrez pas le mot de passe pendant que vous le tapez.

e- À la demande de Nouveau mot de passe, saisissez **r8ting4str**, puis appuyez sur Entrée.

f- Retapez **r8ting4str** comme nouveau mot de passe, puis appuyez sur Entrée.

![](https://imgur.com/QaSoHcd.png)

## 5 Change a User's Passsword

a- Tapez **su -c "passwd schawla"** et appuyez sur Entrée.

b- Tapez **1worm4b8** et appuyez sur Entrée pour le mot de passe de l'utilisateur root.

Vous ne verrez pas le mot de passe pendant que vous le tapez.

c- Tapez **G20oly04** et appuyez sur Entrée pour le nouveau mot de passe du compte utilisateur schawla.

d- Tapez **G20oly04** comme nouveau mot de passe et appuyez sur Entrée.

![](https://imgur.com/xqxBPj6.png)

## 6 Lock and Unlock User Accounts

1. Verrouillez les comptes requis.

  a. Depuis la barre des favoris, sélectionnez Terminal.

  b. À l'invite, tapez **usermod -L vedwards** ou **passwd -l vedwards**, puis appuyez sur Entrée pour verrouiller le compte utilisateur.

  c. Tapez **usermod -L cflynn** ou **passwd -l cflynn**, puis appuyez sur Entrée pour verrouiller le compte utilisateur.

  d. Tapez **usermod -L bkahn** ou **passwd -l bkahn**, puis appuyez sur Entrée pour verrouiller le compte utilisateur.

2. Déverrouillez les comptes requis.

  a. Tapez **usermod -U mbrown** ou **passwd -u mbrown**, puis appuyez sur Entrée pour déverrouiller le compte utilisateur.

  b. Tapez **usermod -U bcassini** ou **passwd -u bcassini**, puis appuyez sur Entrée pour déverrouiller le compte utilisateur.

  c. Tapez **usermod -U aespinoza** ou **passwd -u aespinoza**, puis appuyez sur Entrée pour déverrouiller le compte utilisateur.

3. Vérifiez les modifications.

  a. Tapez **cat /etc/shadow** pour vérifier les modifications. La présence du point d'exclamation (!) dans le champ du mot de passe indique que le compte est désactivé.

![](https://imgur.com/OKgGSjG.png)
