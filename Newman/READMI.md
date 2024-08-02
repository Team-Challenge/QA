## Newman is a tool that allows you to run and test Postman collections directly from the command line, allowing you to integrate with continuous integration servers


### Comand install Newman 

```
npm install -g newman 
```

### Running a collection via the command line

``` 
newman run Name_of_the_collection.postman_collection.json 
```

### Newman-html-reporter will be used to generate the report. To install it, you need to execute the command

```
npm install -g newman-reporter-html
```

``` 
newman run Name_of_the_collection.postman_collection.json -r html
```

### Or a team

``` 
newman run Name_of_the_collection.postman_collection.json --insecure --reporters cli,htmlextra --reporter-htmlextra-export "report.html" 
``` 

### When Newman works with files, you need to write the full path to it in the .json file

```
{
							"key": "image",
							"description": "(Required) ",
							"type": "file",
							"src": "foto_profil/PNG.png"
						}
```

