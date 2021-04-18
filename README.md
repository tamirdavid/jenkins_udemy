# jenkins_udemy
<h4>Jenkins udemy course repo <h4/>

> ssh-keygen -f remote-ki -m PEM - to create public and private key <br>
>docker cp remote-ki jenkins:/tmp/remote-ki - copy private key to the remote-host docker image <br>
>docker exec -u root jenkins bash -c "chown 1000:1000 /tmp/remote-ki" - chmod the permissions on that file <br>
>docker-compose build <br>
>docker-compose up <br>
<br>
After finished the instructions above you should be able communicate from jenkins to remote host using ssh without password
<br>
>ssh -i /tmp/remote-ki remote_user@remote_host
<br>
If it works configure a new host in jenkins UI ( store creds inside jenkins credentials, the creds will be username and ssh key)

