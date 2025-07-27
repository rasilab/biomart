# biomaRt Docker Container

This repository contains the Dockerfile for the biomaRt R package container.

## Container Details

- **Base Image**: `ghcr.io/rasilab/r_python:1.3.0`
- **Package Version**: biomaRt 2.54.0 (Bioconductor)
- **Registry**: `ghcr.io/rasilab/biomart`

## Usage

```bash
docker pull ghcr.io/rasilab/biomart:2.54.0
```

## Running the Container

```bash
docker run -it --rm ghcr.io/rasilab/biomart:2.54.0 bash
source activate R
R
```

## Features

- biomaRt R package for accessing BioMart databases
- Configured with Fred Hutch conda proxy
- Installed from bioconda channel

## Building

```bash
docker build -t ghcr.io/rasilab/biomart:2.54.0 .
```