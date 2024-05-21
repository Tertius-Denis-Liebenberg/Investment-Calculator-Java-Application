# Investment Calculator Application

This Java program is designed to serve as an investment calculator, utilizing Swing components to create a graphical user interface (GUI) for user interaction. The application allows users to input their investment details, such as the customer's name, the amount invested, the type of investment (moderate or aggressive), and the term of the investment (5, 10, or 15 years). It then calculates the investment report, displaying the original amount, the years invested, and the final amount after applying the interest.

## Key Components

### InvestmentPanel Class

- **Description**: Manages the UI components for collecting investment details from the user.
- **Components**:
  - Text fields for customer name and investment amount.
  - A combo box for selecting the investment type (moderate or aggressive).
  - Radio buttons for choosing the investment term (5, 10, or 15 years), grouped using a `ButtonGroup`.
- **Methods**:
  - **Constructor**: Initializes the components.
  - **createInvestmentPanel()**: Sets up the layout and adds all components to the panel.
  - **Getter and Setter Methods**: Allows access and modification of component values.

### InvestmentFrame Class

- **Description**: Manages the overall frame, including the menu bar and menu items.
- **Components**:
  - A menu bar with "File" and "Tools" menus.
  - Menu items for exiting the application, calculating investments, and clearing the form.
- **Method**: **showFrame()** initializes the frame, sets up the menu items with action listeners, and adds the `InvestmentPanel` to the content pane.

### MenuItemsAction Class

- **Description**: Handles actions triggered by menu items, such as exiting the application, calculating investments, and clearing the form.
- **Methods**:
  - **actionPerformed()**: Determines which menu item was clicked and executes the appropriate action.
  - **calculate()**: Calculates the investment amount based on the entered amount, investment type, and term.
  - **clear()**: Clears all text fields and resets the investment type selection.

### InvestmentCalculator Class

- **Description**: The main class that starts the application.
- **Method**: **main()** creates an instance of `InvestmentFrame` and displays it, starting the application.

## Additional Notes

- **Decimal Format**: Uses `DecimalFormat` to format the final investment amount, ensuring it's displayed with two decimal places.
- **Interest Calculation**: Assumes a fixed annual interest rate applied monthly. Interest rates vary depending on the investment type.
- **Error Handling**: Consider adding error handling for cases where the user enters non-numeric values or selects an invalid investment term.

## Author

**Tertius Denis Liebenberg**  

For any questions or feedback, please contact [tertiusliebenberg7@gmail.com].