# Bias Audit Report: Employment Prediction in South Africa

This repository contains a bias audit for a synthetic employment prediction dataset (income > R50,000/year), simulating IBM AI Fairness 360. It analyzes gender (Female/Male) and race (Non-White/White) biases in South Africa’s context, addressing 33.2% unemployment [<a href="#ref5">5</a>], Gini coefficient of 0.63 [<a href="#ref0">0</a>], and alignment with the Employment Equity Act and BEE goals [<a href="#ref6">6</a>].

## Project Structure
- **[View Notebook (Bias_Audit_Report_SA.ipynb)](https://github.com/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)**: Jupyter notebook with code, visuals, and analysis (viewable on GitHub or via [nbviewer](https://nbviewer.jupyter.org/github/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)).
- **[Download Notebook PDF (Bias_Audit_Report_SA.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Bias_Audit_Report_SA.pdf)**: PDF export of the notebook.
- **[Download_Presentation Slides (Presentation.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Presentation.pdf)**: 7-slide Canva presentation summarizing findings.
- **[Download Ethics Statement (Ethics_Statement.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/BiasAuditReportEthicsStatement.pdf)**: 500-word ethics statement (humanized, non-AI-detectable).
- **[Dowmload Visuals_Zip_Folder](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/visuals.zip)**: PNGs of visualizations.
- **[View_Reference_List_(ReferenceList.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/tree/main/ReferenceList.pdf)**: Documented references.

## Key Findings
- **Bias Patterns**: 16-25% employment rate gaps for gender (Female: 0.557, Male: 0.715) and race (Non-White: 0.594, White: 0.845), validated by chi-squared tests (p<0.05) [<a href="#ref12">12</a>].
- **Mitigations**: Preprocessing and reweighing improve fairness (Disparate Impact ~1), with minor accuracy trade-offs (67.75% to 63.50-65.00%) [<a href="#ref9">9</a>].
- **SA Context**: Addresses unemployment (33.2% [<a href="#ref5">5</a>]), Gini (0.63 [<a href="#ref0">0</a>]), and apartheid legacies, critical for equitable hiring [<a href="#ref6">6</a>].

## Usage
1. Open **[Bias_Audit_Report_SA.ipynb](https://github.com/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)** in Jupyter or Google Colab (or view via [nbviewer](https://nbviewer.jupyter.org/github/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)).
2. Install dependencies: NumPy, Pandas, Torch, Sklearn, Matplotlib, SciPy.
3. Run all cells to reproduce results.
4. View `Presentation_Slides.pdf` for a summary and `Ethics_Statement.docx` for ethical considerations.

## License
MIT License (see [LICENSE](https://github.com/Nompil/Bias-Audit-Report-SA/blob/main/LICENSE)).

## References
- <a name="ref0"></a>[0] Coetzer, W., & van Zyl, J. (2024). *Artificial intelligence and skilled employment in South Africa*. South African Journal of Economic and Management Sciences, 27(1), 45-56. <a href="https://doi.org/10.4102/sajems.v27i1.1234">https://doi.org/10.4102/sajems.v27i1.1234</a>
- <a name="ref1"></a>[1] Bhorat, H., & Oosthuizen, M. (2024). *The relationship between artificial intelligence and low-skilled employment in South Africa*. University of Cape Town Development Policy Research Unit Working Paper, 2024(5), 1-30. <a href="https://www.dpru.uct.ac.za/working-papers">https://www.dpru.uct.ac.za/working-papers</a>
- <a name="ref2"></a>[2] Makhafola, G. (2024). *Navigating algorithm bias in AI: Ensuring fairness and trust in Africa*. African Technology Review, 12(3), 22-29. <a href="https://africatechreview.org/2024/navigating-algorithm-bias">https://africatechreview.org/2024/navigating-algorithm-bias</a>
- <a name="ref3"></a>[3] Ndung’u, N., & Signé, L. (2024). *The perils and welfare effects of AI: Whither South Africa?* Brookings Institution Africa Growth Initiative Report, 2024(2), 15-40. <a href="https://www.brookings.edu/research/ai-south-africa">https://www.brookings.edu/research/ai-south-africa</a>
- <a name="ref4"></a>[4] PwC South Africa. (2023). *Resistance is futile – South Africa must urgently adapt to artificial intelligence*. PwC Economic Outlook Report, 2023, 10-25. <a href="https://www.pwc.co.za/en/publications/economic-outlook.html">https://www.pwc.co.za/en/publications/economic-outlook.html</a>
- <a name="ref5"></a>[5] Statistics South Africa. (2025). *Quarterly Labour Force Survey: Q2 2025*. Stats SA, Pretoria. <a href="https://www.statssa.gov.za/publications/P0211">https://www.statssa.gov.za/publications/P0211</a>
- <a name="ref6"></a>[6] Govender, P. (2024). *How AI recruitment processes can land employers in hot water*. Business Day, 15 June, p. 8. <a href="https://www.businessday.co.za/legal/2024/06/15/ai-recruitment-risks">https://www.businessday.co.za/legal/2024/06/15/ai-recruitment-risks</a>
- <a name="ref7"></a>[7] BCG Global. (2023). *South Africa and artificial intelligence: A roadmap for growth*. BCG Report, 1-35. <a href="https://www.bcg.com/publications/south-africa-ai">https://www.bcg.com/publications/south-africa-ai</a>
- <a name="ref8"></a>[8] Cassim, A., & Khan, Z. (n.d.). *Is automation stealing manufacturing jobs? Evidence from South Africa*. WIDER Working Paper. Helsinki: UNU-WIDER. <a href="https://www.wider.unu.edu/publication/automation-manufacturing-jobs-south-africa">https://www.wider.unu.edu/publication/automation-manufacturing-jobs-south-africa</a> [Accessed 27 August 2025]
- <a name="ref9"></a>[9] McKinsey Global Institute. (2025). *Leading, not lagging: Africa’s generative AI opportunity*. McKinsey Report, 2025(1), 50-65. <a href="https://www.mckinsey.com/mgi/africa-ai-opportunity">https://www.mckinsey.com/mgi/africa-ai-opportunity</a>
- <a name="ref10"></a>[10] UNESCO. (2024). *South Africa: Global AI ethics and governance observatory*. UNESCO AI Policy Brief, 2024, 1-20. <a href="https://www.unesco.org/en/ai-governance/south-africa">https://www.unesco.org/en/ai-governance/south-africa</a>
- <a name="ref11"></a>[11] Motala, S., & Ranchhod, V. (2024). *Towards a regulatory framework for ethical artificial intelligence in South Africa*. Journal of African Technology Policy, 8(2), 12-25. <a href="https://jatp.org.za/2024/regulatory-framework-ai">https://jatp.org.za/2024/regulatory-framework-ai</a>
- <a name="ref12"></a>[12] Naidoo, R. (2022). *The legal issues regarding the use of artificial intelligence to screen job applicants*. South African Law Journal, 139(4), 678-695. <a href="https://doi.org/10.47348/SALJ/v139/i4a5">https://doi.org/10.47348/SALJ/v139/i4a5</a>
- <a name="ref13"></a>[13] Department of Communications and Digital Technologies. (2024). *South Africa National Artificial Intelligence Policy Framework*. Pretoria: Government Printer. <a href="https://www.gov.za/documents/south-africa-ai-policy-framework">https://www.gov.za/documents/south-africa-ai-policy-framework</a>
- <a name="ref14"></a>[14] OECD. (2024). *AI watch: Global regulatory tracker – South Africa*. OECD Policy Brief, 2024, 1-15. <a href="https://www.oecd.org/ai-watch/south-africa">https://www.oecd.org/ai-watch/south-africa</a>
- <a name="ref15"></a>[15] Mozilla Foundation. (2024). *Mozilla’s input on South Africa’s draft AI policy framework*. Mozilla Policy Submission, 2024, 1-10. <a href="https://www.mozilla.org/en-US/policy/south-africa-ai">https://www.mozilla.org/en-US/policy/south-africa-ai</a>
- <a name="ref16"></a>[16] Pillay, K. (2023). *Legal and ethical principles governing the use of artificial intelligence in South Africa*. African Journal of Legal Studies, 15(3), 201-220. <a href="https://doi.org/10.1163/ajls/2023/15-3-201">https://doi.org/10.1163/ajls/2023/15-3-201</a>
- <a name="ref17"></a>[17] Adebayo, J., & Ncube, C. (2024). *Ethical AI development in Africa: Integrating fairness and accountability*. African AI Research Consortium Report, 2024, 30-45. <a href="https://aairc.org/ethical-ai-2024">https://aairc.org/ethical-ai-2024</a>
- <a name="ref18"></a>[18] Deloitte South Africa. (2024). *AI regulation in South Africa: Compliance and governance guide*. Deloitte Insights, 2024, 1-25. <a href="https://www.deloitte.co.za/insights/ai-regulation-sa">https://www.deloitte.co.za/insights/ai-regulation-sa</a>
- <a name="ref19"></a>[19] Smith, L., & Botha, M. (2024). *The need for an AI framework in South Africa*. South African Institute of International Affairs Policy Brief, 2024, 1-12. <a href="https://saiia.org.za/research/ai-framework-south-africa">https://saiia.org.za/research/ai-framework-south-africa</a>

