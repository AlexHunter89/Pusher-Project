# Pusher Space Optimization Script

## Overview

This project is focused on optimizing the use of shelf space in retail environments, particularly where products are displayed using pusher fixtures. Pusher fixtures are designed to hold products in place on a shelf by latching onto a railing system. However, due to the fixed notches on the railing, pushers can only be moved in 0.5 cm increments, with a minimum spacing of 4.5 cm between them. 

This script converts product widths provided in inches to centimeters, adjusts them to the nearest fit based on the pusher spacing constraints, and calculates the space lost due to these constraints. The goal is to minimize wasted space on the shelf and ensure that products fit within the allotted space as efficiently as possible.

## Problem Statement

In retail environments, merchandisers face challenges when placing products on shelves with pusher fixtures. The space between pushers can only be adjusted in increments of 0.5 cm, with a minimum distance of 4.5 cm. This often results in wasted space when product widths do not perfectly align with the available space. 

For example:
- A product with a width of 1 inch (2.54 cm) will require a minimum of 4.5 cm of space, resulting in a loss of 1.96 cm (0.77 inches) of shelf space.

Over a long run of shelves, this seemingly small loss can add up to a significant amount of wasted space, potentially leading to products not fitting as planned.

## Script Description

The script performs the following steps:

1. **Generate Product Widths**: Randomly generates a list of 75 product widths (in inches) to simulate a retail environment.

2. **Convert to Centimeters**: Converts the product widths from inches to centimeters.

3. **Adjust for Pusher Constraints**: Rounds the converted measurements up to the nearest 0.5 cm increment, ensuring a minimum distance of 4.5 cm between pushers.

4. **Reconvert to Inches**: Converts the adjusted measurements back to inches for comparison.

5. **Calculate Space Loss**: Determines the difference between the original and adjusted measurements to calculate the space lost due to pusher constraints.

6. **Summary Statistics**: Provides a summary of the total space required, the space lost, and the average and maximum space loss per product.

## Usage

To use this script:

1. Ensure you have Python installed on your machine.
2. Copy the script into a `.py` file.
3. Run the script using a Python interpreter.

The script will output a list of the original product widths, the adjusted widths after accounting for pusher constraints, and the difference in space. It will also provide a summary of the total space required and the space lost.

### Example Output

```
The original measurements total up to X inches.
The new measurements total up to Y inches.
With pushers, you will need an additional Z inches of space to fit all of the products.
The biggest loss for a single product in terms of space is A inches.
The average loss per product in terms of space is B inches.
```

## Conclusion

This script is a tool to help merchandisers and retail planners optimize shelf space when using pusher fixtures. By understanding the space lost due to fixed pusher constraints, retailers can better plan their shelving layouts, reducing wasted space and improving product placement efficiency.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.