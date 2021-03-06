# Installation Options and Troubleshooting

## Install with pip

Make sure you have Python installed, then run:

```bash
pip install mxnet-model-server
```

If you're upgrading from a previous version of MMS, use the following:

```bash
pip install -U mxnet-model-server
```

## Install from Source

Alternatively, you may clone MMS from source:

```bash
git clone https://github.com/awslabs/mxnet-model-server.git && cd mxnet-model-server
```

Then using the following will install from source:
```bash
pip install .
```

Or use the following to upgrade from source:
```bash
pip install -U .
```

## Development Installation

If you plan to develop with MMS and change some of the source, then use the `-e` option.
Then using the following will install from source and make your changes executable:

```bash
pip install -e .
```

Or use the following to upgrade from source and make your changes executable:
```bash
pip install -U -e .
```

## Installation Troubleshooting

| Issue | Platform | Solution |
|---|---|---|
| Could not find "protoc" executable! | Ubuntu: | `sudo apt-get install protobuf-compiler libprotoc-dev` |
|   | MacOS: | `conda install -c conda-forge protobuf` |
| Missing [LibGFortran](https://gcc.gnu.org/onlinedocs/gfc-internals/LibGFortran.html) library | Ubuntu: | `apt-get install libgfortran3` |
|   | Amazon Linux: | `yum install gcc-gfortran` |
