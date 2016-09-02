# df-para-plot
## About
Ever had x-y-Data in a Dataframe that you wanted to plot depending on different columns
df-para-plot is a wrapper around matplotlib doing exaktly that. You can specify
* a column as parameter for line color
* a column as parameter for data marker
* a column as parameter for linestyle
df-para-plot will handle everything else for you

## Usage

Currently consits of a single function:

pplot(df, x=None, y=None, marker=None, linestyle=None, color=None)

parameters are:
 *  df: the pandas dataframe containing the data
 *  x: The column containing the x-values for the plot. if nothing is specified, index column will be used
 *  y: the column containing the y-values. If nothing is specified, the first column will be used.
       maybe in furture update: plotting all possible columns in different subplots
 *  color : the column containing the parameter for the linecolor
 *  marker : the column containing the paramter for the marker
 *  linestyle : the column containing the paramter for the linestyle
 *  **kwdargs : additional arguments are getting passed to matplotlib.pyplot.plot directly

## Future Plans
  * Modficiable Style iterators
  * subplotting for multiple data columns
  * possibilty to submitted axes to use

