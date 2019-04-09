## Python Flask Docker template

This is a template projects for Flask framework.

`docker build -t <myimage> .`

Where `<myimage>` is the name of the image you desire to set to your new proyect.
Also, the ending `.` is related to the directory you are building against.

To run the image into a container, you'll run it with the command:

`docker run -d --name <mycontainer> -p 80:80 <myimage>`

The `-d` is to run the container on detach mode, just the opposite of interactive mode, so the console will return the control to the user.
The `--name mycontainer` is to tag the container with an human-friendly name to make it more recognizable.
The `-p 80:80` is to map the inner port 80 (into the container - right part) to the port 80 onto the host machine - the left part.
Finally, the `<myimage>` is the name of the image we've created early on this example.