cs-user-updater
#
author: mbranche<br>
this is a script to update user time limits, and reservation maxes on Quali Cloudshell
# 
This script takes a csv file, with the following format:<br>
(header)<br>display_name,username,email,time_limit,res_max,group_1,group_2,group_3,group_4,group_5,group_6,group_7,group_8,group_9,<br>
(data)<br>Matt Branche,mbranche,mbranche@email.com,700,1,Primary group,,,,,,,,,								
#
This will update the user with the above time limit, and reservation max<br>
Time is set as follows:<br>
1-99 = 1-99 hours<br>
100+ = days (increments of hundreds)(ex: 700 = 7 days, 1400 = 14 days)<br>
it then uses the time stated, and converts to minutes, which is how cloudshell stores time limits.<br>
