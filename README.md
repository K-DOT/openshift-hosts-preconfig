openshift-hosts-preconfig
=========

Configures hosts for sussessful openshift/okd installation

Role Variables
--------------
 * Origin/OKD version in X.XX format  
 `openshift_version: '3.11'`  
 * Docker version in X.XX.X-XX format  
 `docker_version: '1.13.1-75'`  
 * Docker storage device  
 `docker_storage_device: '/dev/vdb'`  
 * Adds 20% more capacity when the disk usage reaches 80%  
 `docker_storage_thin_pool_autoextend_threshold: 80`  
 `docker_storage_thin_pool_autoextend_percent: 20`  

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - hosts: all
      tasks:
        - name: test
          include_role:
            name: ansible-openshift-config


License
-------

BSD

Author Information
------------------

@K-DOT
