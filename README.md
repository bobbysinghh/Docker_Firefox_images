# Docker_Firefox_image

## To Build the Docker Image
Now build this image using the docker build command.

`docker build -t <image name> .`

Here in my case image name is bobby8249/firefox ."bobby8249" is my account name in docker hub. 

## To Build Download(pull) Docker Image

Run Docker Pull Command
`docker pull bobby8249/firefox`


## Launch GUI application On the Docker container
For a GUI Application to run,

Now, run the container using the above-created image

Note: 

docker run -it is used to launch the container
●       Share the DISPLAY environment variable to the Container OS

   `--env="DISPLAY"`

●       run the OS with Host’s Network driver

      `--net=host`

These extra arguments are used to set up the base OS environment inside the container


`docker run -it --name=GUI_Container --env="DISPLAY" --net=host bobby8249/firefox`
