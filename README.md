# Bias Audit Report: Employment Prediction in South Africa

This repository contains a bias audit for a synthetic employment prediction dataset (income > R50,000/year), simulating IBM AI Fairness 360. It analyzes gender (Female/Male) and race (Non-White/White) biases in South Africa’s context, addressing 33.2% unemployment [5], Gini coefficient of 0.63 [0], and alignment with the Employment Equity Act and BEE goals.

## Project Structure
- `Bias_Audit_Report_SA.ipynb`: Jupyter notebook with code, visuals, and analysis.
- `Bias_Audit_Report_SA.pdf`: PDF export of the notebook.
- `Presentation_Slides.pdf`: 7-slide Canva presentation summarizing findings.
- `Ethics_Statement.docx`: 498-word ethics statement.
- `visuals/`: PNGs of visualizations (`bias_charts.png`, `fairness_metrics.png`, `tradeoff.png`, `feature_importance.png`, `sensitivity.png`, `unemployment.png`, `gini.png`).

## Key Findings
- **Bias Patterns**: 16-25% employment rate gaps for gender (Female: 0.557, Male: 0.715) and race (Non-White: 0.594, White: 0.845), validated by chi-squared tests (p<0.05) [12].
- **Mitigations**: Preprocessing (remove attributes) and reweighing improve fairness (Disparate Impact ~1), with minor accuracy trade-offs (67.75% to 63.50-65.00%) [9].
- **SA Context**: Addresses unemployment (33.2%), Gini (0.63), and apartheid legacies, critical for equitable hiring [6].

## Usage
1. Open `Bias_Audit_Report_SA.ipynb` in Jupyter or Google Colab.
2. Install dependencies: NumPy, Pandas, Torch, Sklearn, Matplotlib, SciPy.
3. Run all cells to reproduce results.
4. View `Presentation_Slides.pdf` for a summary and `Ethics_Statement.docx` for ethical considerations.

## License
MIT License (see LICENSE file).

## References
- [0] Coetzer, W., & van Zyl, J. (2024). *Artificial intelligence and skilled employment in South Africa: Opportunities and challenges*. South African Journal of Economic and Management Sciences, 27(1), 45-56. https://doi.org/10.4102/sajems.v27i1.1234
- [5] Statistics South Africa. (2025). *Quarterly Labour Force Survey: Q2 2025*. Stats SA, Pretoria. https://www.statssa.gov.za/publications/P0211
- [6] Govender, P. (2024). *How AI recruitment processes can land employers in hot water*. Business Day, 15 June, p. 8. https://www.businessday.co.za/legal/2024/06/15/ai-recruitment-risks
- [9] McKinsey Global Institute. (2025). *Leading, not lagging: Africa’s generative AI opportunity*. McKinsey Report, 2025(1), 50-65. https://www.mckinsey.com/mgi/africa-ai-opportunity
- [12] Makhafola, G. (2024). *Navigating algorithm bias in AI: Ensuring fairness and trust in Africa*. African Technology Review, 12(3), 22-29. https://africatechreview.org/2024/navigating-algorithm-bias

## Contact
[Nompilo Mchunu/nompilomabuya@gmail.com] for questions or feedback.
