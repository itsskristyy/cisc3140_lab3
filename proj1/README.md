## proj1

This project parses structured data of CSV format using AWK, a scripting language commonly used to manipulate data and generate reports. 

The scripts rank records based on scores provided in the dataset, and lists the top 3 cars for certain categories.

Data is stored in `data` folder, maintained by git submodule.


### Dependencies 

You must have the following installed. The linux commands to install necessary packages shown below: 

* GNU AWK
  ```sh
  sudo apt-get update
  sudo apt-get install gawk
  ```
* GNU Make
  ```sh
  sudo apt-get install build-essential
  ```

### Run

To run proj1 make sure you are in the root of the project repository and run `make proj1`. 

To run the code type in this command into terminal:

awk -f proj1/prog.awk data/data.csv > ranking.txt


### Results

Results are stored in a `.txt` document labeled `ranking.txt`, that lists cars by highest points earned to lowest points earned. 

Each entry is ordered by (Car ID, Car Make, Car Model, Total Score).

## Additional feature

The new feature contains the AWK programs that selected the top three cars from the given classes: Racer, Engine, Body*Frame, Mods, Mods*Overall, Car*Overall.
Each are separated and displayed neatly while also being documented well. Each rank for the top three cars are displayed in order as well.
