#Epistemics 
##Factorial Analysis of Personal Epistemology

This is a side-project dealing with high-school students and young graduate adults
'personal epistemologies' (Hofer and Pintrich, 1995). Rather than a set of beliefs, said epistemologies are dealt with
as coherent professional ideologies (Althusser, 1990, 2008), acquired via institutional initiation, after high school. 
A 9-dimensional instrument is constructed on the basis 
of meta-scientific bibliography (Brown, 1993; Hacking, 1983, 1999; Hanson, 1958; Kuhn, 2012; Lakatos, 1980), 
and explored with Principal Components Analysis in young graduate
adults, 12th graders with either humanties or science as a major orientation and 10th graders, without 
specific formal orientation. 

## References
Althusser, L. (1990). Philosophy and the Spontaneous Philosophy of the Scientists & Other Essays. Verso.
Althusser, L. (2008). Ideology and Ideological State Apparatuses.
Brown, H. I. (1993). Perception, Theory, and Commitment: The New Philosophy of Science. University of Chicago Press.
Chalmers, A. F. (1999). What Is This Thing Called Science?. Univ. of Queensland Press.
Hacking, I. (1983). Representing and Intervening: Introductory Topics in the Philosophy of Natural Science. Cambridge University Press.
Hacking, I. (1999). The Social Construction of What?. Harvard University Press.
Hanson, N. R. (1958). Patterns of Discovery: An Inquiry Into the Conceptual Foundations of Science. CUP Archive.
Hofer, B. K., & Pintrich, P. R. (1997). The Development of Epistemological Theories: Beliefs about Knowledge and Knowing and Their Relation to Learning. Review of Educational Research, 67(1), 88–140. doi:10.2307/1170620
Kuhn, T. S. (2012). The Structure of Scientific Revolutions: 50th Anniversary Edition. University of Chicago Press.
Lakatos, I. (1980). Mathematics, Science and Epistemology: Volume 2, Philosophical Papers. Cambridge University Press.


# Data Sets

## Files: Student Data - 'esri_pilot_3.txt' is a tab delimited text file with the following structure:

## gend    gender, m= male, f= female
## year    school-grade, 1=10th gr., 3=12th gr.
## spec    orientation, 1=humanities, 2=science, 3= technology/economics
## 1:117   questionnaire item, see Codebook for more details. 

### These data were collected in classroom, by pen and paper completion and were manually introduced
### into the computer. The printed questionnaire was random ordered. 

## Files: Graduate Data - 'epistemics28.dat' is a tab-delimited text file with the following structure:
##        Age
##        Studies Orientation
##        Level
##        questionnaire item, see Codebook for more details.

## The 1:3 columns are noisy, because participants were allowed to specify their response in a blank field. 
## Note that you may need to enable unicode in order to read greek fonts. These datasets read fine in a 
## Windows 7 64bit system, using R, versions 2.x and 3.x, with a Greek System Locale, 'cp1253' encoding. 
## Greek is the language set for use by 'programs not supporting unicode' in Control Panel/Region and Language/Administrative.

## This data-set was collected online, with a qualtrics free account. The administration was randomized. 
## A .sav file was downloaded from the site and then the above columns were extracted into a dat file. 
## The rest were dropped due to including locations and IP's
## of the respondents.  

######################################################3 esri-key ?????????
######################################################3 esri-items and directions ?????????

# Analysis Overview

## The student data need to be ordered, according to the esri_key object. When ordered, they match
## the order of the graduate data. 

## Both student and graduate data contain reversed items. I.e. items that support the opposite 
## direction than the scale on which they are supposed to load. This information is found in the
## esri_key object

## Subscale information is found in the esri object in the workspace. ##############################33 you will need to change that.

## After these arrangements, the rest of the analysis is pretty straightforward. 

## Item Analysis - classical approach, for each of the 9- suscales, psych::alpha
		## Produce table 1 in Yialloussis(2015)
		
## Principal Component Analysis - unrotated, for adults, FactoMineR::PCA
		## Several plots with FactoMineR::PCA.plot

## Produce the comprehensive correlation matrix in table 2 of Yialloussis(2015)

















