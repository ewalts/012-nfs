# 012-nfs  NFS Exports

NOTE: This is currently being updated.
I put this together very quickly. Great for someone knowledgable in Iptables, NFS and Ansible. Others might have questions.

* Task List
    -  Update/Install Iptables  
    -  Configure Iptables Chain rules, Save
    -  Update/Install NFS Server
    -  Configure Exports, Reload NFS


Variable List
```
home_net: x.x.x.x/24
ca_cert_dir: '/etc/pki/ca'
node_cert_dir: /etc/pki/nodes
ca_subject: "/C=US/ST=Hawaii/L=Honolulu/O=MyOrg/OU=My Department/CN=mydomain.org"
nodes:
  - name: 'bkp1'
    domain: 'mydomain.org'
    ip: 'x.x.x.x'
exports:
  - path: '/data0/backups'
    remote_host: 
```
