# FindImageDupes
# This script will look at images in one folder and report duplicates to a text file
# execute in bash
# specify folder containing all images
folder=(~/dir/dir/)
#specify threshold
val=85%
findimagedupes --recurse --threshold=$val $folder | awk '{ print $0 }' > duplicatefiles85.txt

All of this was made possible by http://www.jhnc.org/findimagedupes/manpage.html 

see also http://www.jhnc.org/findimagedupes/ 
