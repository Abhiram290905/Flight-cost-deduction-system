# Flight Ticket Price Prediction

This C program predicts ticket prices for a flight over a given number of days based on demand and seat availability. It simulates price fluctuations by considering a demand function that reacts to changes in ticket prices and days left until departure.

## Features
- Takes user input for total seats, days until departure, and base ticket price.
- Uses a demand function to simulate ticket price adjustments.
- Adjusts prices based on demand and random fluctuations within limits.
- Outputs a predicted price trend per day until departure.

## How It Works
1. **Demand Function**: Determines demand based on price and days left.
2. **Price Prediction**:
   - If demand is lower than available seats, prices may increase slightly.
   - If demand is higher than available seats, prices decrease.
   - Prices stay within reasonable limits (50% to 150% of base price).
3. **Output**: Prints the predicted price for each day leading up to departure.

## Compilation and Execution
### Compile the Program:
```sh
gcc -o flight_price_predictor flight_price_predictor.c
```

### Run the Program:
```sh
./flight_price_predictor
```

## Example Usage
```sh
Enter total seats on the flight: 100
Enter number of days until departure: 10
Enter base ticket price: 200
```
_Output:_
```
Predicted Prices Per Day Until Departure:
Day 1: $205
Day 2: $210
...
Day 10: $200
```

## Dependencies
- Standard C libraries (`stdio.h`, `stdlib.h`)
- GCC compiler (or any C compiler of choice)

## Notes
- The pricing adjustments include randomness to simulate real-world variations.
- Prices are bounded to avoid extreme fluctuations.
- The demand function is a simple model and may not reflect real-world pricing strategies.

## License
This project is open-source and free to use under the MIT License.

---
Developed as a simple simulation to understand ticket price behavior based on demand trends.

