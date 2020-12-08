CBSD
====
All files in this directory are modifications of originals from
[CBSD](https://cbsd.io) or CBSD outputs, updated in most cases to provide
support for passing Kubernetes-specific key-value pairs via cloud-init.

See this directory's parent README for more information.

## Files

### Configuration inputs

* `initenv.conf` - seed file for configuring CBSD installation
* `instance.jconf` - input for `cbsd bcreate`

### VM profile

(Assumes CBSD's user's home directory at `/usr/cbsd`)

* `usr.cbsd/etc/defaults/vm-linux-cloud-ubuntuserver-kubernetes-amd64-20.04.conf`
- Destination: 
`usr/cbsd/etc/defaults/vm-linux-cloud-ubuntuserver-kubernetes-amd64-20/04/conf`

### Cloud-init template

* `usr.local.cbsd/modules/bsdconf.d/cloud-tpl/kubernetes` - Destination: 
`/usr/local/cbsd/modules/bsdconf.d/cloud-tpl/kubernetes`

### Scripts
* `usr.local.cbsd/modules/bsdconf.d/cloudinit` - Destination:
`/usr/local/cbsd/modules/bsdconf.d/cloudinit`
* `usr.local.cbsd/sudoexec/bcreate` - Destination:
`/usr/local/cbsd/sudoexec/bcreate`
