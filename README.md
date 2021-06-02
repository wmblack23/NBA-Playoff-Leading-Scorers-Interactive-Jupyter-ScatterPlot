# NBA-All-Time-Playoff-Leading-Scorers

## Playoff Points Leaders.ipynb
With this file, we access all of our NBA Playoff Points stats using the NBA API.

We call the playerinfo API and create a DataFrame with basic player info, and then we use all ~5000 player_id's from this DataFrame to retrieve postseason information from the careerstats API.

We make around ~5k calls to this API.  When we have succesfully got the data we want for every player who has ever played in an NBA Playoff game into a dictionary, we then convert it into a DataFrame and save it as an Excel sheet.  This way, we don't have to run this code again, as the ~5k API calls takes some time.

## Playoff Leaders with Excel file.ipynb
For this code we simply load the Excel file from the first program (I have it included it here: 'Playoff DataFrame.xlsx') and graph it.

> We use the magic command %matplotlib notebook to create an **interactive scatter plot within our Jupyter Notebook**.  What this allows us to do is zoom in on various subsets of our graph to better view dense clusters of data.  Examples included.

> We also use a mplcursors function which allows us to **retrieve data from any point on the graph simply by hovering our cursor over top of it**.  When we do so, we see the name of the player, their rank on the All-Time Playoff scoring list, and the number of playoff points they have scored.  When we zoom in using the live notebook features, we are still able to use our cursor to gather information.

You can use this .ipynb file and the Excel file to try it yourself.

Enjoy!

*Michael Black*
