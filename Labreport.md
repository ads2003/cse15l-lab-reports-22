# Lab Report 2 - Servers and SSH Keys (Week 3)

## Part 1(Web Server)

~~~
import java.io.IOException;
import java.net.URI;

// Interface to handle URL requests
interface URLHandler {
    String handleRequest(URI url);
}

// Implementation of URLHandler for handling chat-related requests
class ChatHandler implements URLHandler {
    private String chatHistory = "";

   
    public String handleRequest(URI url) {
        if (url.getPath().equals("/add-message")) {
            String[] parameters = url.getQuery().split("&");


            if (parameters.length == 2) {
                String message = parameters[0].split("=")[1];
                String user = parameters[1].split("=")[1];
                chatHistory += user + ": " + message + "\n";
                return "Message added successfully: " + user + ": " + message;
            } else {
                return "Invalid request. Both 's' and 'user' parameters are required.";
            }
        }
        return chatHistory;
    }
}

// Main class to start the chat server
class ChatServer {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number! Try any number between 1024 to 49151:");
            return;
        }

        int port = Integer.parseInt(args[0]);
        Server.start(port, new ChatHandler());
    }
}
~~~
<img width="401" alt="avani lab 2" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/58e421f0-b141-4bfb-a820-e1c86b40a41b">

<img width="590" alt="Aditya lab 2 r" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/0090bcc0-0205-4818-8a85-af4a7159d005">

**In the first of the two screenshots, the main function and handleRequest are called. The URL is the parameter to call handleRequest, and port 5001 is the argument to call the main function. The value of s is appended and a new line is added each time a new message is added via the website or after the survey is completed. In addition to moving to the next line each time, the new message is appended to the initial empty String s, where path[1] is the new message added.
A relevant field is chat history and before making add message request it is an empty string. When i make the add message request the chat history field changes from an empty string to "avani.. namaste/n". When i do this for the second add message request the chat history field changes from "avani.. namaste/n" to "avani.. namaste/nAditya:Whats up/n" ** 

## Part 2
<img width="396" alt="private key" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/4d4a5949-2467-47da-ba21-c99c950faa00">

<img width="398" alt="public key " src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/de20642e-4de3-48e9-8ff0-0cc2e9fa79ae">

<img width="767" alt="login without pass" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/b8eb6963-91f7-4d51-8d22-f0b5123c286c">





## Part 3(What did I learn till now)

**Creating your first webpage from scratch. What software bugs and symptoms are. Primarily, I gained knowledge about junit testing, which is highly relevant to CSE programming assignments.**


