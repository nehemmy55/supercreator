script that make directory and then create number of file you want inside your directory 



#!/bin/bash

read -p "please enter name of ur dir " dir 
mkdir $dir

cd $dir
read -p "enter number of file " filenum
counter=0
while [[ counter -le filenum ]]
do 
     touch "file$counter.txt"
     ((counter++))
done
