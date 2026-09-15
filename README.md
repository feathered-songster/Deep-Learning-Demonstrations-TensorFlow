## Running

This project is intended to run in Docker. Build and start the environment with:

```bash
docker compose up --build
```

The project directory is mounted into the container at `/workspace`, so changes to notebooks and code remain on the host.

JupyterLab will be available at `http://localhost:8888`. The access token can be found in the container output when started.


