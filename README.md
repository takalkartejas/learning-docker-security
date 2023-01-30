# learning-docker-security

# learning_docker

Video link - https://www.youtube.com/watch?v=KINjI1tlo2w&t=303s

---

## Theory


---

## Learning steps:

   


   1. Create a demo docker file and images called protect
   2. If we run a normal docker container it shows root which gives anyone root access to our docker.
   3. Create two users tejas and alex where only tejas is added to the sudo group
   4. After running docker using each of this users there name is visible instead of root
   ``` bash
   docker run -u alex -it --rm protect /bin/bash

   ```

   5. If we try to edit the text.txt file and save, it says permission denied
   6. We can use sudo but it needs password which needs to be somehow set


---

## Usefull commands:
### 1. Docker images
   1. 



