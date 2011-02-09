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
Done in 8 millis.
Final Memory: 1724kB/83008kB
Final Memory: 773kB/83008kB (after GC)
==============
ZipInputStream
==============
Total of 829 entries.
Done in 587 millis.
Final Memory: 1454kB/83008kB
Final Memory: 762kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 114 millis.
Final Memory: 2125kB/83008kB
Final Memory: 779kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 49 millis.
Final Memory: 1476kB/83008kB
Final Memory: 774kB/83008kB (after GC)
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
Done in 652 millis.
Final Memory: 1454kB/83008kB
Final Memory: 762kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 117 millis.
Final Memory: 2125kB/83008kB
Final Memory: 779kB/83008kB (after GC)
===============
TrueZip ZipFile
===============
Total of 829 entries.
Done in 72 millis.
Final Memory: 1476kB/83008kB
Final Memory: 774kB/83008kB (after GC)
cstamas@marvin target$ 
</pre>

Have fun,  
~t~
