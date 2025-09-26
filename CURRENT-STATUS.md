# Repository Status

This repository is currently set up with basic configuration files for OntoSpreadEd but is missing the Excel (.xlsx) files that contain the actual ontology data.

## Current Files:
- `.onto-ed/config.yaml` - Repository configuration for OntoSpreadEd
- `.onto-ed/release_script.json` - Release automation configuration
- `ontology.owl` - Example OWL file
- `classes.csv` - Sample classes data (needs to be converted to Excel)
- `properties.csv` - Sample properties data (needs to be converted to Excel)

## To Make This Repository Functional:

1. **Create Excel files**:
   - Convert `classes.csv` and `properties.csv` to sheets in `ontology-data.xlsx`
   - Or create `ontology-data.xlsx` manually with proper sheet structure

2. **Update configuration**:
   - Uncomment the `indexed_files` section in `.onto-ed/config.yaml`
   - Adjust other settings as needed

3. **Test with OntoSpreadEd**:
   - Push changes to GitHub
   - Reload repository in OntoSpreadEd settings