# TyphoidRx
AI-driven model that predicts effective typhoid treatment, expected healing time, resistance risk, and diagnosis likelihood using clinical, engineered, and metabolomics features.




















Methodology: End-to-end study workflow. Clinical and laboratory data were pre-processed and transformed into engineered features, used to train multi-task XGBoost models, and a counterfactual drug-simulation module estimated patient-specific alternative antibiotic options. ![image](https://github.com/SsemuyigaMHC/TyphoidRx/blob/main/Results/Figures/Figure%201.png).

Results

Model Evaluation: ROC and Residual Plots for Classification and Regression Models. (A) and (B) show ROC curves for the outcome and suspected typhoid classifiers, respectively, indicating strong discriminative ability. (C) display residual plot for resistance proxy regression model, showing tight error distributions without systematic deviation. ![image](https://github.com/SsemuyigaMHC/TyphoidRx/blob/main/Results/Figures/Figure%203.png)

Clustering Analysis: Low-dimensional projection of patient-level SHAP value vectors across all three predictive models using UMAP (left) and t-SNE (right). Each point represents a patient colored by cluster membership derived from attribution patterns. Distinct cluster separation indicates the presence of latent patient subgroups characterized by similar combinations of explanatory feature contributions across the models. ![image](https://github.com/SsemuyigaMHC/TyphoidRx/blob/main/Results/Figures/Figure%207.png)


Match Analysis: Match-based evaluation of treatment recommendation performance. (a) Treatment success rate by match type between the recommended drug and the actual prescribed drug. (b) Distribution of treatment outcomes across match categories shown as a stacked bar chart. (c) Predicted resistance proxy score stratified by match type. (d) Original treatment duration by match type. Together, these panels assess how agreement between model-recommended and prescribed treatments relates to treatment success, predicted resistance, and treatment duration. ![image](https://github.com/SsemuyigaMHC/TyphoidRx/blob/main/Results/Figures/Figure%209.png)


Risk Stratification: Resistance risk stratification across patient quartiles (Q1-Q4) based on predicted resistance proxy scores. Patients were grouped from lowest risk (Q1) to highest risk (Q4). (A) Mean resistance proxy score within each quartile. (B) Distribution of predicted resistance proxy scores across all patients. ![image](https://github.com/SsemuyigaMHC/TyphoidRx/blob/main/Results/Figures/Figure%2012.png)

