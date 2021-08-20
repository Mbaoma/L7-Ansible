## Ansible as a configuration management tool
Ansible is agentless-it does not need to be installed on the host machine for it to run. It can be used to manage Operating systems, servers, networks and infrastructure and other needs as defined by the user.

Some of its advantages are:
-   It is extensible
-   It is agentles
-   It is free and effective

## Ansible Vs Terraform
| Ansible | Terraform |
| ----------- | ----------- |
| It is agentless | It is not agentless |
| Focuses on configuration management with limited support for infrastructure | Mainly used for infrastructure automation |
Uses imperative language | Uses declarative language 

## Running ansible on localhost
```
---
  - name: "Playing with Ansible and Git"
    hosts: localhost
    connection: local 
    tasks:

    - name: "just execute a ls -lrt command"
      shell: "ls -lrt"
      register: "output"

    - debug: var=output.stdout_lines
```

![image](https://user-images.githubusercontent.com/49791498/130294325-30daf8f1-5dc9-4f60-91b3-dc780d2ab5d3.png)
*terminal result*

## Installing Ansible on an Ubuntu control node
