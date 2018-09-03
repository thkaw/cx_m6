# build
docker build -t cx_m6 .

# run
docker run -v /home/nathan/cx/codebase/imx6_android_M6.0.1_2.1.0-ga/:/var/aosp6/ -i -t --name cx_m6_01 cx_m6 bash

# resume
docker start -i -a cx_m6_01 

# remove
docker container rm cx_m6_01 
