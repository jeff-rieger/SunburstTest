# SunburstTest
Attempting to get a sunburst chart working

The CSV
There are 3 CSV files in there - one that is extremely simple; one that is a representation of the branch depth but only has the main branches as labels (so the branches are like `Apparel-Apparel-Apparel-end` instead of `Apparel-BootsShoes-HikingBoots-end`); and one CSV where it has the actual branch names broken out, as in `Apparel-BootsShoes-HikingBoots-end`
The extremely simple CSV has fake counts.
The other 2 CSV’s have real counts of keywords per branch as of the DE-KERFFULER today.

It would seem that the `sequences.js` code will figure out how many child nodes root back to a parent node, and sum up the count of child nodes, so parent nodes are always bigger. This is of course necessary where the first branch of `Apparel` has a small number of keywords, but the 3rd and 4th branches have far more keywords.
