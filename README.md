# CSDA-1050
Final Project

1)   Kijiji-Scraper.py   is the scraper 

2)   main.py   in this code, I called the scraper and pass over the parameters, to create txt files.  
       Including:  
                      kijiji_GTA.txt (any types of rental AD in GTA);
                      kijiji_GTA_basement.txt  (basement rental AD in GTA);
                      kijiji_GTA_apt.txt       (apartment)
                      kijiji_GTA_house.txt   (house)
                      kijiji_GTA_one_bed.txt    (one bed room)
                      kijiji_GTA_two_bed.txt     (two bed room)
3)  Convert_CSV.py  I converted the text files into csv files with new separators (&=), removed empty lines (\n), add rent unite type as a new column ;
4)  read_csv.py   I read all the csv files, append them into a big df, then dropped the duplicates based on first column (AD_ID), then save into a new csv: data_all_test;
5)  Insert_Table.py  This is the code I wrote to upload the csv values up to google cloud table (postgres).  This is the code I wrote for the second class, so it might not work with the new csv file I generated on 4).  I will debug it when I get time.
6) data_all_test.csv is the final csv file I generated on file 4) read_csv.py.   In the end I have 7561 AD, not as many as I thought.
