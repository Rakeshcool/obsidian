- set -x  ## stands for debug mode
- ps -ef ## -ef give details of process in full format
- ps  -ef | grep "amazon" ##grep is used to get specific sentence output in this case we are using amazon as keyword
- awk : used to filter out something specific



ps -ef | grep rakesh | awk -F" " '{print $2}' 

###input:
UID        PID  PPID  C STIME TTY          TIME CMD
root         1     0  0 15:07 ?        00:00:00 /init
root        53     1  0 15:14 ?        00:00:00 /init
root        54    53  0 15:14 ?        00:00:00 /init
rakesh      55    54  0 15:14 pts/0    00:00:00 -bash
rakesh     167    55  0 16:37 pts/0    00:00:00 ps -ef

##output:
55
168
169
170

### this awk command is going to help us get the specific column of the statement and print is process id in this example is the row number 



