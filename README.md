This was part of the Latent Space hackathon. 

The impetus was to solve for someone navigating the Latent Space podcast for the first time and celebrate their 1 year anniversary. For a new listener, it is difficult to know where to start or what is most relevant. 
Someone can go chronolocially, search for subjects, or explore the substack, but it is hard to fully wrap your head around all the content out there

The live demo can be seen here - https://app.flow.gl/flow/sz77u9r
This link will work in all browsers on computers, mobile, and AR/VR headsets (except Vision pro until Safari gets their WebXR act together)

Please note that not all of the data processed correctly so there are bugs on many of the episode summaries etc. I used Flow as that is what I'm most familiar with as it was my most recent startup. 

The process for this hack was 

1. Consuming the RSS feed
2. Parsing the releveant data including the link to the .mp3 and image assets
3. Seperating out the transcript, chapters, and other information in the RSS feed
4. Removing html and timestamps from the transcript
5. Running each full transcript to GPT-4-Turbo to have a large enough context window for the full episode.
6. Using AI to summarize each episode, assigning categories (based upon what was in the Substack), identifying quotes with timestamps, and highlighting key insights

Using the result, I put the data into Flow a.flow.gl to visualize and make it interactive. 
I created a 12 vertex shape to be a representation of the categories covered
Each vertex acts as a center of gravity pulling a dot (episode) closer to it
So the 3d structure acts as a sort of guide on what the episode is most likely to be about.

Not perfect, but was a fun side project.

Sharing the code I created to do this as the resulting full .csv contains quite a lot of good information. There were bugs etc, but open to anyone else jumping onboard here to take it further.

