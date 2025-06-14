# DUE-from-zonda

***DUE-from-zonda** is an easy and light-weight DUE so it's not that powerful.*  

## Initialization

Download and Initialize by 
```sh  
git clone https://github.com/zonda-tsai/DUE-from-zonda
bash DUE-from-zonda/initial.sh
```
  
## settings

   - `-reset`     : Reset the DUE  
   - `-uninstall` : Uninstall this DUE
   - `--help`     : Show this README.md

## +
   - `file_name.file_type` : Using the template of that file_type.  

## compile

   - `[arg 1]` : Types. Initial one only provide c and cpp (e.g. -c, -cpp)  
   - `[arg n]` : for n >= 1, you can assign specific files.

## run
   - `-type`, `-char_ins`, `-valgrind` and `-test` can be suffixed at the same time.  
&emsp;// ***Type should always be the first argument after run***  
   - ``run``                 : run all. **It'll include all files in that directory**  
   - ``run -char_ins``       : run with ascii inspector.  
   - ``run -valgrind``       : run with valgrind, memory inspector.  
   - ``run -test``           : run all with testfile. e.g. `./a < a.test`  
   - ``run -type``           : run all the files with that type. e.g. run -c (-test)  
   - ``run executable_file`` : run all assigned executable_file and files prefixed shebang

## clean
   - This can clean by all makefiles. If you want to clean specific type, add `-type` after it

## char_ins
   - ``--help``        : show the usage of char_ins
   - ``--ascii_table`` : show the ascii table (in HEX)  

## tfmanager
   - ``-merge``  : merge all .test file into all.test  
   - ``-divide`` : divide all.test into original .test files  
