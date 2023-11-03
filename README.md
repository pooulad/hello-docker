# hello-docker

Say hello to docker<br/>

<img width="271" alt="iot_containers" src="https://github.com/pooulad/hello-docker/assets/86445458/ec4b8e1f-92f2-4feb-8b8f-8eae4c7bed4d">

## What you need? :

Just make sure you have nginx in your images<br/>
Download nginx image: 
```bash
  sudo docker pull nginx
```

## Build image :

First in the root of project run: 
```bash
  sudo docker build -t html-server-image:v1 .
```

## How to run :

Now its time to create your container: 
```bash  
  sudo docker run --rm -d -p 8080:80 html-server-image:v1
```

Open your browser and open -> localhost:8080/app.html
You should see this page :

![Screenshot from 2023-11-02 14-18-23](https://github.com/pooulad/hello-docker/assets/86445458/557e0bca-1c0c-4866-8be7-0e6fd2852389)

Or you can curl in terminal:
```bash
  curl localhost:8080/app.html
```
![image](https://github.com/pooulad/hello-docker/assets/86445458/3d25394e-128e-4d35-ae95-21c9e51b8eee)


Congratulations :) you did it.
