# Web-Design-Challenge

Okay got around not being able to add the index.html by adding a notebook and changing it to index.html

I had a technical difficulty with this assignment in that none of the GitLab lessons, days 1 to 3, didn't have anything in them. Typically there are 10 to 15 assignments for each of the days, but all of these were marked down with a '=========' and nothing else.
Did not impact any of the other lessons, but I could not stash and delete the currupted files on my end and then re-pull, since git said that it was already up to date. I went thru line by line to make sure that my conda had the correct installations, both base(the default and my PythonData) had everything that I needed. GitLab was the same, each one of the lessons was marked down with those slashes, so I reached out to my class and support classmates thru slack, no resolution there.
I was forced to watch the zoom videos to have a reference point for the creation of the website and that is not nearly as efficent as just being able to read. 

The issue has been resolved, but it came this afternoon. So I am still working on this and will resubmit as soon as it is something that resembles the requirements.

So I have a few days to revisit this and fully intend to finish the necessary updates, fully understand why the central grader gave the comments that they did, it looks as though I did not update the remote to even a fraction of what I have in my local repository,
I mean, to be sure, a lot of this is going to be trashed outright or salvage maybe 2 or 3 lines of code that get incorporated into the final push but still surprising to see the differential. I pushed it all since I am just now getting my bearings again on this topic 
and cant definitaviely say one way or the other if something is going to have long term value or not. To the larger scope of the project, the issues that I was experiencing earlier with the python challenge and the mars scrapping challenges, knock on wood, seem to have disappeared. Even if I don't consider myself to be fatalistic, I have a certain expectation that by simply calling the 'all clear' status outloud will,
undoubtedly turn the gaze of Olympus upon my endeverors and bring forth long term issues for my completion of this project.

I say, let it be thus.

Okay but seriously, if we stop using a latin text script placeholder for future content, ill stop pontificating old testiment style. Things to do, populate the 4 charts as the instructions specify, they're all static it seems, derived from a csv. Second step is to find a dataset that will server the purposes of the bonus challenge, Google's datasearch had a really interesting analysis of online datsets using dataset search, published in part, as a dataset (link) https://www.kaggle.com/googleai/dataset-search-metadata-for-datasets,
I was tempted to go with it based off the summary report article I read, the kaggle metadataset is actually 11.43 GB so that snuffed out that idea rather quickly, even if it meta-ness made the idea appealing, think I'll go with a water quality dataset, sort of fits the theme of the suggested data which was weather.

So I need the header element for the 4 suggested charts, with a dropdown element that selects the charts, a comparison of X chart to Y chart element in the header, and a data element which looks just to be an individual summary of each of the four.
All four seem to require a summary paragraph and so will need to do that for the other 4 charts as well.

Got the charts made, found a somewhat similar dataset that looked at social and economic indicators of cities all over the globe, its 257 so about half the size of the weather data, same concept really, just look at latitudes effect on a variety of indicators, which I know
is going to have some correlation just because of the disparities between the global north and the global south, not going to try to incorporate it all into one dataset, besides city name and lat lng values there really is nothing in common between the two sets in terms of other columns. This dataset comes from Orhan Karaman's 'City Quality of Life Dataset' found on Kaggle, link("https://www.kaggle.com/orhankaramancode/city-quality-of-life-dataset"). Its about 20 years more uptodate then the weather one listed in the resources, 
this one being published less then a year ago and the time stamps from the  weather one seem to be early 2000's. Got all the Charts to run as in a jupyter notebook, exported the png's and uploaded the notebook. 

Got a bit of the way thru the index.html, got an icon, a name of the site situated on the left, and on the right of the header are the 'data','comparisonss', and three drop down menus, 'latitude weather plots', 'latitude social plots', and 'latitude economic plots'.

Okay so I figured out why my index would work but the rest of my duitfully created various plots, turns out it was that the bootstrap.css was in the base folder, as was the index10.html, which was also in there, so when I would live load the landingpage, which was all the index10 was, it would naturally load.
What I hadn't figured out was that the visualizations pages, all of the various htmls that I was told to create, like the data, comparisons and the other tabs, were nested in the visualizations folder. 
I couldn't navigate to them on click like I was supposed to be able to because they had the wrong reference point. Life lesson learned.

I put the bootstrap css folder in the correct folder, and  went thru all of the href links and added to the front of every one of them a ./example.html inside the quotes, and it liked that.
On load of any page, I would be able to navigate to another page. great. 
This also solved all of my headscratchting as to why none of the dutifully created, and hopefully appreciated to you dear grader at central, the plots in the theme of the rest of the web page. so the text is in the correct color and the numbers of of x and y's and because they are all scatter
the points are in the correct color, ie the secondary theme color of the package that I went with which is 'Morph' a Bootswatch template, but they say that you just call it like a bootstrap template but I figured I would give credit where credit is due. 

From there it was just a bunch of corrections, to make sure that it loaded on a small screen I checked thru my phone and it does, and then I went back and pruned the rest of the indexing system so that the working directory is a lot cleaner.
I also realized that I was using the div class row function too spairingly when looking at the templates, each of the comparison charts are supposed to load one on left and one on right
but because it thought that it was all in the same row they were printing over one another. Got that fixed, 
and then I had to go back and make sure that the header was being called correctly in each of the pages, and that the links would work. they all do although I am having some trouble with the dropdown links still, to no avail.

Im going to publish and resubmit the pages to githubpages and ask the tutor or ta about why my drop down menus won't load, other than that its a pretty functional website and looks pretty nice.
