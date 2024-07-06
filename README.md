# DockerPractical
I had used css free template for practical.
https://www.free-css.com/free-css-templates/page296/carvilla

1. create Dockerfile - nginxDockerfile
2. created nginx configured file from chatgpt - nginx.conf
3. extraced the download file on the same location of Dockerfile.
4. on nignx.config file, added the root location for the index file.
       - /usr/share/nginx/html/assets   -- at nginx.conf
       - index.html to /usr/share/nginx/html/index.html    -- copy command at dockerfile.
5. check if the image is there -- docke images
6. build the image form docker file  -- docker build -t my-nginx -f nginxDockerfile .
7. run the conainter -- docker run -d -p 80:80 my-nginx
8. check the container running -- docker ps
9. check ip
10. check the website with your ip : http://yourip
