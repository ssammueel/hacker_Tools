# dirb

- is a cmd ool that automates the process of discovering hidden files and directories on a website.
- websites tend to hide pages that may not be linked from the main site, sensitive files that should not be publicly accessible, but can be acessed if one knew the url
- here is where dirb comes in place it works by sending a series of requests to the website, each with a different word or phrase as the requested URL.
- after it shows the url that can be aceed in this manner

example 

![Image](https://github.com/user-attachments/assets/f9f0bf7f-d50d-4296-8963-b8c711bbdc99)

in this we have used the default wordlist /usr/share/dirb/wordlists/common.txt

you can olso use alternative wordlists

      dirb <target url> wordlist path

most commonly used options include:

‘-r’: to recursively scan subdirectories
‘-o’: to specify an output file for storing the results
‘-c’: to specify the number of concurrent connections to use
‘-w’: to ignore warnings
‘-a’: to specify the user-agent string
‘-f’: to force the use of a specific HTTP method (GET or POST)
‘-u’: to specify the username and password for basic authentication.
