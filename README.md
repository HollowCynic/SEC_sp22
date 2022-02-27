# SEC_sp22

Description: 
This bash program allows the user to quickly look up the top and latest stories from Hackernews.com in their terminal. Moreover, one can also use the program to search for stories with keywords and open the story in the browser to view it in full.

Utility/Justification:
Hackernews is a widely used resource for pertinent news in computer science and cybersecurity fields. For an average user, this program streamlines the searching experience by allowing the user to find stories without having to go to the website. For cybersecurity professionals, it can be used to quickly and periodically (using cron) check for top stories relating to a company, exploit, or any other job-related topic. Stories and their URLs can also be saved by redirecting the output (>) to a text file. 

Who would use this?:
Cybersecurity professionals or regular users who want to more easily track up to date cybersecurity news.

How to use:
By simpling executing ./hn, the program will prompt the user to look up top or new stories or look for a story with a keyword in the title. Next, the program will prompt the user on how many stories they want. Finally, the program will ask the user if they want to open any of the stories in their browser.

Using the flag -t followed by a number will return the top stories up to the provided number.

Using the flag -n followed by a number will return the newest stories up to the provided number.

Using the flag -s followed by a word and a number (in quotes) will get top stories with the keyword in the title. Additionally, adding the word “date” as a third argument will get the newest stories with the keyword. Ex: ./hn -s “microsoft 10 date” Output: 10 newest stories with Microsoft in the title.

The -o (open) flag must be the first flag provided and must be provided with other flags (t, n, s). It will prompt the user if they would like to open any of the searched stories in their browser.

Using the -h (help) flag will print the description and options of the program.
