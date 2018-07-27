# COPPER 

**Contents**: This repository contains the *COPPER (COsmological Parametrized PERturbations)* package - a Mathematica notebook building on xIST (https://github.com/noller/xIST) to investigate cosmological scalar-tensor theories. Note that an older version of this notebook is also distributed with the xIST package itself. The latest version and release date is:

*COPPER*, version 0.8.4, {2018, 7, 6} 

CopyRight (C) 2016-18, *Johannes Noller*, under the General Public License. 


**Installation notes**: xIST and COPPER require a working installation of Mathematica and xAct. For details, downloads and documentation for xAct please go to http://www.xact.es. For xIST (and especially for detailed installation instructions for xIST) go to https://github.com/noller/xIST. 


**Methodology and computation notes**: The COPPER notebook takes the general ansatz for a quadratic action of perturbations for a tensor and a scalar in an FRW-like background as discussed in the accompanying paper *A general theory of linear cosmological perturbations: scalar-tensor and vector-tensor theories (http://arxiv.org/abs/1604.01396)* and as is already contained in the xIST package. It then computes all Noether constraints from requiring this action to be diffeomorphism-invariant. Finally it solves all constraints and in that way obtains the true number of independent background functions/coefficients in the full quadratic perturbative action. We present the full actions derived in this way and expressions relating the free coefficients to the original ansatz.


**Comparison with accompanying paper "arXiv:1604.01396"**: The Lagrangians used in the \`\`Lagrangian setup" sections throughout COPPER are imported from the xIST package and should be compared with equations 4.5-4.9 and G.1-G.2 of the accompanying *arXiv:1604.01396*. Note that, while in the paper different letters (T's and L's) are used for background (time-dependent) coefficients in this action, in the COPPER file we stick with a uniform convention of labelling all coefficients in our starting action as L's. Otherwise our starting expressions are identical and the final answers expressed in terms of \`\`alpha'' coefficients are equivalent, see e.g. equation 4.15 as compared to the final action in the 3rd order \`\`Beyond Horndeski'' case computed in COPPER or equation 3.30 in the paper as compared to the final action in the GR case computed in COPPER (final actions in COPPER are expressed in Fourier-space, whereas in the paper we have kept explicit spatial derivatives in the final actions).


**Known issues and bugs**: All the individual sections in COPPER can be computed without any known issues/problems arising. However, when computing the \`\`Lagrangian setup'' sections of several of the sections in COPPER in succession (e.g. as part of evaluating the full notebook), a problem with the internal vbundles and index recognition appears. This is due to a bug when calling the xAct MakeRule function (giving rise to a "VBundleOfIndex::unknown" error that aborts the computation). If this occurs, the simplest solution is to re-start the kernel/only carry out the computations in one of the sections at a time and re-starting the kernel and re-loading xIST whenever one would like to move on. I'm working to resolve this issue fully so no such manual workaround is required. 
