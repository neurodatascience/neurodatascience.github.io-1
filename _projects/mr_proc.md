---
title: mr_proc - a reproducible computational workflow for standardized data curation and processing pipelines 
subtitle: A neurobagel complement project
status: active
layout: project
people:
  - Nikhil, Vincent, Michelle
---

# mr_proc
*Process long and prosper*

---

## What is mr_proc? 

mr_proc is a workflow manager for:

1. MRI and tabular data curation
2. Standardized processing 
3. Raw + processed data tracking

## Modules

1. `Code`: mr_proc [repo](code_org.md)
2. `Data`: A [dataset](data_org.md) organized in a specific directory structure
3. `Containers`: Singularity containers encapsulating your processing pipelines


## Objectives
1. Standardized data i.e. convert DICOMs into BIDS
2. Run commonly used image processing pipelines e.g. FreeSurfer, fMRIPrep
3. Organize processed MR data inside `derivatives` directory
4. Organize demographic and clinical assessment data inside `tabular` directory
5. Run tracker scripts to populate `bagel.csv` with tabular and processing pipeline metadata
6. Provide metadata to [NeuroBagel](https://www.neurobagel.org/documentation/) to allow dashboarding and querying participants across multiple studies
    
## Documentation
Detailed documentation is provided [here](https://www.neurobagel.org/documentation/mr_proc/overview/)
