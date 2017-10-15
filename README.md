#Pitanje 1:
Nakon što smo dodali class library kao referencu, u folderu Bin/Debug pojavile su se datoteke ClassLibrary1.dll i ClassLibrary1.pdb.
Nakon uklanjanja .dll class librarya te prilikom pokretanja aplikacie javlja se iznimka:
Unhandled Exception: System.IO.FileNotFoundException: Could not load file or assembly 'ClassLibrary1'
Problem je u tome što je programu nužna .dll datoteka kako bi mogao raditi jer se u njoj nalazi dio izvršnog koda (asemblija) koji mu je potreban za rad.
Kako bi ova aplikacija radila potrebne su .dll i .exe datoteke.

#Pitanje 2:
Nakon izmjene stringa u metodi PrintHelloWorld() i ponovnog pokretanja aplikacije bez prevođenja class library projekta, konzolna aplikacija je koristila i dalje staru verziju class library asemblija. Razlog je u tome što bez prevođenja nismo napravili novu verziju asemblija odnosno .dll datoteku.

#Pitanje 3:
Prilikom buid procesa obrisani direktorij packages se ponovno pojavio u solutionu te je aplikacija uspješno prevedena.
 


