Simple comparison of memory consumption and speed of various Zip solutions in Java.


Results
=======

Example "session":

<pre>
cstamas@marvin target$ l nexus-oss-webapp-1.10-SNAPSHOT-bundle.zip 
-rw-r--r--  1 cstamas  staff  28783146 Feb  9 14:11 nexus-oss-webapp-1.10-SNAPSHOT-bundle.zip
cstamas@marvin target$ java -jar ziptest-1.0.0-SNAPSHOT-cli.jar all nexus-oss-webapp-1.10-SNAPSHOT-bundle.zip 
=======
ZipFile
=======
Total of 829 entries.
Done in 7 millis.
Final Memory: 1724kB/83008kB
Final Memory: 773kB/83008kB (after GC)
==============
ZipInputStream
==============
Total of 829 entries.
Done in 592 millis.
Final Memory: 1454kB/83008kB
Final Memory: 762kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 80 millis.
Final Memory: 2125kB/83008kB
Final Memory: 779kB/83008kB (after GC)
=============
TrueZip TFile
=============
Total of 2 entries.
Done in 283 millis.
Final Memory: 6946kB/83008kB
Final Memory: 867kB/83008kB (after GC)
cstamas@marvin target$ java -jar ziptest-1.0.0-SNAPSHOT-cli.jar all nexus-oss-webapp-1.10-SNAPSHOT-bundle.zip 
=======
ZipFile
=======
Total of 829 entries.
Done in 6 millis.
Final Memory: 1724kB/83008kB
Final Memory: 773kB/83008kB (after GC)
==============
ZipInputStream
==============
Total of 829 entries.
Done in 590 millis.
Final Memory: 1454kB/83008kB
Final Memory: 762kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 97 millis.
Final Memory: 2125kB/83008kB
Final Memory: 779kB/83008kB (after GC)
=============
TrueZip TFile
=============
Total of 2 entries.
Done in 253 millis.
Final Memory: 6946kB/83008kB
Final Memory: 867kB/83008kB (after GC)
cstamas@marvin target$ java -jar ziptest-1.0.0-SNAPSHOT-cli.jar all nexus-oss-webapp-1.10-SNAPSHOT-bundle.zip 
=======
ZipFile
=======
Total of 829 entries.
Done in 6 millis.
Final Memory: 1724kB/83008kB
Final Memory: 773kB/83008kB (after GC)
==============
ZipInputStream
==============
Total of 829 entries.
Done in 592 millis.
Final Memory: 1454kB/83008kB
Final Memory: 762kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 84 millis.
Final Memory: 2125kB/83008kB
Final Memory: 779kB/83008kB (after GC)
=============
TrueZip TFile
=============
Total of 2 entries.
Done in 266 millis.
Final Memory: 6946kB/83008kB
Final Memory: 867kB/83008kB (after GC)
cstamas@marvin target$ 
</pre>

Have fun,  
~t~
