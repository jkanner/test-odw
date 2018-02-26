
# Notes to use Docker for Open Data Workshop 1

From a terminal window:

 * Pull an image of a machine loaded with pycbc and parts of LALSuite (6 GB download!)
 * Start the docker container
 * Install gwpy using pip
 * Clone the tutorials for the workshop
 * Start a Jupyter Notebook server
 
```
docker pull pycbc/pycbc-el7:v1.9.2  
docker run -it -p 8888:8888 --name pycbc_test pycbc/pycbc-el7:v1.9.2 /bin/bash -l
pip install gwpy
git clone https://github.com/jkanner/test-odw.git
jupyter notebook --ip 0.0.0.0
```

If you are prompted to "Accepting one-time-token-authenticated connection from 127.0.0.1",
you will need to type `A` for "Always", and then `Q` for Quit

```
A
Q
```

Then, copy and paste the displayed URL into your browswer to access the notebook server.


