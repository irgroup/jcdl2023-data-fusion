### Open points and issues 

- [x] Testbed for different fusion algorithms (based on ranx) | [Notebook](./fuse.ipynb)
- [x] Evaluations of TREC PM 2017/18 Abstract task (based on RRF by Cormack et al.) | [Notebook](./fuse.ipynb)
- [x] Measures: nDCG, AP, P@10, Bpref, MRR | [Experimental results](./experimental_results/)
- [x] p-values and differences between baseline and fusion runs | [Experimental results](./experimental_results/)
- [x] run format of TREC PM 2019 Abstract task (additional columns)
- [ ] IDs in run files of TREC PM CDS tasks do not match with our citations/altmetrics data
- [ ] missing citations for TREC PM 2020


The `trec-pm/` directory should contain the following sub-directories and files:

<details>
<summary>Directory tree</summary>

```
trec-pm
├── trec-pm-2017-abstracts
│   ├── input.aCSIROmedAll.gz
│   ├── input.aCSIROmedMCB.gz
│   ├── input.aCSIROmedMGB.gz
│   ├── input.aCSIROmedNEG.gz
│   ├── input.aCSIROmedPCB.gz
│   ├── input.Broad.gz
│   ├── input.cbnuSA1.gz
│   ├── input.cbnuSA2.gz
│   ├── input.cbnuSA3.gz
│   ├── input.DUTIR003.gz
│   ├── input.ECNU_M_1.gz
│   ├── input.ECNU_M_2.gz
│   ├── input.ECNU_M_3.gz
│   ├── input.ECNU_M_4.gz
│   ├── input.ECNU_M_5.gz
│   ├── input.eth_a_gws.gz
│   ├── input.eth_a_luc.gz
│   ├── input.eth_a_nn.gz
│   ├── input.eth_a_ws.gz
│   ├── input.eth_a_ws_q.gz
│   ├── input.Focused.gz
│   ├── input.GP14Medline.gz
│   ├── input.GP16Medline.gz
│   ├── input.Gwave.gz
│   ├── input.ielabRun1.gz
│   ├── input.ielabRun21.gz
│   ├── input.ielabRun22.gz
│   ├── input.ielabRun23.gz
│   ├── input.ielabRun3.gz
│   ├── input.KISTI01.gz
│   ├── input.KISTI02.gz
│   ├── input.KISTI03.gz
│   ├── input.KISTI04.gz
│   ├── input.KISTI05.gz
│   ├── input.kkseabs1.gz
│   ├── input.kkseabs3.gz
│   ├── input.kkseabs4.gz
│   ├── input.mayonlppm1.gz
│   ├── input.mayonlppm2.gz
│   ├── input.mayonlppm3.gz
│   ├── input.mayonlppm4.gz
│   ├── input.mayonlppm5.gz
│   ├── input.MedIER_sa1.gz
│   ├── input.MedIER_sa2.gz
│   ├── input.MedIER_sa3.gz
│   ├── input.MedIER_sa4.gz
│   ├── input.medline1.gz
│   ├── input.medline2.gz
│   ├── input.medline3.gz
│   ├── input.medline4.gz
│   ├── input.medline5.gz
│   ├── input.mRun1Bsl.gz
│   ├── input.mRun2BslOth.gz
│   ├── input.mRun3MRF.gz
│   ├── input.mRun4MRFrf.gz
│   ├── input.mRun5MRFBow.gz
│   ├── input.mugpubbase.gz
│   ├── input.mugpubboost.gz
│   ├── input.mugpubdiseas.gz
│   ├── input.mugpubgene.gz
│   ├── input.mugpubshould.gz
│   ├── input.NOVAsa1.gz
│   ├── input.NOVAsa2.gz
│   ├── input.NOVAsa3.gz
│   ├── input.Ontological.gz
│   ├── input.pms_run1.gz
│   ├── input.pms_run2_abs.gz
│   ├── input.pms_run3_abs.gz
│   ├── input.pms_run4_abs.gz
│   ├── input.pms_run5_abs.gz
│   ├── input.POZabsBB2GRn.gz
│   ├── input.POZabsBB2sn.gz
│   ├── input.POZabsLGDGRn.gz
│   ├── input.SDSFU_Ensem.gz
│   ├── input.SDSFU_Jnal.gz
│   ├── input.SDSFU_Lambda.gz
│   ├── input.SDSFU_PF_SA.gz
│   ├── input.SDSFU_PU_SA.gz
│   ├── input.Semantic.gz
│   ├── input.SIBTMlit1.gz
│   ├── input.SIBTMlit2.gz
│   ├── input.SIBTMlit3.gz
│   ├── input.SIBTMlit4.gz
│   ├── input.SIBTMlit5.gz
│   ├── input.Textual.gz
│   ├── input.UCASBASEa.gz
│   ├── input.UCASSEM1a.gz
│   ├── input.UCASSEM2a.gz
│   ├── input.UCASSEM3a.gz
│   ├── input.UCASSEMUMLSa.gz
│   ├── input.udelT1Base.gz
│   ├── input.udelT1Comb.gz
│   ├── input.udelT1GeMeSH.gz
│   ├── input.udelT1Gene.gz
│   ├── input.udelT1PRF.gz
│   ├── input.UD_GU_SA_1.gz
│   ├── input.UD_GU_SA_2.gz
│   ├── input.UD_GU_SA_3.gz
│   ├── input.UD_GU_SA_4.gz
│   ├── input.UD_GU_SA_5.gz
│   ├── input.UDInfoPMSA2.gz
│   ├── input.UDInfoPMSA3.gz
│   ├── input.UDInfoPMSA5.gz
│   ├── input.UDInfoPMSA6.gz
│   ├── input.UDInfoPMSA7.gz
│   ├── input.UKY_AGG.gz
│   ├── input.UKY_BASE.gz
│   ├── input.UKY_CJT.gz
│   ├── input.UKY_COM.gz
│   ├── input.UKY_MAN.gz
│   ├── input.UNTIIADW.gz
│   ├── input.UNTIIAGA.gz
│   ├── input.UNTIIAIS.gz
│   ├── input.UNTIIALQ.gz
│   ├── input.UNTIIASY.gz
│   ├── input.UTDHLTAF.gz
│   ├── input.UTDHLTFF.gz
│   ├── input.UTDHLTJQ.gz
│   ├── input.UTDHLTSF.gz
│   ├── input.UTDHLTSQ.gz
│   ├── input.UWMSOIS5.gz
│   ├── input.UWMSOIS6.gz
│   ├── input.UWMSOIS7.gz
│   ├── input.UWMSOIS8.gz
│   ├── input.UWMSOIS9.gz
│   └── qrels-final-abstracts.txt
├── trec-pm-2018-abstracts
│   ├── input.aCSIROmedAll.gz
│   ├── input.aCSIROmedMCB.gz
│   ├── input.aCSIROmedNEG.gz
│   ├── input.bool51.gz
│   ├── input.cbnuSA1.gz
│   ├── input.cbnuSA2.gz
│   ├── input.cbnuSA3.gz
│   ├── input.cubicmnzAbs.gz
│   ├── input.cubicsumWAbs.gz
│   ├── input.doc2vec_run2.gz
│   ├── input.doc2vec_run.gz
│   ├── input.ECNU_S_Run1.gz
│   ├── input.ECNU_S_Run2.gz
│   ├── input.ECNU_S_Run3.gz
│   ├── input.ECNU_S_Run4.gz
│   ├── input.ECNU_S_Run5.gz
│   ├── input.elastic_run.gz
│   ├── input.hpipubbase.gz
│   ├── input.hpipubboost.gz
│   ├── input.hpipubclass.gz
│   ├── input.hpipubcommon.gz
│   ├── input.hpipubnone.gz
│   ├── input.IKMLAB_1.gz
│   ├── input.IKMLAB_2.gz
│   ├── input.IKMLAB_3.gz
│   ├── input.IKMLAB_4.gz
│   ├── input.IKMLAB_5.gz
│   ├── input.imi_mug_abs1.gz
│   ├── input.imi_mug_abs2.gz
│   ├── input.imi_mug_abs3.gz
│   ├── input.imi_mug_abs4.gz
│   ├── input.imi_mug_abs5.gz
│   ├── input.KL18AbsFuse.gz
│   ├── input.KL18absHY.gz
│   ├── input.KL18absWV.gz
│   ├── input.KLPM18T2Bl.gz
│   ├── input.mayomedcomp.gz
│   ├── input.mayomedcreat.gz
│   ├── input.mayomedsimp.gz
│   ├── input.mayopubtator.gz
│   ├── input.MedIER_sa11.gz
│   ├── input.MedIER_sa12.gz
│   ├── input.MedIER_sa13.gz
│   ├── input.MedIER_sa14.gz
│   ├── input.MedIER_sa15.gz
│   ├── input.method_fu.gz
│   ├── input.minfolabBA.gz
│   ├── input.minfolabBC.gz
│   ├── input.minfolabBD.gz
│   ├── input.minfolabTH.gz
│   ├── input.mnzAbs.gz
│   ├── input.MSIIP_BASE.gz
│   ├── input.MSIIP_PBAH.gz
│   ├── input.MSIIP_PBH.gz
│   ├── input.MSIIP_PBL.gz
│   ├── input.MSIIP_PBPK.gz
│   ├── input.para_fusion.gz
│   ├── input.PM_IBI_run1.gz
│   ├── input.PM_IBI_run2.gz
│   ├── input.PM_IBI_run3.gz
│   ├── input.raw_medline.gz
│   ├── input.rbf.gz
│   ├── input.RSA_DSC_LA_1.gz
│   ├── input.RSA_DSC_LA_2.gz
│   ├── input.RSA_DSC_LA_3.gz
│   ├── input.RSA_DSC_LA_4.gz
│   ├── input.RSA_DSC_LA_5.gz
│   ├── input.SIBTMlit1.gz
│   ├── input.SIBTMlit2.gz
│   ├── input.SIBTMlit3.gz
│   ├── input.SIBTMlit4.gz
│   ├── input.SIBTMlit5.gz
│   ├── input.SINAI_Base.gz
│   ├── input.SINAI_FU.gz
│   ├── input.SINAI_FUO.gz
│   ├── input.sumAbs.gz
│   ├── input.sumEW.gz
│   ├── input.two_stage.gz
│   ├── input.UCASSA1.gz
│   ├── input.UCASSA2.gz
│   ├── input.UCASSA3.gz
│   ├── input.UCASSA4.gz
│   ├── input.UCASSA5.gz
│   ├── input.UDInfoPMSA1.gz
│   ├── input.UDInfoPMSA2.gz
│   ├── input.UDInfoPMSA3.gz
│   ├── input.UDInfoPMSA4.gz
│   ├── input.UDInfoPMSA5.gz
│   ├── input.UNTIIA_DGES.gz
│   ├── input.UNTIIA_DGEWS.gz
│   ├── input.UNTIIA_DGEWU.gz
│   ├── input.UNTIIA_DGS.gz
│   ├── input.UNTIIA_WTU.gz
│   ├── input.UTDHLTRI_NL.gz
│   ├── input.UTDHLTRI_RA.gz
│   ├── input.UTDHLTRI_RF.gz
│   ├── input.UTDHLTRI_SF.gz
│   ├── input.UTDHLTRI_SS.gz
│   ├── input.UVAEXPBOOST.gz
│   ├── input.UVAEXPBSTDIF.gz
│   ├── input.UVAEXPBSTEXT.gz
│   ├── input.UVAEXPBSTNEG.gz
│   ├── input.UVAEXPBSTSHD.gz
│   └── qrels-treceval-abstracts-2018-v2.txt
└── trec-pm-2019-abstracts
    ├── input.absrun1.gz
    ├── input.absrun2.gz
    ├── input.bm25_6801.gz
    ├── input.BM25.gz
    ├── input.BM25neop01.gz
    ├── input.BM25neopcomd.gz
    ├── input.BM25neopgngm.gz
    ├── input.cbnuSA1.gz
    ├── input.cbnuSA2.gz
    ├── input.cbnuSA3.gz
    ├── input.cbnuSA4.gz
    ├── input.ccnl_sa1.gz
    ├── input.ccnl_sa2.gz
    ├── input.ccnl_sa3.gz
    ├── input.ccnl_sa4.gz
    ├── input.ccnl_sa5.gz
    ├── input.default100k.gz
    ├── input.default1m.gz
    ├── input.dfr_9464.gz
    ├── input.DutirRun1.gz
    ├── input.DutirRun2.gz
    ├── input.DutirRun3.gz
    ├── input.DutirRun4.gz
    ├── input.DutirRun5.gz
    ├── input.et_8435.gz
    ├── input.imi_mug1.gz
    ├── input.imi_mug2.gz
    ├── input.imi_mug2_t.gz
    ├── input.imi_mug3.gz
    ├── input.imi_mug3_t.gz
    ├── input.jlpmcommon2.gz
    ├── input.jlpmletor.gz
    ├── input.jlpmltrin.gz
    ├── input.jlpmtrboost.gz
    ├── input.jlpmtrcommon.gz
    ├── input.MedIR1.gz
    ├── input.MedIR2.gz
    ├── input.MedIR3.gz
    ├── input.MedIR4.gz
    ├── input.MedIR5.gz
    ├── input.run3.gz
    ├── input.run4.gz
    ├── input.run5.gz
    ├── input.sa_base.gz
    ├── input.sa_base_rr.gz
    ├── input.SA_bc.gz
    ├── input.SA_DPH_letor.gz
    ├── input.sa_ft.gz
    ├── input.sa_ft_rr.gz
    ├── input.SA_LGD_letor.gz
    ├── input.SAsimpleLGD.gz
    ├── input.SIBTMlit1.gz
    ├── input.SIBTMlit2.gz
    ├── input.SIBTMlit3.gz
    ├── input.SIBTMlit4.gz
    ├── input.SIBTMlit5.gz
    ├── input.sils_run1.gz
    ├── input.sils_run2.gz
    ├── input.sils_run3.gz
    ├── input.sils_run4.gz
    ├── input.top4fusion.gz
    ├── input.xgb_5113.gz
    └── qrels-treceval-abstracts.2019.txt

3 directories, 293 files
```