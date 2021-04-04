# Let's Play with Erlang Language

```text
$ az group create --name pk-group-erlang-01 --location westeurope
...
```

```text
$ az vm create \
  --resource-group pk-group-erlang-01 \
  --name pk-vm-01 \
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
$ az vm show --show-details --name pk-vm-01 --resource-group pk-group-erlang-01
{
  ...
  "publicIps": <Public IP adrress>
  ...
}
```

```text
$ ssh radicel@<Public IP adrress>
```

```text
$ sudo apt-get update
...
$ sudo apt-get upgrade
...
$ sudo apt-get install erlang
...
```

```text
$ erl
Erlang/OTP 20 [erts-9.2] [source] [64-bit] [smp:1:1] [ds:1:1:10] [async-threads:10] [kernel-poll:false]

Eshell V9.2  (abort with ^G)
1> 
```

## References

* https://www.erlang.org/downloads
