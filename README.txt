Assumptions:
1. Inputs JSON is enclosed within parenthesis.
The inner paranthesis are added if not provided.

Limitations:
1. If the input JSON object provided to the program does not have " with espace character, integer values of the keys would be considered as Strings.
2. If directory path is not provided for the database to be created, it would be created on the current directory of its run.
3. The log file by default is created from the location where this program is run.


Test Commands:
The following are the different test cases that could be executed:

1. (R)ead a key (1)  
java -jar freshWorksAssess_SK.jar R 1

2. (C)reate a key (1) with json object as provided without escape characters 
java -jar freshWorksAssess_SK.jar C 1 "{"Name":"tom"}"

3. (C)reate a key (2) with json object as provided with escape characters 
java -jar freshWorksAssess_SK.jar C 2 "{\"Name\":\"shiva\",\"place\":\"loc\"}"
 
4. (C)reate the same key (2) with any value  
java -jar freshWorksAssess_SK.jar C 2 "{\"Name\":\"reapeat\",\"place\":\"loc\"}"

5. (D)elete any of the existing key
java -jar freshWorksAssess_SK.jar D 2 




