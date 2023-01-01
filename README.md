# Exam Project for HSLU Module "Modern Data Engineering"

Lukas Erdin, Leo Rettich

Fall semester 2022

## Exam 1 (HOP)

The project for exam 1 contains a HOP project and a Tableau visualization. 

### HOP Project

`full_workflow.hwf`: HOP workflow combining all the following pipelines to one executable unit. 

`prepare_database.hpl`: HOP pipeline for preparing the Azure SQL database. All necessary tables are created by this pipeline. (Host specific necessary adaptions: Database connection named "azure_sql_db".)

`load_metadata.hpl`: HOP pipeline for loading the metadata to the database. (Host specific necessary adaptions: Paths to the two Excel files, database connection named "azure_sql_db".)

`load_xml_files.hpl`: HOP pipeline for loading the actual data from the XML files to the database. (Host specific necessary adaptions: Path to the folder containing all XML files, database connection named "azure_sql_db".)

`transform_job_data.hpl`: HOP pipeline for transforming the staged data to prepare it for the visualization. (Host specific necessary adaptions: Database connection named "azure_sql_db".)

### Visualization

`Dashboard.twb`: Tableau dashboard visualizing the data from database table `job_storage`.
