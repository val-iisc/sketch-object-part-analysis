# sketch-object-part-analysis

The documentation below pertains to the approach presented in our ACMMM-2016 paper for analyzing part importance of category-epitomes, 
a novel visual representation for sketches developed by us. 

Project Page : http://val.serc.iisc.ernet.in/eotd/epipartviz/

You can access our ACMMM-2016 paper 'Analyzing structural characteristics of object category representations from their semantic-part distributions' [here.](https://arxiv.org/abs/1509.04399)

Our ACMMM-2015 paper which introduces category-epitome, 'Eye of the Dragon : Exploring discriminatively minimalist sketch-based abstractions for object categories' can be accessed [here.](http://val.serc.iisc.ernet.in/eotd-preprint.pdf)

### Citation

Please cite our paper in your publications if you use our dataset or if it helps your research.
		
      @article{DBLP:journals/corr/Sarvadevabhatla15b,
      author    = {Ravi Kiran Sarvadevabhatla and R. Venkatesh Babu},
      title     = {Analyzing structural characteristics of object category representations from their semantic-part distributions},
      journal   = {CoRR},
      volume    = {abs/1509.04399},
      year      = {2015},
      url       = {http://arxiv.org/abs/1509.04399},
      timestamp = {Thu, 01 Oct 2015 14:28:48 +0200},
      biburl    = {http://dblp.uni-trier.de/rec/bib/journals/corr/Sarvadevabhatla15b},
      bibsource = {dblp computer science bibliography, http://dblp.org}
      }

### Instructions for running (MATLAB) code 

To obtain the relative importance of semantic-parts in a given category, assuming a particular sketch stroke order, run the following MATLAB script: 

```bash
get_epitome_part_stats_driver
```
Modify the above script by following the comments in the corresponding .m file (get_epitome_part_stats_driver.m)

To obtain a numerical characterization of semantic-part distribution histogram for a given sketch stroke ordering, run  part_distribution_stats.m

Example :
```bash
part_distribution_stats('results','temporal')
```
### Additional information and Datasets 

annotated-final : This is the directory containing the final set of sketch part contour annotations for the 13 object categories-original

results : This directory contains the per-category histogram of relative part importances for different sketch stroke orderings

160-pp/annotated-images : This directory contains the guideline images used by annotators while annotating sketch part contours

160-pp/categories-original : This directory contains selected object category images from the TU-Berlin sketch database (http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/sketches_png.zip) 

160-pp/categories-part-names : This directory contains part names for each category. It is for these parts that contour annotations are added on a per-object category basis.

Contact Ravi Kiran (ravika@gmail.com) in case you have questions, comments or suggestions.
