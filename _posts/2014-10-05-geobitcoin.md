---
layout: post
title: geobitcoin - a thought experiment
---

<h1>{{ page.title }}</h1>


<p class="meta">12 October 2014 - Cambridge, MA</p>

<a href="http://blogs.wsj.com/accelerators/2014/10/10/weekend-read-the-imminent-decentralized-computing-revolution/"><i>The block chain is essentially a giant distributed cryptographic ledger shared amongst all nodes participating in the network, and keeps a record of every single successful transaction. This allows for trustless transactional activity. It facilitates ownership, storage, transfer and processing of information without the need for a middleman or identity information clearinghouse.

What this really means is that transactions, identity verification, trust, reputation and payments become quantifiable and programmable.</i></a>


One interesting consequence of a distributed economic transaction system, like <a href="http://en.wikipedia.org/wiki/Bitcoin">bitcoin</a>, is the difficulty in stabilizing the currency. Stabilization mechanisms for currencies are important as they can provide slower feedback to a system that responds rapidly to fluctuations. These fluctuations can be caused by changes in investor/user sentiment, security breaches, or other external macro-economic trends. Most government backed currencies give us the belief that our money will not evaporate when there is a crisis somewhere in the world; we no longer live in fear of our cash savings disappearing overnight (as was the case in <a href="http://en.wikipedia.org/wiki/Bank_run">bank-runs</a> in the 1930s) even though we have had economic crises on a much larger scale since then.

One huge challenge for a distributed economic system, is to regulate it in such a way that it behaves like a normal currency with stability and a collective belief in the value it holds. I'm not sure how <i>bitcoin</i> can be regulated overall, but I wanted to explore how to influence <i>bitcoin</i> transactions when considering geographic location. This modified cryptocurrency is named the <i>geobitcoin</i>!

The <i>geobitcoin</i> considers the geographic location of the <i>bitcoin</i> owner when they are performing a transaction. The key elements required for the transaction are:
* a method to identify the location of the user, providing an initial (untrusted) location
* a method of validating the untrusted location of the user, through a peer network
* the application of a monetary policy based on the location of the user for this transaction

This also assumes that we split the world into 10km grids and that there is a univeral monetary policy for each grid across the world. This would be performed using the following steps:

1. Person A who wishes to make a transaction, receives several GPS signals on their phone. These signals are transmitted as part of the transaction.

2. Peers (P) within a certain radius of A have to transmit timestamped GPS signals, within a certain time period to help validate the original location of A. A minimum of three peers are required and they need to be close enough such that they receive at least one common GPS signal to A, but far enough away so that A could not travel to those locations within fractions of a second.

3. Peers (identifed through GPS signal) have to send a message to A over a cellphone network, which is also relayed in a second step for the transaction. The latency of the message sent from each peer to A, is then used to assess the truthfullness of A's location.

4. The decentralized bitcoin mining process is used to compare the GPS signals from A, the cellphone messages sent from P to A, and assesses if A is providing a valid location.

Using this approach to verify the user's location means without any major infrastructure changes the system can then assess the truthfullness of A's location. If A's location is verified, then the appropriate monitory policy is applied to the transaction based on the quadrant that A is located within. There needs to be some benefit to A for verification; perhaps this transaction could have the value backed by an organization. If the location is unverified, it falls outside the guaranteed system.

Finally, one important reason that people want to use <i>bitcoin</i> is for privacy. The approach described above could reduce the anonymity associated with using this currency for transactions; it is important that it would be implemented in such a way that all locations are obfuscated.


<i>My thanks to <a href="http://twitter.com/@szelenagray">Szelena Gray </a> and <a href="http://twitter.com/@davidzwarg">David Zwarg</a> for discussing this crazy idea with me!</i>


<div id="disqus_thread"></div>
<script type="text/javascript">
    var disqus_shortname = 'djq';
    (function() {
        var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
        dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
        (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
    })();
</script>
<noscript>Please enable JavaScript to view<a href="http://disqus.com/?ref_noscript">comments</a></noscript>


<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-55619867-1', 'auto');
  ga('send', 'pageview');

</script>




