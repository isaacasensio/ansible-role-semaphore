Semaphore
=========

Semaphore is a responsive web UI for running Ansible playbooks.

This Ansible role installs Semaphore as a Docker service.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):


```
semaphore_ui_image: "semaphoreui/semaphore:latest"
```
The version of the docker image to run as a container.

```
semaphore_db_image: "postgres:14"
```
Database docker image version

```
semaphore_db_user: "semaphore"
```
Database user

```
semaphore_db_password: "semaphore"
```
Database password

```
semaphore_db_name: "semaphore"
```
Database name

```
semaphore_db_host_port: 5432
```
Database exported port in host

```
semaphore_ui_host_port: 3000
```
Semaphore UI host port

```
semaphore_ui_admin_username: admin
```
Semaphore UI admin user

```
semaphore_ui_admin_password: admin
```
Semaphore UI admin password

```
semaphore_ui_admin_email: admin@localhost
```
Semaphore UI admin email

```
semaphore_ui_access_key_encription: gs72mPntFATGJs9qK0pQ0rKtfidlexiMjYCH9gWKhTU=
```
Semaphore UI access key encription. 


```
semaphore_host_config_path: /etc/semaphore
```
Host path which stores semaphore configuration.

```
semaphore_host_db_path: /var/lib/semaphore/postgresql/data
```
Host path which stores semaphore database.

```
semaphore_container_user: semaphore
```
user running the container 

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.semaphore

License
-------

MIT

