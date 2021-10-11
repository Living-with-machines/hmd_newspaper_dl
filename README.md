
# hmd_download
> Bulk download Heritage Made Digital digitised newspapers from the British Library Research Repository 


This tool is intended to make it easy to bulk download [Heritage Made Digital Newspapers](https://bl.iro.bl.uk/collections/353c908d-b495-4413-b047-87236d2573e3?utf8=%E2%9C%93&sort=score+desc%2C+system_create_dtsi+desc&per_page=100&locale=en) from the [British Library](https://www.bl.uk/) [Research Repository](https://bl.iro.bl.uk/). 

## Install

```bash
git clone https://github.com/Living-with-machines/hmd_newspaper_dl
```
and then use pip install inside a virtual environment:

```bash
pip install -e .
```

## How to use

If you use pip install like this you will also have made available a console script `hmd_download`:

    usage: hmd_download [-h] [--n_threads N_THREADS] [--subset SUBSET] save_dir
    
    Download HMD newspaper from iro to `save_dir` using `n_threads`
    
    positional arguments:
      save_dir               Output Directory
    
    optional arguments:
      -h, --help             show this help message and exit
      --n_threads N_THREADS  Number threads to use (default: 8)
      --subset SUBSET        Download subset of HMD

