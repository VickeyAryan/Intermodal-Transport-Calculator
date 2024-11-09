# Intermodal Transport Calculator

This web-based calculator helps users balance cost and time for intermodal shipments by selecting optimal routes based on various route options. It calculates a total score based on user-selected routes, offering a customized solution for managing shipping priorities.

## Features
- Users can select between different route options with varying costs and delivery times.
- Calculates a total score based on the selected options, with a customizable formula balancing cost and time.
- Provides a user-friendly interface with an intuitive layout.

## How It Works
The calculator uses a table with pre-defined routes, each offering two options for cost and time. Users choose one option per route, and the calculator computes a total score that combines the costs and times of the selected routes.

The formula for the total score is:
\[
\text{Total Score} = (\text{Total Cost} \times 0.9) + (\text{Total Time} \times 0.1)
\]
where the cost is weighted at 90% and the time at 10%.

## Usage

1. **Select Route Options**: For each route (e.g., A->B, B->C), choose between Option 1 and Option 2.
   - Each option displays the cost and estimated time for that leg of the journey.
2. **Calculate the Score**: Click the **Calculate** button to compute the total score.
3. **View the Total Score**: The result, displayed at the bottom, shows the total score based on your selections.

## Example Routes and Options

| Route | Option 1 (Cost, Time) | Option 2 (Cost, Time) |
|-------|------------------------|------------------------|
| A->B  | £20, 1 Day            | £7, 3 Days            |
| B->C  | £12, 5 Days           | £6, 12 Days           |
| C->D  | £18, 21 Days          | £80, 2 Days           |
| D->E  | £11, 4 Days           | £9, 8 Days            |
| E->F  | £18, 1 Day            | £8, 3 Days            |

## Project Structure

- **HTML**: Provides the structure for the calculator, including the options for each route.
- **CSS**: Styles the calculator layout, including buttons, table, and explanatory text.
- **JavaScript**: Contains the calculation logic that processes user input and generates the total score.

## Future Improvements
- **Customizable Input Options**: Allow users to input custom costs and times for each route, making the calculator more flexible for various scenarios.
- **Variable Weighting Factors**: Enable users to adjust the weighting of cost and time in the score formula (e.g., 70% cost, 30% time) for a more personalized calculation.
- **Detailed Breakdown of Results**: Display a breakdown of total costs and times separately, helping users understand the score calculation in more detail.
