![image](https://github.com/user-attachments/assets/c8a5ea12-aba5-491a-82b3-3447c93c4b3f)

![image](https://github.com/user-attachments/assets/486c25c3-03d8-473e-9809-43951e85e983)

3) Verification Utilisateurs et Groupes
   A) Utilisateur
![image](https://github.com/user-attachments/assets/6a714545-62c2-4145-838b-966381b6126b)

 B) Groupes
 ![image](https://github.com/user-attachments/assets/8b5e156a-a973-494b-a7c3-061c8ce0b772)

4) Permission du dossier data
A)création du dossier
mkdir data à la racine

B) droits commande ls et getfacl data
ls
![image](https://github.com/user-attachments/assets/1747c538-5efb-4c83-93f2-59d24a35aa1c)

getfacl data
![image](https://github.com/user-attachments/assets/12e443d3-2410-43ef-a95a-f2af563543fd)

5) Configuration SSH / UFW
A) Modification du fichier de config /etc/ssh/sshd_config
![image](https://github.com/user-attachments/assets/cf37c3a3-3f8a-459d-b8d3-6674eb9fa57e)

systemctl enable ssh
![image](https://github.com/user-attachments/assets/829725d5-4dda-487a-8469-f03bee15ff99)

Tentative de connection SSH depuis terminal Powershell sur le port 4242
![image](https://github.com/user-attachments/assets/c60440ec-af85-480c-a80d-aff8d30f7de6)

Configuration des regles ufw 
![image](https://github.com/user-attachments/assets/6214d121-ffe7-4205-8292-36bc4d80e218)

6) Renommer la machine et Politique de mot de passe
A) renommer la machine en "julienlinux"
cat /etc/hostname
![image](https://github.com/user-attachments/assets/71ad5bf5-422f-4ae0-92c9-40147b18beab)

cat /etc/host
![image](https://github.com/user-attachments/assets/1e302d7b-d07f-425b-a637-222dbbf4d09b)

B) Politique de mot de passe
modification du fichier /etc/login.defs 
![image](https://github.com/user-attachments/assets/8998b618-0518-47f8-83b7-34446320c69b)

Modification du fichier /etc/pam.d/common-password
![image](https://github.com/user-attachments/assets/29a2259a-4da6-412b-b3f2-b6589d9cb6a4)

chage -l julien
![image](https://github.com/user-attachments/assets/22294ce7-d11a-4922-a6c3-dc534fc2aae6)

test du mot de passe "mypasw" qui ne remplit pas les conditions
![image](https://github.com/user-attachments/assets/55e0c95b-bc36-48ff-804c-a27f8dbb2c3e)

test du mot de passe "mypasw0"
![image](https://github.com/user-attachments/assets/080d5af3-f6cf-4660-950a-233dd1c82ecd)

test du mot de passe "Mypasw0"
![image](https://github.com/user-attachments/assets/cf07ea35-f9cd-416c-ab7c-fd144ba6150c)

Les régles s'appliquent! Nous allons maintenant rentrer un mot de passe qui respectes toutes ses régles: "$up3rP@sswd"
![image](https://github.com/user-attachments/assets/89039488-3254-4a28-acda-ee33ccb03420)

Le mot de passe est accepté car il respecte notre politique de mot de passe!
(Note: dans l'absolu il faudrait egalement éviter le Leap Speak)

6) Configuration sudo
Mise en place des régles:
![image](https://github.com/user-attachments/assets/a4e7a0eb-4ba4-4d08-b028-1819e5f673d4)

