---
layout: default
title: Basic Docker Commands
order: 2
---

{% highlight bash %}

docker run -i -t stackbrew/ubuntu:14.04 env

docker run -i -t stackbrew/ubuntu:14.04 echo "hi workshop peeps"

docker run -d -t stackbrew/ubuntu:14.04 sleep 1000

docker ps

docker ps -q

ID=$(docker ps -q)

docker inspect $ID

docker kill $ID

docker kill $(docker ps -q)
{% endhighlight %}

Exercises
---------

 * Using `fig log` check the stdout of a container
 * Try out `fig attach` on a detached running container
 * With an interactive container, pipe the output to a file or another bash command