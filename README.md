# Machine Learning Playground

Here is a environment to explore machine learning methodologies setup with Docker. The Docker image contains tools like
- [sklearn](http://scikit-learn.org/)
- [Numpy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [Tensorflow](https://www.tensorflow.org/)

and installs [Jupyter](https://jupyter.org/) as an interactive enviroment to get your hands dirty.

Jupyter is started on port 8888 and authentication is turned off.

# Build

Clone this repository and run

```
docker build . -t <image-name-here>
```

# Run

```
docker run -d -p 8888:8888 -v [your-local-folder-containing-jupyter-notebooks]:/notebooks <image-tag-here>
```
