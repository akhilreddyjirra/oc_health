# Environment health checks

playbook are wirrten using the refrence https://docs.openshift.com/container-platform/3.11/day_two_guide/environment_health_checks.html

### Playbook
1. Checking complete environment health

This will create project `validate` , create `nginx` app and show the status 

    `ansible-playbook health-check/app.yml --tags=newapp`
<<<<<<< HEAD

=======
    
>>>>>>> 3dff3c77b0c4373adf9f392eff44f681c6c771d1
after completion this will delete the `validate` namespace

    `ansible-playbook app.yml --tags=deletens`


<<<<<<< HEAD
2. Host health 
=======
2. Host health
>>>>>>> 3dff3c77b0c4373adf9f392eff44f681c6c771d1

This will check the nodes status and etcd health

    `ansible-playbook app.yml --tags=nodes`
<<<<<<< HEAD

=======
    
>>>>>>> 3dff3c77b0c4373adf9f392eff44f681c6c771d1
peding etcd health yml files

3. Router and registry health

This is check the Router and registry health in default project

<<<<<<< HEAD
    `ansible-playbook rr_health.yml`
=======
    `ansible-playbook rr_health.yml`
>>>>>>> 3dff3c77b0c4373adf9f392eff44f681c6c771d1
