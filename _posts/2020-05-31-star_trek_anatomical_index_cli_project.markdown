---
layout: post
title:      "Star Trek Anatomical Index CLI Project "
date:       2020-05-31 19:53:35 -0400
permalink:  star_trek_anatomical_index_cli_project
---


For my project I decided to pull from a Star Trek API that contains a list of all the species in the Star Trek franchise, with each species containing an internal list of specific information, such as homeworld, home quadrant, and several physiological attributes. 

At first I decided that I wanted to have two different search parameters: one through which the use could search for species by first entering a letter to bring up an alphabetical list of every species whose name starts with that letter, and then from that list, the user could choose an index number for a species to learn the rest of the information. Aside from home world and home quadrant, all of the physiological attributes are listed as true or false (not boolean values, just strings), so I initially thought that I would like to have the index return only "true" values, but after testing, that list ended up being pretty short for some species that didn't have many true values. For the sake of having a fuller looking index, I made the decision to return all of the physiological attributes and then answer each with true or false. This task on its own seemed daunting initially, so I cut my goals down to having just this singular search index. After completing it, however, I decided I did want to put the extra work in to include the secondary search option by quadrant.

Because quadrant and homeworld all had unique values (as opposed to true vs false), and also because some didn't have listed information for one or both, I had to write that code a little differently, so it returned the unique response for each query or a "no information" answer if there was no information. This was actually a lot easier than I anticipated and I'm glad I made the decision to include this in my code. It also presents the option of further building on this project in the future to incude other distinct search parameters, such as searching for every species that returns "true" on a specific physiological attribute, etc. I expect I will develop this further for my portfolio before I start looking for jobs.

I also decided for the fun of it and for the sake of a nicer looking menu to experiment with using ASCII, which turned out to be very easy. All I had to do was create a class for the ASCII and then call on it in my menu method.

After completing my project, I realized that this API is a little old and doesn't include all up-to-date information for the entire franchise, which is unfortunate, but doesnt affect the quality of the code or the functionality of my project.

In all, I'm very happy with this project and how it turned out and feel that I learned a lot from building it from scratch. 

