# Demo for https://github.com/opensearch-project/security/issues/2054

if the max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]

`sudo sysctl -w vm.max_map_count=262144`

please note also the above command will be reseted after rebooting your machine, you need to set the value in /etc/sysctl.conf to make it permenant.
