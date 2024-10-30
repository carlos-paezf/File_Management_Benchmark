# File Management Benchmark

This repository contains a Python script for automating file processing based on keywords and measuring execution time. It reads input files, searches for matching files in a specified directory, copies found files to a destination, and logs information on the number of processed lines.

## Features

- *Execution Time Measurement*: Measures the time taken to run each main function using a custom Python decorator.
- *Keyword-Based File Search*: Reads keywords from input files and finds matching files in a designated directory.
- *File Copying and Output Generation*: Copies found files to a destination folder and generates output files with matching lines.
- *Directory Configuration*: Configurable directories for input, search, and output.

## Directory Structure

- Search Directory: Z:\OPXGRSS (where files are searched based on keywords)
- Destination Directory: Z:\OPXGRSSPROD (where matching files and outputs are stored)
- Input Files: Z:\OPXGRSS\GRSSYREY.g0X
- Output Files: Z:\OPXGRSSPROD\GRSSYREY.g0X

## Getting Started

### Prerequisites

- Python 3.x
- shutil and os modules (part of Python standard library)

### Installation

1. Clone this repository:

    ```bash
    git clone <https://github.com/yourusername/file-processor-timer.git>
    cd file-processor-timer
    ```

2. Ensure Python is installed.

### Usage

1. Main Functions:

    - *process_files*: Reads input files, searches for matching files, copies them to the destination directory, and generates output files.
    - *validate_code*: Reads a single input file, searches for matching files based on keywords, and prints the results.

2. Running the Script*: Modify the main section of the script to run either process_files or validate_code:

    ```py
    if __name__ == '__main__':
        # Uncomment the function you'd like to run:
        # process_files()
        validate_code()
    ```

    Then execute the script:

```language
python main.py
```

## Code Explanation

- *measure_run_time*: A decorator function that measures and prints the execution time of the wrapped function.
- *process_files*: Reads lines from input files, extracts keywords, searches for matching files, and copies them to the output directory.
- *validate_code*: Reads an input file, extracts keywords, searches for files, and logs the results.

## Example Output

```txt
Reading file: Z:\OPXGRSS\GRSSYREY.g01. Number of lines in file: 200
---> Generated file: Z:\OPXGRSSPROD\GRSSYREY.g01. Number of lines in file: 150

>>> Function process_files took 5.678 seconds to execute
```

## License

This project is licensed under the MIT License.
