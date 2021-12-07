disable-login-list 
=========

Ansible role to disable login list on Graphic terminal for both CentOS/RedHat 8 and Ubuntu 18/20  
Also, allows you to create a custom banner message on the login console.

Requirements
------------

System running Gnome/Wayland.

Role Variables
--------------

These are the default values.

disable_user_list_var: 'true'
banner_message_enable_var: 'true'
banner_message_var: 'Customized.local \n Authorized Users Only. \n********************'


Dependencies
------------

none

Example Playbook
----------------
<pre>
  hosts: all
  become: yes

  roles:
    - role: disable-login-list
      vars:
        banner_message_var: 'Customized Technology\n     Customized.local \n Authorized Users Only. \n********************'


</pre>

License
-------

MIT

Author Information
------------------

Roy Kim
https://github.com/customizedcode
customizedcode.us
This is part of a tutorial for creating portable roles from playbooks.
Please see the playbook this came from if your interested.
