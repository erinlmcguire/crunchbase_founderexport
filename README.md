## crunchbase_founderexport
This repo takes a list of company names and pulls the founder names and degrees from Crunchbase.  The end product is two csv files - one with startup names linked to founder names and the other with startup names, founder names, and degrees of the founders. 

The script was written to create data for the analysis in my paper "Can Equity Crowdfunding Mitigate the Gender Gap in Startup Finance?"  In that paper, I investigate whether equity crowdfunding increased financing to female-led startups.  As startup financing data is often proprietary, I used CrunchBase API to create a dataset that includes startup information, founder information, and external financing information.  Using a difference-in-differences, fixed effects model, I find that aggregate external financing received by female firms increased after the US legalization of equity crowdfunding.  Check out the paper [here.](https://drive.google.com/file/d/12mmszX8Vky_AUmXfxCFLiDC7Ht_Wd6bk/view)


## Configuration

-Insert your Crunchbase API key in the notebook.  Crunchbase gives out API keys to approved researchers and you can request one from their site.    
-Export all company names from Crunchbase using their daily csv export. I pulled all the names from the database because I wanted to maximize my sample size, but you can filter by industry or location after you export.     
-Save a csv with all the names of the companies and update the file in the Jupyter notebook.    

## Deployment    
-Install Python 3 using Anaconda or another method.    
-Install Jupyter Notebook.    
-Install the Python requirements with pip install -r requirements.txt.     
-Run the program in Jupyter notebook. Results will be exported to the current working directory.     
