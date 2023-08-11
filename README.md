# #dzdt (or, can you do geomorphology with ICESat-2?)
Inspired by [this paper](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020EA001538), our team spent time investigating whether ICESat-2 products like ATL06 are suitable for topographic change detection at high latitudes. Originally, we wanted to create a cloud-based workflow where a user can (1) query a region over a permafrost landscape with an AOI, (2) divide data into seasonal (intra-year) and multiannual, end-of-summer time chunks and (3) compute ICESat-2-derived surface subsidence/uplift from crossovers/repeat tracks for the timeframe of interest. This workflow would reveal both seasonal freezing and thawing of the active layer as well as any permanent topographic change associated with thaw-driven erosion (slumps etc). Ideally ArcticDEM and/or visible imagery can be used as a basemap in an interactive map that shows the results. 

## Outcomes

1. Repeat ground tracks and ground track crossovers are rare below ~69 degrees N latitude (see map below)
2. Even when we filtered the dataset to try to look at only snow-free days, height differences for points that fell within the instrument's footprint (~7 m) collected only a few years apart were sometimes on the scale of 10s of centimeters up to ~2 m, which does not seem realistic and implies (1) major instrument-based noise and/or (2) pernicious snowcover effects
3. Collecting pointwise topographic heights from ATL06 tracks from the Michaelides et al 2021 study area (see below) was pretty noisy, and comparing them to ArcticDEM did not reveal systematic errors that made any sense to us

So, our assessment after one week of work seems to be <b> measuring and analyzing topographic change with ICESat-2 is challenging </b>.

## Background

Below is Figure 11 from [Markus et al](https://www.sciencedirect.com/science/article/pii/S0034425716305089). It is an illustration of one day of ICESat-2 orbits. The blue and red orbit sections indicate where the pointing transitions from the polar “repeat-track mode” to “land/vegetation mode”, respectively. The transition regions have been defined for all 1387 ground tracks and can be updated on orbit:
![repeat vs map mode](https://ars.els-cdn.com/content/image/1-s2.0-S0034425716305089-gr11.jpg) 

You can see that most of the land is not in repeat mode but (1) some tracks can overlap and (2) in those red boxes around Beringia, northern Siberia, and the High Canadian Arctic archipelago have many repeat tracks so we might zoom in there!

## Future work 

This tool could be poised to be cross-referenced with the upcoming [OPERA DISP](https://www.jpl.nasa.gov/go/opera/products) product which will provide cloud-based InSAR displacement data for Alaska starting Fall 2024.



## Collaborators on this project
- [Joanmarie Del Vecchio](https://github.com/jmdelvecchio) (**Project Lead**)
- [Matt Olson](https://github.com/mattols)
- [Shashank Bhushan](https://github.com/ShashankBice)
- [Scott Henderson](https://github.com/scottyhq)



## Files

* `.gitignore`
<br> Globally ignored files by `git` for the project.
* `environment.yml`
<br> `conda` environment description needed to run this project.
* `README.md`
<br> Description of the project. [Sample](https://geohackweek.github.io/wiki/github_project_management.html#project-guidelines)

## Folders

### `contributors`
Each team member has it's own folder under contributors, where he/she can
work on their contribution. Having a dedicated folder for one-self helps to 
prevent conflicts when merging with master.

### `notebooks`
Notebooks that are considered delivered results for the project should go in
here.

### `scripts`
Helper utilities that are shared with the team

