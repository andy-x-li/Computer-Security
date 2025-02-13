# Certificate-Parser

A Python program I wrote that takes a list of websites and retrieves and analyzes their web certificates.

The file `tranco-top-1m.csv` contains the top million most popular websites and orders them by descending popularity. 

The file `Certificate_Parser.py` takes in the csv file and attempts to revieve the web certificates to the top 1000 cites. 

`Certificate_Parser.py` then analyzes these certificates to find: <br>
> **1)** The most common certificate authorities <br>
  **2)** The range of valid certificate times <br>
  **3)** The most common issuer country <br> 
  **4)** Any patterns in CA state/province names <br>
  **5)** The types and most common public keys <br>
  **6)** The key lengths for each type of public keys <br>
  **7)** Any patterns in the associated exponent of public keys <br>
  **8)** The most common signature algorithm <br>
  **9)** Any connections between the number of extensions of a certificate to its webpage or CA <br>
  **10)** The most common organization name for the top 1000 sites and the top 50 sites

To run this code: <br>
> **1)** Create a folder that contains `Certificate_Parser.py` and `tranco-top-1m.csv` <br>
  **2)** Run via cmd line `python3 Certificate_Parser.py`
  
**Note**: *There are comments in the code highlighting which sections answer which problems. Please comment out all other problems besides your problem of interest. If the comments don't specify what to set as x in the for loop (int(row[0]) <= x), please set x as 1000 (x represents how many websites are analyzed starting from the top of the list). Remember to also comment out the corresponding print sections found at the bottom of the code.*

Below is the code run on its current state:

<img width="500" alt="Screen Shot 2023-09-10 at 5 06 05 PM" src="https://github.com/andy-x-li/Certificate-Parser/assets/125074849/b7da97fb-a874-4885-8574-74f718fb3a19"> <br> *The most common organization names for the top 50 websites.*
