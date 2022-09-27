# kubectlexec-filemanager

- docker build -t filegator .
- docker run -p 8000:80 -d filegator

# Cleanup
- git add -A .
- git commit -am "removing"
- git push -u origin main


# Build
## remove zip file 
- rm -rf filegator_latest.zip
## Save the changes and zip the file
- zip -r filegator_latest.zip filegator

