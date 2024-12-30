# Expo CLI Development Server Intermittency

This repository demonstrates a bug encountered with the Expo CLI, where the development server randomly stops responding without providing clear error messages. The issue is intermittent and affects multiple projects, hindering the development workflow.

## Reproduction Steps

1. Clone this repository.
2. Navigate to the project directory.
3. Run `expo start`.
4. Observe the development server for periods of unresponsiveness.  There's no specific trigger; it appears random.

## Expected Behavior

The development server should consistently remain responsive unless an actual error occurs in the application code or a related process.

## Actual Behavior

The development server intermittently stops responding.  The browser shows a loading state indefinitely, and the CLI provides no useful error messages.  A manual restart of the server is required to resume development.

## Solution

The solution, detailed in the `expoBugSolution.js` file is often a combination of clearing the cache and restarting the system.  Sometimes checking for conflicting ports or processes running on the development server is also necessary.  If the issue persists please file a bug report in the Expo repository.