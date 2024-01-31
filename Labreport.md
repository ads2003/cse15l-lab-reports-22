#Lab Report 2 - Servers and SSH Keys (Week 3)

##Part 1(Web Server)

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
**In the first of the two screenshots, the main function and handleRequest are called. The URL is the parameter to call handleRequest, and port 5001 is the argument to call the main function. The value of s is appended and a new line is added each time a new message is added via the website or after the survey is completed. In addition to moving to the next line each time, the new message is appended to the initial empty String s, where path[1] is the new message added.** 

