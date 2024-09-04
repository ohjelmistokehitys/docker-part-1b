# Part 1 section 5: Interacting with the container via volumes and ports

The theory for the following exercises is presented at https://devopswithdocker.com/part-1/section-5.

> [!WARNING]
> Security reminder: Opening a door to the internet
>
> Since we are opening a port to the application, anyone from the internet could come in and access what you're running.
>
> Don't haphazardly open just any ports - a way for an attacker to get in is by exploiting a port you opened to an insecure server. An easy way to avoid this is by defining the host-side port like this -p 127.0.0.1:3456:3000. This will only allow requests from your computer through port 3456 to the application port 3000, with no outside access allowed.
>
> The short syntax, -p 3456:3000, will result in the same as -p 0.0.0.0:3456:3000, which truly is opening the port to everyone.
>
> Usually, this isn't risky. But depending on the application, it is something you should consider!
>
> *Source: https://devopswithdocker.com/part-1/section-5*


## Exercise 1.9: Volumes *(10 %)*

> In this exercise we won't create a new Dockerfile.
>
> Image `devopsdockeruh/simple-web-service` creates a timestamp every two seconds to `/usr/src/app/text.log` when it's not given a command. Start the
> container with bind mount so that the logs are created into your filesystem.
>
> Submit the command you used to complete the exercise.
>
> **Hint:** read the note that was made just before this exercise!
>
> *Source: https://devopswithdocker.com/part-1/section-5#exercise-19*

**Save the command(s) you used to complete the exercise in the file [ex-1-09.txt](./ex-1-09.txt).**


## Exercise 1.10: Ports open *(10 %)*

> In this exercise, we won't create a new Dockerfile.
>
> The image `devopsdockeruh/simple-web-service` will start a web service in port `8080` when given the argument "server". In [Exercise 1.8](https://devopswithdocker.com/part-1/section-3#exercises-17---18) you already did a image that can be used to run the web service without any argument.
>
> Use now the -p flag to access the contents with your browser. The output to your browser should be something like:
> `{ message: "You connected to the following path: ...`
>
> Submit your used commands for this exercise.
>
> *Source: https://devopswithdocker.com/part-1/section-5#exercise-110*

**Save the command(s) you used to complete the exercise in the file [ex-1-10.txt](./ex-1-10.txt).**
