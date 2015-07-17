docker run -d -p 6060:80 -v /var/nod32/:/var/www/html/ -v /etc/localtime:/etc/localtime:ro -e NOD_LANGS=1049 -e NOD_VERSIONS=v5 ghostku/nod32-update-mirror
docker run -it -p 6060:80 -v /var/nod32/:/var/www/html/ -v /etc/localtime:/etc/localtime:ro -e NOD_LANGS=1049 -e NOD_VERSIONS=v5 ghostku/nod32-update-mirror
docker build -rm -t ghostku/nod32-update-mirror ./
