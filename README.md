narrative-clip-hacks
====================

#hack 1 - rename files to maintain order when making a timelapse

1. hack 1 - since the narrative clip as of 26 march 2014, splits up files into 1 directory per day and reuses file names in different directories, to maintain the order you need to rename the files in the other directories, hence rename-starting-with.py
2. so find the last file name in day 1 and rename day 2 and day 3
3. e.g. if the last file name on march 25 is: 000999.jpg then 

        cd day march26; ./rename-starting-with-py 1000  #(no need for leading zeros, rename-starting-with-py will add leading zeroes to the filename to maintain sort order)

5. then symbolically link these files into day 1 and then make your timelapse!
6. code to sort files copied (thanks) from: http://stackoverflow.com/questions/12093940/reading-files-in-a-particular-order-in-python
