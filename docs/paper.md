Electric Vehicle Adoption Across U.S.: Economic Patterns, Market Dynamics, and Future Projections



M. Jian

University High School, United States



J. Sun

Eleanor Roosevelt High School, United States



Abstract

The rapid growth of electric vehicle (EV) adoption in the United States is fueled by new technology and changing factors. Yet, states differ individually in their economic conditions, infrastructure, and policy, resulting in adoption rates varying from state to state. This study investigates patterns from the past to provide projections of EV adoption throughout the US. Using manually compiled datasets from research and government sources, we analyze adoption rates relative to factors such as median income, fuel and electricity prices, policies and incentives, and urbanization. The research is broken up into three components: (1) a 2023 snapshot analysis, (2) a spatial-temporal panel analysis of adoption from 2016 to 2023 over different states, and (3) a growth prediction model for California using sigmoidal functions and Bass diffusion models. Results from using correlation and regression models show how higher income, greater gasoline prices, more incentives, higher vehicle usage, and greater urban road ratios are positively associated with EV adoption; higher electricity costs are found to be negatively correlated. Spatial-temporal analysis shows how regional clustering affects states that are closer together and adoption of EVs might spread from states that have adopted EVs early such as California to other regions. Forecasting results using a logistic growth model projects California to reach ~50% EV adoption by 2035 before the rate of adoption plateaus; a bass diffusion model leads to a similar prediction. With these findings, we can see the importance of considering economic conditions and other factors to ensure future planning to continue driving EV adoption growth.





Key Words: electric vehicles, adoption, snapshot analysis, spatial-temporal panel analysis, growth prediction model



Introduction

The transition to electric vehicles (EVs) has been a vital part of U.S. clean transportation policies over the past decade. While national EV adoption rates remain fairly low relative to the number of total vehicles, the pace of growth of the number of EVs between 2016 and 2023 has been rapid. As a result of a combination of technological advancements, policy support, and shifts in specific economics, electric vehicles have been quickly adopted by various states within the country. These plug-in light-duty vehicles include battery electrics (BEVs) and plug-in hybrids (PHEVs). According to the International Council on Clean Transportation, in 2023, the U.S. new EV light-duty sales were approximately 1.4 million, about 9% of new light-duty sales. Furthermore, according to the U.S. Energy Information Administration, despite fast growth, plug-ins still remained less than 2% of all registered light-duty vehicles in 2023. For that reason, per-capita scaling is extremely important. However, EV adoption still remains very uneven across states, showing differences in policy, infrastructure, prices, and demographics (Siti Norhidayah Toolib, 2023).

One of the main factors driving the adoption of EVs in many states is infrastructure access. As of late 2023, the U.S. had a total of over 168,000 public EVSE charging ports, including more than 43,000 DC fast chargers (Alternative Fuels Data Center). However, access is unevenly distributed in many regions within the country. A study from the Pew Research Center has revealed that 60% of urban residents live within two miles of a public charger, compared to only 17% of rural residents who have convenient access. This urban-rural divide in access shows certain infrastructure patterns and possibly barriers to usage among different groups of individuals.

Another factor affecting the adoption of EVs would be certain economic considerations. The U.S. Department of Energy’s “eGallon” metric shows that, on average, fueling an EV remains less costly and less price-volatile than fueling a gasoline vehicle during current times (U.S. Department of Energy). At 2023 electricity rates, EVs could deliver per-mile fuel costs in the range of $0.06-$0.09, compared to approximately $0.14 for a gasoline vehicle at gas prices of $3.50 per gallon. Maintenance savings also make EVs have more cost advantages. A consumer report finds that EV owners spend about half as much money on maintenance over a vehicle’s lifetime as gasoline vehicle owners (Harto, 2020).

As a whole, these infrastructures and varying costs are shaped by state policy variations and market availability, suggesting that EV adoption is uneven during varying time periods and different regions of the U.S. For instance, states with similar policy diffusion ties might develop at similar paces, while bordering states might also affect the rate of EV adoption. This study seeks to answer the following questions:

What are the key factors influencing EV adoption rates across U.S. states in recent years (2023)?

How has electric vehicle adoption spread across states from 2016 to 2023, and can we predict future EV adoption trends based on these patterns?

This study looks at three different concepts: a 2023 snapshot analysis, a 2016-2023 spatial-temporal panel analysis, and a forecasting model for California. By taking a variety of approaches, this study seeks to address both the current state of EV adoption and its projected trajectory for future implementation of policies and infrastructure.

The 2023 snapshot analysis provides an up-to-date picture of current U.S. EV conditions at the most recent point of complete data availability. By looking at present data, we are able to understand the relationship between EV adoption and factors such as income, gas prices, electricity prices, incentives, and urban EV infrastructure density. The 2016-2023 panel analysis allows us to examine the diffusion of EV adoption over a period of time and across a variety of regions. By looking at multiple years, we can investigate patterns of growth as a result of time and regional clustering (Soltani-Sobh et al., 2017). Finally, the California forecasting component projects future adoption in a state that is currently an EV leader in the U.S. California’s future trajectory can provide information about how an EV market may develop that may be applicable to other states as they continue with EV adoption.

This study is limited by certain items, such as EV adoption being measured with registrations instead of sales, AFDC data being rounded, and results only showing trends at the state level, which may not show differences at the local level. Furthermore, policies were treated equally despite some policies having a more significant impact than others.

Literature Review

Throughout the past few years, the adoption of new technology, specifically EVs, has been growing significantly. This was mainly caused as a result of the incentives due to environmental benefits and policy cost-effectiveness. Another reason is that consumer response to energy prices is asymmetric. According to Xing et al. (2021), EV sales are several times more sensitive to gasoline prices than to electricity prices. This means that oil price cycles can change EV demand more than just retail electricity price changes.

Charging availability and reliability are also other reasons for changes in demand. At a national scale, the number of non-home chargers (public + publicly accessible workplace) reached approximately 204,000 by the end of 2024. This was a growth that was roughly 25% annually since 2019 and provides families with assurance for long-distance travel and for households without a garage, where they are able to install these types of EV chargers. However, reliability and uptime of these chargers also resulted in a reduction in the number of EV adoption. According to Powell and Johnson (2024), outages and performance issues reduce the number of EV purchase intents and use.

Lastly, policies also encourage people to purchase EVs. California’s Zero-Emission Vehicle (ZEV) mandate shows how tightening the requirements in terms of EVs can result in the number of new technologies in the market going up (Mcconnell et al., 2019). Non-price incentives like HOV lane access also have a pretty significant effect on the number of EV registrations. This is especially true for individuals who are living in busier and compact areas (Sheldon & DeShazo, 2017). At the federal level, the Inflation Reduction Act estimated reductions in effective EV prices and faster ways to get more EVs on the road. These programs are very important for consumers as they reduce the upfront price of EVs.





Methods

We compiled our own data by researching and compiling information from government and research institutes. First, we began by searching for data that government institutions and nonprofit institutions provided to ensure that we had reputable datasets with accurate information that is relevant to our research question. We utilized datasets that met the following three criteria:

Public availability and documentation

Covers relevant years and information

Data was accurate and complete



Table 1: Sources utilized to compile the dataset that was used for analysis







Table 2: Descriptive Statistics of State-Level Vehicle & Infrastructure Data



Because not all variables were directly available from public sources, we derived additional measures for our analysis. Specifically, three new variables were constructed from the compiled datasets, as summarized in Table 3, which lists their definitions and temporal coverage.

Table 3: Variables created from the compiled dataset.



2023 Snapshot Analysis

To examine factors associated with electric vehicle (EV) adoption across the United States, we did a cross-sectional analysis using 2023 data. The EV adoption rate, defined as the proportion of registered EVs among all registered vehicles, served as the response variable.

We first performed an exploratory analysis to understand the distribution of individual variables. Next, we explored pairwise relationships between the EV adoption rate and several socioeconomic and infrastructural factors, including median household income, charging station density, gasoline price, vehicle miles traveled per capita, urban road ratio, and the presence of state-level incentives. The Pearson correlation coefficients were summarized and visualized.

To evaluate the relative importance of different socioeconomic and infrastructural factors, we applied a multiple linear regression model. To reduce redundancy among predictors, we employed Lasso regression and stepwise feature selection to refine the model.



2016-2023 Spatial-Temporal Panel Analysis

Next, we aimed to characterize temporal dynamics and spatial diffusion patterns in EV adoption by expanding our analysis to a panel dataset spanning 2016 to 2023. Through heatmaps and line plots, we visualized electric vehicle adoption trends over the years and states. We decided to apply a log transformation to EV adoption rates because the log-transformed data shows a clear linear increasing trend over time.

Our spatial-temporal panel analysis accounts for the influence of previous adoption rates within a state along with policy and adoption levels in neighboring states, we created a model that employed the use of spatial and temporal lags. Ideally, in addition to the state-specific effect, we would like to include the following variables: a temporal lag, a spatial lag for border adjacency, a lag for policy diffusion ties (PDT), and a time effect:

,

where

: adoption level (after log-transfromation) in state i at time t

: state-specific fixed effect capturing unobserved heterogeneity across states

: temporal effect, measuring the effect of a state’s own adoption in the previous year on its current adoption

: linear time trend, controlling for common temporal dynamics across states

​: spatial effect for border adjacency, showing spillover effects from geographically neighboring states’ past adoption,  is proportional to the average adoption of neighboring states

: policy diffusion tie (PDT) effect, showing the influence of adoption levels in states with policy diffusion ties to state i;  is higher if policy network is more similar. The PDT network information is part of the State-State Network Data, with details provided in Table 1.

: error term



Due to the high multicollinearity between the variables, we also considered the effects of temporal effect, border adjacency, policy diffusion ties, and time trend on adoption rates individually. Then, the models are examined and compared.





Prediction for California

California stands out among all states due to its distinctive EV policies, infrastructure, consumer adoption trends, and its early initiation. We characterized its temporal pattern of EV adoption by modeling the adoption rate over time using three commonly used growth functions.



Exponential growth. With a log transformation, California’s EVE adoption rate showed an approximately linear trend, suggesting that exponential growth may be reasonable for an early stage – the stage during which data are available. An exponential growth function takes the following form:

,

where A is the initial adoption rate, r is the growth rate, and t is time.



Sigmoidal growth. However, an exponential growth model assumes that EV adoption increases continuously at a constant rate and has unlimited growth without saturation. Because EV adoption rates are naturally bounded between 0 and 1, sigmoidal models might be a better choice, especially for predicting what will happen many years later. There are a family of sigmoidal functions, all capture the typical S-shaped trajectory of growth that starts slowly, accelerates during the expansion phase, and finally slows down to reach a plateau as the market saturates. We considered three commonly used sigmoidal functions:

Logistic Growth Model: where  is the carrying capacity,  is the growth rate, and  is the inflection point.

Gompertz Growth Model:  where  are as above; inflection occurs earlier than in the logistic model.

Richards Growth Model: where  controls the asymmetry of the curve. This model generalizes the logistic model.



We compared the sigmoidal models described above using the Akaike information criterion (AIC) to determine which model should be used for California’s EV adoption data, this is because AIC balances model complexity and model fit, which is better than relying on model fit (such as likelihood), as the Richards model has one more parameter than the other two models.



In addition to the purely mathematical growth functions , we evaluated the Bass Diffusion Model. This model extends the concept of sigmoidal growth by incorporating behavioral mechanisms that drive adoption. Specifically, the model separates adoption into two mechanisms: the innovation effect, which reflects early adoption due to influence from external factors such as technology incentives, and the imitation effect, which represents adoption by followers influenced by social contagion. This model not only reproduces the S-shaped adoption curve but also provides interpretable parameters with p for innovation and q for imitation to characterize the dynamic adoption. Furthermore, the Bass model has been widely used for EV adoption and policy analyses. Studies such as California adopter-heterogeneity work utilized Bass (Lee et al., 2019). Ultimately, the Bass model could help us determine what stage of EV adoption California is in.





Results

2023 Snapshot Analysis

We computed and visualized Pearson’s correlation coefficient in Figure 1. The heatmap shows that EV adoption is most strongly correlated with state incentives and income, suggesting that higher income levels and better policies and incentives are associated with greater EV adoption. Gasoline cost also shows a moderate strong positive correlation. This shows how higher fuel gas prices encourage more EV adoption. Urban road ratio also has a moderate positive correlation, implying that urban infrastructure may allow for more adoption. On the other hand, charging station density has a very weak correlation with EV adoption which shows how infrastructure alone may not increase adoption of EVs. Vehicle miles traveled per capita is negatively correlated with EV adoption, showing how states with more driving intensity tend to have lower EV adoption rates.

For each feature, we fit a simple linear regression to examine whether it is significantly correlated with EV adoption rate. All features, except charging station density, are significant at level 0.05.



![Figure 1](/EV-Adoption-Across-United-States/docs/assets/image1.png)



Figure 1: Pairwise correlation between Electric Vehicle Ratio and selected features







We ran Lasso Regression, along with forward and backwards selection to select features that jointly explain EV adoption rate across states. Our Lasso model dropped Charging Station Density.  Both forward and backwards selections dropped Charging Station Density, Urban Road Ratio, and Electricity Cost. Since all models gave similar R2, we chose the model formed by using forward and backwards selection, as this model uses few variables, which might be less prone to overfitting or affected by collinearity.  By analyzing the residual plot for the model, we found no obvious outliers, and although California seemed like an outlier individually, excluding it did not significantly affect the model.







Table 4: The final model, which was chosen by forwards and backwards selection results





Table 4 shows the regression output after applying Forward and backwards selection. From the estimate, income has a significant positive effect, showing how higher income levels are associated with greater EV adoption. Gas cost also shows a strong positive association, meaning that higher gasoline prices are linked to increased EV adoption. Incentives are highly significant, showing how state-level policies and incentives encourage more EV adoption. Vehicles miles traveled per capita is significant as well, showing that driving intensity also contributes to patterns of adoption. Lastly, urban road ratio is also significant, implying that urban infrastructure correlates positively with adoption. Overall, this shows how various factors such as socioeconomic factors, fuel prices, and state infrastructure and incentives might impact EV adoption.





2016-2023 Spatial-Temporal Panel Analysis

We first created a chronological heatmap to visualize the change in EV adoption rate from 2016-2023. The chronological heatmap in Figure 2 shows the progression of EV adoption rates across U.S. states from 2026 to 2023. In 2016, adoption rates were uniformly low nationwide, with only a few states such as California showing noticeable early adoption. From 2017 to 2019, adoption expanded gradually, with growth along the West Coast and some activity in the Northeast. By 2020 and 2021, adoption accelerated, with California and neighboring western states showing much darker shading, showing more EV adoption. By 2022 and especially 2023, the map shows widespread increases in EV adoption across the country, although there are still some regional disparities. California continues to have the highest adoption rate while several Mountain West and Southern states still have relatively low adoption levels. Figure 2 shows two key points: first EV adoption is no longer only for states with early adoption, but has become more nationwide; second, significant geographic inequality is still present, which shows how local policies and socioeconomic factors may affect EV adoption.

![Figure 2](/EV-Adoption-Across-United-States/docs/assets/image2.png)



Figure 2: Heatmap that shows multiple years of EV adoption rates from 2016-2023

After this, we plotted lines over time to see how the values changed for each state. As shown in Figure 2, taking the log transformation for the lines causes it to appear linear, which suggests a log transformation.



![Figure 3](/EV-Adoption-Across-United-States/docs/assets/image3.png)



Figure 3: State values over time graph of  EV adoption. The left graph is not transformed but the right graph utilized log transformation.



As described in Methods, initially, we planned to include temporal lag, spatial lag, policy diffusion ties, and time in one model to characterize the dynamic spatial pattern. However, each of these four features are highly correlated, so we also fit and compared individual models:





Table 5: Estimates, p-values, and R-squared for individual variables evaluating temporal and dynamic patterns. EV_prev: Previous Adoption rates in the same state;  Time: Overall national adoption over time;  EV_border: Adoption rates of neighboring states,  EV_PDT: Adoption rates based on state policy



Based on the results in Table 5, all four predictors are individually significant at the 0.0001 level with high explanatory power (R2 = 0.96). We also found that these variables are highly correlated, meaning that while each variable shows an important part of diffusion, their explanatory power overlaps significantly and it is not feasible to distinguish them. Despite the high collinearity, we fit the model with all four predictors included. All predictors are still high significant, except that EV_border is marginally significant (p=0.057) after adjusting for the other three predictors. This multiple regression increases R2 slightly: R2=0.978 and adjusted R2=0.974.



The high collinearity between these variables is likely due to the almost perfect linear (after log transformation) growth trends of individual states, as shown in Figure 3. From 2016 to 2023, all the states were in the log-linear growth stage and with a similar shared growth rate.  As a result, a state can be predicted quite well no matter whether we use its previous data or other states’ data. Consequently, we are not able to distinguish their effects from each other from the data. Nevertheless, the small improvement in R2 from using individual predictors to all predictors suggest that border effects and PDT might affect the adoption of a state, although the effects might be small.



Prediction in California

In this section, we focus on California to illustrate the model’s predictions over time, particularly for the year that the EV adoption rate is predicted to be 50%. The fitted growth curve using the exponential function and three sigmoidal functions are shown in Figure 4.





![Figure 4](/EV-Adoption-Across-United-States/docs/assets/image4.png)



Figure 4: Fitted growth curve using exponential and sigmoidal functions.



Exponential models assume growth that is unbounded, meaning that adoption accelerates infinitely and past 100%. In reality, EV adoption must plateau as the market becomes saturated. As shown in Figure 5, according to the exponential model, the predicted adoption rate reaches 50% at 2031 but exceeds 100% at 2033, which is unrealistic.



![Figure 5](/EV-Adoption-Across-United-States/docs/assets/image5.png)



Figure 5: Exponential model versus logistic model fit on the forecast of EV adoption in California.



Therefore, we switched to sigmoidal models. A smaller AIC value is preferred, so based on AIC,  a logistic model is the best choice among the three sigmoidal models we examined. The logistic model introduces a carrying capacity, meaning that the model tapers off near the end to show the stabilization in EV adoption rates. According to the logistic growth model, half of California’s registered vehicles will be electric by 2035.



Finally, we compared electric vehicle adoption in other states to California, to envision how much time would pass before those states would appear like California. We did this by aligning the adoption rate of each state with that of California’s, and compared how many years it would take for the 2016 value to reach that of California’s 2016 value.



![Figure 6](/EV-Adoption-Across-United-States/docs/assets/image6.png)



Figure 6: Lag in EV Adoption compared to California









We also ran a Bass Diffusion Model because a Bass Diffusion model is a powerful to separate adoption into two main components:

Innovation (p): Some people adopt because of outside influences (media campaigns, technological incentives.)

Imitation (q): Others adopt because they see people around them already using it (neighbors, friends, etc.)

When we initially ran the bass Diffusion model, we were unable to get interpretable results with our 8 data points from 2016 to 2023. As a result, we obtained data from California’s Energy website, which had data from 2010 to 2024, albeit the numbers varied slightly.



Table 6: Results from Bass Diffusion Model.

The Bass model estimation yielded a near-zero innovation coefficient (𝑝). This small value suggests that early adoption in California was not strongly driven by innovators acting independently. The strong coefficient of imitation (q=0.3219, highly significant at p < 0.0001) shows how contagion effects are very important when it comes to adoption. California appears to be adopting EVs in large numbers because people in California see other individuals adopting EVs. Residents may see their neighbors, friends, and coworkers purchasing EVs, and this results in them wanting to buy an EV for themselves. This can also be applied to a statewide level, where policies and incentives affecting EV adoption in one state may affect another state’s policies and adoption rates. Mathematically, when 𝑝 approaches zero, the Bass model converges to a logistic form. Thus, our findings suggest that California’s EV adoption trajectory closely follows a logistic diffusion pattern. Indeed, we found that the two models provide a similar prediction – EV adoption rate increases to 50% by 2035.



Discussion

Overview

This study focuses on a 2023 cross-sectional snapshot, a 2016-2023 spatial-temporal panel, and a California-focused forecast to explain why EV adoption differs across states and how it spreads over time. Together, the results show consistent patterns within states, spillovers across neighboring states, and the role of policies when it comes to EV adoption.



Factors Associated with EV Adoption

Economic capacity and policy support: In 2023, adoption is most strongly tied to state incentives and household income, with higher gasoline prices encouraging people to switch more toward EVs. When EVs are more affordable upfront and fuel savings are more meaningful to consumers, adoption rates tend to rise.



Operating costs: Higher residential electricity prices are associated with lower EV adoption, since they reduce the advantage of cheaper running costs compared to gasoline vehicles.



Infrastructure and urban form: At the state level, charging-station density has a weak direct relationship with adoption. This is most likely due to the fact that many owners charge at home, and charging infrastructure tends to expand after demand increases. By contrast, a higher share of urban roads is modestly linked to higher adoption. Shorter trips, more visible EV infrastructure, and policy activity encourage people to adopt EVs.



Travel intensity: Vehicle miles traveled per capita shows a negative correlation with adoption in our analysis. This suggests that more rural, long-distance driving makes EVs less favorable to some people.



Diffusion Across States

Adoption follows a diffusion pattern of starting on the West Coast and slowly moving eastward over time. Log-transformed trends are close to linear, which shows how many states are still accelerating in terms of EV adoption. Persistence within states, neighbor effects, policy diffusion, and nationwide trends all impact EV adoption rates.



California as a Case Study

Model comparison favors a sigmoidal model. The logistic model projects that about 50% of registered vehicles in California will be electric around 2035, showing the acceleration of EV adoption while avoiding the over-prediction that comes with an exponential model. A Bass diffusion fit on a longer series shows a very small innovation effect and a large imitation effect. This shows how social contagion (adopting after peers) is very important to EV adoption rates.



Limitations

1. Measurement: Adoption is measured via registrations rather than sales; AFDC counts are rounded; Charging is summarized as stations per area rather than access on the household level.



2. Aggregation: State-level analysis does not show the metro-rural differences or the differences in terms of the number of EV dealers present; counting incentives may treat programs of very different impact as equal.



3. Forecast sensitivity for California: Major technology or policy changes could alter the projected trajectory.



4. Identification: Strong Collinearity across temporal, spatial, policy-network, and time effects limits the study’s ability for causal separation.



Policy and Future Recommendations

1. Increase financial incentives in low-adoption but high-potential states to lower upfront EV costs for first-time buyers.



2. Address high electricity costs with EV-specific tariffs (e.g., off-peak rates or subscriptions) and support for rooftop solar paired with home charging.



3. Increase access in underserved areas - particularly rural regions and multi-unit housing - through community hubs and shared chargers.



4. Coordinate policies regionally so neighboring states align incentives and can co-invest in cross-border infrastructure. This is shown by the observed clustering and spillovers as identified in the study.



Summary

EV adoption in the U.S. shows both market fundamentals in the market - income, incentives, and energy prices - and social diffusion. California represents an EV fast start state where adoption rates slowly plateau. Sustaining the national momentum in EV adoption will require a balance of affordability incentives, built-out infrastructure, and coordinated policy at the regional level.





Acknowledgments

The authors thank the UCI ICS Summer Academy 2024, where they first met and discovered a shared interest in studying energy efficiency. MJ also appreciates the opportunity to learn data science through UCI Cosmos. They are grateful to their mentors, Professor Tingting Nian UCI, for her very helpful comments such as the suggestion of Bass diffusion models.



References

2023 Transportation Electrification Scorecard. (2023). Aceee.org.

Alternative Fuels Data Center: Maps and Data - Electric Vehicle Laws and Incentives by State. (n.d.). Afdc.energy.gov.

Alternative Fuels Data Center: Vehicle Registration Counts by State. (2023). Energy.gov.

Average Electricity Price. (2022). Eia.gov.

Average Gas Price. (2023). Eia.gov.

Bestvater, S., & Shah, S. (2024, May 23). Electric Vehicle Charging Infrastructure in the U.S. Pew Research Center.

Commission, California Energy. “New ZEV Sales in California.” Www.energy.ca.gov,

Electric vehicle market and policy developments in U.S. states, 2023 - International Council on Clean Transportation. (2023). International Council on Clean Transportation.

Engel, K., & Posey, K. (2024). Household income in states and metropolitan areas: 2023.

Hybrid vehicle sales continue to rise as electric and plug-in vehicle shares remain flat - U.S. Energy Information Administration (EIA). (2025). Eia.gov.

Mcconnell, V., Leard, B., & Kardos, F. (2019). California’s Evolving Zero Emission Vehicle Program: Pulling New Technology into the Market.

Motor Vehicle Registrations, 2000 - 2023 (MV-1). (2025, March 6). Transportation.gov.

Powell, B., & Johnson, C. (2025). Impact of Electric Vehicle Charging Station Reliability, Resilience, and Location on Electric Vehicle Adoption. Nrel.gov.

Sheldon, T. L., & DeShazo, J. R. (2017). How does the presence of HOV lanes affect plug-in electric vehicle adoption in California? A generalized propensity score approach. Journal of Environmental Economics and Management, 85, 146–170.

State Networks | Institute for Public Policy and Social Research. (2020). Msu.edu.

States, U. (2024). Explore Census Data. Census.gov.

Table HM-20 - Highway Statistics 2022 - Policy | Federal Highway Administration. (2022). Archive.org.

Table HM-20 - Highway Statistics 2023 - Policy | Federal Highway Administration. (2023). Dot.gov.

Table MV-1 - Highway Statistics 2023 - Policy | Federal Highway Administration. (2023). Dot.gov.

Table VM-2 - Highway Statistics 2023 - Policy | Federal Highway Administration. (2023). Dot.gov.

US Census Bureau. (2010). State Area Measurements and Internal Point Coordinates. The United States Census Bureau.

Winikoff, J. B. (2024). Economic specialization, infrastructure, and rural electric vehicle adoption. Energy Policy, 195, 114380.

(2025). Energy.gov.

Xing, J., Leard, B., & Li, S. (2021). What does an electric vehicle replace? Journal of Environmental Economics and Management, 107, 102432.

