# Example Ontology Data

This is a template Excel file structure. In a real setup, you would create an Excel (.xlsx) file with the following structure:

## Required Sheets:

### 1. Classes Sheet
Columns should include:
- ID: Unique identifier (e.g., EX_0000001)
- Label: Human-readable name
- Definition: Clear definition of the class
- Parent: Parent class ID
- Status: Curation status (proposed, approved, etc.)
- Curator: Person responsible for this term

### 2. Properties Sheet  
For object and data properties:
- ID: Unique identifier
- Label: Property name
- Definition: What this property represents
- Domain: What types of entities can have this property
- Range: What types of values this property can have
- Status: Curation status

### 3. Annotations Sheet
For additional metadata and annotations on terms.

## To create the actual Excel file:
1. Create a new Excel file named 'ontology-data.xlsx'
2. Add the sheets described above
3. Include sample data following your domain

## Example data structure:

Classes:
ID          | Label        | Definition                    | Parent      | Status
EX_0000001  | Thing        | The root class               |             | approved  
EX_0000002  | Material     | Physical material entities   | EX_0000001  | proposed
EX_0000003  | Process      | Occurrent processes          | EX_0000001  | proposed

Properties:  
ID          | Label        | Definition                    | Domain      | Range       | Status
EX_0000101  | part_of      | A is part of B               | EX_0000001  | EX_0000001  | approved
EX_0000102  | has_quality  | Entity has some quality      | EX_0000002  | EX_0000003  | proposed