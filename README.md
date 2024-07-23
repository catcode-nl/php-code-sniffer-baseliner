# PHP Code Sniffer Baseliner

A project that can be used to add a `// phpcs:ignoreFile baseline` statement to php and phtml files.    
The goal of this project is to not force the user that adds a new phpcs rule towards the ruleset, to have to adjust all 
existing code.  
To make sure the new code rules are still being added to the existing code a pre commit hook can be added that reminds 
the developer which edits a file if the baseline marker is still there, and that it should be removed.  

## How to use

When the phpcs command is installed, the following command can be executed to add the ignoreFile statement to all files 
with issues.  
```
./vendor/catcode-nl/php-code-sniffer-baseliner/bin/phpcs-baseliner
```

When it is preferred to have an ignoreFile statement in all php/phtml files in a given folder, the following command 
can be used:  
```
./vendor/catcode-nl/php-code-sniffer-baseliner/bin/phpcs-baseliner ./src
```
The `./src` in above command can be replaced with any folder that is required.
