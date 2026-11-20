# Monte-Carlo-Dice

This code uses a Monte Carlo simulation to estimate the probability that two fair six-sided dice add up to exactly 7.

It randomly generates two dice rolls and adds them together. If the total equals 7, it records a success. It repeats this experiment 10,000 times, then divides the number of successes by the total number of trials to estimate the probability.

Finally, it compares the simulated estimate with the exact probability of \(1/6 \approx 0.1667\). The estimate will vary between runs because the rolls are random, but using more trials generally improves its accuracy.
import numpy as np  # Use NumPy to generate random dice rolls

# Set how many times we will roll the pair of dice
n = 10000

# Start the success counter at zero
# A success means the two dice add up to exactly 7
successes = 0

# Repeat the experiment n times
# i takes the values 0, 1, ..., n - 1
for i in range(n):

    # Randomly roll the first die
    # randint includes 1 but excludes 7, so outcomes are 1 to 6
    die1 = np.random.randint(1, 7)

    # Randomly roll the second die
    die2 = np.random.randint(1, 7)

    # Add the two dice together
    total = die1 + die2

    # Check whether the total equals 7
    # == checks equality, whereas = assigns a value
    if total == 7:

        # Increase the success counter by 1
        successes += 1

# After all trials, estimate the probability:
# number of successes divided by total number of trials
probability = successes / n

# Display the results
print("Number of trials:", n)
print("Number of successes:", successes)
print("Estimated probability:", probability)

# Compare our estimate with the exact probability
# There are 6 successful outcomes out of 36 equally likely pairs
print("Exact probability:", 6 / 36)
