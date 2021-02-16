---
functions:
  shell:  
    - code: |
        GROUPNAME=users
        sg $GROUPNAME -c "/bin/sh"
  command:
    - code: |
        COMMAND=whoami   
        GROUPNAME=users
        sg $GROUPNAME -c $COMMAND
  sudo:
    - code: |
        GROUPNAME=users
        sudo sg $GROUPNAME -c "/bin/sh"
---
