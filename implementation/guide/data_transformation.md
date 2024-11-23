## 🚀 Data Transformation

We utilized **Azure Databricks** to execute pipelines using **PySpark**. These pipelines are designed to process newly arrived data in the containers created by ADF, apply a series of transformations, and load the processed data into the appropriate containers.

## 👨‍💻 **Tasks Overview**  

We leveraged **Azure Databricks** to execute pipelines using **PySpark**. These pipelines are designed to process newly arrived data in the containers created by ADF, apply a series of transformations, and load the processed data into the appropriate containers.  

### **Pipelines Overview**  

1. **Storage Mount Pipeline**:  
   This pipeline creates a storage mount within the Databricks workspace, enabling access to the data required for transformations.  

2. **Bronze to Silver Pipeline**:  
   Reads raw data from the Bronze container (imported via ADF from SSMS), applies basic transformations, and loads the transformed data into the Silver container.  

3. **Silver to Gold Pipeline**:  
   Takes data from the Silver container, performs advanced transformations, and loads the refined results into the Gold container.  

### Output Format
- The output of each pipeline is stored in **Parquet format**, ensuring efficient storage and compatibility for downstream processing.

## 📸 Snapshots