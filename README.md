# Responsive Number Grid with Infinite Scroll

## Overview

This project is a simple, interactive HTML page that displays a responsive grid of sequential numbers in any base from 2 to 36. Users can select their preferred base, and the grid dynamically updates to represent numbers in the chosen base using uppercase letters for values above 9 (e.g., A=10, B=11, ..., Z=35). The grid supports infinite scrolling, allowing users to explore an endless sequence of numbers seamlessly.

## Features

- **Responsive Design**: The grid layout adapts to various screen sizes, ensuring a consistent and user-friendly experience across devices.

- **Base Selection**: Choose any numerical base between 2 and 36 using a dropdown selector. The first two cells of the grid are reserved for the base selector, replacing the numbers 0 and 1.

- **Infinite Scrolling**: As you scroll down, additional numbers are loaded automatically, providing an uninterrupted browsing experience.

- **Interactive Highlighting**:
  - **Select a Number**: Click on any number in the grid to highlight its three highest prime factors.
  - **Color Coding**: Multiples of these prime factors are colored using distinct RGB combinations (Red, Green, Blue) to visualize their relationships.
  - **Dynamic Updates**: Newly loaded numbers via infinite scrolling are automatically checked and highlighted based on the current selection.

- **Dark Theme**: The page features a sleek black background (`#000000`) with numbers displayed in a dark shade of grey (`#666666`) by default, enhancing visual appeal and reducing eye strain.

## How It Works

1. **Base Selector**:
   - Located in the first two cells of the grid.
   - The first cell displays the label "Base".
   - The second cell contains a dropdown menu allowing users to select a base from 2 to 36.

2. **Grid Layout**:
   - Numbers start from 2 and are displayed sequentially in the selected base.
   - The grid automatically adjusts the number of columns based on the screen size, ensuring that all rows are fully populated without incomplete rows.

3. **Infinite Scrolling**:
   - As users scroll towards the bottom of the page, more numbers are loaded automatically.
   - The grid ensures that new numbers maintain the layout consistency by loading them in multiples of the current number of columns.

4. **Interactive Highlighting**:
   - Clicking on a number calculates its unique prime factors.
   - The top three highest prime factors are identified and assigned distinct colors:
     - **Red** for the highest prime factor.
     - **Green** for the second highest.
     - **Blue** for the third highest.
   - All multiples of these prime factors in the grid are highlighted with their corresponding colors.
   - If a number is a multiple of multiple prime factors, the colors are combined (e.g., a number divisible by both the highest and second highest primes will appear yellow).

## Getting Started

### Prerequisites

- A modern web browser (e.g., Chrome, Firefox, Edge, Safari).

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/responsive-number-grid.git
   ```
2. **Navigate to the Project Directory**:
   ```bash
   cd responsive-number-grid
   ```
3. **Open the HTML File**:
   - Locate the `index.html` file in the project directory.
   - Open it with your preferred web browser by double-clicking the file or using the browser's "Open File" option.

## Usage

1. **Select a Base**:
   - Use the dropdown menu in the second cell of the grid to select your desired numerical base (ranging from 2 to 36).

2. **Explore the Grid**:
   - Scroll down to load more numbers automatically.
   - Click on any number to highlight its three highest prime factors and their multiples within the grid.

3. **Interact and Discover**:
   - Observe how multiples of different prime factors are color-coded.
   - Change the base selection to see the grid update accordingly.

## Customization

- **Number Range**: Adjust the initial number range or the batch size loaded during infinite scrolling by modifying the JavaScript section in the HTML file.
- **Styling**: Customize the appearance by editing the CSS styles within the `<style>` tags.
- **Prime Factor Colors**: Change the RGB values in the JavaScript to modify how prime factors and their multiples are highlighted.

## Contributing

Contributions are welcome! If you'd like to enhance this project, feel free to fork the repository and submit a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments

- Inspired by the need for an interactive and educational tool to explore number bases and prime factors.
- Utilizes modern web technologies for a seamless and responsive user experience.