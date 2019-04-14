# jenkins-vm-vagrant

Jenkins VM with vagrant and ansible

Install:

```bash
vagrant up
```

Post installation:

```bash
vagrant ssh -c "sudo cat /var/lib/jenkins/secrets/initialAdminPassword"
```

open url <http://192.168.56.200:8080>
