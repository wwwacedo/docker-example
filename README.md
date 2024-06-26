# Create a docker image

1. Clone the repository with HTTPS:
	```bash
	git clone https://github.com/wwwacedo/docker-exemple.git
	```

<br>

2. Access the directory:
	```bash
	cd app-exemplo
	```

<br>

3. Generate the image from the Dockerfile, using -t to create a tag:
	```bash
	docker build -t mmm/app-node:1 .
	```

	- In the command above: 
		- `:1` is used to specify version;
		- `.` refers to the current directory.  

<br>

4. In the terminal, to create the container:
	```bash
	docker run -d -p 8080:3000 mmm/app-node:1
	```

<br>

5. In the browser, access the application at http://localhost:8080 

