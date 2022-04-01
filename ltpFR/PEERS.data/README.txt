This archive contains a contains the behavioral data from the Penn Electrophysiology of Encoding and Retrieval Study (PEERS).

This data has been used in several publications including:

Lohnas, L. J., Polyn, S. M., and Kahana, M. J. Expanding the scope of memory search: Intralist and interlist effects in free recall. Psychological Review. 
Long, N. M., Danoff, M. S., and Kahana, M. J. Recall dynamics reveal the retrieval of emotional context. Psychonomic Bulletin and Review. 
Healey, M. K., Crutchley, P., and Kahana, M. J. (2014). Individual differences in memory search and their relation to intelligence. Journal of Experimental Psychology: General, 143(4), 1553–1569
Healey, M. K. and Kahana, M. J. (2014). Is memory search governed by universal principles or idiosyncratic strategies? Journal of Experimental Psychology: General, 143, 575–596. 
Lohnas, L. J. and Kahana, M. J. (2014). Compound cuing in free recall. Journal of Experimental Psychology: Learning, Memory and Cognition, 40(1), 12-24.
Long, N. M., Burke, J. F., and Kahana, M. J. (2014). Subsequent memory effect in intracranial and scalp eeg. NeuroImage, 84, 488–494.  

Refer to these manuscript for the methods of the experiment, and description of the 
analyses that we carried out on these data.

%%%%%%%%%%%%%%%%%%%

This particular file written by Karl Healey (healeym@sas.upenn.edu) and Nicole Long (niclong@sas.upenn.edu)

(adapted from one by Sean Polyn sean.polyn@vanderbilt.edu)

Send word if you find anything weird or out of sorts with the data, or the explanation of the organization of the data!

Behavioral Toolbox (Release 1) analysis code available from:
http://memory.psych.upenn.edu/behavioral_toolbox

%%%%%%%%%%%%%%%%%%%

A quick tour of the data structure.

%%%%%%%%%%%%%%%%%%%

PEERS_older_adult_subject_list.txt % PEERS includes both younger adult (<35 years of age) and older adult (>60 years of age) participants. This file gives the subject numbers of the older adult participants so analyses can be restricted to one age group or the other.

ltpFR_lsa.mat		% These are the LSA values used for the semantic analyses. This is a matlab format file.

Within the ltpFR directory, there is a subdirectory for each subject in PEERS (e.g. ltpFR/LTP063). Within each subjects directory there is a subdirectory for each of their experimental sessions (e.g., ltpFR/LTP063/session_0). Within each session directory you will find two types of files: .par and .log

.log files record details of every stimuli presented to the subject and can be used to determine which words were presented on each list. Each column gives a different piece of information:
1 - clock time
2 - NA
3 - event type 
4 - list number
5 - word string
6 - word number (corresponds to 1:1638 in word pool)
7 - task 
8 - response
9 - RT


.par files record details of participants vocal responses. 0.par - 15.par are for free recall lists. ffr.par is for the final free recall period. r0.par - r15.par are for the recognition task. Within these files the first column gives the reaction time, in ms relative to the beginning of the recall period. The second column gives item number of the recalled period (corresponds to columns/rows of lsa.mat). The third column gives the word itself.
