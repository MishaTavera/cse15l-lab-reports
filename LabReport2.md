# Lab Report 2 
## Misha Tavera
---

## Part 1

Below is the code for the web server 'ChatServer' that supports the appropriate paths and behaviors for Lab 2. 

    import java.io.IOException;
    import java.net.URI;

    class Handler implements URLHandler {
        String messageString="";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format("enter message: %s", messageString);
        } else if (url.getPath().contains("/add-message")) {
            String[] parameters = url.getQuery().split("&");

            String user = "";
            String message = "";

            for (String param : parameters) {
                String[] keyValue = param.split("=");
                if (keyValue.length == 2) {
                    String key = keyValue[0];
                    String value = keyValue[1];

                    if ("user".equals(key)) {
                        user = value;
                    } else if ("s".equals(key)) {
                        message = value;
                    }
                }
            }

           if (user != null && message != null) {
                messageString += user + ": " + message + "\n";
                return messageString;
            }
        }

        return "404 Not Found!";
    }
    }

    class ChatServer {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);
        Server.start(port, new Handler());
    }
    }


![Image](image1LR2.png)

Upon creating a server the image above is what appears prompting us to enter a message. 
"https://0-0-0-0-1551-7ospflere607e0lv1591qpk9ok.us.edusercontent.com"

![Image](image2LR2.png)

I add the message "hello" from myself as the user with the request `/add-message?s=hello&user=mish`. The complete link is located just below. 

Here, the method in my code that is called is the `handleRequest` method. The relevant argument is `URI url` which represents an instance of a `URI`. When we use `/add-message?s=hello&user=mish` I am providing and instance of a `URI`. The method then uses this information, which follows the format as constructed in the code, to update our relevant field `messageString`. This string in this instance is initially set to be an empty string. After running the path that contains `/add-message` with query parameters `s=hello` and `user=mish` the field `messageString` is accordingly updated. This can be explained by following the code above, specifically, `else if (url.getPath().contains("/add-message"))`. As our request contains this `/add-message` the `message` and `user` are taken and then added to `messageString` and concatenated in this specific format. The value of `messageString` is now updated to the value `"hello"` appended to `"mish: "` (i.e. `"mish: hello"` followed by a new line) which is printed as shown above after the user's name. 

Example of what the complete link looked like for reference: 
`https://0-0-0-0-1551-7ospflere607e0lv1591qpk9ok.us.edusercontent.com/add-message?s=hello&user=mish`

![Image](image3LR2.png)

I add the message `"yay"` from the user `"maya"` with the request `/add-message?s=yay&user=maya`. The complete link for this is also shown below.

Once again the method from my code that is called here is the `handleRequest` method. The argument here is the `URI url` instance. In this case `/add-message?s=yay&user=maya`. As this is run on the server following the previous message we added, the initial field value here has the last added message `"mish: hello /n"`. Then after running this path with the new value `"yay"` and new user `"maya"`, which looks like `maya: yay` this value is added to the field. This can be explained similarly to what I have mentioned here and that is that the path contains `add-message` and therefore the `user` and `message` are added to the value in `messageString`. That is, in the `messageString` value is now `"mish: hello"` and `"maya: yay"` separated by a new line as written in the code. Here, the `messageString` value is not necessariy changed as our previous message is still a value but more is added. In short, it does not alter previous messages but the `messageString` adds new messages as they are added. This can be explained by looking at our code, ` messageString += user + ": " + message + "\n";`. Everytime a new message from a user is added the `+=` adds the new message to what is already added/stored in `messageString`. This occured as well in our first example only it was not as clear as the new user message was added to the intially empty string value in `messageString`.

Example of what the complete link looked like for reference. 

"https://0-0-0-0-1551-7ospflere607e0lv1591qpk9ok.us.edusercontent.com/add-message?s=yay&user=maya"


## Part 2

Absolute Path To The Private Key:

![Image](PrivateKey.png)

Here, I am using the ls command followed by a path to my own private key, which was created for my own local computer. This absolute path is for `ieng6` in my own computer. 

Absoulte Path To The Public Key:

![Image](PublicKey.png)

In this image I used the ls command followed by `~/.ssh/authorized_keys` to display the absolute path to my public key. Which is a path on `ieng6` file system 

Password No Longer Required:

After following these steps of the lab I am no longer required to enter a password to log into my `ieng6` acccount. 

![Image](nopassword.png)

## Part 3 

In week 2 and 3 I learned and practiced how to build and run a server. This is all very new to me so I did not know the process of any of it. I learned how to run the serve in my EdStem workspace `javac`,`java` commands, and a port number. I did not know what this was either, but now to my understanding it identifies the port number that the server runs on which is apart of a URL. Along with this I also learned how to use paths/queries in URL's which made changes depending on the code!
