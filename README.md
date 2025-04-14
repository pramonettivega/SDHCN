# Fire-Ready-Forests-Data-Challenge



## 📊 Data Description

This project uses two primary datasets for training and evaluation:

1. **Field-Collected Treelist Data**  
   Sourced from standardized forest inventory surveys across multiple sites in California, this dataset includes in-situ measurements of individual trees. Key attributes include tree height, diameter, and species annotations. 
   Data files:  
   - `01_plot_identification.csv`  
   - `03_tree.csv`

3. **FastFuels (FF) Treelist Data**  
   Derived from TLS (Terrestrial Laser Scanning) analysis and modeling, this dataset provides estimated structural characteristics (e.g., height and diameter) along with species codes inferred from remote sensing methods. 
   Data file:  
   - `FF_treelist_all.csv`

To support classification tasks such as predicting plant functional types (PFT), genus, and species, we also use:

- **Species-to-PFT Mapping**  
  A reference table mapping species codes and names to standardized genus and PFT labels.  
  Data file:  
   - `FIATreeSpeciesCode_pft.csv`

## 🌲 TLS Data Description (Test Data)

The TLS (Terrestrial Laser Scanning) dataset is used as the test set for evaluating model predictions. It contains tree-level structural measurements extracted from high-resolution LiDAR scans, and serves as the target for predicting labels such as Plant Functional Type (PFT), genus, and species. 
 Data file:  
   - `TLS_treelist.csv`


## 🚀 Running the Project

### 1. Install Dependencies

Make sure you have Python 3.8+ and `pip` installed. From the root directory of the project, install all required dependencies using:

```bash
pip install -r requirements.txt
```

### 2. Launch Jupyter Notebook

To run the modeling pipeline and reproduce results:

1. Open the Jupyter environment:
    ```bash
    jupyter notebook
    ```

2. In your browser, open the notebook file:
    ```
    sprint4-SDHCN.ipynb
    ```

3. Run all cells sequentially to process data, train models, and generate results.

> 📁 Ensure all necessary data files (e.g., `01_plot_identification.csv`, `FF_treelist_all.csv`, etc.) are located in the correct paths as expected by the notebook, typically in a `data/` directory.




## 🔗 References
