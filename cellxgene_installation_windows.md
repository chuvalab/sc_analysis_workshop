### How to install and use cellxgene (tested on a Windows 10 machine)
* You need to install Python 3.7. Download the executalble from [here](https://www.python.org/ftp/python/3.7.2/python-3.7.2-amd64.exe)
* Follow the instructions in [this webpage](https://www.digitalocean.com/community/tutorials/install-python-windows-10). When it comes to the Python version installed, use the previously downloaded file
* After instalation is completed, open Windows PowerShell and type `pip install cellxgene`
* During the installation process, you might get this error message: `botocore 1.31.27 has requirement urllib3<1.27,>=1.25.4, but you'll have urllib3 2.0.4 which is incompatible.`. To resolve it, type ` pip install "urllib3==1.25.4"` in PowerShell 
* Go to the directory where `tyser.h5ad` is stored by typing something like `cd c:/Users/my_name/Downloads/Workshop`
* Type `cellxgene launch tyser.h5ad`
* Open the provided url in your browser. Do NOT close the PowerShell window!
