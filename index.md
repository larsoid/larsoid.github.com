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
