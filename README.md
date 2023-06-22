# Lexical & Syntax Analysis

improving the lexical analyser in the Sebesta book. The improved version of the lexical analyser is now be able to (i) report errors in the identifiers and integer literals, (ii) Able to recognize assignment operator and certain keywords. 

the lexical analyser in the book is not able to report errors in identifiers and integer literals. Hence, appropriate changes has been made to the state transition diagram and the code to enable the lexical analyser to report the errors. Additionally, the lexical analyser is now able to handle assignment operators and certain keyword. After the latter it is now be able to handle assignment statements and keywords: ‘if’, ‘then’ and ‘else’.

Furthermore a syntax analyser (parser) has been added to it. The syntax analyser will handle expressions described by the EBNF The parser will be based on recursive-descent parsing algorithm and the outline C code for the parser additionally improve it by adding error handling capability. 
To handle the error-handling an error() function has been implemented. This function  reports errors and also indicates what is expected by the parser in case a wrong token is found at the input.
