# conda-export
Smple bash script to export every environment defined by conda to a yml file. 



# Usage Examples 

Full export of every environment 
```
user@server:~/conda_evns$ ./conda-export -v
Will serach for existing environments...
Found environments: env_test1 env_test2 base
Exclude environments: base
Include environments: env_test1 env_test2
Export environments: env_test1 env_test2
Export env_test1 to /home/user/env_test1.yml
Export env_test2 to /home/user/env_test2.yml
FINISHED
```

Export with exclude

```
user@server:~/conda_evns$ ./conda-export -e base,env_test2 -v
Will serach for existing environments...
Found environments: env_test1 env_test2 base
Exclude environments: base env_test2
Include environments: env_test1 env_test2
Export environments: env_test1 env_test2
Export env_test1 to /home/user/env_test1.yml
FINISHED
```
