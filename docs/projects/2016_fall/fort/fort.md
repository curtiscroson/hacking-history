# Hacking into Food Sustainability’s Event Horizon

>Having never given much thought to the nature of food sustainability, I had a simple definition in mind of what it was: being able to continuously grow enough food to, across time, feed an expanding population. As I began my internet search for organizations involved with food sustainability, I soon realized that the subject was a universe unto itself. The task seemed beyond daunting and impossible for one person to research and present a meaningful synopsis of the concept of hacking into food sustainability within the confines of an undergraduate term paper. A monograph seemed more appropriate. On the positive side, there is no shortage of literature regarding food sustainability. An online search of the University of South Florida library revealed well over 200,000 academic, peer reviewed and trade journal publications on food sustainability and sustainable agriculture: this included both domestic and foreign publications. The obstacles I immediately ran into were definition, scope, expertise, sourcing, and data extraction. For the undergraduate researcher or data hacker, each of these obstacles must be considered, planned for, and addressed before and during research or data mining. My plan of action in investigating the, for me, unknown country of “food sustainability” was to explore the general (defining it) and uncover the specifics based on the content of the various definitions. This approach was not overly cumbersome nor problematic and after several long and short definitions were examined I gained an appreciable understanding of the vastness of the food sustainability concept.

### What is Food Sustainability?
  
Organizations involved in food sustainability are both governmental and nongovernment organizations (NGOs). Federal and state institutions, private agricultural advocacy and research organizations are, upon an initial internet search, numerous and globally represented. Their characterizations of food sustainability are as diverse and plentiful as the variety of organizations concerned with food sustainability. Also, the terms “food sustainability” and “sustainable agriculture” are sometimes used interchangeably. Some definitions are brief while others are quite extensive. For example, in the United States, GRACE Communications Foundation, a food sustainability advocacy group, has the following definition: “In simplest terms, sustainable agriculture is the production of food, fiber, or other plant or animal products using farming techniques that protect the environment, public health, human communities, and animal welfare.  This form of agriculture enables us to produce healthful food without compromising future generations' ability to do the same."  As food sustainability is a global concern, it behooves the researcher consider global sources. Similar in sentiment but opposite in length to GRACE Communication’s definition, the city government of Calgary, Canada has a definition that consumes an entire page. It can be accessed online at http://www.calgary.ca/CA/cmo/Pages/Definition-of-a-Sustainable-Food-System.aspx. These and other definitions of food sustainability open the door to the complexities of the food sustainability concept. Elements that comprise the definitions—farming, environment, pest control, disease, production, transport, and animal welfare, among others—can be their own topic of extensive research and data collection. 

### Scope

Once an awareness of the broad scope of food sustainability is established, a narrow focus is required before embarking upon hacking data resources. For instance, if agricultural pests and diseases are an area of interest the choice should be narrowed to pests or disease. Either one is time consuming to research. Furthermore, if, for example, agricultural pests are the focus, it quickly becomes apparent that the type of crop infested also needs to be narrowed to something like citrus or grain crops. Finally, if citrus crops are chosen, what type? The need to have a particularly narrow focus extends to all topics regarding food sustainability. Once a topic’s data has been sufficiently hacked, cleaned, and presented another topic can be tackled and when done perhaps combined or measured against the previous topic’s data to look for connections and correlations. If possible, concurrent research and data mining should be a group effort because of the huge amount of data available on most subtopics of food sustainability.

### Expertise

Expertise or familiarity with language and concepts pertaining to a topic can be problematic for researches outside of disciplines that generate much of the data being accessed. Using the previous example of crop pests, much of the terminology is difficult for a non-entomologist to comprehend and slows the research and data collection as a dictionary is frequently consulted. The same is true for many arcane words and terms associated with farming, livestock, environmental, disease, and other topics under food sustainability. This complicates understanding and utilizing tables and spreadsheets found on websites and in databases. The risk is that valuable but difficult to interpret data will not be utilized.

### Data

As I have not attempted to scrape any of the many websites that I have encountered due to time constraints, I don’t believe that it would be much of a problem for someone with the basic skills and tools such as Web Scraper to scrape the sites. While searching websites for data, I noticed that many of them, NGOs and government, seemed to have a love affair, understandably, with formatting their tables, text, and other data in pdf format. This was a problem since some of the sites that I accessed were using image based pdfs which I could not manipulate or extract the table from. However, the U.S. Department of Agriculture (USDA) is a data rich resource with lots of data available for download in csv format . There is one caveat, however, to utilizing the USDA website; it’s huge and requires hours (I spent about 4 hrs. on it) just getting familiar with what data is available from the various agencies that have data relevant to food sustainability. A good example is USDA’s National Agricultural Statistics Service (NASS); it has, at this time, 34,092,503 records. The good news is that when you find relevant data you’ve hit pay dirt (no agricultural pun intended here). Notably, the Research, Education, and Economics Information System (REEIS) of the USDA is loaded with Excel files. I was curious about federal research and education support to state food sustainability initiatives and stumbled upon REEIS while trying to learn my way around USDA online resources . Here is the link for Florida’s REEIS data: https://portal.nifa.usda.gov/lmd5/bix_reportlet/show_public/state_snapshots_funding_mechanism_hierarchy?i[year][selected_member]=2014&i[state][selected_member]=Florida. On this REEIS webpage, charts and visualizations with selectable data parameters for funding sources and years are provided. The visualizations are basic but the data can be downloaded in Excel files, allowing one to use a visualization tool such as Tableau to craft a different visualization with the downloaded data or combine other data with it to render a different take on the visualization. 
	There are also a range of government and NGO institutions in Florida that focus on the state’s food sustainability initiatives. Many of them use USDA data resources and are recipients of USDA grants. However, when available, most their own data is in pdf format.  The Sustainable Agriculture Research and Education Program (SARE) is one such institution and is worth looking into. They support “farmers, researchers, educators, non-profits, community based organizations and community activists in the agricultural community.” 

### Methods

In becoming acquainted with the food sustainability concept, my primary tool was the internet. For this reason, I highly recommend, regardless of research topic, a solid understanding of internet research basics. For instance:
* Use the minus operator (-) to narrow the search. It’s a not symbol used to exclude unwanted results. For example, Atlas -inc removes inc from search   results, avoiding including businesses with Atlas in their name.
* Use the plus operator (+) to include certain words in the search results.
* Use quotation marks around desired exact words or phrases.
* Omit common terms like a and the. They are stop words that are usually ignored. 

These are only a few search tips that I remember without digging through my notes but, nonetheless, cutting down on useless search results streamlines the search process. Naturally, a good understanding of the university online library system is required to track down scholarship on desired topics. 
 I previously mentioned my problem with extracting tables from pdfs. I do have a work-around that yielded some results. Having an annual ($15.00 I think it was) subscription to Adobe, I converted the pdfs to Word documents then transferred the tables to Excel, fixed any irregularities, then saved them as xlsx files. Before that, I tried using Tabula, a tool for extracting tables from pdfs, but it seemed to get confused, unable to interpret the column and row structure, or just generally scrambled the entire table, not to mention being slow sometimes.  
### Scholarship
I purposely placed this section near the end of my paper because I found scholarly information on food sustainability but none on this paper’s topic—hacking food sustainability.
In regards to food sustainability scholarship, an online search of the University of South Florida library showed extensive literature on food sustainability and sustainable agriculture. This is good if, besides mining data, one wanted to learn about these subjects. To illustrate, a basic search limited to peer reviewed publications published since 1980, in English, and in the United States yielded 2,568 publications. Using the same search criteria for sustainable agriculture yielded 6,034 publications.  While scanning the listing of books and journals I notice the broad interdisciplinary nature of food sustainability. Each of the following disciplines were represented among the approximately 100 titles that I scanned:

* Anthropology
* Agriscience and Technology
* Agribusiness Management
* Agroecology
* Biology
* Ecology
* Education
* Environmental Science
* Entomology
* Psychology
* Sociology

Keep in mind that these are not the total of disciplines involved in food sustainability; it’s only what I noticed—a sample. However, I found no related historiography on the subjects. For the researcher intending to use data hacking skills, the extensive scholarship combined with government and NGO data resources contain a wealth of information to work with. Unsurprisingly, I found no literature and historiography related specifically to data mining food sustainability. This will change in the years ahead. For now, those who have begun, and will begin, hacking into food sustainability are and will be the pioneers of this endeavor. 



### Closing Remarks

I have developed a keen interest in all aspects of food sustainability. The many issues involved with feeding an always expanding global population are complex and urgent. Food sustainability is by nature an interdisciplinary field of study and practice. The varied conceptions of food sustainability complicate research because of varying perspectives, data incompatibilities, discipline specific language, the need to be extremely focused in topic research, and the immense magnitude of internet accessible data. In addition, one must be aware of the many disciplines within and outside of academia involved with food sustainability. Food sustainability within the context of data hacking is, because of its importance and data rich nature, for undergraduates enrolled in courses teaching data mining skills, a worthwhile semester long project. Once past the initial fog—the event horizon—surrounding the food sustainability concept, you are sucked into, much like a cosmic black hole, an immensely data dense environment. This work must be pursued to discover the many undiscovered connections and correlations that hacking can reveal. I think that giving careful thought to data from sources outside of food sustainability and looking at possible influences or connections holds promise as a hacking methodology. Something as simple as a data visualization using USDA or NGO data tied into immigration and population trends could shed light on the origins of problems or previously unseen problem solutions.
 Food sustainability is not a recent concern. For early humans, hunting a prey species into near extinction or extinction was a food sustainability issue. Native Americans who long ago burned clearings to recycle nutrients and grow crops then rotate to a new clearing while letting the previous one replenish soil nutrients practiced food sustainability. What is new about food sustainability is the computational power to amass previously unheard of amounts of data and sift relevance and meaning from it.



##### Sources

1 GRACE Communications Foundation, “Sustainable Agriculture - The Basics,” GRACE Communications Foundation, sec. Sustainable Agriculture, accessed December 5, 2016,
http://www.calgary.ca/CA/cmo/Pages/Definition-of-a-Sustainable-Food-System.aspx


2  “U.S. Department of Agriculture,” sec. Home, accessed December 8, 2016, http://www.usda.gov/wps/portal/usda/usdahome.

3 “REEIS Home | REEIS,” Home, accessed December 8, 2016, https://reeis.usda.gov/.

4 “Southern SARE,” Home, accessed December 8, 2016, http://www.southernsare.org/.











