# Password Generator

A simple and secure command-line password generator written in Python that creates strong, customizable passwords based on user preferences.

## Features

- **Customizable Length**: Generate passwords of any length (minimum 4 characters)
- **Character Type Selection**: Choose which character types to include:
  - Lowercase letters (always included)
  - Uppercase letters
  - Special characters
  - Digits
- **Guaranteed Character Types**: Ensures at least one character from each selected type is included
- **Random Shuffling**: Final password is randomly shuffled for maximum security
- **Input Validation**: Validates user input to prevent errors

## Requirements

- Python 3.x
- No external dependencies required (uses only built-in Python modules)

## Installation

1. Clone or download this repository
2. Navigate to the `password_generator` directory
3. Run the script directly with Python

## Usage

Run the password generator:

```bash
python password_generator.py
```

The program will prompt you for:
1. **Password length**: Enter a number (minimum 4 characters)
2. **Include uppercase letters**: Type "yes" or "no"
3. **Include special characters**: Type "yes" or "no" 
4. **Include digits**: Type "yes" or "no"

### Example Session

```
Enter the desired password length: 12
Include uppercase letters? (yes/no): yes
Include special characters? (yes/no): yes
Include digits? (yes/no): yes
Kj8#mN2$pL9x
```

## How It Works

1. **Input Collection**: Gathers user preferences for password length and character types
2. **Character Pool Creation**: Builds a pool of available characters based on user selections
3. **Required Characters**: Ensures at least one character from each selected type is included
4. **Random Generation**: Fills the remaining length with random characters from the pool
5. **Shuffling**: Randomly shuffles the final password for enhanced security
6. **Output**: Displays the generated password

## Security Features

- Uses Python's `random` module for cryptographically secure random number generation
- Guarantees inclusion of selected character types
- Random shuffling prevents predictable patterns
- Input validation prevents invalid inputs

## Error Handling

The program includes error handling for:
- Invalid length input (non-numeric values)
- Length less than 4 characters
- Invalid yes/no responses

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve this password generator.

## Disclaimer

This password generator is designed for educational and personal use. For critical applications requiring high-security passwords, consider using established password management tools.
