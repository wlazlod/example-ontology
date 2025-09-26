# Example Ontology Repository

This repository contains an example ontology that can be used with [OntoSpreadEd](https://github.com/ontology-tools/onto-spread-ed).

## Structure

- `.onto-ed/config.yaml` - Configuration for OntoSpreadEd integration
- `.onto-ed/release_script.json` - Release automation configuration  
- `ontology-data.xlsx` - Main ontology data in spreadsheet format
- `ontology.owl` - Generated OWL file (created during releases)
- `README-Spreadsheet-Structure.md` - Documentation of the spreadsheet structure

## Usage with OntoSpreadEd

1. Make sure this repository is accessible to your OntoSpreadEd instance
2. Add the repository name to your `startup-repositories.yaml` or load it through the Settings page
3. The ontology will be available for collaborative editing through the spreadsheet interface

## Customization

1. **Update `.onto-ed/config.yaml`**:
   - Change `full_name` to match your repository
   - Update `short_name` with your ontology abbreviation
   - Modify `prefixes` to include your ontology namespace
   - Adjust `indexed_files` to match your file structure

2. **Create your ontology spreadsheet**:
   - Replace this example with your actual `ontology-data.xlsx` file
   - Follow the structure described in `README-Spreadsheet-Structure.md`
   - Include appropriate sheets for Classes, Properties, and Annotations

3. **Customize release process**:
   - Modify `.onto-ed/release_script.json` to match your release workflow
   - Update dependencies and artifacts as needed

## Getting Started

1. Fork or clone this repository
2. Replace example content with your ontology data
3. Update the configuration files
4. Push to GitHub
5. Add to your OntoSpreadEd instance

## Requirements

- GitHub repository (public or accessible to your OntoSpreadEd instance)
- Excel files with proper ontology data structure
- ROBOT tool (optional, for release automation)