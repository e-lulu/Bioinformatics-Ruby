BI TP 1, Lucie Vigreux, Edouard Delbar, groupe 2

----

**Question 9**

    ebola-t phage-lambda  4   1.0
    ebola-t phage-lambda  8   0.49244505494505497
    ebola-t phage-lambda  12  0.0029063622912703447
    ebola-t phage-lambda  16  0.0
    ebola-t phage-lambda  20  0.0

    ebola-z ebola-t       4   1.0
    ebola-z ebola-t       8   0.3799071338117349
    ebola-z ebola-t       12  0.025754697065653368
    ebola-z ebola-t       16  0.009396114864864864
    ebola-z ebola-t       20  0.0041182682154171065

La différence est significative sur des kmers de taille >= 12. On voit que les deux virus ebola sont plus proches que ebola-t et phage-lamba.

----

**Question 10**

    > ./bioseq random-mutations 2 test1.fasta | tail -n 1 ; echo ; tail -n 1 test1.fasta
    ATACTATACC
    ATACTGTACT

----

**Question 11**

    ebola-z ebola-mutant-10     12  0.9937196537893181
    ebola-z ebola-mutant-100    12  0.9392020265991133
    ebola-z ebola-mutant-1000   12  0.5282351699387798
    ebola-z ebola-mutant-10000  12  0.00506649778340722

On remarque que plus il y a de mutations moins il y a de kmers communs entre les 2 ADNs.

----

**Question 12**

    > ./bioseq list-spaced-kmers '##-##' test1.fasta 
    ATCT
    TATG
    ACGT
    CTTA
    TGAC
    GTCT

