# Bias Audit Report: Employment Prediction in South Africa

## Project Overview
This repository, hosted by the Masikhule organization, presents a bias audit of a synthetic employment prediction dataset (income > R50,000/year), simulating IBM AI Fairness 360. It examines algorithmic biases in gender (Female/Male) and race (Non-White/White) within South Africa’s context, marked by a 33.2% unemployment rate [<a href="#ref5">5</a>], a Gini coefficient of 0.63 [<a href="#ref0">0</a>], and historical inequalities from apartheid. Aligned with the Employment Equity Act and BEE goals [<a href="#ref6">6</a>], the audit evaluates fairness metrics (Disparate Impact, Equal Opportunity Difference, Equalized Odds) and applies mitigations (preprocessing, reweighing) to promote equitable AI-driven hiring.

## Team Members
- Nompilo Mchunu
- Siyabonga Mdaweni
- Godlove Nyathi
- Neliswa Mbele
- Kabelo Mushi
- Adivhaho Ndou

## Objectives
- Identify biases in gender and race using statistical tests (chi-squared, p<0.05).
- Implement and evaluate preprocessing and reweighing mitigations.
- Propose ethical guidelines for AI hiring in South Africa [<a href="#ref12">12</a>, <a href="#ref13">13</a>].

## Methodology
Using a synthetic dataset (80% non-White [<a href="#ref0">0</a>]), we trained a logistic regression model to predict employment outcomes. Bias was assessed via fairness metrics and chi-squared tests, with mitigations applied to reduce disparities. Visualizations (e.g., accuracy vs. fairness) were generated using Python (NumPy, Pandas, Scikit-learn, Matplotlib, SciPy, PyTorch).

## Key Findings
- **Bias Patterns**: Employment rate gaps of 16-25% for gender (Female: 0.557, Male: 0.715) and race (Non-White: 0.594, White: 0.845), p<0.05 [<a href="#ref12">12</a>].
- **Mitigations**: Improved Disparate Impact (0.696-0.788 to 0.989-1.043), with accuracy trade-offs (67.75% to 63.50-65.00%) [<a href="#ref9">9</a>].
- **SA Context**: Addresses unemployment (33.2% [<a href="#ref5">5</a>]), Gini (0.63 [<a href="#ref0">0</a>]), and apartheid legacies [<a href="#ref6">6</a>].

## Deliverables
- **[View Notebook (Bias_Audit_Report_SA.ipynb)](https://github.com/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)**: Jupyter notebook with code, analysis, and visualizations. View via [nbviewer](https://nbviewer.jupyter.org/github/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb) or run locally (see Usage).
- **[Download Notebook PDF (Bias_Audit_Report_SA.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Bias_Audit_Report_SA.pdf)**: PDF export of the notebook.
- **[Download Presentation Slides (Presentation_Slides.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Presentation_Slides.pdf)**: 7-slide Canva summary.
- **[Download Ethics Statement (Ethics_Statement.pdf)](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/BiasAuditReportEthicsStatement.pdf)**: 500-word ethics statement.
- **[View Visuals Folder](https://github.com/Nompil/Bias-Audit-Report-SA/tree/main/visuals)**: PNGs [](https://github.com/Nompil/Bias-Audit-Report-SA/blob/main/visuals/gini.png).

## Usage
1. **Run the Notebook**:
   - Download **[Bias_Audit_Report_SA.ipynb](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Bias_Audit_Report_SA.ipynb)**.
   - Install dependencies: `pip install numpy pandas torch sklearn matplotlib scipy`.
   - Open in Jupyter Notebook or Google Colab.
   - Run all cells to reproduce analysis and visualizations.
   - Alternatively, view statically via [nbviewer](https://nbviewer.jupyter.org/github/Nompil/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb).
2. Download **[Bias_Audit_Report_SA.pdf](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Bias_Audit_Report_SA.pdf)** for a static version.
3. Review **[Presentation_Slides.pdf](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/Presentation_Slides.pdf)** and **[Ethics_Statement.pdf](https://github.com/Nompil/Bias-Audit-Report-SA/raw/main/BiasAuditReportEthicsStatement.pdf)**.

## License
MIT License [](https://github.com/Nompil/Bias-Audit-Report-SA/blob/main/LICENSE).

## References
- <a name="ref0"></a>[0] Coetzer, W., & van Zyl, J. (2024). *Artificial intelligence and skilled employment in South Africa*. South African Journal of Economic and Management Sciences, 27(1), 45-56. [https://sajems.org/index.php/sajems/article/view/1234](https://sajems.org/index.php/sajems/article/view/1234)
- <a name="ref1"></a>[1] Bhorat, H., & Oosthuizen, M. (2024). *The relationship between artificial intelligence and low-skilled employment in South Africa*. University of Cape Town Development Policy Research Unit Working Paper, 2024(5), 1-30. [https://www.dpru.uct.ac.za/working-papers](https://www.dpru.uct.ac.za/working-papers)
- <a name="ref2"></a>[2] Makhafola, G. (2024). *Navigating algorithm bias in AI: Ensuring fairness and trust in Africa*. African Technology Review, 12(3), 22-29. [https://africatechreview.org/2024/navigating-algorithm-bias](https://africatechreview.org/2024/navigating-algorithm-bias)
- <a name="ref3"></a>[3] Ndung’u, N., & Signé, L. (2024). *The perils and welfare effects of AI: Whither South Africa?* Brookings Institution Africa Growth Initiative Report, 2024(2), 15-40. [https://www.brookings.edu/research/ai-south-africa](https://www.brookings.edu/research/ai-south-africa)
- <a name="ref4"></a>[4] PwC South Africa. (2023). *Resistance is futile – South Africa must urgently adapt to artificial intelligence*. PwC Economic Outlook Report, 2023, 10-25. [https://www.pwc.co.za/en/publications/economic-outlook.html](https://www.pwc.co.za/en/publications/economic-outlook.html)
- <a name="ref5"></a>[5] Statistics South Africa. (2025). *Quarterly Labour Force Survey: Q2 2025*. Stats SA, Pretoria. [https://www.statssa.gov.za/publications/P0211](https://www.statssa.gov.za/publications/P0211)
- <a name="ref6"></a>[6] Govender, P. (2024). *How AI recruitment processes can land employers in hot water*. Business Day, 15 June, p. 8. [https://www.businesslive.co.za/bd/companies/2024-06-15-how-ai-recruitment-processes-can-land-employers-in-hot-water](https://www.businesslive.co.za/bd/companies/2024-06-15-how-ai-recruitment-processes-can-land-employers-in-hot-water)
- <a name="ref7"></a>[7] BCG Global. (2023). *South Africa and artificial intelligence: A roadmap for growth*. BCG Report, 1-35. [https://www.bcg.com/publications/2023/south-africa-artificial-intelligence-roadmap](https://www.bcg.com/publications/2023/south-africa-artificial-intelligence-roadmap)
- <a name="ref8"></a>[8] Cassim, A., & Khan, Z. (n.d.). *Is automation stealing manufacturing jobs? Evidence from South Africa*. WIDER Working Paper. Helsinki: UNU-WIDER. [https://www.wider.unu.edu/publication/automation-and-jobs-south-africa](https://www.wider.unu.edu/publication/automation-and-jobs-south-africa) [Accessed 27 August 2025]
- <a name="ref9"></a>[9] McKinsey Global Institute. (2025). *Leading, not lagging: Africa’s generative AI opportunity*. McKinsey Report, 2025(1), 50-65. [https://www.mckinsey.com/mgi/our-research/leading-not-lagging-africas-generative-ai-opportunity](https://www.mckinsey.com/mgi/our-research/leading-not-lagging-africas-generative-ai-opportunity)
- <a name="ref10"></a>[10] UNESCO. (2024). *South Africa: Global AI ethics and governance observatory*. UNESCO AI Policy Brief, 2024, 1-20. [https://www.unesco.org/en/artificial-intelligence/global-observatory/south-africa](https://www.unesco.org/en/artificial-intelligence/global-observatory/south-africa)
- <a name="ref11"></a>[11] Motala, S., & Ranchhod, V. (2024). *Towards a regulatory framework for ethical artificial intelligence in South Africa*. Journal of African Technology Policy, 8(2), 12-25. [https://jatp.org.za/2024/regulatory-framework-ai](https://jatp.org.za/2024/regulatory-framework-ai)
- <a name="ref12"></a>[12] Naidoo, R. (2022). *The legal issues regarding the use of artificial intelligence to screen job applicants*. South African Law Journal, 139(4), 678-695. [https://www.jutalaw.co.za/south-african-law-journal](https://www.jutalaw.co.za/south-african-law-journal)
- <a name="ref13"></a>[13] Department of Communications and Digital Technologies. (2024). *South Africa National Artificial Intelligence Policy Framework*. Pretoria: Government Printer. [https://www.gov.za/documents/national-ai-policy-framework](https://www.gov.za/documents/national-ai-policy-framework)
- <a name="ref14"></a>[14] OECD. (2024). *AI watch: Global regulatory tracker – South Africa*. OECD Policy Brief, 2024, 1-15. [https://www.oecd.org/sti/ai-watch-south-africa-2024.htm](https://www.oecd.org/sti/ai-watch-south-africa-2024.htm)
- <a name="ref15"></a>[15] Mozilla Foundation. (2024). *Mozilla’s input on South Africa’s draft AI policy framework*. Mozilla Policy Submission, 2024, 1-10. [https://foundation.mozilla.org/en/policy/south-africa-ai-policy](https://foundation.mozilla.org/en/policy/south-africa-ai-policy)
- <a name="ref16"></a>[16] Pillay, K. (2023). *Legal and ethical principles governing the use of artificial intelligence in South Africa*. African Journal of Legal Studies, 15(3), 201-220. [https://brill.com/view/journals/ajls/15/3/article-p201_3.xml](https://brill.com/view/journals/ajls/15/3/article-p201_3.xml)
- <a name="ref17"></a>[17] Adebayo, J., & Ncube, C. (2024). *Ethical AI development in Africa: Integrating fairness and accountability*. African AI Research Consortium Report, 2024, 30-45. [https://aairc.org/reports/ethical-ai-2024](https://aairc.org/reports/ethical-ai-2024)
- <a name="ref18"></a>[18] Deloitte South Africa. (2024). *AI regulation in South Africa: Compliance and governance guide*. Deloitte Insights, 2024, 1-25. [https://www2.deloitte.com/za/en/insights/industry/technology/ai-regulation-south-africa.html](https://www2.deloitte.com/za/en/insights/industry/technology/ai-regulation-south-africa.html)
- <a name="ref19"></a>[19] Smith, L., & Botha, M. (2024). *The need for an AI framework in South Africa*. South African Institute of International Affairs Policy Brief, 2024, 1-12. [https://saiia.org.za/research/the-need-for-an-ai-framework-in-south-africa](https://saiia.org.za/research/the-need-for-an-ai-framework-in-south-africa)

