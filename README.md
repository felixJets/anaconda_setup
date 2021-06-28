# anaconda_setup

### Install Anaconda and PyCharm in Linux

#### Anaconda
1. Go to [Anaconda Installer](https://www.anaconda.com/products/individual#linux) and download the respective file for your system
2. Calculate the hash and compare it to the hash at [Anaconda installer file hashes](https://docs.anaconda.com/anaconda/install/hashes/)
    ```bash
	 $ sha256sum ~/Downloads/Anaconda3-2021.05-Linux-x86_64.sh
    ```
3. Install with: 
    ```bash
	 $ bash ~/Downloads/Anaconda3-2021.05-Linux-x86_64.sh
    ```
4. View the license terms and continue if you agree 
5. Initialize Anaconda3 if you want to
	* Notice that this changes your default python to the newly installed anaconda-python
	* You can check it with:
	```bash
	$ which python
	/home/felix/anaconda3/bin/python
	```
####  PyCharm

1. Go to [Install Pycharm](https://www.jetbrains.com/help/pycharm/installation-guide.html#standalone) and download the tarball for Linux
2. Calculate the hash and compare it to the hash provided at the download page
    ```
	$ sha256sum ~/Downloads/pycharm-community-2021.1.2.tar.gz
   ```
3. Extract the data to your desired location (/opt is recommended) 
    ```bash
   $ sudo tar -xzf Downloads/pycharm-community-2021.1.2.tar.gz -C /opt/
    ```
4. Go to the new bin directory and start PyCharm
     ```bash
	$ cd /opt/pycharm-community-2021.1.2/bin/
	/opt/pycharm-community-2021.1.2/bin$ sh pycharm.sh
	```
5. To conveniently start Pycharm per terminal, you can add an alias to your .bashrc file at your home directory
   ```bash
   alias pycharm="sh /opt/pycharm-community-2021.1.2/bin/pycharm.sh"
   ```
   and then simply start it with:
   ```bash
   $ pycharm
   ```
