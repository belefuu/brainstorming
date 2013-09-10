# Open/Save As Dialog Brainstorming

## Parts

### Common

* Top level container
* Project label
* Action toolbar
* ScorecardTree pane
* Diagram list pane
* Cancel button

### Open only

* Project chooser
* Open button

### Save As only

* Project name
* Name & Description fields
* Cancel button

## Parts/Components Breakdown

### Top level container

* Only specialty item is the splitter... as of now BorderContainer is the only thing

### Project label

* Just a label

### Project chooser

* `CommonRequests.getAllProjects()` should work
* `FilteringSelect` for the dropdown ?

### Action toolbar

* Fairly standard Toolbar

### ScorecardTree pane

* ScorecardTree with `contentType = SCORECARD`, `selectionMode = SINGLE`

### Diagram list pane

* A dgrid, pretty straightforward

## File Structure

## Workflows

### Bootstrapping

1. Open action initiated from *File* menu
