# Let's Play with Go Language

```text
$ az group create --name pk-group-go-01 --location westeurope
...
```

```text
$ az vm create \
  --resource-group pk-group-go-01 \
  --name vm-01 \
  --image UbuntuLTS \
  --admin-username radicel \
  --generate-ssh-keys
{
  ...
  "publicIpAddress": <Public IP adrress>
  ...
}
```

or

```text
$ az vm show --show-details --name vm-01 --resource-group pk-group-go-01
{
  ...
  "publicIps": <Public IP adrress>
  ...
}
```

```text
$ ssh radicel@<Public IP adrress>
radicel@vm-01:~$
```

```text
$ sudo apt-get update
...
$ sudo apt-get upgrade -y
...
```
