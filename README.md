# Abstract-Generator
LLM model which summarizes academic article into an abstract paragraph.

The summarization is done by finetunning a pre-trained model - BERT, on a dataset of academic articles.

The body of the aricles has been used as data and the abstract of the article was used as label for the taining process.

The data was gathered from the open-source database of NCBI - The National Center for Biotechnology Information.

Result demonsration:

The Text Generated by my summarization model for the article: "Comparison of Cox regression and generalized Cox regression models to machine learning in predicting survival of children with diffuse large B-cell lymphoma"

Generated:

"Diagnosis of diffuse large B-cell lymphoma (DLBCL) in children is challenging due to the immature immune system. This study used regression analysis to identify prognostic factors for overall survival (OS) in DLBCL in children diagnosed between 2000 and 2019. These factors included age, sex, surgery, primary surgical procedure, radiotherapy, chemotherapy, systemic therapy, Ann Arbor stage, year of diagnosis, histological grade, surgical method, tumor location, primary tumor location and primary tumor type. The primary outcome measure considered was overall survival, defined as the interval from the time of the histopathological diagnosis until death. We used Cox regression to construct the selected prognostic feature of children diagnosed with diffuse large DlBCL. Generalized Cox regression and XGBoost were used to screen out prognostic variables. The results indicated that within the threshold of 0.87, the net benefit rates of the novel models exceeded those of traditional international prognostic index prognostic score. This suggests that novel models have better clinical value and utility in evaluating overall survival in children. However, more research is needed to confirm the predictive value of these novel models.."

Original:

" The incidence of diffuse large B-cell lymphoma (DLBCL) in children is increasing globally. Due to the immature immune system in children, the prognosis of DLBCL is quite different from that of adults. We aim to use the multicenter large retrospective analysis for prognosis study of the disease. For our retrospective analysis, we retrieved data from the Surveillance, Epidemiology and End Results (SEER) database that included 836 DLBCL patients under 18 years old who were treated at 22 central institutions between 2000 and 2019. The patients were randomly divided into a modeling group and a validation group based on the ratio of 7:3. Cox stepwise regression, generalized Cox regression and eXtreme Gradient Boosting (XGBoost) were used to screen all variables. The selected prognostic variables were used to construct a nomogram through Cox stepwise regression. The importance of variables was ranked using XGBoost. The predictive performance of the model was assessed by using C-index, area under the curve (AUC) of receiver operating characteristic (ROC) curve, sensitivity and specificity. The consistency of the model was evaluated by using a calibration curve. The clinical practicality of the model was verified through decision curve analysis (DCA). ROC curve demonstrated that all models except the non-proportional hazards and non-log linearity (NPHNLL) model, achieved AUC values above 0.7, indicating high accuracy. The calibration curve and DCA further confirmed strong predictive performance and clinical practicability. In this study, we successfully constructed a machine learning model by combining XGBoost with Cox and generalized Cox regression models. This integrated approach accurately predicts the prognosis of children with DLBCL from multiple dimensions. These findings provide a scientific basis for accurate clinical prognosis prediction. "
