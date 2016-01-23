---
layout: page
title: Theory and practice
tagline: In theory there is no difference between theory and practice. In practice there is.
---
{% include JB/setup %}

<h3>mysqldump: Error: Binlogging on server not active</h3>

Error: Binlogging on server not active
<p>Solution:</p> 

1) Option "--master-data" in your mysqldump should be removed
<br>(Note: this will cause mysql to skip replication position)

2) Edit you mysql server configuration (my.cnf) and add log-bin=mysql-bin
<br>(Note: restart MySQl Server after change)

<hr>
Piet Hein wrote this "short verse" that has been an inspiration to me when 
feeling that things are ... not happening fast enough:

"
<h3>T. T. T.</h3>
<br>
Put up in a place
where it's easy to see
the cryptic admonishment
<b>T. T. T.</b>
<br>
When you feel how depressingly
slowly you climb,
it's well to remember that
<b>Things Take Time!</b>
"
<hr>
<br>
Thinking about writing a verse of my own with the title: "E.E.E" 
<br>
<b>Escaping Explicit Expectations</b>  
