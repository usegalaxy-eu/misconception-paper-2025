# Scripts and Data associated Galaxy Misconception Paper 2025

This repository includes all the scripts written to produce figures in the paper along with the resulted figures

## Requirements

- Install [conda](https://conda.io/miniconda.html)

    ```
    $ make install-conda
    ```

- Create the conda environment

    ```
    $ make create-env
    ```

## Usage

- Launch [Jupyter](https://jupyter.org/) to access the notebooks to generate graphs

    ```
    $ make run-jupyter
    ```

- Go to [http://localhost:8888](http://localhost:8888) (a page should open automatically in your browser)
- Open 
    - `explore_publications.ipynb` to retrieve publications and citations
    - `extract_tool_changes.ipynb` to retrieve tool updates on Galaxy Europe

        Before running the notebook, a GitHub token needs to be provided by creating a `.env` file and filling it like with:

        ```
        GITHUB_TOKEN="<your_github_token>"
        ```

    
    - `plot_usegalaxy_stats.ipynb` to plot the number of distinct users and jobs per month on the EU, ORG, and AUS servers
