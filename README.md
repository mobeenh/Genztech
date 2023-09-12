# Genztech

# Flow-1: Pull Docker Image from Docker Hub and Run it

## Step-1: Verify Docker version and also login to Docker Hub
```
docker version
docker login
```

## Step-2: Pull Image from Docker Hub
```
docker pull tomcat
```

## Step-3: Run the downloaded Docker Image & Access the Application
- Copy the docker image name from Docker Hub
```
docker run -d --name mytomcatcontainer -p 8082:8080 tomcat
http://localhost:8082


```

## Step-4: List Running Containers
```
docker ps
docker ps -a
docker ps -a -q
```

## Step-5: Connect to Container Terminal
```
docker exec -it <container-name> /bin/sh
```

## Step-6: Container Stop, Start 
```
docker stop <container-name>
docker start  <container-name>
```

## Step-7: Remove Container 
```
docker stop <container-name> 
docker rm <container-name>
```

## Step-8: Remove Image
```
docker images
docker rmi  <image-id>
```
## Tomcat is a web server and servlet container that is used to host and run Java-based web applications. It's like a bridge between your web application and the internet, making it accessible to users through their web browsers. Here's a simple explanation with an example:

```
Imagine you have built a website using Java programming language. Your website has interactive features like user registration, login, and dynamic content generation. To make this website accessible on the internet, you need a web server, and this is where Tomcat comes in.
```

## Example:
Let's say you created a Java-based online store. When a user visits your online store's website, their web browser sends a request to view a product page. This request goes to Tomcat.

```
1. Tomcat receives the request: Tomcat is responsible for handling this request. It understands Java code, so it knows how to process it.
```
2. Tomcat runs your Java code: In your online store's Java code, you might have instructions to fetch product information from a database, format it into a webpage, and send it back to the user's browser.

3. Tomcat sends the response: After running your Java code, Tomcat sends the generated webpage back to the user's browser as a response.

4. User sees the webpage: The user's web browser receives the response from Tomcat and displays the product page on their screen.

## So, in simple terms, Tomcat serves as a middleman that understands Java and helps your web application communicate with users' web browsers. It takes requests, processes them using your Java code, and sends back the appropriate web pages. This way, your Java-based web application can be accessed and interacted with on the internet.
