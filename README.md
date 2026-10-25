# ID3 Decision Tree Simulator

An interactive, browser-based visualization of the **ID3 Decision Tree algorithm** using the classic **Play Tennis dataset**. The simulator demonstrates how entropy and information gain are used to select attributes and build a decision tree step by step.

## Features

- Explore the 14-instance Play Tennis dataset.
- View the target distribution: 9 **Yes** and 5 **No** examples.
- Follow the root entropy calculation.
- Compare weighted entropy and information gain for Outlook, Temperature, Humidity, and Wind.
- Watch the tree grow step by step using the simulation controls.
- Use Next, Previous, Reset, and Auto-play controls.
- Adjust Auto-play speed.
- Test feature values in the prediction demo and view the decision path.
- Switch between light and dark themes.
- Browse the built-in theory guide and mini quiz.

## Decision Tree Produced

The simulator builds the following tree:

```text
Outlook
├── Sunny
│   └── Humidity
│       ├── High   → No
│       └── Normal → Yes
├── Overcast       → Yes
└── Rain
    └── Wind
        ├── Weak   → Yes
        └── Strong → No
```

The root entropy is approximately **0.940 bits**. Outlook is selected as the root because it has the highest information gain in the dataset (approximately **0.246**).

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Bootstrap 5
- Font Awesome
- SweetAlert2

The page loads Bootstrap, Font Awesome, Google Fonts, and SweetAlert2 from external CDNs, so an internet connection is needed for those external assets to load.

## How to Run

1. Download or clone this repository.
2. Open `hello.html` in a modern web browser.
3. Click **Start Simulation**.
4. Use **Next** to step through the dataset calculations and tree construction, or choose **Auto-play**.
5. Use the Prediction Demo to test a set of weather conditions.

No backend, database, or build step is required.

## Deploy with GitHub Pages

For the simplest GitHub Pages setup, rename `hello.html` to `index.html`, commit the change, and enable GitHub Pages in the repository settings. Select the branch and root folder that contain `index.html`.

## Learning Objectives

This project is intended for learning and demonstrating:

- Decision tree terminology: root, branch, internal node, and leaf node
- Entropy as a measure of uncertainty
- Information gain as a criterion for selecting a split
- Recursive construction of a decision tree
- Following decision paths to make predictions

## Dataset

The built-in Play Tennis dataset contains 14 examples with four input features—Outlook, Temperature, Humidity, and Wind—and one target label, Play Tennis (`yes` or `no`).

## License

No license has been specified yet. Add a license file if you want to define permissions for reuse and distribution.
