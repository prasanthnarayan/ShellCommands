# ShellCommands

#Starting a new project Just to keep the Shell commands that might be useful in dat-today activities.


#find the filename containg 'search_text'
#
grep -n 'search_text' <filename>

eg: grep -n 'search_text' *


#find the number of non-whitespace characters in a file

tr -d '[:space:]' <filename.txt |wc -c

Redirection
2>&1

exampe: hive -f <script file> > out_file 2>&1


Find Class in jar files.

for i in *.jar; do jar -tvf "$i" | grep -Hsi ClassName && echo "$i"; done
