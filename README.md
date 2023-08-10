# #dzdt
Inspired by [this paper](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020EA001538), our team will create a cloud-based workflow where a user can (1) query a region over a permafrost landscape with an AOI, (2) divide data into seasonal (intra-year) and multiannual, end-of-summer time chunks and (3) compute ICESat-2-derived surface subsidence/uplift from crossovers/repeat tracks for the timeframe of interest. This workflow would reveal both seasonal freezing and thawing of the active layer as well as any permanent topographic change associated with thaw-driven erosion (slumps etc). Ideally ArcticDEM and/or visible imagery can be used as a basemap in an interactive map that shows the results. This tool would also be poised to be cross-referenced with the upcoming [OPERA DISP](https://www.jpl.nasa.gov/go/opera/products) product which will provide cloud-based InSAR displacement data for Alaska starting Fall 2024.

Below is Figure 11 from [Markus et al](https://www.sciencedirect.com/science/article/pii/S0034425716305089). It is an illustration of one day of ICESat-2 orbits. The blue and red orbit sections indicate where the pointing transitions from the polar “repeat-track mode” to “land/vegetation mode”, respectively. The transition regions have been defined for all 1387 ground tracks and can be updated on orbit:
![repeat vs map mode](https://ars.els-cdn.com/content/image/1-s2.0-S0034425716305089-gr11.jpg) You can see that most of the land is not in repeat mode but (1) some tracks can overlap and (2) in those red boxes around Beringia, northern Siberia, and the High Canadian Arctic archipelago have many repeat tracks so we might zoom in there!

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

