Step 0. Create docker network
`docker network ls | grep web || docker network create web`

Step 1. Deploy Script
Refer to (deploy script)[./Taskfile], in function `baseDeployScript`

Step 2. Configure ENV variables, and set Traefik Dashboard password
!!! Recommended doing via SSH, even you could fdo it from Forge's UI "Run command"
```
./Taskfile copyEnv
./Taskfile auth username password

```
