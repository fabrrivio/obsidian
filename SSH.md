<h1>Ajouter des accès SSH vers une machine</h1>
sudo nano ~/.ssh/config 

Host wz3uy        
    HostName wz3uy.ftp.infomaniak.com
    User wz3uy_fabrriv

Copier la clé public SSH sur le serveur:

ssh-copy-id -o 'IdentitiesOnly=yes' -i ~/.ssh/<clepublique> <prefix>_<votrenom>@<prefix>.ftp.infomaniak.com

Example: ssh-copy-id -o 'IdentitiesOnly=yes' -i ~/.ssh/id_ed25519.pub wz3uy_fabrriv@wz3uy.ftp.infomaniak.com




