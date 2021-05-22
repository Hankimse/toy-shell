# toy-shell
자동차IT융합 20163364 김세한

My code is compiled in Linux

char* USERNAME=getenv("USER");  // getenv searches for the environment string pointed to by name and returns the associated value to the string

char HOSTNAME[1000];  // Declare strings in array form

gethostname(HOSTNAME, 999); // gethostname returns the null-terminated hostname in the character array name

char cwd[1000]; // Declare strings in array form

getcwd(cwd, sizeof(cwd)); // The getcwdfuction copies an absolute pathname of the current working directory

printf("%s@%s%s$", USERNAME, HOSTNAME, cwd);
