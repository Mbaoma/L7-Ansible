# L7-Ansible
This repo focuses on using Ansible as an Infrastructure as code tool, and is a part of the SCA-DevOps Levelled membership program


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