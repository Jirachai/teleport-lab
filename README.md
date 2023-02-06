# teleport-lab
Deploy teleport lab 

 - docker-compose -f teleport-lab.yml up -d
 
 This compose have 3 container for lab 
   1. teleport
   2. openssh server
   3. term

 - exec to cli term and try to use command 
   ssh root@luna.teleport
   ssh root@mars.openssh.teleport
   cd /etc/teleport.d/ansible && ansible all -m ping
   tsh ssh root@env=example hostname
   tsh ls

 - Explore web UI 
   tctl users add testuser --roles=editor,access --logins=root,ubuntu

   after do this command will promt link token for signin teloport web
   user localhost
  
