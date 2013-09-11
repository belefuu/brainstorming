# Open/Save As Dialog Brainstorming



## Parts/Components Breakdown

### Common
* Top level container
  * Only specialty item is the splitter... as of now BorderContainer is the only thing
* Project label
  * Just a label
* Action toolbar
  * Fairly standard Toolbar
* ScorecardTree pane
  * ScorecardTree with `contentType = SCORECARD`, `selectionMode = SINGLE`
* Diagram list pane
  * A dgrid, pretty straightforward
* Cancel button
  * Self explanatory

### Open only

* Project chooser
  * `CommonRequests.getAllProjects()` should work
  * `FilteringSelect` for the dropdown ?
* Open button
  * Get the selected diagram and initiate open

### Save As only

* Project name
  * Just a label
* Name & Description fields
  * Just inputs
* Save button
  * Gets the name, description, and location, and initiates Save As



## File Structure

* *stm/diagram/edit/view/DiagramNavigatorView.js*
  
  "Abstract" module to house common view code

* *stm/diagram/edit/view/OpenDiagramView.js*

  Specific open diagram view code
  
* *stm/diagram/edit/view/SaveAsDiagramView.js*
  
  Specific save as diagram view code

* *stm/diagram/edit/controller/DiagramNavigatorController.js*

  "Abstract" module to house common controller code

* *stm/diagram/edit/controller/OpenDiagramController.js*

  As you'd expect

* *stm/diagram/edit/controller/SaveAsDiagramController.js*

As you'd expect



## Workflows

### Bootstrapping

1. Open action initiated from *File* menu
