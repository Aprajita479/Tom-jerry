# Tom-jerry    

This is a Python script that uses the `turtle` module to draw shapes based on data extracted from a Microsoft Word document.

## Requirements

- Python 3.x
- `turtle` module
- `docx` module

You can install the required modules using `pip`:

```
pip install turtle
pip install python-docx
```

## Usage

1. Make sure you have a Microsoft Word document in the same directory as this script. The document should contain specific patterns of coordinates and colors.
2. Modify the `source` variable in the script to match the name of your Word document (without the extension).
3. Run the script using the command:

```
python script.py
```

The script will read the Word document and extract the coordinates and colors. It will then use the `turtle` module to draw the shapes based on the extracted data.

## How it works

1. The script imports the necessary modules: `turtle`, `re` (regular expressions), and `docx` (for working with Word documents).
2. It initializes empty lists to store the extracted coordinates and colors.
3. It opens the Word document specified in the `source` variable using the `docx` module.
4. It loops through each paragraph in the Word document and tries to extract coordinate and color data using regular expressions.
5. The extracted data is processed and added to the respective lists.
6. The script sets up the turtle graphics environment by creating a turtle object (`pen`) and a screen object (`screen`).
7. It configures some settings for the turtle, such as tracer speed, hiding the turtle cursor, and making the screen fullscreen.
8. It iterates over the extracted coordinates and colors to draw the shapes using the turtle.
9. Finally, the turtle hides and the screen enters the event loop to display the drawn shapes.

Note: The script assumes that the Word document follows a specific pattern for coordinate and color data extraction. Make sure your document adheres to this pattern for the script to work correctly.

Feel free to customize and modify the script according to your needs. Enjoy drawing shapes with the turtle!
