# Registration Form App – Jetpack Compose

This Android application is a simple Registration Form developed using Jetpack Compose and Material 3.  
It allows users to enter personal details, select a role, and validates the input before registration.


## Project Description

The Registration Form App collects the following details from the user:
- Name
- Email
- Phone Number
- Role (Student / Professional)

If any field is left empty, an error message is shown using a Snackbar.  
If all fields are filled, a success message is displayed.


## Technologies Used

- Kotlin
- Jetpack Compose
- Material 3
- Android Studio
- Kotlin Coroutines


## File Structure

com.example.compose
│
├── RegestrationFormCa2.kt
│ ├── RegestrationFormCa2 (Main Activity)
│ ├── RegistrationApp (Composable Function)
│ └── GreetingPreview10 (Preview Function)


## App Workflow

1. Application starts from `RegestrationFormCa2`.
2. `RegistrationApp()` is set as the UI using `setContent`.
3. User enters name, email, phone number, and selects a role.
4. On clicking the Register button:
   - If any field is empty, a Snackbar shows an error message.
   - If all fields are filled, a Snackbar shows a success message.


## Validation Logic



name.isBlank()
email.isBlank()
phone.isBlank()
role.isBlank()


If any of the above conditions is true, registration is not allowed.

## UI Components Used

- Scaffold
- Column
- Row
- Text
- TextField
- RadioButton
- Button
- SnackbarHost
- MaterialTheme


## Preview Support

The app includes a Compose Preview to test the UI without running the application.

## How to Run the Project

1. Open the project in Android Studio.
2. Ensure Jetpack Compose is enabled.
3. Run the application on an emulator or physical device.


## Future Enhancements

- Email format validation
- Phone number length validation
- Database integration (Room / Firebase)
- Navigation to another screen after registration

## Conclusion

This project demonstrates the use of Jetpack Compose for building modern Android UIs with proper state handling and validation.


## License

This project is created for educational purposes and can be freely modified and reused.

## Package Name

