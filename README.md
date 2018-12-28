# cvlib

Runs https://github.com/arunponnusamy/cvlib inside docker.

# Install
```
docker build github.com/handflucht/cvlib
```

or get image from


Working directory is ```/cvlib/examples```.

# Example Usage
```bash
docker run -ti --rm handflucht/cvlib python3 face_detection.py images/face_detection_input.jpg
Using TensorFlow backend.
[[510, 113, 645, 318], [1588, 97, 1748, 298], [1176, 76, 1316, 263], [188, 223, 345, 437], [811, 201, 937, 383]]
[0.990442, 0.9830966, 0.9760147, 0.9192408, 0.8850806]
: cannot connect to X server
```

You can provide the display variable to view the output:
```
docker run -ti --rm -e DISPLAY=<....> ...
```