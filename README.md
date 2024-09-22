# DVC ML Pipeline Demo for AIOps

This project implements a machine learning pipeline using Data Version Control (DVC) to manage datasets and experiments effectively. The workflow consists of several key steps to set up a reproducible environment for machine learning tasks.

## Workflow Steps

1. **Create a Remote Repository**: 
   - An empty remote repository is created on GitHub to store the project.

2. **Initialize a Git Local Repository**: 
   - A new local Git repository is initialized, and a README file is created.
   - The local repository is connected to the remote repository, and the initial commit is pushed to the main branch.

3. **Set Up Environment**: 
   - A Conda environment named `dvc-ml` is created and activated to manage dependencies.

4. **Create a Setup File**: 
   - A `setup.py` file is generated to define the package metadata and dependencies, including DVC, pandas, and scikit-learn.

5. **Create Requirements File**: 
   - A `requirements.txt` file is created to list the project dependencies, and they are installed.

6. **Initialize DVC**: 
   - The DVC tool is initialized in the project, enabling version control for datasets and machine learning models.

7. **Create Directory Structure**: 
   - A basic directory structure is established, including directories for source code (`src`), utilities (`utils`), and configuration files (`config`).

8. **Create Configuration File**: 
   - A `config.yml` file is created to define the data source and artifact directories, facilitating flexible configuration management.

9. **Stage 01: Load and Save Data**: 
   - Python scripts for loading and saving data are created in the `src` directory. The utility functions are stored in `src/utils/all_utils.py`.

10. **Create DVC Stages**: 
    - A `dvc.yaml` file is created to define the first stage of the pipeline, which loads the data using the specified Python script. This includes the command, dependencies, and outputs.

11. **Run DVC Repro**: 
    - The command `dvc repro` is executed to reproduce the pipeline, ensuring that all steps are carried out and outputs are generated as defined.

12. **Push Changes to Remote Repository**: 
    - All changes are added to the Git staging area, committed, and pushed to the main branch of the remote repository, finalizing the initial setup of the ML pipeline.

## Conclusion

This project sets a solid foundation for managing machine learning projects through version control and reproducibility practices using DVC. Each step is carefully documented and structured, allowing for easy scalability and collaboration in the development of machine learning models.
