# Docker image for MRI online course

<b>🐳 Running with Docker </b> </font> <br>

If you have Docker installed on your computer and running, you can run the code 
in the same environment described in this repository using `repo2docker`. 

1. Simply install `repo2docker` from pyPI: 
```
pip install jupyter-repo2docker
```
2. Run the following command in your terminal:
```
jupyter-repo2docker https://github.com/neurolibre/myelin-meta-analysis
```

After building (it might take a while!), it should output in your terminal 
something like:

```
Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://0.0.0.0:36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0
```

This should start a Jupyter session on your browser and make all the resources 
you see when you [launch a Binder](https://mybinder.org/v2/gh/neurolibre/myelin-meta-analysis/master) for this repository. 

To re-use your container built by repo2docker, do the following: 

1. Run `docker images` command and copy the `IMAGE ID` to your clipboard 
2. Run the following command to start the container:
```
docker run -it --rm -p 8888:8888 `PASTE IMAGE ID HERE` jupyter notebook --ip 0.0.0.0
```


<br>


<p align="center">
<img src="https://avatars3.githubusercontent.com/u/63861117?s=200&v=4" style="width:12px;"></img> <br>
This repository is created by <a href="https://github.com/Notebook-Factory">Notebok-Factory</a>. 
</p>
