# IP-Extractor
This a IP extractor tool that can extract IP addresses from text files

This is a Go program that extracts IP addresses from a text file called "input.txt" and writes the unique addresses to a new text file called "output.txt".
The program opens the input file and uses the bufio package to read it line by line. It uses a regular expression to search for IP addresses in each line, which are then added to a map with the key as the IP address and value as true. This is done to avoid duplicate IP addresses.
It then uses the net package's ParseIP function to check if the extracted IP is a valid IP address.
Then it opens the output file and writes the unique IP addresses to it using the fmt package.
The program also has error handling to catch any errors that may occur while opening or creating the input or output file
