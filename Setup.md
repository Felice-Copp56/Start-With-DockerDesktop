Prima di procedere al primo esempio di docker container è necessario scaricare il docker desktop per la tua versione di sistema operativo.

Puoi scaricare la versione per Windows da qui <a href="https://docs.docker.com/docker-for-windows/install/" rel="nofollow">Windows</a>

Una volta scaricata, installala seguendo i passi esposti dall'installer.

Dopo aver scaricato e installato il file è possibile usare Powershell per testare e verificare la corretta installazione tramite il comando:

<pre><code>$ docker run hello-world
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
03f4658f8b78: Pull complete
a3ed95caeb02: Pull complete
Digest: sha256:8be990ef2aeb16dbcb9271ddfe2610fa6658d13f6dfb8bc72074cc1ca36966a7
Status: Downloaded newer image for hello-world:latest

Hello from Docker.
This message shows that your installation appears to be working correctly.
...
</code></pre>

Vai al file per l'esempio [Docker first run](docs/dockerun.md)
