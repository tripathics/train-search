# Train Search on Make My Trip automate with Selenium and Java

## Pre-requisite
- Java 8
- Maven
- Chrome Browser

## How to run
- Clone the project
- Download Chrome and ChromeDriver for your operating system from [here](https://googlechromelabs.github.io/chrome-for-testing/)
- Extract the ChromeDriver and set the `CHROME_DRIVER_PATH` environment variable to the path of the ChromeDriver.
- Run the `trainsearch.jar` file with java

```bash
java -jar trainsearch.jar
# or
java -jar trainsearch.jar <fromCity> <toCity> <date> <class>
```

The first command will run the program with default values. The default values are:

- `fromCity`: LUCKNOW
- `toCity`: DELHI
- `date`: 2024-02-02 (yyyy-mm-dd)
- `class`: 3A (3rd AC)

## Dependencies
- Selenium