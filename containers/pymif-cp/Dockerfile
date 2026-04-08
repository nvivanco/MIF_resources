FROM condaforge/miniforge3

WORKDIR /app

COPY environment.yml .
COPY pymif-cellpose-env-clean.txt .

# Create environment (use mamba for speed)
RUN mamba env create -f environment.yml && \
    conda clean -a -y

# Use the environment by default
# SHELL ["conda", "run", "-n", "myenv", "/bin/bash", "-c"]

# CMD ["python"]
