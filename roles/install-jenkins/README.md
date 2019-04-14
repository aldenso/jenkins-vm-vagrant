Role Name
=========

Install a Jenkins server.

Requirements
------------

NA.

Role Variables
--------------

NA

Dependencies
------------

NA

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      connection: local
      gather_facts: yes
      become: yes
      vars:
        MAVEN_VERSION: "3.5.4"
        DEFAULT_MAVEN_DIR: "/opt/maven"
        GRADLE_VERSION: "4.3"
        DEFAULT_GRADLE_DIR: "/opt/gradle"
        JENKINS_USER: "jenkins"
        JENKINS_GROUP: "jenkins"
      roles:
        - { role: install-jenkins }

License
-------

MIT

Author Information
------------------

Aldo Sotolongo (aldenso@gmail.com)
