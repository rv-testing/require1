#command to install roles from a requirements file <br>
#(make sure you have tasks and meta folder and the file should be in roles folder):

ansible-galaxy install -r requirements.yml
  
Call from remote yml with tag:  

- name: call require1 role
  hosts: all
  become: true
  roles:
    \- { role: require1 }  
  tags: test

