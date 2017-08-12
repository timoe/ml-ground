# Machine Learning Playground

Here is a environment to explore machine learning methodologies setup with Docker. The Docker image contains tools like
- [sklearn](http://scikit-learn.org/)
- [Numpy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [Tensorflow](https://www.tensorflow.org/)

and installs [Jupyter](https://jupyter.org/) as an interactive enviroment to get your hands dirty.


Pull it from Docker Hub [https://hub.docker.com/r/timoeause/ml-ground/](https://hub.docker.com/r/timoeause/ml-ground/)
```
docker pull timoeause/ml-ground
```

and run

```
docker run -d -p 8888:8888 timoeause/ml-ground:latest
```

Jupyter is started on port 8888 and authentication is turned off. Just open [http://localhost:8888](http://localhost:8888)
A volume `notebook` is created for mounting your Jupyter Notebooks. Just use

```
docker run -d -p 8888:8888  -v [your-local-folder-containing-jupyter-notebooks]:/notebooks timoeause/ml-ground:latest
```

Have a lot of fun.
