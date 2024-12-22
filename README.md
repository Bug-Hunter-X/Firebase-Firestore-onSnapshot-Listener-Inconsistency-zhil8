# Firebase Firestore onSnapshot Listener Inconsistency

This repository demonstrates an unusual bug encountered with Firebase Firestore's `onSnapshot` listener.  The issue involves intermittent data updates; even with offline persistence enabled, the UI doesn't always reflect changes in the Firestore database.

The `firestoreBug.js` file shows the original code with the problematic `onSnapshot` listener.  `firestoreBugSolution.js` provides a corrected version which uses a more robust approach to handle potential issues with listener consistency. The solution uses multiple error handling techniques and ensures data is correctly handled even in case of failures.

## Steps to Reproduce

1. Clone this repository.
2. Configure a Firebase project.
3. Install necessary dependencies: `npm install firebase`
4. Replace placeholders in the code with your Firebase configuration.
5. Run `firestoreBug.js` and observe intermittent data updates.
6. Run `firestoreBugSolution.js` to see the improved behavior.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or alternative solutions.