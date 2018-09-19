# Thermo mass spectrometer raw file reading in linux
A repository explaining how to read thermo orbitap mass spectrometry raw files in linux.

### Pre-requisite

1.  Mono installed on ubuntu (Tested on ubuntu 16.04)
2.  Thermo RawFileReader downloaded in your system

### Getting Started

Download the RawFileReader Folder from OneDrive. 
Open the terminal and upzip the RawFileReaderExample.zip file through terminal.

```
unzip RawFileReaderExample.zip
```

Go to RawFileReaderExample File

```
cd RawFileReaderExample
```

The executable file is present in the release folder inside the bin directory.

To read the file execute following command
```
mono bin/Release/ExampleDotNet.exe "PATH TO Raw file"
```

For Example
```
mono bin/Release/ExampleDotNet.exe /home/ubuntu/test.raw 
```

The output can be seen on the console window. 

If you want to store the output in the file, store the STDOUT in a file
```
mono bin/Release/ExampleDotNet.exe "PATH TO RAW FILE" >"PATH TO OUTPUT FILE"

## Example
mono bin/Release/ExampleDotNet.exe /home/ubuntu/test.raw >/home/ubuntu/test_rawfile_output.txt
```
