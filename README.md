# Ubuntu dotnet DinD (Docker in Docker) Image

🤓 The **dotnet** image with **DinD** support!

🐳 **DinD** (**Docker** in *Docker*) allows you to use docker inside of this image. This is supported by running dockerd. This is **the** image for simulating build pipeline machines which rely heavily on docker support for **dotnet** pipelines.

⚠️ This image requires to run in **privileged** mode. 
``docker run --privileged karolczajkowski/dotnet-ubuntu-dind``

## Environment

* Ubuntu **20.04**
    * **dotnet** SDK 3.1
    * **asp.net core** runtime 3.1
    * **pwsh** (PowserShell 7)
    * **git**
    * **docker** 19.03.11
    * **docker-compose** 1.26.0
    * **wget**

## How to use

````bash
docker run -it --privileged karolczajkowski/dotnet-ubunt-dind
````

Will run a shell with a completely seperate docker environment.

## Source

I took inspiration from [cruizba/ubuntu-dind](https://github.com/cruizba/ubuntu-dind).


