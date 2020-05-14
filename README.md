# OLACEFS DAM

Este projeto de pesquisa objetiva desenvolver metodologias para prospectar instrumentos que permitam incorporar geotecnologias no processo de seleção de objetos de controle relacionados à área ambiental.

Especificamente, o projeto se baseia em uma parceria da Organização Latino-Americana e do Caribe de Entidades Fiscalizadoras Superiores (OLACEFS) com o laboratório Pattern Recognition and Earth Observation – Patreo/DCC/UFMG.

São propostos dois temas para serem explorados nesse projeto:
  * Monitoramento de barragens de rejeitos de minérios
  * Identificação de desmatamentos na região amazônica por meio de radar


### Prerequisites

What things you need to install the software and how to install them

```
Docker Engine
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Docker Engine: https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository
Nvidia-Docker (for gpu support)
```

And repeat

```
# Docker installing steps
sudo apt-get install     apt-transport-https     ca-certificates     curl     software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
sudo docker run hello-world

# Nvidia-Docker installing steps
curl -s -L https://nvidia.github.io/nvidia-docker/gpgkey |   sudo apt-key add -
distribution=$(. /etc/os-release;echo $ID$VERSION_ID)
curl -s -L https://nvidia.github.io/nvidia-docker/$distribution/nvidia-docker.list |   sudo tee /etc/apt/sources.list.d/nvidia-docker.list
sudo apt-get update
sudo apt-get install -y nvidia-container-toolkit
sudo reboot
```

End with an example of getting some data out of the system or using it for a little demo

## Running the docker container

```
docker run -it --gpus all --ipc=host --name=olacef_container -w /home -v /home:/home edemirfaj/patreo_bot:gpu-py3 bash
```

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Authors

* **Alice Gomes** - *Initial work* - []()
* **Edemir Ferreira** - *Initial work* - [edemir-matcomp](https://github.com/edemir-matcomp)
* **Ester Fiorillo** - *Initial work* - []()
* **Matheus Brito** - *Initial work* - [mbfaria](https://github.com/mbfaria)
* **Pedro Fonseca** - *Initial work* - [PedroFW](https://github.com/PedroFW)



See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.


## Acknowledgments

* Organização Latino-Americana e do Caribe de Entidades Fiscalizadoras Superiores (OLACEFS)


