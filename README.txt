VCF2PopTree is a client-side software written in Javascript and it runs
purely within the user’s computer/browser.  VCF2PopTree is compatible
with all population browsers including Chrome, Opera, Edge and Firefox
and works equally efficient in Mac, Windows and Linux (Ubuntu). 
Furthermore, it displays the tree in a mobile phone (iPhone and Android)
if the input file size is small.

CITATION: Subramanian, S., Ramasamy, U. and Chen, D. (2019). 
VCF2PopTree: a client-side software to construct population phylogeny
from genome-wide SNPs.  Peer J. x:yy.

INSTALLATION Since this is a client-side software, VCF2PopTree.html has
to be downloaded to the local computer as “Download Zip” from the github
server (https://github.com/sansubs/vcf2pop) or could be cloned to run on
the desktop.  To run the program a simple double click on
VCF2PopTree.html link will result in opening the program in the default
web browser.

FEATURES

Reading a VCF file The main web page of VCF2PopTree has three major
sections.  First section primarily performs file reading and pairwise
distance calculations.  VCF2PopTree reads VCF or compressed (gzipped)
VCF files by selecting appropriate radio button.  The user has options
to filter SNPs based on quality (Phred) scores and depth of coverage.
The threshold values have to be entered before loading the input file.
If the user changes the threshold values, the input file has to be 
reloaded again.  After the input file is chosen a progress bar is 
displayed to inform whether the file is being read or the pairwise 
distance is being calculated.  Once the above steps are completed the 
distance matrix is kept in the memory and hence users now could use the 
matrix to construct and draw trees and display pairwise distances in 
MEGA/PHYLIP format or the tree in the newick (parenthetical) format. 
An alert window will show up if correct VCF files formats are not 
selected.

Options available The phylogeny could be inferred using all genomes or
only a set of selected genomes (at least four) by entering the names in
the text area, which appears only if the latter option is selected.  Note 
that at least four genomes are required to build a tree.  If no names are 
entered in the text area for genome selection the program will use all 
genomes.  Incorrect names (including spellings) of genomes will invoke a 
windows alert.  The program calculates genetic and drift distances (please 
refer the publication for details) upon choosing the relevant radio buttons.  
Pairwise matrices could be calculated using the number of differences, 
p-distance or with Jukes-Cantor correction. This is achieved by checking 
the relevant radio buttons and the genome size has to be provided in the 
textbox to compute p- and JC distances - fail enter this will in result 
in the invocation of a warning alert window.  The textbox will appear only 
if p- or JC distances are selected.

There are two radio buttons to infer phylogenetic relationship between
populations using UPGMA and Neighbour-Joining algorithms and the latter
method produces an unrooted tree.  Two more radio buttons are provided
to draw the phylogenetic tree in a rectangular or circular style.  Apart
from drawing trees VCF2PopTree also produces the tree file in the
popular newick format by checking the radio button “Newick format”. 
Finally, this program produces pairwise diversity matrix in the popular
MEGA and PHYLIP formats and the last two radio buttons should be used
for this purpose respectively.

Display Once the relevant radio buttons are checked and information are
entered in the text areas/boxes the red button Draw should be clicked
and this will result in the display of the tree or text area containing
pairwise divergences or the newick tree beneath the button.  These
displays can be redrawn multiple times by changing different options
without reading the input file as the pairwise distance matrix has
already been stored in the memory.

Test VCF file To examine the functionality of the software we obtained a
compressed VCF file (test.vcf.gz) from the Simons Genome Diversity
Project containing about half a million SNPs from ten human populations
(Mallick et al. 2016 Nature).

