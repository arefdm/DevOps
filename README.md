<h2>list of docker command</h2>
<h3>Pulling</h3>
<ul>
<li>docker pull nginx</li>
</ul>
<h3>running</h3>
<ul>
<li>docker run -dp hostPort:containerPort --name containerName imageRepositoryName</li>
<li>docker start containerNameOrId (for stoped containers)</li>
</ul>
<h3>checking</h3>
<ul>
<li>docker ps </li>
<li>docker ps -a</li>
<li>docker logs containerNameOrId</li>
<li>docker images</li>
</ul>
<h3>stopping</h3>
<ul>
<li>docker stop containerNameOrId</li>
<li>docker rm containerNameOrId (to remove stoped containers)</li>
</ul>
<h2>Reflection questions</h2>
<ul>
<li>Actually, docker image is like a immutable blueprint or template that contains the application code, dependencies, configuration files,...; It's like a instruction to create a container. Docker container is a running instance of a docker image, it's an isolated environmet where an application runs. we can create multiple containers from the same image. </li>
<li>When we try to connect our container with the host we should select one of the host ports if another process or container is already using that port we will get that error. to improve this error we should select another host port</li>
<li>docker logs is a useful tool for monitoring docker container. Whit this command we can debuge and improve container problem specially when container is ran on background. it shows container activity or troubleshoot issues.</li>
</ul>
<h2>Screenshots</h2>
<img src:"./browser.png" />
<img src:"./running-container.png" />
<h2>Challenges faced<h2>
<caption>The first challenge for me was pulling the image, before I ran docker desktop or docker application I couldn't pull image or use other docker command but when I ran docker desctop this problem fixed.another problem that maight happend is squence of flags, names, repository in a command if we dont consider this sequence the command wont work properly docker --help can helps us to use flags correctly.</caption>