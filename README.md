📱 Registration Form App (Jetpack Compose)

A simple Android Registration Form built using Jetpack Compose and Material 3.
This app collects user details and validates input before showing feedback using a Snackbar.

🚀 Features

Modern UI using Jetpack Compose

Material 3 design components

User input fields:

Name

Email

Phone Number

Role selection using Radio Buttons

Student

Professional

Input validation

Snackbar messages for:

Missing fields

Successful registration

Preview support using @Preview

🛠️ Tech Stack

Language: Kotlin

UI Toolkit: Jetpack Compose

Design System: Material 3

Architecture: Single Activity (Compose-based)

Async Handling: Kotlin Coroutines

📂 Project Structure
com.example.compose
│
├── RegestrationFormCa2.kt
│   ├── RegestrationFormCa2 (Activity)
│   ├── RegistrationApp (Composable)
│   ├── GreetingPreview10 (Preview)

🧩 How the App Works

App launches RegestrationFormCa2 activity.

RegistrationApp() composable is set as the UI.

User enters:

Name

Email

Phone number

Selects a role

On clicking Register:

If any field is empty → Snackbar shows an error message.

If all fields are filled → Snackbar shows success message.

🖼️ UI Components Used

Scaffold

Column, Row, Spacer

TextField

RadioButton

Button

SnackbarHost

MaterialTheme

🔍 Validation Logic
if (name.isBlank() || email.isBlank() || phone.isBlank() || role.isBlank()) {
    // Show error snackbar
} else {
    // Show success snackbar
}

🧪 Preview

The app includes a Compose preview:

@Preview(showBackground = true)
@Composable
fun GreetingPreview10() {
    RegistrationApp()
}


This allows UI testing directly inside Android Studio without running the app.

▶️ How to Run

Open the project in Android Studio

Make sure:

Kotlin is enabled

Jetpack Compose is properly configured

Click Run ▶️

Test the registration form on an emulator or real device

📌 Future Enhancements (Optional)

Email & phone number format validation

Save data using Room or Firebase

Add dropdown for role selection

Navigation to another screen after successful registration

Dark mode support

📜 License

This project is created for educational purposes and can be freely modified and reused.
