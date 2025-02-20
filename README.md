# Homework 3: Big Data Analysis

The due date is Feb 27 at midnight. Please follow the [code squad rules](https://junwei-lu.github.io/bst236/chapter_syllabus/syllabus/#code-squad). If you are using the late days, please note in the head of README.md that “I used XX late days this time, and I have XX days remaining”. 

The main purpose of this homework is to help you:
- Use Hash Table in Python
- Process big data in python
- Process big data in R
- Learn how to visualize and share the results.

## Problem 1: Leetcode for Hash Table and Pandas

Complete the following problems on Leetcode. 
- [Number of good pairs](https://leetcode.com/problems/number-of-good-pairs/)
- [Binary Subarrays With Sum](https://leetcode.com/problems/binary-subarrays-with-sum/)
- [Fill missing data](https://leetcode.com/problems/fill-missing-data/)

Add your code to `leetcode.py` and add a screenshot of the Leetcode submission result to `README.md`. To practice your coding skills, we suggest you try to solve the problems without the help of AI at least for the first attempt.


## Problem 2: Big Data Analysis in Python


- Run `python3 -m pip install -r requirements.txt` and then `python3 createMeasurements.py` to create the data. 
- Write a python script called `calculate_MED_STD.py` that computes (and prints) the median and standard deviation of temperature measurements per station, alphabetically ordered. The program should print out the median and standard deviation values per station, alphabetically ordered like so:
```
{Abha=18.0/10.0, Abidjan=26.0/10.0,..., İzmir=17.9/10.0}
```
Note that all packages needed should be added to the `requirements.txt` file.
- In the `README.md#Report`, report the running time of the program and memory usage. Analyze the bottleneck of your code. Though not required, we encourage you to try different approaches and report how the running time is improved. However, you can only have one `calculate_MED_STD.py` in the root directory of your submission.

## Problem 3: Big Data Analysis in R

- Write R script `calculate_Temp.R` to output the min, mean, and max values per station, alphabetically ordered like so:
```
{Abha=5.0/18.0/27.4, Abidjan=15.7/26.0/34.1, Abéché=12.1/29.4/35.6, Accra=14.7/26.4/33.1, Addis Ababa=2.1/16.0/24.3, Adelaide=4.1/17.3/29.7, ..., İzmir=-33.5/17.9/69.1}
```
Save the output to `result_R.txt`.
You are allowed to use any R packages. Note that all packages needed should be added to the `renv.lock` file. You may also need to upload `renv/activate.R` for the automated checks to pass (note that this is by default added to `.gitignore`). 
- In the `README.md#Report`, report the running time of the program and memory usage. Analyze the bottleneck of your code. Though not required, we encourage you to try different approaches and report how the running time is improved. However, you can only have one `calculate_Temp.R` in the root directory of your submission.

### **Bit Battle** 🎮

Problem 3 is a bit battle event. You need to make your `calculate_Temp.R` as fast as possible. Note that your code will be run on a single core. We will rank based on the running time using the following command:
```bash
start=$(date +%s.%N)
Rscript calculate_Temp.R
end=$(date +%s.%N)
        
runtime=$(echo "$end - $start" | bc)
echo "Rscript calculate_Temp.R ran in ${runtime} seconds."
```


## Problem 4: Interactive Visualization

- Create an interactive webpage to visualize the data.  You can decide what to visualize. One motivating demo example is [GWAS diverse monitor](https://gwasdiversitymonitor.com/). We recommend using AI to help design the visualization. 
- Deploy the webpage on Github. You can add it to your Coding Blog. Add the link to the webpage in the `README.md`.
