# shrinksvg
reduce SVG size

This Perl script optimizes SVG files by reducing precision, converting polygons to paths.
It minimizes the file size while preserving the visual integrity of the SVG.

## Features

- **Precision Reduction**: Adjusts the precision of coordinates based on the size of the SVG.
- **Polygon to Path Conversion**: Converts `<polygon>` elements to optimized `<path>` elements.

## Usage

To use the script, pipe an SVG file into it via standard input and capture the optimized SVG from the output:

```bash
cat input.svg | ./shrinksvg > output.svg

## Dependencies

- Perl 5
- XML::LibXML module
