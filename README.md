# 5 number summary
import numpy as np

def five_number_summary(data):
    minimum = np.min(data)
    q1 = np.percentile(data, 25)
    median = np.median(data)
    q3 = np.percentile(data, 75)
    maximum = np.max(data)
    return minimum, q1, median, q3, maximum

data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
minimum, q1, median, q3, maximum = five_number_summary(data)
print("Minimum:", minimum)
print("Q1:", q1)
print("Median:", median)
print("Q3:", q3)
print("Maximum:", maximum)
