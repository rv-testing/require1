#command to install roles from a requirements file <br>
#(make sure you have tasks and meta folder and the file should be in roles folder):

ansible-galaxy install -r requirements.yml
  
Call from remote yml with tag:  

\- name: call require1 role <br>
   &nbsp;&nbsp;hosts: all <br>
   &nbsp;&nbsp;become: true <br>
   &nbsp;&nbsp;roles: <br>
   &nbsp;&nbsp;&nbsp;&nbsp;\- { role: require1 }  <br>
   &nbsp;&nbsp;tags: call_require1 <br>

