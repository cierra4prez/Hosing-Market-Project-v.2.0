{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# King County Housing Prices\n",
    "\n",
    "## Overview\n",
    "\n",
    "This project seeks to develop a model in order to predict housing prices in King County, Seattle. Model and findings are based on the file `'kc_house_data_test_features.csv'`, which is a dataframe of houses sold within the past 10 years in King County, Seattle.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Business Problem\n",
    "We will explore the following business questions:\n",
    "\n",
    "- How much does the number of bedrooms and bathrooms determine the selling price of a house?\n",
    "\n",
    "- How does the condition of a house determine selling price?\n",
    "\n",
    "- How does the age of a house determine selling price?\n",
    "\n",
    "- How does the square footage determine selling price?\n",
    "\n",
    "- How does the renovation of a house influence the selling price?"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "![heatmap](./Resources/heatmap.png)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Analysis\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "A first look at an initial heatmap of our features shows us which features have meaningful correlations with one another. We can see that the variables with the strongest correlation to `price` are the square footage of the living space (`sqft_living`), building construction rating (`grade`), and the neighbors' interior living space (`sqft_living15`). \n",
    "\n",
    "New features have been added in order to find additional relationships to enhance the model. Added features which have had the most influence on the final model include binning `condition` into 2 distinct categories (`condition2_1`), the the number of `bathrooms`, and also the square footage of the 15 closest neighbor's homes in comparison to the house sold (`neighbors_compared`)  "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Findings\n",
    "\n",
    "\n",
    "We can deduce that the highest selling homes are large houses in neighborhoods with other large homes, and where a high level of attention is paid to construction.\n",
    "\n",
    "I was particularly suprised that a property's view, building construction rating, and the number of bedrooms were fairly weak indicators of price. With so many outliers, we may need additional information in order to better fit our model. "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Next Steps\n",
    "I would like to take a closer look at outliers more closely in order to bin categories to keep the model more streamlined. I would also seek outside sources such as information on school districts records of parks and local attractions"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.6.9"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 4
}
