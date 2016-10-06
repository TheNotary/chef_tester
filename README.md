# Chef Test

This is a vagrant box for testing Chef configurations and stuff on (just Ubuntu).  

## Usage

Destroy the VM:

```
$ vagrant destroy
```

Create the VM:

```
$ vagrant up
```

Manually ssh into the VM:

```
$ vagrant ssh
```

Note that the VM's port 22 is being forwarded to the host as port 2222.  This means you can setup the `~/.ssh` files per usual, eg:

```
Host chef_tester
HostName 127.0.0.1
User vagrant
Port 2222
IdentityFile ~/.ssh/id_rsa
IdentitiesOnly=yes
StrictHostKeyChecking no
```
