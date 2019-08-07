# Fiat-Shamir-prototype
A coding exercise using gawk and shasum to implement and test a cryptographic protocol

    Coding exercise implementing Fiat-Shamir protocol with gawk and
    shasum.

    This was part of a coding test for a job interview.  The key
    aspect here is using existing low level tools to prototype
    and test a small library for some cryptographic protocols.
    More should be done to make this a production version, including 
    making more unit tests and linting the source code.

    Note that awk features are used to implement the testing harness.
    The coding time for this was under a couple of hours, while the debugging
    time took the better part of a working day.


    The scripts are schunit2.txt and schunit3.txt .
    The test files are smtest.txt mdtest.txt lgtest.txt and bgtest.txt .
    To handle both multiprecision arithmetic and dealing with hexadecimal
    use -M and -n options.  To alter DEBUG value to 0 , run an example
    like the following:

    gawk -M -n -f schunit3.txt -v DEBUG=0 smtest.txt

    Note the variable option for DEBUG goes before the input file (test vectors)
    and after the unit test program.  You can also run in default mode as:

    gawk -M -n -f schunit2.txt mdtest.txt

    Copyright 2019 Sheperd Systems.  See License in repository for details
