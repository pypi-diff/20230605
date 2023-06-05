# Comparing `tmp/SBILoops-0.1.tar.gz` & `tmp/SBILoops-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILoops-0.1.tar", last modified: Mon Jun  5 20:01:32 2023, max compression
+gzip compressed data, was "SBILoops-0.2.tar", last modified: Mon Jun  5 20:35:16 2023, max compression
```

## Comparing `SBILoops-0.1.tar` & `SBILoops-0.2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.609391 SBILoops-0.1/
--rw-r--r--   0 patrick    (501) staff       (20)      220 2023-06-05 20:01:32.610174 SBILoops-0.1/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 17:30:37.000000 SBILoops-0.1/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.266150 SBILoops-0.1/SBI/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.281716 SBILoops-0.1/SBI/SBILoops.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)      220 2023-06-05 20:01:32.000000 SBILoops-0.1/SBI/SBILoops.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     3742 2023-06-05 20:01:32.000000 SBILoops-0.1/SBI/SBILoops.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-05 20:01:32.000000 SBILoops-0.1/SBI/SBILoops.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-05 20:01:32.000000 SBILoops-0.1/SBI/SBILoops.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)       60 2023-06-05 20:01:32.000000 SBILoops-0.1/SBI/SBILoops.egg-info/top_level.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.310179 SBILoops-0.1/SBI/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4497 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11690 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14924 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2923 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.1/SBI/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.327558 SBILoops-0.1/SBI/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.371168 SBILoops-0.1/SBI/databases/
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8403 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13608 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5564 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5346 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6698 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9105 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1786 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5721 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7083 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7048 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7140 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.377482 SBILoops-0.1/SBI/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4768 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8163 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.394237 SBILoops-0.1/SBI/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.396603 SBILoops-0.1/SBI/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.408698 SBILoops-0.1/SBI/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2246 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2217 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.415952 SBILoops-0.1/SBI/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3321 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3603 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.427410 SBILoops-0.1/SBI/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9086 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12567 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23479 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8066 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/external/blast/blast_parser.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.431580 SBILoops-0.1/SBI/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.442234 SBILoops-0.1/SBI/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6322 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4862 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15039 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.452801 SBILoops-0.1/SBI/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43520 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.462059 SBILoops-0.1/SBI/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    20840 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.472863 SBILoops-0.1/SBI/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3749 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.488775 SBILoops-0.1/SBI/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19958 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13255 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2760 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6874 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4982 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.496314 SBILoops-0.1/SBI/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9007 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3405 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.507858 SBILoops-0.1/SBI/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3803 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3272 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.514651 SBILoops-0.1/SBI/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.527516 SBILoops-0.1/SBI/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11112 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.560170 SBILoops-0.1/SBI/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2279 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3821 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2005 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14751 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1196 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      938 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7642 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8524 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2418 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18690 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14365 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8538 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.591232 SBILoops-0.1/SBI/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19059 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19197 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:01:32.607724 SBILoops-0.1/SBI/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10768 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10715 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5354 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.1/SBI/structure/residue/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-05 20:01:32.611480 SBILoops-0.1/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      449 2023-06-05 20:01:12.000000 SBILoops-0.1/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.447921 SBILoops-0.2/
+-rw-r--r--   0 patrick    (501) staff       (20)      220 2023-06-05 20:35:16.448207 SBILoops-0.2/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 17:30:37.000000 SBILoops-0.2/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.321856 SBILoops-0.2/SBI/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.333814 SBILoops-0.2/SBI/SBILoops.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)      220 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     3742 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       60 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.342584 SBILoops-0.2/SBI/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4497 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11690 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14924 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2923 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2/SBI/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.349709 SBILoops-0.2/SBI/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.366255 SBILoops-0.2/SBI/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8403 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13608 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5564 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5346 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6698 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9105 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1786 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5721 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7083 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7048 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7140 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.368631 SBILoops-0.2/SBI/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4768 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8163 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.373000 SBILoops-0.2/SBI/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.373987 SBILoops-0.2/SBI/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.379007 SBILoops-0.2/SBI/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2246 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2217 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.381204 SBILoops-0.2/SBI/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3321 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3603 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.385593 SBILoops-0.2/SBI/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9086 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12567 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23479 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8066 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/blast_parser.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.387319 SBILoops-0.2/SBI/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.393825 SBILoops-0.2/SBI/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6322 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4862 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15039 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.397600 SBILoops-0.2/SBI/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43520 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.401806 SBILoops-0.2/SBI/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    20840 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.406555 SBILoops-0.2/SBI/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3749 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.412100 SBILoops-0.2/SBI/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19958 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13255 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2760 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6874 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4982 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.414934 SBILoops-0.2/SBI/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9007 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3405 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.420532 SBILoops-0.2/SBI/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3803 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3272 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.423590 SBILoops-0.2/SBI/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.428324 SBILoops-0.2/SBI/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11112 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.436707 SBILoops-0.2/SBI/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2279 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3821 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2005 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14751 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1196 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      938 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7642 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8524 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2418 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18690 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14365 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8538 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.443766 SBILoops-0.2/SBI/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19059 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19197 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.447172 SBILoops-0.2/SBI/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10768 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10715 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5354 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-05 20:35:16.449450 SBILoops-0.2/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      449 2023-06-05 20:34:54.000000 SBILoops-0.2/setup.py
```

### Comparing `SBILoops-0.1/README.md` & `SBILoops-0.2/README.md`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/SBILoops.egg-info/SOURCES.txt` & `SBILoops-0.2/SBI/SBILoops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/Executable.py` & `SBILoops-0.2/SBI/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/File.py` & `SBILoops-0.2/SBI/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/IndexedNum.py` & `SBILoops-0.2/SBI/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/Path.py` & `SBILoops-0.2/SBI/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/StorableObject.py` & `SBILoops-0.2/SBI/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/butler.py` & `SBILoops-0.2/SBI/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/beans/singleton.py` & `SBILoops-0.2/SBI/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/Alphabet.py` & `SBILoops-0.2/SBI/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/AminoAcids.py` & `SBILoops-0.2/SBI/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/AtomVariants.py` & `SBILoops-0.2/SBI/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/Element.py` & `SBILoops-0.2/SBI/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/Properties.py` & `SBILoops-0.2/SBI/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/SetDict.py` & `SBILoops-0.2/SBI/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/data/__init__.py` & `SBILoops-0.2/SBI/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/CATHlink.py` & `SBILoops-0.2/SBI/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/DrugBanklink.py` & `SBILoops-0.2/SBI/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/Enzymelink.py` & `SBILoops-0.2/SBI/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/GOlink.py` & `SBILoops-0.2/SBI/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/PDBTMlink.py` & `SBILoops-0.2/SBI/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/PDBeChemlink.py` & `SBILoops-0.2/SBI/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/PDBlink.py` & `SBILoops-0.2/SBI/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/SCOPlink.py` & `SBILoops-0.2/SBI/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/TaxIDlink.py` & `SBILoops-0.2/SBI/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/Uniprotlink.py` & `SBILoops-0.2/SBI/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/__Uniprotlink.py` & `SBILoops-0.2/SBI/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/__init__.py` & `SBILoops-0.2/SBI/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/dblink.py` & `SBILoops-0.2/SBI/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/uniprot/connect.py` & `SBILoops-0.2/SBI/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/databases/uniprot/uniprot.py` & `SBILoops-0.2/SBI/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/error/BlastError.py` & `SBILoops-0.2/SBI/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/error/FileError.py` & `SBILoops-0.2/SBI/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/error/SeqAliError.py` & `SBILoops-0.2/SBI/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/CDhit/CDhit.py` & `SBILoops-0.2/SBI/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/CDhit/CDhitExe.py` & `SBILoops-0.2/SBI/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/CDhit/CDhitHomolog.py` & `SBILoops-0.2/SBI/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/CDhit/CDhitList.py` & `SBILoops-0.2/SBI/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/DSSP/DSSP.py` & `SBILoops-0.2/SBI/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/DSSP/DSSPExe.py` & `SBILoops-0.2/SBI/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/blast/BlastExe.py` & `SBILoops-0.2/SBI/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/blast/BlastHit.py` & `SBILoops-0.2/SBI/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/blast/BlastResult.py` & `SBILoops-0.2/SBI/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/external/blast/blast_parser.py` & `SBILoops-0.2/SBI/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/math/stats.py` & `SBILoops-0.2/SBI/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/Fasta.py` & `SBILoops-0.2/SBI/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/IndexedSeqAli.py` & `SBILoops-0.2/SBI/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/SeqAli.py` & `SBILoops-0.2/SBI/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/Sequence.py` & `SBILoops-0.2/SBI/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/alignment/Needleman_Wunsch.py` & `SBILoops-0.2/SBI/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/alignment/SeqAli.py` & `SBILoops-0.2/SBI/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/sequence/alignment/SimilarityMatrix.py` & `SBILoops-0.2/SBI/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/PDB.py` & `SBILoops-0.2/SBI/structure/PDB.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/atom/Atom.py` & `SBILoops-0.2/SBI/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/atom/AtomOfAminoAcid.py` & `SBILoops-0.2/SBI/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/atom/AtomOfNucleotide.py` & `SBILoops-0.2/SBI/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/atom/AtomSeries.py` & `SBILoops-0.2/SBI/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/chain/Chain.py` & `SBILoops-0.2/SBI/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/chain/ChainFrame.py` & `SBILoops-0.2/SBI/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/chain/ChainOfNucleotide.py` & `SBILoops-0.2/SBI/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/chain/ChainOfProtein.py` & `SBILoops-0.2/SBI/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/chain/ProteinChainFrame.py` & `SBILoops-0.2/SBI/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/Complex.py` & `SBILoops-0.2/SBI/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/InnerContacts.py` & `SBILoops-0.2/SBI/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/contact/Contact.py` & `SBILoops-0.2/SBI/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/contact/ContactAA.py` & `SBILoops-0.2/SBI/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/contact/ContactAH.py` & `SBILoops-0.2/SBI/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/contact/ContactAN.py` & `SBILoops-0.2/SBI/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/inner/PHInnerContact.py` & `SBILoops-0.2/SBI/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/inner/PPInnerContact.py` & `SBILoops-0.2/SBI/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/interface/Interface.py` & `SBILoops-0.2/SBI/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/interface/PHInterface.py` & `SBILoops-0.2/SBI/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/interface/PNInterface.py` & `SBILoops-0.2/SBI/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/contacts/interface/PPInterface.py` & `SBILoops-0.2/SBI/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/BioMolecule.py` & `SBILoops-0.2/SBI/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/DBreference.py` & `SBILoops-0.2/SBI/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/Experiment.py` & `SBILoops-0.2/SBI/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/Header.py` & `SBILoops-0.2/SBI/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/HeteroAtom.py` & `SBILoops-0.2/SBI/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/MiniRes.py` & `SBILoops-0.2/SBI/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/Molecule.py` & `SBILoops-0.2/SBI/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/SecondaryStructure.py` & `SBILoops-0.2/SBI/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/Site.py` & `SBILoops-0.2/SBI/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/header/__init__.py` & `SBILoops-0.2/SBI/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/parse_mmCIF.py` & `SBILoops-0.2/SBI/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/parse_pdb.py` & `SBILoops-0.2/SBI/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/protein/Arch.py` & `SBILoops-0.2/SBI/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/protein/SShelper.py` & `SBILoops-0.2/SBI/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/protein/SecondaryStructure.py` & `SBILoops-0.2/SBI/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/protein/Sequencer.py` & `SBILoops-0.2/SBI/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/residue/Residue.py` & `SBILoops-0.2/SBI/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/residue/ResidueOfAminoAcid.py` & `SBILoops-0.2/SBI/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.1/SBI/structure/residue/ResidueOfNucleotide.py` & `SBILoops-0.2/SBI/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

