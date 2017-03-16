### Dockerfile
```
FROM ubuntu:14.04
MAINTAINER Misa Ogura "misa.ogura01@gmail.com"

RUN apt-get -y update && apt-get install -y cowsay fortunes
ENV PATH $PATH:/usr/games/

CMD fortune -a | cowsay
```
-----
### Instruction
1. Pull & run the programme - cow will give you a wise advise
`$ docker run misaogura/wise-cowsay`
```
  _________________________________________
/ "Lines that are parallel meet at        \
| Infinity!" Euclid repeatedly, heatedly, |
| urged.                                  |
|                                         |
| Until he died, and so reached that      |
| vicinity: in it he found that the       |
| damned things diverged.                 |
|                                         |
\ -- Piet Hein                            /
 -----------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

2. Try again for some more wise insights
`$ docker run misaogura/wise-cowsay`

```
 ________________________________________
/ "Home life as we understand it is no   \
| more natural to us than a cage is to a |
| cockatoo."                             |
|                                        |
\ -- George Bernard Shaw                 /
 ----------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```
-----
### Links
- Wise whalesay: https://hub.docker.com/r/misaogura/wise-whalesay/

-----
### Authour
Misa Ogura
