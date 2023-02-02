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
trec-pm/
├── dir.txt
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
├── trec-pm-2017-cds
│   ├── input.1_ec_simple.gz
│   ├── input.2_ec_complex.gz
│   ├── input.Broadc.gz
│   ├── input.cbnuCT1.gz
│   ├── input.cbnuCT2.gz
│   ├── input.cbnuCT3.gz
│   ├── input.cCSIROmedAll.gz
│   ├── input.cCSIROmedHGB.gz
│   ├── input.cCSIROmedMCB.gz
│   ├── input.cCSIROmedMCM.gz
│   ├── input.cCSIROmedNEG.gz
│   ├── input.cRun1Bsl.gz
│   ├── input.cRun2BslOth.gz
│   ├── input.cRun3MRF.gz
│   ├── input.cRun4MRFrf.gz
│   ├── input.cRun5MRFBow.gz
│   ├── input.DA_IICTrun1.gz
│   ├── input.DA_IICTrun3.gz
│   ├── input.DA_IICTrun4.gz
│   ├── input.DA_IICTrun5.gz
│   ├── input.dumbmethod.gz
│   ├── input.DUTIR004.gz
│   ├── input.ECNU_C_1.gz
│   ├── input.ECNU_C_2.gz
│   ├── input.ECNU_C_3.gz
│   ├── input.ECNU_C_4.gz
│   ├── input.ECNU_C_5.gz
│   ├── input.eth_t_gwsq.gz
│   ├── input.eth_t_luc.gz
│   ├── input.eth_t_nn.gz
│   ├── input.eth_t_wsb_q.gz
│   ├── input.eth_t_ws.gz
│   ├── input.Focusedc.gz
│   ├── input.GP14Trail.gz
│   ├── input.GP16Trail.gz
│   ├── input.Gwave_ct.gz
│   ├── input.KISTI01CT.gz
│   ├── input.KISTI02CT.gz
│   ├── input.KISTI03CT.gz
│   ├── input.KISTI04CT.gz
│   ├── input.KISTI05CT.gz
│   ├── input.kksetri1.gz
│   ├── input.kksetri2.gz
│   ├── input.kksetri4.gz
│   ├── input.LDGprfStrict.gz
│   ├── input.LGDnoprfGOpt.gz
│   ├── input.LGDprfGOpt.gz
│   ├── input.LGDraw.gz
│   ├── input.LGDStrict.gz
│   ├── input.mayonlpct1.gz
│   ├── input.mayonlpct2.gz
│   ├── input.mayonlpct3.gz
│   ├── input.mayonlpct4.gz
│   ├── input.mayonlpct5.gz
│   ├── input.MedIER_ct1.gz
│   ├── input.MedIER_ct2.gz
│   ├── input.MedIER_ct3.gz
│   ├── input.MedIER_ct4.gz
│   ├── input.mugctbase.gz
│   ├── input.mugctboost.gz
│   ├── input.mugctdisease.gz
│   ├── input.mugctgene.gz
│   ├── input.mugctmust.gz
│   ├── input.NOVAtr1.gz
│   ├── input.NOVAtr2.gz
│   ├── input.NOVAtr3.gz
│   ├── input.NOVAtr4.gz
│   ├── input.NOVAtr5.gz
│   ├── input.Ontologicalc.gz
│   ├── input.pms_run1_tri.gz
│   ├── input.pms_run2_tri.gz
│   ├── input.pms_run3_tri.gz
│   ├── input.pms_run4_tri.gz
│   ├── input.pms_run5_tri.gz
│   ├── input.SDSFU_BASE.gz
│   ├── input.SDSFU_PF.gz
│   ├── input.SDSFU_PFUMLS.gz
│   ├── input.SDSFU_UMLS.gz
│   ├── input.Semanticc.gz
│   ├── input.SIBTct1.gz
│   ├── input.SIBTct2.gz
│   ├── input.SIBTct3.gz
│   ├── input.SIBTct4.gz
│   ├── input.SIBTct5.gz
│   ├── input.teckro1.gz
│   ├── input.teckro2.gz
│   ├── input.teckro3.gz
│   ├── input.teckro4.gz
│   ├── input.teckro5.gz
│   ├── input.Textualc.gz
│   ├── input.trial1.gz
│   ├── input.trial2.gz
│   ├── input.trial3.gz
│   ├── input.trial4.gz
│   ├── input.UCASBASE.gz
│   ├── input.UCASSEM1.gz
│   ├── input.UCASSEM2.gz
│   ├── input.UCASSEM3.gz
│   ├── input.UCASSEMUMLS.gz
│   ├── input.udelT2Base.gz
│   ├── input.udelT2Comb.gz
│   ├── input.udelT2GeMeSH.gz
│   ├── input.udelT2Gene.gz
│   ├── input.udelT2PRF.gz
│   ├── input.UD_GU_CT_1.gz
│   ├── input.UD_GU_CT_2.gz
│   ├── input.UD_GU_CT_3.gz
│   ├── input.UD_GU_CT_4.gz
│   ├── input.UD_GU_CT_5.gz
│   ├── input.UDInfoPMCT10.gz
│   ├── input.UDInfoPMCT3.gz
│   ├── input.UDInfoPMCT4.gz
│   ├── input.UDInfoPMCT6.gz
│   ├── input.UDInfoPMCT8.gz
│   ├── input.UKY_T2.gz
│   ├── input.UKY_T3.gz
│   ├── input.UKY_T4.gz
│   ├── input.UKY_TRL.gz
│   ├── input.UNTIIACTDW.gz
│   ├── input.UNTIIACTGA.gz
│   ├── input.UNTIIACTIS.gz
│   ├── input.UNTIIACTLQ.gz
│   ├── input.UNTIIACTSY.gz
│   ├── input.UTDHLTAFT.gz
│   ├── input.UTDHLTFFT.gz
│   ├── input.UTDHLTJQT.gz
│   ├── input.UTDHLTSFT.gz
│   ├── input.UTDHLTSQT.gz
│   ├── input.UWMSOIS0.gz
│   ├── input.UWMSOIS1.gz
│   ├── input.UWMSOIS2.gz
│   ├── input.UWMSOIS3.gz
│   ├── input.UWMSOIS4.gz
│   └── qrels-final-trials.txt
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
├── trec-pm-2018-cds
│   ├── input.BB2_sq_nprf.gz
│   ├── input.BB2sqw2vprf.gz
│   ├── input.BB2_vq_noprf.gz
│   ├── input.BB2vqw2vprf.gz
│   ├── input.cbnuCT1.gz
│   ├── input.cbnuCT2.gz
│   ├── input.cbnuCT3.gz
│   ├── input.cCSIROmedAll.gz
│   ├── input.cCSIROmedHGB.gz
│   ├── input.cCSIROmedNEG.gz
│   ├── input.cubicmnz.gz
│   ├── input.cubicsumEW.gz
│   ├── input.cubicsumW.gz
│   ├── input.ECNU_C_Run1.gz
│   ├── input.ECNU_C_Run2.gz
│   ├── input.ECNU_C_Run3.gz
│   ├── input.ECNU_C_Run4.gz
│   ├── input.ECNU_C_Run5.gz
│   ├── input.hpictall.gz
│   ├── input.hpictbase.gz
│   ├── input.hpictboost.gz
│   ├── input.hpictcommon.gz
│   ├── input.hpictphrase.gz
│   ├── input.IKM_trail_1.gz
│   ├── input.IKM_trail_2.gz
│   ├── input.IKM_trail_3.gz
│   ├── input.IKM_trail_4.gz
│   ├── input.IKM_trail_5.gz
│   ├── input.imi_mug_ct1.gz
│   ├── input.imi_mug_ct2.gz
│   ├── input.imi_mug_ct3.gz
│   ├── input.imi_mug_ct4.gz
│   ├── input.imi_mug_ct5.gz
│   ├── input.IMS_NO_PRF.gz
│   ├── input.IMS_PRF.gz
│   ├── input.IMS_TERM.gz
│   ├── input.irit_prf_cli.gz
│   ├── input.KL18TrialBF.gz
│   ├── input.KL18TrialWV.gz
│   ├── input.KL18TriFuse.gz
│   ├── input.KL18TriHY.gz
│   ├── input.KLPM18T1Bl.gz
│   ├── input.mayoctcomp.gz
│   ├── input.mayoctscreat.gz
│   ├── input.mayoctsimp.gz
│   ├── input.mnz.gz
│   ├── input.MSIIP_TRIAL1.gz
│   ├── input.MSIIP_TRIAL2.gz
│   ├── input.MSIIP_TRIAL3.gz
│   ├── input.MSIIP_TRIAL4.gz
│   ├── input.MSIIP_TRIAL5.gz
│   ├── input.m_trial1.gz
│   ├── input.NS_PM_1.gz
│   ├── input.NS_PM_2.gz
│   ├── input.NS_PM_3.gz
│   ├── input.NS_PM_4.gz
│   ├── input.NS_PM_5.gz
│   ├── input.para_trial.gz
│   ├── input.raw_trials.gz
│   ├── input.rfb_trial1.gz
│   ├── input.RSA_DSC_CT_1.gz
│   ├── input.RSA_DSC_CT_2.gz
│   ├── input.RSA_DSC_CT_3.gz
│   ├── input.RSA_DSC_CT_4.gz
│   ├── input.RSA_DSC_CT_5.gz
│   ├── input.SIBTMct1.gz
│   ├── input.SIBTMct2.gz
│   ├── input.SIBTMct3.gz
│   ├── input.SIBTMct4.gz
│   ├── input.sq.gz
│   ├── input.sum.gz
│   ├── input.tinfolabBF.gz
│   ├── input.tinfolabBK.gz
│   ├── input.tinfolabF.gz
│   ├── input.two_trial1.gz
│   ├── input.UCASCT1.gz
│   ├── input.UCASCT2.gz
│   ├── input.UCASCT3.gz
│   ├── input.UCASCT4.gz
│   ├── input.UCASCT5.gz
│   ├── input.UDInfoPMCT1.gz
│   ├── input.UDInfoPMCT2.gz
│   ├── input.UDInfoPMCT3.gz
│   ├── input.UDInfoPMCT4.gz
│   ├── input.UDInfoPMCT5.gz
│   ├── input.UTDHLTRI_NLT.gz
│   ├── input.UTDHLTRI_RAT.gz
│   ├── input.UTDHLTRI_RFT.gz
│   ├── input.UTDHLTRI_SFT.gz
│   ├── input.UTDHLTRI_SST.gz
│   └── qrels-treceval-clinical_trials-2018-v2.txt
├── trec-pm-2019-abstracts
│   ├── input.absrun1.gz
│   ├── input.absrun2.gz
│   ├── input.bm25_6801.gz
│   ├── input.BM25.gz
│   ├── input.BM25neop01.gz
│   ├── input.BM25neopcomd.gz
│   ├── input.BM25neopgngm.gz
│   ├── input.cbnuSA1.gz
│   ├── input.cbnuSA2.gz
│   ├── input.cbnuSA3.gz
│   ├── input.cbnuSA4.gz
│   ├── input.ccnl_sa1.gz
│   ├── input.ccnl_sa2.gz
│   ├── input.ccnl_sa3.gz
│   ├── input.ccnl_sa4.gz
│   ├── input.ccnl_sa5.gz
│   ├── input.default100k.gz
│   ├── input.default1m.gz
│   ├── input.dfr_9464.gz
│   ├── input.DutirRun1.gz
│   ├── input.DutirRun2.gz
│   ├── input.DutirRun3.gz
│   ├── input.DutirRun4.gz
│   ├── input.DutirRun5.gz
│   ├── input.et_8435.gz
│   ├── input.imi_mug1.gz
│   ├── input.imi_mug2.gz
│   ├── input.imi_mug2_t.gz
│   ├── input.imi_mug3.gz
│   ├── input.imi_mug3_t.gz
│   ├── input.jlpmcommon2.gz
│   ├── input.jlpmletor.gz
│   ├── input.jlpmltrin.gz
│   ├── input.jlpmtrboost.gz
│   ├── input.jlpmtrcommon.gz
│   ├── input.MedIR1.gz
│   ├── input.MedIR2.gz
│   ├── input.MedIR3.gz
│   ├── input.MedIR4.gz
│   ├── input.MedIR5.gz
│   ├── input.run3.gz
│   ├── input.run4.gz
│   ├── input.run5.gz
│   ├── input.sa_base.gz
│   ├── input.sa_base_rr.gz
│   ├── input.SA_bc.gz
│   ├── input.SA_DPH_letor.gz
│   ├── input.sa_ft.gz
│   ├── input.sa_ft_rr.gz
│   ├── input.SA_LGD_letor.gz
│   ├── input.SAsimpleLGD.gz
│   ├── input.SIBTMlit1.gz
│   ├── input.SIBTMlit2.gz
│   ├── input.SIBTMlit3.gz
│   ├── input.SIBTMlit4.gz
│   ├── input.SIBTMlit5.gz
│   ├── input.sils_run1.gz
│   ├── input.sils_run2.gz
│   ├── input.sils_run3.gz
│   ├── input.sils_run4.gz
│   ├── input.top4fusion.gz
│   ├── input.xgb_5113.gz
│   └── qrels-treceval-abstracts.2019.txt
└── trec-pm-2019-cds
    ├── input.bc.gz
    ├── input.bm25_ct_25.gz
    ├── input.bm25_ct_f_61.gz
    ├── input.BM25ct.gz
    ├── input.BM25neop01r.gz
    ├── input.BM25solid01o.gz
    ├── input.BM25solid01r.gz
    ├── input.cbnuCT1.gz
    ├── input.cbnuCT2.gz
    ├── input.cbnuCT3.gz
    ├── input.cbnuCT4.gz
    ├── input.ccnl_trials1.gz
    ├── input.ccnl_trials2.gz
    ├── input.cl_base_rr.gz
    ├── input.cl_ft_agg.gz
    ├── input.cl_ft_rr.gz
    ├── input.clinic_base.gz
    ├── input.clinic_ft.gz
    ├── input.DFRInL2_f.gz
    ├── input.Dutir_Cli1.gz
    ├── input.Dutir_Cli2.gz
    ├── input.eged.gz
    ├── input.egnd.gz
    ├── input.jlctgenes.gz
    ├── input.jlctletor.gz
    ├── input.jlctltrin.gz
    ├── input.jlctphrase.gz
    ├── input.jlctprec.gz
    ├── input.ngnd.gz
    ├── input.rf1_f_100.gz
    ├── input.rf2_f_50.gz
    ├── input.rrf_1.gz
    ├── input.rrf_2.gz
    ├── input.SIBTMct1.gz
    ├── input.SIBTMct2.gz
    ├── input.SIBTMct3.gz
    ├── input.SIBTMct4.gz
    ├── input.SIBTMct5.gz
    ├── input.simple.gz
    ├── input.simple_letor.gz
    ├── input.tk1allbinary.gz
    ├── input.tk1allfuzzy.gz
    ├── input.tk3allfuzzy.gz
    ├── input.tk3nodemogr.gz
    ├── input.tk3onlygnds.gz
    ├── input.top3fusion.gz
    ├── input.trial_run3.gz
    ├── input.trial_run4.gz
    ├── input.trial_run5.gz
    ├── input.trialsrun1.gz
    ├── input.trialsrun2.gz
    ├── input.w2v_letor.gz
    ├── input.w2v_noletor.gz
    └── qrels-treceval-trials.38.txt

6 directories, 573 files
```