![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Codeanywhere Template Instructions

Welcome,

This is the Code Institute student template for Codeanywhere. We have preinstalled all of the tools you need to get started. It's perfectly ok to use this template as the basis for your project submissions. Click the `Use this template` button above to get started.

You can safely delete the Codeanywhere Template Instructions section of this README.md file,  and modify the remaining paragraphs for your own project. Please do read the Codeanywhere Template Instructions at least once, though! It contains some important information about the IDE and the extensions we use. 

## How to use this repo

1. Use this template to create your GitHub project repo

1. Log into <a href="https://app.codeanywhere.com/" target="_blank" rel="noreferrer">CodeAnywhere</a> with your GitHub account.

1. On your Dashboard, click on the New Workspace button

1. Paste in the URL you copied from GitHub earlier

1. Click Create

1. Wait for the workspace to open. This can take a few minutes.

1. Open a new terminal and <code>pip3 install -r requirements.txt</code>

1. In the terminal type <code>pip3 install jupyter</code>

1. In the terminal type <code>jupyter notebook --NotebookApp.token='' --NotebookApp.password=''</code> to start the jupyter server.

1. Open port 8888 preview or browser

1. Open the jupyter_notebooks directory in the jupyter webpage that has opened and click on the notebook you want to open.

1. Click the button Not Trusted and choose Trust.

Note that the kernel says Python 3. It inherits from the workspace so it will be Python-3.8.12 as installed by our template. To confirm this you can use <code>! python --version</code> in a notebook code cell.


## Cloud IDE Reminders

To log into the Heroku toolbelt CLI:

1. Log in to your Heroku account and go to *Account Settings* in the menu under your avatar.
2. Scroll down to the *API Key* and click *Reveal*
3. Copy the key
4. In your Cloud IDE, from the terminal, run `heroku_config`
5. Paste in your API key when asked

You can now use the `heroku` CLI program - try running `heroku apps` to confirm it works. This API key is unique and private to you so do not share it. If you accidentally make it public then you can create a new one with _Regenerate API Key_.

## Dataset Content
* The dataset is sourced from [Kaggle](https://www.kaggle.com/codeinstitute/housing-prices-data). We then created a fictitious user story where predictive analytics can be applied in a real project in the workplace. 
* The dataset has almost 1.5 thousand rows and represents housing records from Ames, Iowa, indicating house profile (Floor Area, Basement, Garage, Kitchen, Lot, Porch, Wood Deck, Year Built) and its respective sale price for houses built between 1872 and 2010.

|Variable|Meaning|Units|
|:----|:----|:----|
|1stFlrSF|First Floor square feet|334 - 4692|
|2ndFlrSF|Second-floor square feet|0 - 2065|
|BedroomAbvGr|Bedrooms above grade (does NOT include basement bedrooms)|0 - 8|
|BsmtExposure|Refers to walkout or garden level walls|Gd: Good Exposure; Av: Average Exposure; Mn: Minimum Exposure; No: No Exposure; None: No Basement|
|BsmtFinType1|Rating of basement finished area|GLQ: Good Living Quarters; ALQ: Average Living Quarters; BLQ: Below Average Living Quarters; Rec: Average Rec Room; LwQ: Low Quality; Unf: Unfinshed; None: No Basement|
|BsmtFinSF1|Type 1 finished square feet|0 - 5644|
|BsmtUnfSF|Unfinished square feet of basement area|0 - 2336|
|TotalBsmtSF|Total square feet of basement area|0 - 6110|
|GarageArea|Size of garage in square feet|0 - 1418|
|GarageFinish|Interior finish of the garage|Fin: Finished; RFn: Rough Finished; Unf: Unfinished; None: No Garage|
|GarageYrBlt|Year garage was built|1900 - 2010|
|GrLivArea|Above grade (ground) living area square feet|334 - 5642|
|KitchenQual|Kitchen quality|Ex: Excellent; Gd: Good; TA: Typical/Average; Fa: Fair; Po: Poor|
|LotArea| Lot size in square feet|1300 - 215245|
|LotFrontage| Linear feet of street connected to property|21 - 313|
|MasVnrArea|Masonry veneer area in square feet|0 - 1600|
|EnclosedPorch|Enclosed porch area in square feet|0 - 286|
|OpenPorchSF|Open porch area in square feet|0 - 547|
|OverallCond|Rates the overall condition of the house|10: Very Excellent; 9: Excellent; 8: Very Good; 7: Good; 6: Above Average; 5: Average; 4: Below Average; 3: Fair; 2: Poor; 1: Very Poor|
|OverallQual|Rates the overall material and finish of the house|10: Very Excellent; 9: Excellent; 8: Very Good; 7: Good; 6: Above Average; 5: Average; 4: Below Average; 3: Fair; 2: Poor; 1: Very Poor|
|WoodDeckSF|Wood deck area in square feet|0 - 736|
|YearBuilt|Original construction date|1872 - 2010|
|YearRemodAdd|Remodel date (same as construction date if no remodelling or additions)|1950 - 2010|
|SalePrice|Sale Price|34900 - 755000|


## Business Requirements

As a trusted friend, I've been approached by a close friend who recently inherited properties from her great-grandfather in Ames, Iowa. She has tasked me with maximizing the sales value of these properties.

My friend is quite knowledgeable about property values in her own state and area, but she's concerned that this knowledge might not accurately apply to Ames. Aware of the regional differences in what makes a property desirable, she wisely decided to use a more data-driven approach. She's provided me with a public dataset containing property prices in Ames, which I'll use for this analysis.

There are two main objectives for this project:

* BR1 - The client is interested in discovering how the house attributes correlate with the sale price. Therefore, the client expects data visualisations of the correlated variables against the sale price to show that.
* BR2 - The client is interested in predicting the house sale price from her four inherited houses and any other house in Ames, Iowa.


## Hypothesis and how to validate?
* Property Size Impact: My theory posits that the bigger a property is, the more it should fetch in the market. To test this, I'll analyze the relationship between house size metrics and their sale prices.

* Importance of Quality and Condition: I believe that the quality and condition of a house greatly affect its market value. Higher quality ratings, like those for the kitchen or the overall construction, should correlate with higher prices. I'll verify this by examining how these quality indicators relate to the sale price.

* Age and Renovation Influence: My assumption is that a property's age and any recent renovations play a crucial role in determining its value. I intend to investigate this by looking at the construction year, any recent remodels, and how these factors influence the property’s market value.

## The rationale to map the business requirements to the Data Visualisations and ML tasks

* For Business Requirement 1 (BR1): Focusing on Data Visualization and Correlation Analysis
   
   * I plan to delve into the sale prices in our dataset by creating histograms to visualize their distribution. This will provide a clearer understanding of the price range and spread.

   *  I'll conduct a detailed correlation analysis between various house attributes and their sale prices. This involves computing both Pearson and Spearman correlations to grasp both linear and rank correlations.

   * To further clarify these relationships, I'll graphically represent the key variables in relation to the sale prices of the houses, demonstrating how they are interconnected.

   * A dedicated notebook for correlation study will cover all aspects of this business requirement.

* For Business Requirement 2 (BR2): Implementing Regression Analysis
   
   * Given that our goal is to predict a continuous variable - the sale price, regression analysis will be my primary tool. Should the regression model underperform, I may consider reframing this as a classification challenge.

   * Understanding that not all house attributes equally impact sale price, my objective is to pinpoint those factors that have the most significant influence. Techniques like Principal Component Analysis (PCA) might be employed to identify these key variables.

   * A specialized notebook for modeling and evaluation, titled "Predict House Prices," will be used to fulfill this business requirement.


## ML Business Case

  ### Predict House Sales Price 
   
   #### Regression Model

    * To fulfill our second business requirement (BR2), our plan is to develop a Machine Learning (ML) model.

    * This model's purpose is to assist our client in estimating the sale prices of four specific inherited properties, as well as for any other comparable properties.

    * We've chosen to employ a regression model for this task, as our primary variable of interest – the sale price – is a numeric value

    * This task will be handled as a supervised learning problem focusing on a single dimension.
    
         * Our objective is to provide the client with valuable insights into the characteristics of houses that can potentially enhance their sale value. We've set specific performance targets for the model: achieving a minimum R2 score of 0.75 in both training and testing phases.

         * A prediction accuracy drop below 75% for any individual property will be considered a failure of the model. 

    * The model's output will be the projected sale price in U.S. dollars, based on the relevant house attributes.

    * The client has provided data on four inherited properties, and our model will predict both individual and cumulative sale prices for these.

        * Additionally, the model will support real-time predictions for other properties, allowing users to input key features for immediate price estimates. This dual functionality caters to the client’s current and future property valuation needs.

    * To avoid the potential inaccuracies of heuristic valuations, we are adopting a data-driven approach. The client’s local real estate knowledge may not accurately reflect the property values in Ames, Iowa, hence the reliance on a more analytical approach.
    * Our model, named 'HousePriceIssue' (House Price Issues), will utilize a public dataset from Ames, Iowa. This dataset comprises around 1,500 property listings with 22 features. During the data preparation phase, we'll exclude variables with significant missing data. Our focus will be on the 'SalePrice' as the target variable, with all other relevant features included in the analysis.    


## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other items that your dashboard library supports.
* Eventually, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but eventually you needed to use another plot type)



## Unfixed Bugs
* You will need to mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a big variable to consider, paucity of time and difficulty understanding implementation is not valid reason to leave bugs unfixed.

## Deployment
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. At the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.

## Main Data Analysis and Machine Learning Libraries
* Here you should list the libraries you used in the project and provide example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* In case you would like to thank the people that provided support through this project.

