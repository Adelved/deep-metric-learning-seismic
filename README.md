## Running Notebooks in Google Colab

This repository contains Google Colab notebooks designed to be run in the Google Colaboratory environment. The notebooks are pre-configured with default data, but you can also use your own data. Here's how to run these notebooks:

1. **Open Google Colab**: Go to [Google Colab](https://colab.research.google.com/).

2. **Load the Notebook**: 
   - Click on "File" > "Open notebook"
   - Select the "GitHub" tab
   - Enter the URL of this repository: https://github.com/Adelved/deep-metric-learning-seismic
   - Choose the notebook you want to run from the list

3. **Using Default Data**:
   - The notebooks are configured to download and use default data using `gdown`.
   - Simply run the cells as they are to use this default dataset.

4. **Using Your Own Data**:
   If you prefer to use your own data:
   
   a) **Mount Your Google Drive**:
      - Run the cell that mounts your Google Drive. It will look similar to this:
        ```python
        from google.colab import drive
        drive.mount('/content/drive')
        ```
      - Follow the authentication steps when prompted.
   
   b) **Update Data Paths**:
      - Locate the cells where data is loaded.
      - Replace the `gdown` commands or default file paths with the paths to your data in Google Drive.
      - Typically, your Google Drive will be mounted at `/content/drive/MyDrive/`.

5. **Run the Notebook**:
   - You can now run the cells in the notebook sequentially.
   - Make sure to read any instructions or comments in the notebook for specific setup or data requirements.

6. **Note on Runtime**:
   - For best performance, you may want to change the runtime to GPU:
     - Go to "Runtime" > "Change runtime type"
     - Select "GPU" from the dropdown menu
     - Click "Save"

By following these steps, you can run the notebooks using either the provided default data or your own dataset stored in Google Drive.

## Citation

If you use this software, please cite it as below:
```bibtex
@misc{da_deep_metric_learning_seismic_2024,
  author       = {Adelved, Dennis and Bugge, Aina Juell and Lie, Jan Erik and Bormann, Peter and Faleide, Jan Inge},
  title        = {Code and Resources for "Challenges and Learning from Exploring Deep Metric Learning for Identifying Seismic Stratigraphy"},
  year         = 2024,
  url          = {https://github.com/Adelved/deep-metric-learning-seismic}
}
