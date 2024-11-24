# CloudBridge


##  Project Overview

This project focuses on modernizing data processing system by migrating from a legacy on-premises database architecture to a cloud-native solution on Azure. The migration aims to overcome the limitations of current infrastructure by leveraging cloud capabilities for improved scalability, performance, and maintainability.

## Purpose

The modernization initiative was driven by several critical business needs:

- **Reduce Development Overhead**: The legacy system required extensive manual intervention, with developers spending significant time on workflow development, SSIS package maintenance, and transformation rule implementation.
  
- **Improve Scalability**: The traditional on-premises solution had limitations in handling increasing data volumes and concurrent processing requirements.
  
- **Enhance Maintainability**: The previous architecture involved multiple technology stacks and complex data transformation layers, making maintenance and updates challenging.
  
- **Accelerate Development Cycles**: By streamlining the development process and reducing dependencies, we aimed to speed up feature delivery and reduce time-to-market.

## Architecture

### Legacy


### CloudBridge


## Legacy vs CloudBridge pros & cons

### Legacy Architecture Challenges

| Aspect | Legacy System | Impact |
|--------|--------------|---------|
| Development Time | 3 weeks per feature (1 week each for workflows, SSIS, transformations) | Slow delivery cycles |
| Resource Utilization | 30 developers for maintenance and development | High operational costs |
| Technology Stack | EDS → SSIS → SSMS (3 layers) → Web UI | Complex maintenance |
| Data Processing | Multiple transformation layers with manual interventions | Prone to errors and delays |
| Scalability | Limited by on-premises infrastructure | Performance bottlenecks |

### New Architecture Benefits

| Aspect | Modern System | Impact |
|--------|--------------|---------|
| Development Time | Significantly reduced through automated processes | Faster feature delivery |
| Resource Utilization | Optimized team size with focused roles | Reduced operational costs |
| Technology Stack | Azure Cloud-native services | Simplified maintenance |
| Data Processing | Automated data pipelines with Databricks | Improved reliability |
| Scalability | Cloud-native elastic scaling | Enhanced performance |


### Data Flow:
1. Raw data from EDS is initially stored in SSMS
2. Azure Data Factory orchestrates the data movement to Data Lake containers
3. Data undergoes transformations through Databricks notebooks using PySpark
4. Processed data is stored in Synapse Analytics
5. Power BI provides business intelligence and visualization

## Technologies Used

### Cloud Platform
- **Azure Cloud**: Primary cloud platform hosting all services

### Data Storage & Processing

- **Azure Data Factory**: 
- **Azure Data Lake**: Hierarchical data storage with Bronze, Silver, and Gold containers
- **Azure Synapse Analytics**: Enterprise-scale analytics service
- **Azure Databricks**: Big data processing and analytics platform
- **SQL Server Management Studio (SSMS)**: Initial data repository

### Data Integration & Transformation
- **Azure Data Factory**: Data integration service
- **PySpark**: Data processing and transformation engine
- **Databricks Notebooks**: Development environment for transformation logic

### Visualization & Reporting
- **Power BI**: Business intelligence and data visualization platform

### Source System
- **Enterprise Data Service (EDS)**: Source system for raw data

---

For more information about specific components or implementation details, please contact the development team.
