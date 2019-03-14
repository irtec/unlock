# Unlock
Buka NVidia brae

<pre>apt-get update && apt-get install gcc binutils make linux-source</pre>
<h3>Block modprobe</h3>
<pre>nano /etc/modprobe.d/blacklist-nouveau.conf</pre>
<pre>   blacklist nouveau
   options nouveau modeset=0</pre>
<pre>update-initramfs -u</pre>

<h3>Download driver</h3>
<p><i>https://excellmedia.dl.sourceforge.net/project/restream/NVIDIA-Linux-x86_64-418.43.run<i></p>
<pre>wget https://excellmedia.dl.sourceforge.net/project/restream/NVIDIA-Linux-x86_64-418.43.run</pre>
<pre>chmod +x NVIDIA-Linux-x86_64-418.43.run</pre>
<pre>./NVIDIA-Linux-x86_64-418.43.run</pre>
<h3>Enabled Persistence</h3>
<pre>nvidia-smi -pm 1</pre>
<h3>Check driver</h3>
<pre>nvidia-smi</pre>
<h3>Download patch & install patch driver</h3>
<pre>wget https://raw.githubusercontent.com/irtec/unlock/master/patch.sh</pre>
<pre>bash ./patch.sh</pre>
   
   <p><i>Thanks https://github.com/keylase</p></i>
