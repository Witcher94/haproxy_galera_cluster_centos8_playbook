# haproxy_galera_cluster_centos_8

#### To run the playbook 

`ansible-playbook --fork=1 deploy_galera_cluster.yml -i inventory.yml` for deploying galera cluster.



`ansible-playbook --fork=1 deploy_haproxy_balancer4cluster.yml -i inventory.yml` for adding haproxy balancer.


### For adding new hosts
add hosts to `inventory.yml`

Note: Do not modify the host group names [galera_nodes] and [haproxy_servers] when adding hosts to `inventory.yml` file since it has dependencies inside the playbook. 


P.S. User parameter fork for starting cluster in correct order 
