# P.S.Its easy.

Start Server 

`docker run --rm -d --name ps-its-easy --network <some-network> -v <absolute-path-to-this-repo>:/root rust:alpine /bin/sh ~/entrypoint.sh`  
_Note: Alternatively, you can expose the port instead of using --network, if you don't have a reverse proxy_  
  
For enabling ssh access to the container:  
1. Change the public key in .ssh/authorized_keys, you can generate new ones by using `ssh-keygen -f filename -t ecdsa` on any linux system  
2. If you don't have a reverse proxy, you should expose and map the port 22 of the container to the host using `-p ` in the `docker run` command  
3. ssh using `ssh <path-to-private-key> root@<host-path> -p <port-mapped-in-host>`  
_Note: If you are a new contributor to the official site at psitseasy.ml, please get the ssh keys from another maintainer_
  
A web application to display and browse Practice school stations and its chronicles in a easy to use web interface.

# How to use?
- Go to the website <>, and log in with BITS mail ID. (We had to use Google log in as we letting Allotment details of students on the open internet dint seem like the best idea, so its only to identify user as a BITSIAN, we dont take any other information)

# Features
- See last 4 years CGPA trends for all stations in a intuitive boxplot graph, with search and CGPA fiters.
(The source of the data used was the crowd sourced information collected after PS2 allotment  from 2017 to 2020)

- Browse chronicles of last 4 years (2017-2020) with a few clicks and know first-hand accounts of people's experiences .
(SOURCE:official PS chronicles )
- coming soon - download the latest Project bank from a few clicks into an CSV form. (CSV compatible with PS companion extension)


# Screenshots









# Disclaimer

- The data used in the Boxplots were crowdsourced and thus it doesnt account for every student's entry.
 - Aggregation of Stations for chronicles was done using fuzzy techniques, so please be aware of the names.
 
 
# Contribute
 - We do need volunteers to help maintain this project over the years, 
 as it needs data to be fed in every 6 months as the new PS cycle commences,
  thus we welcome contributors that can help in the same. 
  If this project helped you or your friends please consider contributing.
 - if you have ideas for new features, please consider contributing. 
 
 
 
 
 
 
 __Made with <3 by Tan and Jonny__
 
