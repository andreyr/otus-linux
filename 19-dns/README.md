# Vagrant DNS Lab

A Bind's DNS lab with Vagrant and Ansible, based on CentOS 7.

# Playground

```
   vagrant ssh client1
   vagrant ssh client2
```

  * zones: dns.lab, reverse dns.lab and ddns.lab
  * ns01 (192.168.50.10)
    * master, recursive, allows update to ddns.lab
  * ns02 (192.168.50.11)
    * slave, recursive
  * client1 (192.168.50.15)
    * used to test the env, runs rndc and nsupdate
  * client2 (192.168.50.25)
    * used to test the env, runs rndc and nsupdate
  * zone transfer: TSIG key
