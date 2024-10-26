Build a simple classifier to predict whether a machine will fail
based on temperature and pressure readings.
This code defines a function classify_failure that checks if the temperature or pressure surpasses critical thresholds and then tests this function with sample values
def classify_failure(temp, pressure):
    # Failure happens if temp > 75 or pressure > 120
    if temp > 75 or pressure > 120:
        return "Fail"
    else:
        return "Operational"

# Test with a new machine reading
temperature = 80  # Example temperature
pressure = 115    # Example pressure
result = classify_failure(temperature, pressure)

print(f"The machine’s status is: {result}")
