# python-node-interview-environment
Docker Compose environment for secure coding interviews

To use this environment, first clone the repo, then:

```shell
cd interview-docker
docker compose up -d
docker compose exec interview bash
```

To create a start Node app:

```shell
npm create vite@latest test-app
cd test-app && npm start
```

To interact with the Node app using Python:
```shell
python3 -c "import urllib.request; print(urllib.request.urlopen('http://localhost:5173').read())"
```