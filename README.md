Lucian Sandile Young
- Student Number: ST10039287
 
- Email: luyoung247@gmail.com
  
- ALT email: st10039287@vcconnect.edu.za

- Demo Video: https://youtu.be/lwjmlCZKlKA

----------------------------------------------------------------------------------------------------

# INTRODUCTION:

This is the Keep Your Word app. It is a task management application that aims to improve the daily task management of its users.
The application aims to fulfil this through the unique use of an AI chatbot support system that will guide and support users throughout their days.

----------------------------------------------------------------------------------------------------

# PURPOSE:

The purpose of this application is to improve the daily lives of its users. Artificial intelligence is growing 
with its influence every day. Integrating this robust support system could truly aid those that need to be kept 
accountable each day.

----------------------------------------------------------------------------------------------------

# APP CONFIGURATION PLUGINS:

plugins {
    id("com.android.application")
    id("org.jetbrains.kotlin.android")
    id("com.google.gms.google-services")
}

android {
    namespace = "com.lucian_young.keepyourword"
    compileSdk = 34

    defaultConfig {
        applicationId = "com.lucian_young.keepyourword"
        minSdk = 24
        targetSdk = 34
        versionCode = 1
        versionName = "1.0"

        testInstrumentationRunner = "androidx.test.runner.AndroidJUnitRunner"
    }
    //enables the view binding
    buildFeatures{

        viewBinding = true
        dataBinding = true

    }

    buildTypes {
        release {
            isMinifyEnabled = false
            proguardFiles(
                getDefaultProguardFile("proguard-android-optimize.txt"),
                "proguard-rules.pro"
            )
        }
    }
    compileOptions {
        sourceCompatibility = JavaVersion.VERSION_1_8
        targetCompatibility = JavaVersion.VERSION_1_8
    }
    kotlinOptions {
        jvmTarget = "1.8"
    }
}

dependencies {

    implementation("androidx.core:core-ktx:1.9.0")
    implementation("androidx.appcompat:appcompat:1.7.0")
    implementation("com.google.android.material:material:1.12.0")
    implementation("androidx.constraintlayout:constraintlayout:2.1.4")
    implementation("com.google.firebase:firebase-database-ktx:21.0.0")
    implementation("com.google.firebase:firebase-database:21.0.0")
    implementation("com.google.firebase:firebase-storage-ktx:21.0.0")
    testImplementation("junit:junit:4.13.2")
    androidTestImplementation("androidx.test.ext:junit:1.2.1")
    androidTestImplementation("androidx.test.espresso:espresso-core:3.6.1")

    // Import the BoM for the Firebase platform
    implementation("com.google.firebase:firebase-auth:23.0.0")
    implementation("com.google.firebase:firebase-bom:31.5.0")
    implementation("com.google.firebase:firebase-database-ktx:21.0.0")

    // Also add the dependency for the Google Play services library and specify its version
    implementation ("com.google.android.gms:play-services-auth:21.2.0")

    //facebook implementation
    implementation ("com.facebook.android:facebook-android-sdk:latest.release")

    //circular profile image
    implementation ("com.google.android.material:material:1.9.0")

    //for the Glide implementation
    implementation ("com.github.bumptech.glide:glide:4.12.0")
    annotationProcessor ("com.github.bumptech.glide:compiler:4.12.0")

    //for the chatbot
    implementation ("com.squareup.okhttp3:okhttp:4.9.3")
    implementation ("org.json:json:20210307")
    //implementation ("com.aallam.openai:openai-client:3.8.2")
}

----------------------------------------------------------------------------------------------------

# PROJECT CONFIGURATION:

buildscript {
    repositories{
        google()
        mavenCentral()
    }
    dependencies {
        //noinspection GradleDependency
        classpath("com.google.gms:google-services:4.3.15")
    }
}
// Top-level build file where you can add configuration options common to all sub-projects/modules.
plugins {
    id("com.android.application") version "8.1.4" apply false
    id("org.jetbrains.kotlin.android") version "1.9.0" apply false

}

----------------------------------------------------------------------------------------------------

# BUILT USING:

Android Studio
Giraffe Patch 4: 2022.3.1

- Empty Views Activity

all dependencies and plugins are included in the App and project configurations.

----------------------------------------------------------------------------------------------------

# DEVICE & SYSTEM REQUIREMENTS:

Device:

- API level 27 Operating System.
  
-  ARMv7 or ARM64 processor is recommended.
  
- 2 GB of RAM (4 GB or more recommended for better performance)
  
- At least 50 MB of free storage for app installation.
  
- Screen sizes: Small screens (e.g., 4.0 inches, 480x800) and above
  

----------------------------------------------------------------------------------------------------

# SPECIFICATIONS BEFORE RUNNING:

Before running the application, ensure that:

- Please make sure that the Android SDK is installed with support for the target API level.
  
- Make sure you are using an appropriate version of Gradle that is compatible with your Android Studio version.
  
- All required libraries and dependencies (e.g., Firebase, Glide, etc.) must be included in the build.gradle files and up to date.
  
Supported Devices: Ensure testing is performed on a range of devices, including:
- Minimum Android version (6.0) devices
- Recommended Android version (9.0) devices
- Different screen sizes (phones and tablets)

----------------------------------------------------------------------------------------------------

# ENGAGEMENT STRATEGY IMPLEMENTATION:

- Users can interact free with the chatbot via the chat section of the app

- Users can customize the profiles that they create.

- The application supports English, Afrikaans, and Zulu, and the user can change it in the settings tab.


----------------------------------------------------------------------------------------------------

# FAQs:

What is KeepYourWord?

- KeepYourWord is a time-tracking application designed to help users manage their tasks efficiently and keep track of their time commitments.
- It features a user-friendly interface with functionalities like task management, progress tracking, and profile customization.

What features does the app offer?

- The app will include task management, a chatbot for assistance, and user profile management, and will include statistics and analytics of completed tasks, as well as dark/light mode for user interface customization.

How can I change the app's language?

- You can change the app's language in the Settings section. Simply select your preferred language from the language options available in the dropdown menu.

----------------------------------------------------------------------------------------------------

# ACKNOWLEDGEMENTS:

I would like to acknowledge the support provided by the following platforms and individuals:

1. ChatGPT - For providing solutions to errors faced throughout development, as well as supportive design elements for the front-end dynamic resizing.

2. Android arctic (YouTube) - For aiding with the implementation of the chatbot API.

3. Coding with Zo (YouTube) - Guiding with the addition of light and dark themes.

----------------------------------------------------------------------------------------------------

# REFERENCES:

- Android Arctic (2023). Build Your Own ChatGPT Android App with Kotlin & OpenAI API: Step-by-Step Tutorial #chatgpt. [online] YouTube. Available at: https://www.youtube.com/watch?v=bLktoOzb4R0 [Accessed 30 Sep. 2024].
  
- Coding With Zo (2022). Dark & Light mode | Android Studio | Java. [online] YouTube. Available at: https://www.youtube.com/watch?v=_XN-c5Yz0wk [Accessed 30 Sep. 2024].
  
- ChatGPT. (2024). Response to user query on saving an uploaded image into a database in a Windows Forms application. OpenAI ChatGPT, 25 October. Available at: [https://chat.openai.com/](https://chatgpt.com/c/66f64791-5564-8000-b1ec-ad45802183dd).
  
- www.youtube.com. (n.d.). Bottom Navigation Bar - Android Studio | Fragments | Kotlin | 2023. [online] Available at: https://www.youtube.com/watch?v=L_6poZGNXOo [Accessed 13 May 2024].

- MontreeMT (2019). Food Menu Design to XML use CardView in Android Studio | Android Tutorial App UI | Speed Code. [online] YouTube. Available at: https://www.youtube.com/watch?v=_QgsZ0xd00Q [Accessed 30 Sep. 2024].

