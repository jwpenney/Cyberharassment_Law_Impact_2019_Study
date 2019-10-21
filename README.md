# When Laws Free Us To Speak 

Does Awareness of a Cyberharassment Law Impact on People's Online Speech, Sharing, and Engagement?

Cite: Danielle Keats Citron and Jonathon W. Penney, When Law Frees Us To Speak, Fordham Law Review, 2019, Vol. 87, at p. 2317
Link to Paper: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3309227

## Data and Analysis Repository 

For the study discussed in this article, we use data collected via an online survey in March 2015. The dataset thus constituted 1,296 total survey responses, with sixty-four survey responses excluded for being substantially incomplete (defined by ten or more questions left unanswered—many of these were likely false starts by respondents). 

## Analysis
In the survey case study, ordinary least squares (OLS) regression, a common statistical method for analyzing survey data, was used to statistically analyze findings, as it allowed for all relevant variables to be controlled in order to isolate relationships. 

## Results
The following STATA commands were executed on the relevant variables in the data set (See "When Law Frees Us To Speak Article Data Set). These outputs are set out in Table 1 of the article (see also: "When Law Frees Us To Speak - STATA Outputs (Table 1)") 

==========
. reg q2LawTimeREVERSE ageREC gender EduRECFinal AnnualIncome TimeSpentOnline OnlinePersonalSharing SNScontributions q7eLAWPrivacy

      Source |       SS       df       MS              Number of obs =    1192
-------------+------------------------------           F(  8,  1183) =   11.90
       Model |  39.8195512     8   4.9774439           Prob > F      =  0.0000
    Residual |  494.937999  1183  .418375316           R-squared     =  0.0745
-------------+------------------------------           Adj R-squared =  0.0682
       Total |   534.75755  1191  .448998783           Root MSE      =  .64682

---------------------------------------------------------------------------------------
     q2LawTimeREVERSE |      Coef.   Std. Err.      t    P>|t|     [95% Conf. Interval]
----------------------+----------------------------------------------------------------
               ageREC |   .0784259   .0262067     2.99   0.003      .027009    .1298427
               gender |   .1514352   .0380281     3.98   0.000     .0768251    .2260453
          EduRECFinal |  -.0010591   .0293505    -0.04   0.971    -.0586439    .0565257
         AnnualIncome |  -.0108656    .016602    -0.65   0.513    -.0434383    .0217071
      TimeSpentOnline |   .0271955   .0287655     0.95   0.345    -.0292415    .0836326
OnlinePersonalSharing |  -.0318135   .0196033    -1.62   0.105    -.0702745    .0066476
     SNScontributions |   .0045868   .0160911     0.29   0.776    -.0269834     .036157
        q7eLAWPrivacy |  -.1122944    .014887    -7.54   0.000    -.1415024   -.0830864
                _cons |   2.968735   .1787163    16.61   0.000     2.618099    3.319372
---------------------------------------------------------------------------------------


. reg q3LawSpeakREVERSE ageREC gender EduRECFinal AnnualIncome TimeSpentOnline OnlinePersonalSharing SNScontributions q7eLAWPrivacy

      Source |       SS       df       MS              Number of obs =    1189
-------------+------------------------------           F(  8,  1180) =   11.52
       Model |  76.3881418     8  9.54851773           Prob > F      =  0.0000
    Residual |  977.714465  1180  .828571581           R-squared     =  0.0725
-------------+------------------------------           Adj R-squared =  0.0662
       Total |  1054.10261  1188  .887291757           Root MSE      =  .91026

---------------------------------------------------------------------------------------
    q3LawSpeakREVERSE |      Coef.   Std. Err.      t    P>|t|     [95% Conf. Interval]
----------------------+----------------------------------------------------------------
               ageREC |   .0104065   .0369098     0.28   0.778    -.0620096    .0828227
               gender |   .0692869   .0535762     1.29   0.196    -.0358282    .1744021
          EduRECFinal |   .0012938    .041357     0.03   0.975    -.0798476    .0824351
         AnnualIncome |   .0078957   .0234484     0.34   0.736    -.0381094    .0539009
      TimeSpentOnline |   .0002318    .040521     0.01   0.995    -.0792694     .079733
OnlinePersonalSharing |  -.0142973   .0276376    -0.52   0.605    -.0685216    .0399269
     SNScontributions |    .017105   .0226714     0.75   0.451    -.0273758    .0615859
        q7eLAWPrivacy |  -.1929452   .0210007    -9.19   0.000    -.2341481   -.1517423
                _cons |   3.241197   .2515856    12.88   0.000     2.747592    3.734802
---------------------------------------------------------------------------------------

. reg q4LawShareREVERSE ageREC gender EduRECFinal AnnualIncome TimeSpentOnline OnlinePersonalSharing SNScontributions q7eLAWPrivacy

      Source |       SS       df       MS              Number of obs =    1191
-------------+------------------------------           F(  8,  1182) =   19.78
       Model |  115.268918     8  14.4086148           Prob > F      =  0.0000
    Residual |  861.088765  1182  .728501493           R-squared     =  0.1181
-------------+------------------------------           Adj R-squared =  0.1121
       Total |  976.357683  1190  .820468641           Root MSE      =  .85352

---------------------------------------------------------------------------------------
    q4LawShareREVERSE |      Coef.   Std. Err.      t    P>|t|     [95% Conf. Interval]
----------------------+----------------------------------------------------------------
               ageREC |  -.0044063   .0346037    -0.13   0.899    -.0722978    .0634852
               gender |   .1198142   .0501904     2.39   0.017      .021342    .2182864
          EduRECFinal |   .0256004    .038792     0.66   0.509    -.0505085    .1017093
         AnnualIncome |  -.0106151   .0219018    -0.48   0.628    -.0535859    .0323558
      TimeSpentOnline |   .0380388   .0381501     1.00   0.319    -.0368107    .1128884
OnlinePersonalSharing |  -.0265645   .0258728    -1.03   0.305    -.0773261    .0241971
     SNScontributions |   .0114551   .0212392     0.54   0.590    -.0302157    .0531259
        q7eLAWPrivacy |  -.2362595   .0196451   -12.03   0.000    -.2748026   -.1977163
                _cons |   3.284765   .2365033    13.89   0.000     2.820752    3.748778
---------------------------------------------------------------------------------------


. reg q6LawSnsREVERSE ageREC gender EduRECFinal AnnualIncome TimeSpentOnline OnlinePersonalSharing SNScontributions q7eLAWPrivacy

      Source |       SS       df       MS              Number of obs =    1187
-------------+------------------------------           F(  8,  1178) =   24.98
       Model |  185.369051     8  23.1711313           Prob > F      =  0.0000
    Residual |   1092.8601  1178  .927725041           R-squared     =  0.1450
-------------+------------------------------           Adj R-squared =  0.1392
       Total |  1278.22915  1186  1.07776488           Root MSE      =  .96318

---------------------------------------------------------------------------------------
      q6LawSnsREVERSE |      Coef.   Std. Err.      t    P>|t|     [95% Conf. Interval]
----------------------+----------------------------------------------------------------
               ageREC |   .0046553   .0391518     0.12   0.905    -.0721598    .0814704
               gender |   .1472173   .0567488     2.59   0.010     .0358774    .2585573
          EduRECFinal |  -.0209582   .0439249    -0.48   0.633    -.1071379    .0652215
         AnnualIncome |  -.0254924   .0247599    -1.03   0.303    -.0740709    .0230861
      TimeSpentOnline |  -.0212971    .042919    -0.50   0.620    -.1055034    .0629092
OnlinePersonalSharing |  -.0095154   .0293257    -0.32   0.746    -.0670519    .0480211
     SNScontributions |   .0416418   .0240274     1.73   0.083    -.0054994    .0887831
        q7eLAWPrivacy |  -.2975941   .0221986   -13.41   0.000    -.3411473    -.254041
                _cons |   3.631765   .2665456    13.63   0.000     3.108808    4.154723
---------------------------------------------------------------------------------------

