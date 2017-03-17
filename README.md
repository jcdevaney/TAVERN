# TAVERN
TAVERN: Theme And Variation Encodings with Roman Numerals

The TAVERN corpus contains 27 sets of theme and variations (T&V) for piano by Mozart and Beethoven. There are 17 works by Beethoven and 10 by Mozart for a total of 281 Variations (100 from Mozart and 181 from Beethoven). The themes and variations are divided into 1060 phrases (939 major and 121 minor).

In terms of the comprehensiveness of the dataset, these T&Vs represent the near-complete set by Beethoven, with 17 out of 20 represented; and a majority of Mozart T&Vs with 10 out of 17 represented.)



TAVERN consists of three types of files for each musical phrase, stored in respective folders:

‘analysis’ files

‘score’ files

'joined' (analysis+score) files

These files are represented in Humdrum. The "joined" and "analysis" files are represented in duplicate, one for each annotator ("A" and "B"). The analyses contain both Roman numeral analysis as well as functional analysis, following Steven Laitz's "phrase model" and thus represents function at the level of the phrase, as opposed to representing function at the surface level of each individual harmony. It should be acknowledged that at times the phrases had to be "forced" to fit within the phrase model format. 



## File naming convention and organization

Files are stored separately in folders according to composer. Within each composer folder is another set of folders representing each opus that was encoded. Within each opus folder are three more folders with the analysis files ('Encodings'), score files ('Krn'), and analysis+score files ('Joined'). 

Each individual file begins with a letter representing the letter of the composer (B = Beethoven, M = Mozart), followed by a three character opus ID. Works without opus (WoO) start with a zero, while numbered opuses begin with a capital "O". Thus Beethoven's WoO 63 is represented as B063, and Opus 76 is BO76. 

In the "Joined" folder, the remainder of the filename represents the variation number (themes are labelled "00", variation 1 is "01", etc.) the phrase number (starting at 01), content information*1 about the phrase, and a final lowercase letter indicating the annotator. Thus the structure is as follows:

Composer letter+3-character opus number_Variation number_Phrase number + content letter_Annotator.krn

e.g.: BO76_00_01a_a.krn

(*1: since the naming convention merely counts phrases regardless of content, we wanted to indicate phrase similarity by other means, thus lowercase "content" letters indicate melodic relatedness. For example, if phrase 1 and 3 from the first variation of Opus 76 were identical or near-identical in content, they would be represented as: "BO76_01_01a_x.krn and BO76_01_03a_x.krn. However, if each phrase had unrelated melodic content, then the letters in the "content" position should each be unique.)

The "Encodings" and "Krn" folders have a similar naming convention, except that the end of the filename is different to help distinguish them from the "joined" files. Score files only have one representation and end with "score.krn" while the analysis files are stored in two different subfolders for each annotator and filenames end with "encoderX.krn" (where X is either A or B). 


## Other Files

In addition to this readme file and the data files themselves, there is also a csv file called "var_info" which includes the total number of major to minor phrases in each opus, the opus number and title, and the number of phrases in each variation and their respective keys.




