#xu_data_qp2
#original data from Yi Xu
#testest test test testest testest
all files in this directory and subdirectory are created and modified during analysis of Xu's original data files from June 2014. The data is collected in his 1997 paper of contextual variation of tones, and is reused for Gauthier et al. 2007 on the SOM of tone learning (machine). 

in summer 2014 I ran preliminary analysis and machine learning on this data, (including time series data mining), but didn't document how the files were generated. 

now in Fall of 2014, I am writing my QP2 and don't know where a lot of files came from. I would begin this documentation on Dec.12, 2014. 

#I have identified three files that are of potential clear use: 
xunorm_new.csv, 
allxu_new.csv ,
allxudn_3speakers.csv. 

#allxu_new.csv
I don't know what is the differences between these; but allxu_new seems like comprehensive file that contains all speakers, each line containing 30 point data for one tone, and attributes columns are added such as speaker, pitch-con id, syllable (#1 or #2), etc. 

#problem with original Xu data files
The annoying thing about original data file is that they all contain an extra line of data in the end which I don't know where did it come from, and they all are in two-syllable format (60 point vectors) that I need to separate into single syllable anyway.

#dec.14,2014
I have made some progress in understanding the version history of these files, and today I put together xu_data_qp2 directory under which i store the data files useful for now. 

note on files: 

#Original files: 
the original files from Xu has two files, one for F0 (3 speakers), one for D1 (3 speakers). In each file, 3 speaker data are stored in 3 tabs of the spreadsheet. (these are named normf0_All3, indicating it contains all 3 speakers in one file).

#Indie files: 
we then separate those three speakers into three files, including normf0_All1_indie, normf0_All2_indie, etc, for speakers 1, 2, etc. 

#problem with these files
is that we have no pitch con, which is added in R in the summer. I need to find a better file (maybe a comprehensive one including all 3 speakers in one-syllable 30 point row-wise format) which may also include other features like tone, pitch_con, etc.
