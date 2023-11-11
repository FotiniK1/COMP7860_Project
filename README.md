# COMP7860_Project

In this repository, we have submitted the Google Colab notebooks that were used for the replication of the original data, as well as the notebooks with the new dataset. This is related to the paper chosen for the COMP7860 project: "eleanor: An Open-source Tool for Extracting Light Curves from the TESS Full-frame Images". The project report has been submitted separately through the Macquarie University iLearn platform. The original paper and GitHub repository can be found in the references below.

## Important Notes
1. The order in which the notebooks should be examined is:
   - WASP-100: This notebook demonstrates how eleanor works and it includes the first results we attempt to replicate (creating the light curves). It includes notes from the tutorial (from the authors) as well as additional notes from us on obstacles we encountered, how we overcame them and short discussions about our results. WASP-100 is part of the paper's original dataset.
   - TOI-172: Here we replicate the evaluation process from the paper. TOI-172 is part of the paper's original dataset.
   - TOI-530: In this notebook, we demonstrate how some targets are not suitable for eleanor, as the produced light curves included too much noise to distinguish any transit features. In addition, not all targets have light curves produced by the TASOC and/or Oelkers & Stassun (OS19) pipelines.
   - All other targets: These are the targets acquired for our new dataset and can be viewed at any order.
2. Occasionally, certain cells may take some time to run (usually up to 4-5 minutes).
3. At times, cells retrieving the TASOC or OS19 light curves might produce an error. All targets (except for TOI-530) have light curves in both TASOC and OS19. If such an error occurs, please run the cells again starting from the first cell in the "Crossmatch" section.
4. Some plots in the notebooks may appear slightly different to the plots in the report. This may be due to changes in the TASOC pipeline (producing different light curves), updates to eleanor or new data being added from TESS to our targets. However, the important features remain the same, namely the number, depth and time coordinates of the transits. Therefore, minor differences in the plots do not affect our final results. 


# References
1. Feinstein et al. 2019, PASP, 131, 1003, link: https://ui.adsabs.harvard.edu/abs/2019PASP..131i4502F/abstract
2. GitHub for paper: https://github.com/afeinstein20/eleanor/tree/main
