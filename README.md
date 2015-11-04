# remove_poorqualityreads
This python script was written to follow on from replace_lowqualitybases (https://github.com/cdmarsden/replace_lowqualitybases/) which is a script that replaces bases in a read with 'N' if they are below a user specified quality score.

It takes a sam file and replaces reads below a user specified length, and reads where more than a user specified proportion of the bases are 'N'. A metrics file detailing what passed and failed is automatically produced.

####Usage
    python remove_lowqualreads.py {INFILE} {OUTFILE} {min read length - integer} {max proportion Ns in read - float e.g. 0.5}
    python remove_lowqualreads.py mysamfile.sam qualitysamfile.sam 55 0.2

####Input file
A sam file is required as input

####Dependancies
remove_poorqualityreads.py was written in python 2.6
