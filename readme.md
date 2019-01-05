# LASER - [**L**]c3 [**AS**]sembl[**ER**]

## Description

An assembler for the LC3 written entirely in C. I've been trying to move away from LC3Edit provided by my university, which is old and hurts my eyes, and an assembler was the last thing I needed LC3Edit for.

### Motivation

The completion of this tool allows me to do everything LC3-related from VSCode, my editor of choice. Or it would, except that I've already finished the course and am just using this project to practice my C coding. Hopefully someone down the line will appreciate my efforts in creating a command line LC3 assembler. All in all, this is a wonderful learning experience and I look forward to next semester!

### Usage

Laser is a command line tool, and is relatively simple one at that. Here is how to use it after installation on your system:

```
	laser usage:
		-v to display version number
		-h to display this message again
		-a followed by a file name to generate a loadable OBJ file
		-c followed by a file name to remove all files generated by '-a'
```
You can use the command `laser -a *.asm` or `laser -c *.asm` to assemble or clean all assembly files in a directory. This is particularly handy when dealing with your own service routines or data that needs to be assembled and loaded separately from the main program.

## Building from Source

Please read the notice below explaining what has and has not yet been completed. If you would like to try out the parts that have been completed, here are the steps to building on Mac, Linux, or MINGW:

1. Clone this repository: `git clone https://github.com/PaperFanz/laser.git`
2. `cd laser/src`
3. `make`
4. `sudo make install` (if you want to use it without selecting the directory and using ./laser)

## Notice

The base features of this project are now complete, and the functions listed above in the Usage section are entirely useable. If there are any issues with the assembler (specifically if it hangs, throws an exception, or crashes) please create an issue and I will deal with it ASAP.

I am also planning to slightly extend the features of LC3 Assembly by adding a .ALIAS pseudo-op. This pseudo-op would allow you to create aliases for words, with the intention being that you would alias a register to be able to keep track of it almost like a variable name.

~~NOTE: This project is not yet complete. Here are the things that still need to be implemented:~~

1. ~~Generating the symbol table~~	Completed 12/21/2018
2. ~~Generating the binary file~~	Completed 1/3/2019
3. ~~Generating the hex file~~		Completed 1/3/2019
4. ~~Generating the list file~~		Completed 1/3/2019
5. ~~Error checking~~				Completed 1/4/2019
6. ~~Generating the object file~~	Completed 1/4/2019

~~I've got a lot of work to do.~~ Good thing winter break is forever.