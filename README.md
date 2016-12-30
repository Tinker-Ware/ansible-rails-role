Ansible Rails Role
===

Currently this role installs Ruby V 2.3.3. 

Import this normally on your host.

```
- hosts: myhost
  roles:
    - { role: rails }
```

On your variables file you can define a hash to clone existing
rails repositories. 

```
rails_repos:
  app1:
    name: https://github.com/RailsApps/rails-signup-download.git
    port: 3000
    branch: master
```

Check rails/defaults/main.yml for more info. 
