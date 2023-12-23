# Train Search on Make My Trip automate with Selenium and Java

|Submtted by| |  
|---|---|  
Name:|Chandrashekhar Tripathi
Batch:|B.Tech CSE 4th Year
Insitute:|NIT Arunachal Pradesh


Find video demo of given testcase and source code on [google drive](https://drive.google.com/drive/folders/1j9zG6kniO_Z1vgf8A4d8FgG3YCav68OX?usp=sharing)

## How to run `trainsearch.jar` (program)
- Clone the project
- Download Chrome and ChromeDriver for your operating system from [here](https://googlechromelabs.github.io/chrome-for-testing/)
- Extract the ChromeDriver and set the `CHROME_DRIVER_PATH` environment variable to the path of the ChromeDriver.

    - In Bash (linux or MacOS)  
    ```bash
    export CHROME_DRIVER_PATH=/path/to/chromedriver
    ```

    - In Powershell (Windows)
    ```powershell
    $env:CHROME_DRIVER_PATH = "/path/to/chromedriver"
    ```

    - In CMD (Windows)
    ```cmd
    set CHROME_DRIVER_PATH=/path/to/chromedriver
    ```

- Run the `trainsearch.jar` file with java

```bash
# run with default values
java -jar trainsearch.jar
# or run with custom values 
java -jar trainsearch.jar <fromCity> <toCity> <date> <class>
```

The first command will run the program with default values. The default values are:

- `fromCity`: LUCKNOW
- `toCity`: DELHI
- `date`: 2024-02-02 (yyyy-mm-dd)
- `class`: 3A (3rd AC)

Supported values for:  
- `class`-> 1A, 2A, 3A, 3E, SL, CC, 2S, ALL
- `date`-> yyyy-mm-dd


## Pre-requisite for building
- Java 8
- Maven
- Chrome Browser

## Dependencies
- Selenium

## Screenshots and logs

**Testcase used in the below example:**
* From City: "LUCKNOW"
* To City: "DELHI"
* Date of Journey: "02 Feb 2024"
* Class: "3A" 

1. Checking if landed in the correct page by checking it's title text
	![Screenshot from 2023-12-22 19-08-44.png](images/Screenshot%20from%202023-12-22%2019-08-44.png)

2. Print *URL* and *Title text*
	 ![Screenshot from 2023-12-22 19-09-00.png](images/Screenshot%20from%202023-12-22%2019-09-00.png)

3. Filling the form (from city, to city, date of journey and train class)
 ![Screenshot from 2023-12-22 19-09-10.png](images/Screenshot%20from%202023-12-22%2019-09-10.png)

	**3.1**  Select "from city input" and type in "LUCKNOW" and select the first option from the drop-down.
	![Screenshot from 2023-12-22 19-09-30.png](images/Screenshot%20from%202023-12-22%2019-09-30.png)  
    ![Screenshot from 2023-12-22 19-09-38.png](images/Screenshot%20from%202023-12-22%2019-09-38.png)

	**3.2** After selecting "from city" from the dropdown, input field for "to city" is automatically focused. Type in "DELHI" in "to city". 
	![Screenshot from 2023-12-22 19-10-02.png](images/Screenshot%20from%202023-12-22%2019-10-02.png)  
    ![Screenshot from 2023-12-22 19-10-19.png](images/Screenshot%20from%202023-12-22%2019-10-19.png)

	**3.3** After selecting "to city" from dropdown, date input is automatically focused. We need to scroll to the input date month and select the date- 2 Feb 2024.
	![Screenshot from 2023-12-22 19-10-44.png](images/Screenshot%20from%202023-12-22%2019-10-44.png)  
	![Screenshot from 2023-12-22 19-11-24.png](images/Screenshot%20from%202023-12-22%2019-11-24.png)

	Travel Month was February so it scrolled one time and selected the input date. 
	![Screenshot from 2023-12-22 19-11-52.png](images/Screenshot%20from%202023-12-22%2019-11-52.png)  
    ![Screenshot from 2023-12-22 19-12-09.png](images/Screenshot%20from%202023-12-22%2019-12-09.png)

	**3.4** Select class from dropdown to "3A"
	![Screenshot from 2023-12-22 19-34-22.png](images/Screenshot%20from%202023-12-22%2019-34-22.png)  
	![Screenshot from 2023-12-22 19-34-37.png](images/Screenshot%20from%202023-12-22%2019-34-37.png)

4. Click on "Search" button
	![Screenshot from 2023-12-22 19-15-33.png](images/Screenshot%20from%202023-12-22%2019-15-33.png)

