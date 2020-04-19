# Installation et configuration d'un RPi en hotspot Wifi pour le développement.

## Installation
Le playbook ansible suit l'installation telle que décrite sur la page suivante: https://maker.pro/raspberry-pi/projects/how-to-make-a-raspberry-pi-3-hotspot-and-build-a-stand-alone-network

Pour exécuter le playbook ansible, la présence d'ansible sur votre host est nécessaire.
Le guide d'installation se trouve à l'url suivante: https://docs.ansible.com/ansible/latest/installation_guide/index.html

Pour ce qui concerne le système sur le RPi, je pars d'une raspbian lite car je n'ai pas besoin de la partie desktop.

### Configuration et exécution du playbook
Le fichier [inventory.ini](ansible/inventory.ini) doit être modifié pour mettre le [hostname](ansible/inventory.ini#l2) qui correspond à votre raspberry pi

L'exécution du playbook ansibe s'effectue avec la commande suivante:
```bash
ansible-playbook -i ./ansible/inventory.ini ./ansible/playbook.yml
```
