Serilog in ASP.NET Core MVC

📌 Introduction

This project demonstrates how to integrate Serilog for structured logging in an ASP.NET Core MVC application. Serilog allows logging to various outputs, including the console and a file, with support for structured logging.

🚀 Features

Logs requests and responses automatically.

Captures unhandled exceptions.

Supports logging to both Console and File.

Configurable log levels via appsettings.json.

Rolling file logs stored in /logs directory.

🔧 Setup & Installation

1️⃣ Clone the Repository

2️⃣ Install Dependencies

Ensure you have the required NuGet packages installed:

Alternatively, install via NuGet Package Manager:

Serilog.AspNetCore

Serilog.Settings.Configuration

Serilog.Sinks.Console

Serilog.Sinks.File

3️⃣ Configure Serilog

Modify Program.cs to set up Serilog:

4️⃣ Configure Logging in appsettings.json

Add this configuration under "Serilog":

5️⃣ Run the Application

📝 Log Output Example

After running the project, the console will display logs like this:

📁 Logs in File (logs/log-YYYYMMDD.txt)

🔧 Customization

Adjust Logging Level

Modify MinimumLevel in appsettings.json to Debug, Warning, or Error:

Filter Out Microsoft/System Logs

🛠️ Troubleshooting

Issue: System.IO.InvalidDataException: 'Failed to load configuration from file 'appsettings.json'.'

Ensure appsettings.json is formatted correctly.

Run dotnet clean && dotnet build to refresh dependencies.

🎯 Contributing

Pull requests are welcome! If you find any issues, feel free to open an issue.
