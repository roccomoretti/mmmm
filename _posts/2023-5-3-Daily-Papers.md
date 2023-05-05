---
title: "TCRModel2"
date: 2023-05-03
---

Papers for 3 May 2023
=====================


TCRmodel2
-----------
* Yin R, Ribeiro-Filho HV, Lin V, Gowthaman R, Cheung M, Pierce BG. TCRmodel2: high-resolution modeling of T cell receptor recognition using deep learning. Nucleic Acids Res. 2023 May 4:gkad356. doi: [10.1093/nar/gkad356](https://doi.org/10.1093/nar/gkad356). Epub ahead of print. PMID: 37140040.

Building off of TCRmodel (<https://doi.org/10.1093/nar/gky432>) TCRmodel2 uses AlphaFold2 (with a reduced/tuned sequence & template database) to build the structures of the T-Cell Receptor-peptide-major histocompatibility complex (TCR–pMHC) complexes. 
Regular (non-multimer) AF2 was used, using a chainbreak + residue index shift. Complexes were scored based on predicted TM-score and predicted inter-chain TM score.
Aside from reducing the sequence and template database to TCR & MHC complexes, and performing the template search with only the input sequence (rather than the MSA), no significant pre/post processing changes were noted.
Performance on TCR-pMHC complexes was improved over TRCModel (v1) or plain AlphaFold (Figure 1). Performance on unbound TCRs was better than TCRModel (v1), but about the same as plain AlphaFold.

A server is availible at <https://tcrmodel.ibbr.umd.edu>.
