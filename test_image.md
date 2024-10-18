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

5) Configuration SSH
A) Modification du fichier de config /etc/ssh/sshd_config
![image](https://github.com/user-attachments/assets/cf37c3a3-3f8a-459d-b8d3-6674eb9fa57e)

systemctl enable ssh
![image](https://github.com/user-attachments/assets/829725d5-4dda-487a-8469-f03bee15ff99)

Tentative de connection SSH depuis terminal Powershell sur le port 4242
![image](https://github.com/user-attachments/assets/c60440ec-af85-480c-a80d-aff8d30f7de6)

