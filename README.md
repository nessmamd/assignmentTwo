# assignmentTwo
HOW TO RUN THE PROGRAM
1. Create the container named assigment1: 
  - docker build -t assignment1 .
2. Check if it was created by using this command, if it has been created assignment1 should show up, if not run step one once more.
  - Docker image ls
4. Create the respective volume and run the container
  - docker run -it -v servervol:/serverdata assignment1:latest
5. Test it once more or twice or however many more times by doing the following: 
  - docker run -it -v servervol:/serverdata assignment1:latest /bin/bash
  - cd /serverdata
      - cat random.txt
        - if no data shows up then go cd ../ then python text_gen.py and then repeat the prev two steps again
      - data should show up, then go cd../ then python text_gen.py to overwrite the file and start over again repeating the previous steps 



