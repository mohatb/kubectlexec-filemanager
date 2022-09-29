# kubectlexec-filemanager

- docker build -t filemanager .
- docker run -p 8000:80 -d filemanager

# Push
- git add -A .
- git commit -am "removing"
- git push -u origin main


# Build
## remove zip file 
- rm -rf filegator_latest.zip
## Save the changes and zip the file
- zip -r filegator_latest.zip filegator


# Cleanup
- docker rm -f $(docker ps -a -q)
- docker rmi -f $(docker images -aq)
- docker volume rm $(docker volume ls -q)

