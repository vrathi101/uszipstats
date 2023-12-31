<h1 align="center">
<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/Logo/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
</h1>

TaxFilingFusion stands as the ultimate solution for effortlessly accessing and navigating IRS tax filing data. This powerful package effortlessly transforms complexity into simplicity, empowering users to unlock fresh insights and delve deep into data analysis. Unravel the potential of tax data like never before – whether you're an expert or just starting out, TaxFilingFusion makes IRS data accessible and user-friendly for all.

Call for Contributions
----------------------
It provides:
- sophisticated functions
- a powerful connection between tax filing data and the American geography
- an API with a backend of BigQuery to allow user manipulation of data

Detailed Package Info
----------------------
This Python package provides access to individual income tax statistics for various zip codes using data obtained from the IRS. The data spans the years between 2015 and 2020, and each year's data may have a different format as some attributes may be dropped in certain years, while new attributes may be added. 
The data is ingested into Google BigQuery, where all individual year tables are combined into a single comprehensive table. To enrich the ZipCode data and provide more detailed information, the package utilizes crosswalk files from HUD USPS, which establish links between ZIP codes, state FIPS codes, county FIPS codes, and city FIPS codes. This enriched data allows users to obtain additional details about each ZIP code, such as county, state, region, and other associated information.
Several views, table query functions, and single-valued functions are implemented to support various data needs for the API. These functions are designed to expose the combined and enriched data for public access. By leveraging these APIs, we have created a beautiful and easy-to-use PyPI package that allows the public to interact with and analyze the IRS individual income tax statistics for different ZIP codes, enriched with valuable geographic information.

Call for Contributions
----------------------

The TaxFilingFusion project welcomes everyone's passions, thoughts, ideas, and contributions.

Small improvements or fixes are greatly appreciated. 
If you have any questions, please email: vedrathi10@gmail.com

Our GitHub repository may be small and much simpler than what you would expect of a full-fledged package like NumPy,
but our goal is to continue adding new features to make this data even more accessible for users.
To help contribute to our project, you can:
- review the code and create pull requests via forking the repo
- develop tutorials, presentations, and other educational materials
- help with outreach and publicity


Package Usage
----------------------
To download the package on a command-line interface, run:
    `pip install taxfilingfusion`
<br>  
To download the package on Jupyter Notebooks or IPython environments, run:
    `!pip install taxfilingfusion`
<br>  
To upgrade the package version (CLI), run: 
    `pip install taxfilingfusion --upgrade`.
<br>
To use the functions provided by this package, after downloading, run: 
    `from code_query import irs_data`
<br>
Then a method can be accessed using the dot operator, like:
    `irs_data.{function_name(parameters...)}`
<br>
Refer to [TaxFilingFusion Functions](https://drive.google.com/file/d/1rd2jFGZKyjYnAAWVM4uDio7Oc9cfy8fR/view?usp=sharing) to get a high-level overview of the functions available in this package. 
<br>

Sources
----------------------
- IRS tax filing statistics: https://www.irs.gov/statistics/soi-tax-stats-individual-income-tax-statistics-zip-code-data-soi
- Zip code data crosswalk files: https://www.huduser.gov/portal/datasets/usps_crosswalk.html
