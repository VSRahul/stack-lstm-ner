Installation Steps
======================
These steps have been tested on Ubuntu 16.04 and macOS Sierra.
1. Once this repository has been cloned, the cnn/ submodule needs to be synced

  ```bash
  git submodule init
  git submodule update
  ```
2. This will download the required files to cnn directory. Download the C++ library `eigen` which is used by cnn:
  
  ```bash
  cd $HOME
  hg clone https://bitbucket.org/eigen/eigen/
  cd eigen
  ```
  Note: 
3. Now, create a `build` directory and install eigen:
  ```bash
  mkdir build
  cd build
  cmake ..
  ```
4. Run `sudo make install`. This will push the library files to the local include. On Ubuntu 16.04 and macOS Sierra, there are copied to 

  
