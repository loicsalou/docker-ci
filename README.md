Pour une raison qui m'échappe je dois partager le volume "tmp" et non pas "private" pour pouvoir faire le "docker-compose up".

export hostDir="tmp"
export yourUrl="localhost"

docker-compose up


Si j'essaie de pointer sur "private" par ex avec
export hostDir="private/var/lib/docker/volumes" j'ai un access denied sur la création des volumes.