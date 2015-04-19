# Data Structure GUI Documentation:
## Creating an instance of DS-GUI-Core
* (define gui-core (data-structure-core your-ds))
* NOTE: At this time, "cons" elements are not supported, all structures must be lists or lists of multiple lists

## Commands and Core Procedures
### Issuing commands
* (gui-core 'command)

### Public Commands:
* 'draw -> Draws the data structure
* 'draw-enclosed -> Draws the data structure with the row, column grid
* 'help -> Prints a list of supported commands
* 'save -> Save the table (usually after editing)

### Debugging Commands:
* 'peek-ds -> Gets the current master-ds
* 'peek-table -> Gets the current master-table
* 'load -> Used internally to load the master-ds and master-table

### Top Level Procedures:
These are the functions used by the GUI Core
* (build-table table) -> Table-Construction.rkt
* (build-list table) -> Table-Deconstruction.rkt
* (make-target table) -> Diagram-Drawing.rkt
* (make-dc table) -> Diagram-Drawing.rkt
* (draw-table table) -> Diagram-Drawing.rkt
* (draw-enclosed-table table) -> Diagram-Drawing.rkt

## Source File Information:
### File Descriptions:
* Data-Structure-GUI-Core.rkt - The main interface
* Diagram-Components.rkt - Contains the diagram images used to draw a structure
* Diagram-Drawing.rkt - Contains the drawing procedures for a given table
* Sandbox.rkt - Currently a sandbox for interacting with the Data-Structure-GUI-Core
* Table-Construction.rkt - Contains the table building procedure for a given data structure
* Table-Core-Utils.rkt - Contains counting procedures, table manipulation procedures, and accessors
* Table-Deconstruction.rkt - Contains the list building procedure for a given table
* Table-Sorting.rkt - Contains the sorting procedures for a given table

### File Hierarchy:
Top-Level:
* Data-Structure-GUI-Core.rkt
<br>
Mid-Level:
* Diagram-Drawing.rkt
* Table-Construction.rkt
* Table-Deconstruction.rkt
<br>
Base:
* Diagram-Components.rkt
* Table-Core-Utils.rkt
* Table-Sorting.rkt
