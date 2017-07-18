# winnergroup

*********************************************
Project Setup
*********************************************


1. Go to folder "vm-winner" and Run "vagrant up" and wait.
2. Once vagrant up has finished, 
    - Open browser go to address "http://winnergroup.dev" install Drupal  DB:drupal user:drupal pass:drupal
    - run vagrant ssh to login to your new machine.
3. Install terminus CLI - "composer global require pantheon-systems/terminus"
4. Grab a machine token(https://pantheon.io/docs/machine-tokens/) from Pantheon, and paste this into your VM.
5. Download Drush aliases from pantheon by running "terminus aliases"
6. Add your SSH Key(https://pantheon.io/docs/ssh-keys/) to Pantheon.
7. Copy the database from the dev site to your local "drush sql-sync @pantheon.winnergroup.dev @vm-winner.winnergroup.dev -y"