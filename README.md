# CLIMAIDE
CLImate Modeling Artifical Intelligence assisted Diagnostic Environment

This repository integrates a traditional Fortran-based Global Climate Model (GCM), [ROCKE-3D](https://simplex.giss.nasa.gov/gcm/ROCKE-3D/), with a modern AI research assistant powered by OpenAI models. It enables automated analysis of model code, outputs, documentation, and crash behavior — providing intelligent suggestions and visualizations to accelerate scientific workflows.

## Project Goals

- Build a system that uses LLMs to reason about GCM codebases.
- Automatically summarize and embed Fortran modules and scientific papers.
- Enable GPT to suggest and generate new diagnostics based on existing plots.
- Ingest outputs, documentation, and variable metadata to guide interactive analysis.
- Explore whether AI systems like GPT-4 or o4-mini can act as research collaborators in Earth and planetary science.

## Features

- **Code Parsing & Summarization**: Extracts subroutines/modules from Fortran files and summarizes their function.
- **Retrieval-Augmented Generation (RAG)**: Uses FAISS and OpenAI embeddings to answer user queries based on local code, papers, and documentation.
- **NetCDF Visualization Assistant**: GPT analyzes existing plots and metadata, suggests follow-up plots, and generates matplotlib code to create them.
- **Document & HTML Parsing**: Ingests supplementary resources like Google Docs, ODT files, HTML docs, and variable spreadsheets.
- **Crash Diagnosis Support**: Can be extended to reason over input/output files and known failure modes.

## Requirements

- Python ≥ 3.9
- `openai`, `faiss-cpu`, `xarray`, `matplotlib`, `pandas`, `requests`, `fitz` (PyMuPDF), `bs4`
- OpenAI API key

## Project Status
Recently started, in active development.

## Acknowledgments

Special thanks to the ROCKE-3D team for making this groundbreaking model and its documentation available to the community. This project would not be possible without their continued efforts to support open scientific modeling.

## License
MIT – fully open source. All outputs and datasets will be freely available, including documentation for reproducibility.
