# Code for Triangulating Bird Locations with Microphone Arrays
used in research at the University of New Brunswick

#### Disclaimer: This code was produced with the intent of completing my master's research and, only secondarily, with the intent of sharing. So, though it does work, it has not been raised to any professional or publishable standard (yet). It may require further explanation to be usable in your context. Feel free to reach out; I'm happy to discuss bird triangulation ad nauseam :)

For a brief introduction to what it does, check out [my portfolio site](https://lukemclean-portfolio.vercel.app/projects/triangulation)

### Inputs:
-10 wave files simultaneously recorded with a microphone array  
-csv files (from sonic visualizer) that designate synchronized moments at the beginning and end of recordings  
-a list of microphone gps locations, in the format: [[lat, lon], [lat, lon],...]  
-a [Raven](https://www.ravensoundsoftware.com/) selection table for all the songs on one of the recorders (ideally one with a strong signal)  

### Outputs:
-an array of time lags for each vocalization on each recorder  
-a list of locations (in metres from the centre of the microphone array) for each vocalization  
-a map of song locations  