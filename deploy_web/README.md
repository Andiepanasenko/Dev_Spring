#Result after running playbook
$ansible-playbook deploy_webs.yml 

PLAY [Install differents web_servers] ******************************************

TASK [Gathering Facts] *********************************************************
ok: [10.0.2.7]
ok: [10.0.2.9]

TASK [deploy_web : Install Apache For Debian] **********************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [deploy_web : Start Web Server for Debian] ********************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [deploy_web : Install Nginx web Server for RedHat] ************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

TASK [deploy_web : Start Web Server for RedHat] ********************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

TASK [deploy_web : GENERATE INDEX.HTML file] ***********************************
ok: [10.0.2.7]
ok: [10.0.2.9]

TASK [deploy_web : Copy Img] ***************************************************
ok: [10.0.2.7] => (item=1.jpg)
ok: [10.0.2.9] => (item=1.jpg)

TASK [deploy_web : Check that you can connect (GET) to a page and it returns a status 200] ***
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [deploy_web : Check that you can connect (GET) to a page and it returns a status 200] ***
skipping: [10.0.2.9]
ok: [10.0.2.7]

PLAY RECAP *********************************************************************
10.0.2.7                   : ok=6    changed=0    unreachable=0    failed=0   
10.0.2.9                   : ok=6    changed=0    unreachable=0    failed=0  
