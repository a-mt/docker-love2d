
# Docker-Love2d

Installs

* love2d (framework for 2D games in Lua)
* ZeroBraneStudio (IDE) / lua

## Install

    sudo docker-compose build

## Launch ZeroBraneStudio

    xhost local:root
    sudo docker-compose run --rm love2d
    ./zbstudio.sh /home/project

Change the settings of the editor:  
`Project > Lua interpreter > LÖVE`

When you're finished:

    sudo docker-compose down

---

Ressources that have been useful:  
[@pkulchenko/ZeroBraneStudio](https://github.com/pkulchenko/ZeroBraneStudio)  
[studio.zerobrane.com](https://studio.zerobrane.com/download?not-this-time)