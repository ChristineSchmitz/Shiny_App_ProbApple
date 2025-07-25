# Shiny App for the ProbApple model

## Background
Models, such as the [ProbApple model](https://doi.org/10.5281/zenodo.14202192) are often hard to use without a proper user interface. Therefore we developed a Shiny App to run model. 
A detailed description of the model is published in the research article [ProbApple – Aprobabilistic model to forecast apple yield and quality](https://doi.org/10.1016/j.agsy.2025.104298) (Schmitz et al., 2025)[^1]
In short, ProbApple is a probabilistic model to forecast apple yield and quality at four key time points during the vegetation period: ‘at full bloom’, ‘before fruit thinning’, ‘after June drop’, ‘four weeks before harvest’. 

## Technical requirements
To run the app locally on your computer, you need R and the packages shiny[^2], shinyWidgets[^3], datamods[^4], bslib[^5], reactable[^6], decisionSupport[^7], tidyverse[^8] and patchwork[^9].

## Repository content
[`www`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/tree/main/www)is folder where all pictures needed in the App are stored. 

[`Shiny_App_ProbApple.Rproj`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/Shiny_App_ProbApple.Rproj) is the R project file for running the app

[`app.R`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/app.R) is the main file with the Shiny App and contains the UI and the server part. 

[`apple_estimation_manuscript.csv`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/apple_estimation_manuscript.csv) and [`apple_quality_input_manucript.csv`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/apple_quality_input_manuscript.csv) are files with the initial input parameters

[`functions_v2.R`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/functions_v2.R) contains the yield and quality prediction functions for all forecasting time points

[`management_values.R`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/management_values.R), [`management_values1.R`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/management_values1.R), [`management_values2.R`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/management_values2.R) and [`management_values3.R`](https://github.com/ChristineSchmitz/Shiny_App_ProbApple/blob/main/management_values3.R) help to read in the choosen management measures for the calculation.

## Acknowledgments
Thanks to [Lars Zimmermann](https://github.com/Lars-Zimmermann), [Katja Schiffers](https://github.com/katjaschiffers), Martin Balmer and [Eike Luedeling](https://github.com/eikeluedeling) for their contribution in the development of ProbApple. Furthermore, i thank all experts who contributed their knowledge to the workshop and model building

## Funding
This work was part of the [Experimentierfeld Südwest](https://ef-sw.de/) funded by the German Federal Ministry of Food and Agriculture [grant number: 28DE111B22].

## References

[^1]: Schmitz, C., Zimmerman, L., Schiffers, K., Balmer, M., Luedeling, E., 2025. ProbApple – A probabilistic model to forecast apple yield and quality. Agricultural Systems 226, 104298.
[^2]: Chang W, Cheng J, Allaire J, Sievert C, Schloerke B, Xie Y, Allen J, McPherson J, Dipert A, Borges B (2025).
  _shiny: Web Application Framework for R_. R package version 1.11.1,
  <https://CRAN.R-project.org/package=shiny>.
[^3]: Perrier V, Meyer F, Granjon D (2025). _shinyWidgets: Custom Inputs Widgets for Shiny_. R package version
  0.9.0, <https://CRAN.R-project.org/package=shinyWidgets>.
[^4]: Perrier V, Meyer F, Goumri S, Abeer Z (2024). _datamods: Modules to Import and Manipulate Data in 'Shiny'_. R
  package version 1.5.3, <https://CRAN.R-project.org/package=datamods>.
[^5]: Sievert C, Cheng J, Aden-Buie G (2025). _bslib: Custom 'Bootstrap' 'Sass' Themes for 'shiny' and 'rmarkdown'_.
  R package version 0.9.0, <https://CRAN.R-project.org/package=bslib>.
[^6]: Lin G (2023). _reactable: Interactive Data Tables for R_. R package version 0.4.4,
  <https://CRAN.R-project.org/package=reactable>.
[^7]: Luedeling E, Goehring L, Schiffers K, Whitney C, Fernandez E (2024). _decisionSupport: Quantitative Support of
  Decision Making under Uncertainty_. R package version 1.114,
  <https://CRAN.R-project.org/package=decisionSupport>.
[^8]: Wickham H, Averick M, Bryan J, Chang W, McGowan LD, François R, Grolemund G, Hayes A, Henry L, Hester J, Kuhn
  M, Pedersen TL, Miller E, Bache SM, Müller K, Ooms J, Robinson D, Seidel DP, Spinu V, Takahashi K, Vaughan D,
  Wilke C, Woo K, Yutani H (2019). “Welcome to the tidyverse.” _Journal of Open Source Software_, *4*(43), 1686.
  doi:10.21105/joss.01686 <https://doi.org/10.21105/joss.01686>.
[^9]: Pedersen T (2025). _patchwork: The Composer of Plots_. R package version 1.3.1,
  <https://CRAN.R-project.org/package=patchwork>.