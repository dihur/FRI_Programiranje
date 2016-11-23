# FRI_Programiranje
Repository for test cases for programs from homework and sharing programs after homework due date.

### Table of Contents
**[Structure of test cases](#structure of test cases)**
**[Getting test cases](#getting test cases)**  
**[Installing Git](#installing git)**  
**[Testing](#testing)**    
**[Authors](#authors)**  
**[License](#license)** 

#Structure of test cases
First 10 test cases are public test cases from task and then follows N custom test.
They are usually corner cases and huge test that test lower bounds and upper bound of program.
And in between there are some normal cases so that we can check results by hand.

##Getting test cases

###Non-git way

If you are not using git you can get whole repository by clicking clone or download button and then download zip.
See picture below for explanation.
![alt text][downloadZIP]
If you have some previus folders with test cases and want to download only one(current) directory from repository you must:
1. Copy link from current directory
![alt text][copyLink]
2. Go to this page [DownGit](https://minhaskamal.github.io/DownGit/#/home "DownGit's Homepage")
3. Copy link in field
4. Click download

###Using git

If you don't have git installed first look at the section [Installing Git](#installing git).
When you set up your git you can clone this repository to your local computer with this command:
'''bash
git clone https://github.com/RokKos/FRI_Programiranje.git
'''
Then you can go in repository by:
'''bash
cd FRI_Programiranje/
'''
To get new test cases from server run this comand:
'''bash
git pull origin master
'''
And now you can run commands from section  [Testing](#testing).

##Installing Git

###On Linux

If you’re on Fedora for example, you can use yum:
'''bash
sudo yum install git-all
'''
If you’re on a Debian-based distribution like Ubuntu, try apt-get:
'''bash
sudo apt-get install git-all
'''

###On Windows or Mac
There is special GUI Tool for this two OS on this link [GitHub Desktop](https://desktop.github.com/ "GitHub Desktop's Homepage").
There is also documentation for this GUI on this link [GitHub Desktop documentation](https://help.github.com/desktop/ "GitHub Desktop's Documentation")

Here are [official instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git "Installing Git") for installing git on each OS 


##Testing
You can test on all test cases by runnig this comand:
*On Linux
'''bash
./tj.exe DNxx_yyyyyyyy.java DNxx_customTesti/ rezultati/
'''
*On Windows
'''bash
tj DNxx_yyyyyyyy.java DNxx_customTesti/ rezultati/
'''
*On Mac
'''bash
mono tj.exe DNxx_yyyyyyyy.java DNxx_customTesti/ rezultati/
'''
Where xx is number of task and yyyyyyyy your Vpisna number. 

There are also other options like:
*run only one test case
'''bash
./tj.exe DNxx_yyyyyyyy.java DNxx_customTesti/ rezultati/ -p 15
'''
*run one range of test cases
'''bash
./tj.exe DNxx_yyyyyyyy.java DNxx_customTesti/ rezultati/ -p 15-20
'''
This command also work on Windows and Mac.

## Authors

* **RokKos** - [RokKos](https://github.com/RokKos)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


[downloadZIP]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"
[copyLink]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"
