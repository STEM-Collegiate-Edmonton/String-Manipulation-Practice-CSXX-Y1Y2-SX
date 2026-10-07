# String Manipulation Practice

## Basic Premise

You will be given four separate Python files. Each file contains a variable named `string_to_process` with a different messy string.

Your task is to write code underneath the provided variable that processes the string into the required format and prints the result. You must use the value stored in `string_to_process`; do not replace it with a manually corrected string.

### `format_name.py`

The file will begin with:

```python
string_to_process = "   sMitH, aLeX    "
```

Process the string so that the output is:

```text
Alex Smith
```

### `format_title.py`

The file will begin with:

```python
string_to_process = "t H e , T a L e :: O f , T w O :: c I t I e S"
```

Process the string so that the output is:

```text
The Tale Of Two Cities
```

### `format_list.py`

The file will begin with:

```python
string_to_process = "eggs,cheese,milk,bread,cereal"
```

Process the string so that the output is:

```text
EGGS | CHEESE | MILK | BREAD | CEREAL
```

### `process_numbers.py`

The file will begin with:

```python
string_to_process = "  18,27,35,20  "
```

Process the values as numbers and produce:

```text
Total: 100
Average: 25.0
```

## Basic File Structure

Your starter folder will contain:

```text
basic/
├── format_list.py
├── format_name.py
├── format_title.py
└── process_numbers.py
```

## Basic Requirements

* [ ] In `format_name.py`, remove unnecessary whitespace, format the name so each part begins with a capital letter, remove the comma, and reorder the first and last name.
* [ ] In `format_title.py`, convert the text so each word starts with a capital letter, replace punctuation with spaces, and remove unnecessary white space.
* [ ] In `format_list.py`, separate the items, change the text to uppercase, and join the items using ` | `.
* [ ] In `process_numbers.py`, clean and separate the values and convert each value from a string into an integer.
* [ ] In `process_numbers.py`, calculate and print the total and average of the readings.
* [ ] Use appropriate string methods such as `strip()`, `split()`, `replace()`, `title()`, `lower()`, and `join()` rather than manually replacing `string_to_process` with the finished answer.
* [ ] Use `print()` in each file to display its processed result.

> Fully completing the Basic Requirements earns **16/20 marks, or 80%**.

## Basic Assessment — 16 Marks

| Assessment Item | Criteria | Marks |
|---|---|---:|
| Name Formatting | Correctly removes unnecessary whitespace, removes the comma, reorders the first and last name, and applies appropriate capitalization. | 3 |
| Title Formatting | Correctly removes the unwanted punctuation and whitespace and formats the result using title capitalization. | 4 |
| List Formatting | Correctly separates the comma-separated items, converts them to uppercase, and joins them using ` | `. | 3 |
| Number Processing | Correctly cleans and separates the numeric values, converts them to integers, and calculates the total and average. | 4 |
| Appropriate String Processing | Uses appropriate string methods and numeric conversion to process `string_to_process` rather than manually replacing it with the expected result. | 2 |
|  | **Total** | **16** |

## Advanced Premise

Combine the four types of processing from the Basic activity into a single interactive program.

The program should first ask the user **how they would like their string to be processed**. It should then ask the user to enter a new string and apply the selected processing method.

The available options should be:

```text
1. Format a Name
2. Format a Title
3. Format a List
4. Process Numbers
```

You can begin by copying the processing code from your four Basic files into `main.py` and modifying it so that each option works with user input instead of the original `string_to_process` values.

The program should continue running safely when the user enters invalid information rather than crashing.

## Advanced File Structure

Your starter folder will contain:

```text
advanced/
└── main.py
```

## Advanced Requirements

* [ ] Display the four processing options and use `input()` to ask the user which option they want to use.
* [ ] Ask the user for a new string and apply the selected processing method using the same rules as the corresponding Basic challenge.
* [ ] Ensure that all four processing options work with new input rather than relying on the original Basic strings.
* [ ] Validate the menu selection and any input that must follow a specific format, such as a name requiring a first and last name or numbers requiring numeric values.
* [ ] Use error handling so invalid input does not cause the program to crash.
* [ ] When invalid input is entered, clearly explain the problem and allow the user to try again.

Interacting with the program could look like this (as an example):

```text
Choose how you would like to process a string:

1. Format a Name
2. Format a Title
3. Format a List
4. Process Numbers

Enter your choice: 3
Enter the string to process: apples,oranges,bananas,grapes

Processed String:
APPLES | ORANGES | BANANAS | GRAPES
```

Another example could be:

```text
Enter your choice: 4
Enter the string to process: 12,18,25,5

Total: 60
Average: 15.0
```

## Advanced Assessment — 4 Marks

| Assessment Item | Criteria | Marks |
|---|---|---:|
| Interactive Processing | Allows the user to select any of the four processing options, enter a new string, and receive the correctly processed result. | 1 |
| Reusable Processing | Successfully adapts the processing from the Basic activity so all four methods work with different user-provided values. | 1 |
| Input Validation | Checks menu selections and formatted input where necessary and prevents invalid values from being processed. | 1 |
| Error Handling and Recovery | Prevents expected input errors from crashing the program, explains invalid input, and allows the user to try again. | 1 |
|  | **Total** | **4** |