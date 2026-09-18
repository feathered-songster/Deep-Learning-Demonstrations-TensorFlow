#  TensorFlow Deep Learning Demonstrations

A collection of small demonstrations for learning and experimenting with neural network architectures using **TensorFlow**.

This project is the TensorFlow counterpart to a sister project using PyTorch: **[PyTorch Deep Learning demonstrations](https://github.com/feathered-songster/Deep-Learning-Demonstrations-PyTorch**.

## Running

This project is intended to run in Docker. Build and start the environment with:

```bash
docker compose up --build
```

The project directory is mounted into the container at `/workspace`, so changes to notebooks and code remain on the host.

JupyterLab will be available at `http://localhost:8888`. The access token can be found in the container output when started.


