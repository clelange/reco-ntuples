# reco-ntuples
Home of the Ntuplizer for the HGCAL reconstruction software studies

Ntuple content definitions can be found at [Definitions.md](Definitions.md).

This version is based on >= CMSSW_10_2_0_pre1, instructions below should provide you with the version for the TDR sample production. Please check if there are later `CMSSW_10_2_X` versions available to profit from bugfixes.

```
cmsrel CMSSW_10_2_0_pre1
cd CMSSW_10_2_0_pre1/src
cmsenv
git clone git@github.com:CMS-HGCAL/reco-ntuples.git RecoNtuples
cd RecoNtuples
git checkout -b topic_${USER}
cd ../
scram b -j4
```

The input file needs to be step3 (i.e. RECO). Example configs are provided in [HGCalAnalysis/test](HGCalAnalysis/test).
