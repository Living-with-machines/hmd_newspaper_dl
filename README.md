# hmd_download
> Bulk download Heritage Made Digital digitised newspapers from the British Library Research Repository 


This [command line tool](https://en.wikipedia.org/wiki/Command-line_interface) is intended to make it easy to bulk download [Heritage Made Digital Newspapers](https://bl.iro.bl.uk/collections/353c908d-b495-4413-b047-87236d2573e3?utf8=%E2%9C%93&sort=score+desc%2C+system_create_dtsi+desc&per_page=100&locale=en) from the [British Library](https://www.bl.uk/) [Research Repository](https://bl.iro.bl.uk/). 

The tool has been used by Living with Machines but may be of use to other people. Since the tool is intended to download the collection in 'bulk' it is likely to be useful if you either want:
- all HMD newspapers 
- a random sample i.e. 10 newspaper

This tool was developed for internal use so it might not be suitable for your needs. If you have problems or suggestions with the tool please [open an issue](https://github.com/Living-with-machines/hmd_newspaper_dl/issues/new/choose). 

## Install

The tool was developed using `nbdev` so although all of the code for this tool lives inside a single Jupyter notebook you can still install it as a Python package. At the moment this is done via GitHub:

```bash
python -m pip install git+https://github.com/Living-with-machines/hmd_newspaper_dl
```

It is recommened to install the package insdide a virtual environment. Since this is a command line tool one simple option for installing is [pipx](https://pypa.github.io/pipx/) which will install the tool inside a new virtual environment for you:

```bash
pipx install git+https://github.com/Living-with-machines/hmd_newspaper_dl
```

## How to use

Once you have installed the packaghe you will also have made available a console script `hmd_download`:

    usage: hmd_download [-h] [--n_threads N_THREADS] [--subset SUBSET] save_dir
    
    Download HMD newspaper from iro to `save_dir` using `n_threads`
    
    positional arguments:
      save_dir               Output Directory
    
    optional arguments:
      -h, --help             show this help message and exit
      --n_threads N_THREADS  Number threads to use (default: 8)
      --subset SUBSET        Download subset of HMD


This will by default download all available newspaper titles. If you just want a subset you can pass in a subset parameter to specify how many titles you want. At the moment this is just a random selection. 

## Feedback 

This tool was put together for internal Living with Machines but is shared in case it is helpful for other people. If you have feedback, problems or want to suggest changes please open a [new issue](https://github.com/Living-with-machines/hmd_newspaper_dl/issues/new/choose). 
