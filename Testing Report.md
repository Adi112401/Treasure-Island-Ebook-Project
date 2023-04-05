# Testing Report

## Pirate Press

During the first stage, we tested our HTML files on Google Chrome. It was a simple method to easily verify if the text was running correctly, following the defined hierarchy, and if images were properly linked.

After having cleaned most of the manuscript, and after adding links to images and alt-texts, we moved to Pandoc to create epub files, which we tested on Apple Books and Thorium. We noticed the files displayed differently on each, and we kept going back and forth until everything looked as similar as possible on both. One of the main challenges was to create a break after part titles and before all chapter openings. CSS was added to reflect this styling, but only Apple Books was capturing the instructions. After a long time of researching, we finally discovered that the breaks could be easily made in Sigil.

Once we had good results with both readers, we tested on a Kindle device. The font displayed was not the one defined by the CSS, although it used one with the same style. Otherwise, the epub was working perfectly.

Finally, we ran the file through Ace Tester, which reported some serious violations, mostly related to Schema metadata. We fixed the issue using the Access Aide plugin for Sigil. There were other measures we could take to make the epub more accessible, but they seemed out of the scope of this project.