
<h2><a id="user-content-10-running-your-first-container" class="anchor" aria-hidden="true" href="#10-running-your-first-container"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>1.0 Running your first container</h2>

Se sei qui è perchè l'installazione è andata correttamente e puoi iniziare a lavorare col primo docker run.

Apri il terminale e digita

<pre><code> $ docker pull alpine </code> </pre>

<p> Il comando <code> pull </code> permette di fare il fetch dell'image alpine dal Docker registry e la salva nel tuo sistema. Se sei curioso e vuoi vedere tutte le immagini (image) sul tuo sistema puoi usare questo comando.
<pre><code> $ docker images
REPOSITORY              TAG                 IMAGE ID            CREATED             VIRTUAL SIZE
alpine                 latest              c51f86c28340        4 weeks ago         1.109 MB
hello-world             latest              690ed74de00f        5 months ago        960 B
</code> </pre>
<h2><a id="user-content-10-running-your-first-container" class="anchor" aria-hidden="true" href="#10-running-your-first-container"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>1.1 Docker Run</h2>
<p> Ed ora finalmente puoi eseguire(run) il Docker container basata sull'image della quale è stato fatto il fetch. Esegui questo comando <code>docker run</code>
  
<pre><code>$ docker run alpine ls -l
total 48
drwxr-xr-x    2 root     root          4096 Mar  2 16:20 bin
drwxr-xr-x    5 root     root           360 Mar 18 09:47 dev
drwxr-xr-x   13 root     root          4096 Mar 18 09:47 etc
drwxr-xr-x    2 root     root          4096 Mar  2 16:20 home
drwxr-xr-x    5 root     root          4096 Mar  2 16:20 lib
......
</code></pre>
<p>
Quando lanci ii comando <code>run</code> succedono molte cose
<ol>
  <li>Il Docker client contatta il Docker daemon</li>
  <li>Il Docker daemon verifica sul tuo sistema se l'image è già presente (alpine in questo caso), in caso negativo la scarica dal Docker store</li>
  <li>Il Docker daemon crea il container ed esegue il comando nel container</li>
  <li>Il Docker daemon mostra l'output del comando al client</li>
  
  </p>











