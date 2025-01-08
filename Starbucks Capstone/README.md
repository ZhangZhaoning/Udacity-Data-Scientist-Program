# Starbucks Offer Optimization

## Project Overview
This project analyzes simulated data mimicking customer behavior on the Starbucks rewards mobile app. The main goal is to combine transactional, demographic, and offer data to determine which demographic groups respond best to which type of offer: BOGO (Buy One Get One Free), discount, or informational. By analyzing customer interactions with these offers, the project aims to predict the most effective offers for specific customer segments to increase customer engagement.

## Data Description
The dataset used in this project consists of three main files:
- `portfolio.json` - containing offer ids and metadata about each offer (duration, type, etc.).
- `profile.json` - demographic data for each customer.
- `transcript.json` - records for transactions, offers received, offers viewed, and offers completed.

## Key Insights
Through exploratory data analysis and visualizations, several patterns were observed:
- Offer completion rates vary significantly across different demographic groups.
- There is a noticeable trend in the effectiveness of different types of offers.
- Demographics such as age and income play significant roles in the likelihood of offer completion.

## Models Used
A RandomForestClassifier was employed to predict the most suitable offer type based on user demographics and past transactional behavior. The model provides predictions on whether a particular type of offer (BOGO, discount, informational) should be sent to a customer.

## Usage
- Explore the analysis and modeling through the Jupyter notebooks included in the repo.
- The notebook can be utilized to experiment with model training, parameter tuning, and performance evaluation.
- 
## Dependencies
This project requires the following libraries:
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

## Known Bugs
No known bugs at this time. However, if you encounter any issues, please report them in the issues section of the repository.

## Author
Zhaoning Zhang

## Acknowledgments
- Data provided by Udacity, based on a simulation of the Starbucks app.
- Starbucks Corporation for dataset provision and project inspiration.
