# Jupyterlab in a Docker Container
This is my template for building a development environment for Python with Jupyter Lab, Numpy, Pandas and Matplotlib.

### Prerequisite
Install docker and docker-compose
* https://docs.docker.com/get-docker/
* https://docs.docker.com/compose/install/

Install git or git desktop
* https://desktop.github.com/
* https://desktop.github.com/

<br/>

### Initial use
Clone by using this command below or download this repository from [here](https://github.com/RonBulaon/DockeredJupyterlab/archive/main.zip).
```
git clone https://github.com/RonBulaon/DockeredJupyterlab.git
```

<br />

Initial configuration will install Jupyter Lab and , Numpy, Pandas and Matplotlib. If you need more libraries you can add it at **requirements.txt** before running command below.

Then open a command line and execute this command inside **DockeredJupyterlab** diretory:
```
sudo docker-compose up
```
*note : If you are not using mac or linux, remove **sudo**.*

![alt text](images/dockercompose.gif )

Once done, you will be given a URL. Open the URL on your browser. The url will look like something like this:
```
http://127.0.0.1:8888/lab?token=791b3a7b1384100f39efe063e47b68d03647fa90ff8ba614
```

<br />

### Succeeding Usage

You can always run ```sudo docker-compose up``` again, but you can also start stop the docker images from dashboard. Dashboard is installed together with the docker. Once started, look for the container you have just created and click the play button.
![alt text](images/dashboard.png )
The URL will keep changing at every start of the docker image. You can check the the new URL by double-clicking the container from the dashboard to see the status.
![alt text](images/status.png )
All notebooks will be created at your local directory **notebooks**, including new folders.
![alt text](images/notebook.png)
![alt text](images/testfile.png)

<br />

### Copyright
Licensed under The MIT License (MIT). See [LICENSE](LICENSE) for more info.