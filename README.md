# Unlock
Buka NVidia brae

<pre>apt-get update && apt-get install gcc binutils make linux-source</pre>

<h3>Download driver</h3>
<p><i>https://nchc.dl.sourceforge.net/project/restream/NVIDIA-Linux-x86_64-418.43.run<i></p>
<pre>wget https://nchc.dl.sourceforge.net/project/restream/NVIDIA-Linux-x86_64-418.43.run</pre>
<pre>chmod +x NVIDIA-Linux-x86_64-418.43.run</pre>
<pre>./NVIDIA-Linux-x86_64-418.43.run</pre>
<h3>Check driver</h3>
<pre>nvidia-smi</pre>
<h3>Download patch & install patch driver</h3>
<pre>wget https://raw.githubusercontent.com/irtec/unlock/master/patch.sh</pre>
<pre>bash ./patch.sh</pre>
