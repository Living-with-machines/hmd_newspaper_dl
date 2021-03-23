# hmd newspaper dl
> # TODO


# TODO

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

```
!hmd_download -h
```

    usage: hmd_download [-h] [--n_threads N_THREADS] [--subset SUBSET] save_dir
    
    Download HMD newspaper from iro to `save_dir` using `n_threads`
    
    positional arguments:
      save_dir              Output Directory
    
    optional arguments:
      -h, --help            show this help message and exit
      --n_threads N_THREADS
                            Number threads to use (default: 8)
      --subset SUBSET       Download subset of HMD

