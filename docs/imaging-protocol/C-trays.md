# C Tray Beetle

!!! warning
    Placing two C trays in a single image is not recommended. Ultimately, this workflow created more hassels downstream than time saved in imaging.

### Required Elements in Each Image

- Separate Header tray for each C tray with:  
    - Place cm scale in same focal plane as specimens.
    - Include color calibration chart in each image.
    - Include domain label visible in frame.
    - Ensure species label is clearly visible.
    - Include expert or parataxonomist label.
- Both C trays should be of similarly sized species so that they are all in focus. When in doubt, do only one tray at a time.

### Image Capture

- Zoom into an individual beetle with the magnifying glass on the bottom right of the touch screen.
- Manually focus on the specimen.
- Focus carefully on the top of the specimens, not labels or pins.
- **Move the zoom box to check the specimens in the other tray are also in focus**.
- Take test shot and review for proper exposure, focus, and framing.
- Ensure all required elements are visible in frame.
- Capture final image and verify quality before proceeding.
    - To verify, zoom in on individual beetle to ensure it is clear and in focus, see example photos.

###  Metadata

Because C Trays are imaged two at a time, there is a separate [C Tray Template](https://docs.google.com/spreadsheets/d/11iotlUNbXXv7fLCwbGCAysM07OueoNAwrzWjJZy5lD4/edit?usp=sharing); the column values are defined on the `ColumnNames` Sheet:

- Mark: Record “yes” once the header label of the unit tray has been marked with a pen to denote that imaging has occurred.
- All of the column are the same as the A and B Trays, but there are twice as many columns, with `Tray1_` or `Tray2_` appended to the beginning of the column names to enter data for both trays in a single image (e.g., `Tray_1_IndividualID_1`).
    - If there is ever just one Tray in the image, enter it into `Tray1_` columns, and put NA in to the `Tray2_` columns.
- In some cases, you will not have 4 beetles for the individual ID records, in this case do the following:
    - 1 Beetle: Record the IndividualID in *IndividualID_1* and enter NA to other columns.
    - 2 Beetles: Record the IndividualID in *IndividualID_1* and *IndividualID_n* and enter NA the middle columns (this is very important for querying).
    - 1 Beetles: Record the IndividualIDs in *IndividualID_1, IndividualID_2* and *IndividualID_n* and enter NA the middle column (this is very important for querying).
