# Address Book Application

This is a simple address book application in Python that allows you to manage contacts, including their names, phone numbers, and birthdays. The application also supports saving and loading the address book data using serialization with the `pickle` module.

## Features

1. **Add Contacts**: Add a new contact with name, phone number, and optional birthday.
2. **Edit Contacts**: Update phone numbers for an existing contact.
3. **View Contacts**: Display all saved contacts or search for a specific contact.
4. **Birthday Reminders**: Show upcoming birthdays within the next 7 days.
5. **Data Persistence**: Automatically saves the address book to a file (`addressbook.pkl`) and restores it on the next run.

---

## How to Run

### Prerequisites

- Python 3.x installed on your machine.

### Steps to Run

1. Clone or download this repository.
2. Open a terminal or command prompt.
3. Navigate to the folder containing the files.
4. Run the application with the following command:
   ```bash
   python main.py
   ```

---

## Commands

| Command                                   | Description                                                          |
| ----------------------------------------- | -------------------------------------------------------------------- |
| `hello`                                   | Displays a greeting message.                                         |
| `add <name> <phone> <birthday>(optional)` | Adds a new contact. Optionally, you can add a birthday (DD.MM.YYYY). |
| `change <name> <old_phone> <new_phone>`   | Updates a contact's phone number.                                    |
| `phone <name>`                            | Displays the phone numbers for the specified contact.                |
| `add-birthday <name> <birthday>`          | Adds or updates the birthday for a contact.                          |
| `show-birthday <name>`                    | Displays the birthday of the specified contact.                      |
| `all`                                     | Displays all saved contacts.                                         |
| `birthdays`                               | Shows contacts with upcoming birthdays in the next 7 days.           |
| `close` or `exit`                         | Exits the program and saves the address book data to a file.         |

---

## Data Persistence

The application saves all contact data to a file named `addressbook.pkl` using the `pickle` module. When you restart the application, it automatically loads the data from this file.

- **File Location**: `addressbook.pkl` is created in the same directory as the program.
- **File Format**: The file is a binary file serialized with `pickle`.

---

## Notes

- Phone numbers must be exactly 10 digits.
- Birthdays must follow the format `DD.MM.YYYY`.
- Ensure the `addressbook.pkl` file is in the same directory to restore data during application startup.
