  ### Building riskxvii-vm from Source

# Linux

Dependencies: `gcc, make`

```shell
cd RISKXVII-VM/examples
chmod 755 *
cd RISKXVII/include
chmod 755 *
cd RISKXVII/src
chmod 755 *
make
sudo make install
# alternatively, move the compiled binary to your preferred location
```

# Windows

```shell
cd RISKXVII/src
# invoke the version of make installed on your system
# add the resulting 'laser.exe' to your windows path
```

# Mac OSX

Dependencies: `xcode command line tools`

```shell
xcode-select --install
cd RISKXVII/src
make
sudo make install
# alternatively, move the compiled binary to your preferred location
```
## commands

    -v: 'riskxvii -v' displays version number
    -h: 'riskxvii -h' displays this message again
    -q: 'riskxvii -q' suppresses all warning messages during assembly
    -s: 'riskxvii -s' suppresses all warnings and errors during assembly
    -a: 'riskxvii -a <file>' assembles the specified file
        'riskxvii -a *.asm' assembles all assembly files in current directory
    -p: 'riskxvii -p <file1> <file2>' assembles the specified files as a project
        'riskxvii -p *.asm' assembles all files in current directory as a project
    -c: 'riskxvii -c <file>' removes all files generated during assembly