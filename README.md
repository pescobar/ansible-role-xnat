ansible-role-xnat
=========

Download XNAT files and create the required folders

**This role expects tomcat and postgres to be already configured**

Role Variables
--------------

```
xnat_version: 1.7.6

xnat_top_folder: /data/xnat

xnat_home_folder: "{{ xnat_top_folder }}/home"

xnat_sub_folders:
  - archive
  - build
  - cache
  - ftp
  - home
  - home/config
  - home/logs
  - home/plugins
  - home/work
  - inbox
  - pipeline
  - prearchive

xnat_user: tomcat
xnat_group: tomcat

xnat_db_name: xnat
xnat_db_user: xnatdbuser
xnat_db_pass: xnatdbpass

xnat_tomcat_webapps_path: /opt/tomcat/webapps

xnat_url: http://192.168.111.222:8080
xnat_site_name: "XNAT"
xnat_admin_email: admin@oldschool.edu
xnat_smtp_server: mail.oldschool.edu
```

License
-------

GPLv3

Author Information
------------------

Pablo Escobar Lopez
