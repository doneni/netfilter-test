# netfilter-test

<b>Build</b>
<pre>
  <code>
    gcc -o nfqnl_test nfqnl_test.c -lnetfilter_queue
  </code>
</pre>

<b>Usage</b>
<pre>
  <code>
    netfilter-test <host>
  </code>
</pre>

<b>Iptables</b>
<pre>
  <code>
    sudo iptables -F
    sudo iptables -A OUTPUT -p tcp -j NFQUEUE
    sudo iptables -A INPUT -p tcp -j NFQUEUE
  </code>
</pre>

<br>
This code based on [netfilter.org](https://netfilter.org/projects/libnetfilter_queue/downloads.html) <br>
You should place this repo on <i>libnetfilter_queue-1.0.3/here</i> <br>
