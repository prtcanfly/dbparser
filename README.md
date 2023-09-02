# DBParser
Sort databases with the dbparser.py tool

## BASIC USAGE:
,,,
python dbparse.py -i INPUT_FILE -s SEARCH_TERM
,,,
## EXTRA PARAMETERS:

-o OUTPUTFILE - Default is "dbparse.txt"
-e EXCEPTION - Make exceptions for parsing the database / EXAMPLE: "... -e XBOX" would exclude any results that had XBOX in the line.

### Example:
,,,
python dbparse.py -i gamers.txt -o steamers.txt -e PSN
,,,

This would give you a parsed database of gamers.txt as a file called steamers.txt that only includes Steam profiles,
and specifies that if "PSN" is in the line, not to bring it over to steamers.txt

This could be useful for accounts that have "steam" in the username or email rather than as a signification that it is a Steam profile.

# ENCODING TYPE:

### YOU PROBABLY WONT NEED THIS

Sometimes filetypes are written with different encoding styles. The preset for DBParser is utf-8, but it can be changed in the source code.

It's pretty basic to use, just run encoding_type.py and input the file path. If it's anything other than utf-8; take that encoding type and replace the "utf-8" section in dbparser.py with whatever the output was.
,,,
python encoding_type.py
Enter File Path: [File/Path/Here]

 Encoding: utf-8
,,,
#### But as I said, you probably won't have to do this; as utf-8 is the standard.