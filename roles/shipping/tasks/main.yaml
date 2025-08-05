- name: app setup
  include_role:
    name: common
    tasks_from: app-setup

- name: maven setup
  include_role:
    name: common
    tasks_from: maven

- name: import data
  community.mysql.mysql_db:
    name: all
    login_user: "{{ MYSQL_ROOT_USER }}"
    login_password: "{{ MYSQL_ROOT_PASSWORD }}"
    login_host: "{{ MYSQL_HOST }}"
    state: import
    target: "{{ item }}"
  loop:
  - /app/db/schema.sql
  - /app/db/app-user.sql
  - /app/db/master-data.sql

- name: systemd setup
  include_role:
    name: common
    tasks_from: systemd