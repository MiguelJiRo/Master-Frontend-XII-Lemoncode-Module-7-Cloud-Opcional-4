# Master-Frontend-XII-Lemoncode-Module-7-Cloud-Opcional-4

# Master Frontend XII Lemoncode 🍋

## Module 7 CLOUD

### opcional parte 4

<br>

[Go back - Index](https://github.com/MiguelJiRo/Master-Frontend-XII-Lemoncode)

<br>

<img align="center" src="https://media.giphy.com/media/7j2hfyeVcDtf2/giphy.gif" width="128px">

<br>

### Parte opcional - 4

<ol>
    <li>✅ Desplegar aplicación front con Docker y AWS.</li>
</ol>

Para el desarrollo de esta parte se ha partido del ejemplo de: https://github.com/Lemoncode/master-frontend-lemoncode/tree/master/07-cloud/03-docker/06-aws-deploy

![config](./images/awsconfigcorrect.png)

<br>

sudo yum update -y

<br>

sudo yum install -y docker

<br>

![docker](./images/installdocker.png)

<br>

creamos una imagen de docker de nuestro repositorio:

<br>

![dockerimage](./images/dockerimage.png)

se importa la imagen de docker a docker hub con el comando
<br>
sudo docker run --rm -d -p 80:8000 &&&&&&/my-app
<br>

![dockerlatest](./images/dockerlatest.png)
<br>

Una vez tengo la parte de AWS lista y la parte de Docker hub lista, ejecutamos el servicio de docker en AWS con:
<br>
"sudo service docker start"
<br>
Nos quedaría traernos el contenedor del docker hub con:
<br>
"sudo docker run --rm -d -p 80:8000 &&&&&&/my-app"
<br>
Comprobamos con "sudo docker ps" que tenemos el contenedor funcionando.
<br>

### Resultado

![awsurl](./images/awsurl.png)

<br>

#### URL:

http://ec2-16-171-10-141.eu-north-1.compute.amazonaws.com/

<br>

http://16.171.10.141/

<br>

![direccion](./images/direccion.png)
