# k8-harder-way

Building a k8 bare metal cluster from scratch following https://github.com/kelseyhightower/kubernetes-the-hard-way

---
## Certificates
https://kubernetes.io/docs/concepts/security/controlling-access/

https://github.com/kelseyhightower/kubernetes-the-hard-way/blob/master/docs/04-certificate-authority.md

Run play to create certs from the variables defined in `var/certs.yml`
```
ansible-playbook create_certs.yml
```

When vagrant machines are provisioned these certs are uploaded to the appropriate VMs.