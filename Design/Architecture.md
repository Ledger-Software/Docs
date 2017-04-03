# Project Architecture

We use the Model View Controller (MVC) pattern to handle communication between the User Interface (UI) and the backend. This prevents the UI from having any knowledge of the backend architecture, which should help in separation of concerns.

## User Interface
The user interface is created with JavaFX. It runs independently of the backend by creating asynchronous calls to the controller to modify stored data. The UI was built with FXML and its behavior is determined by UI component specific controllers.

## Backend
The backend is responsible for the manipulation of persisted data. It responds to calls made by the controller to make data model changes. The backend also handles relational complexity with regards to the application's data models. This includes things like database communication and file imports.

## Controller
The controller is responsible for tying together the user interface and the backend. It responds to the calls from the user interface by asynchronously transferring these calls to the backend. This allows the UI to make data model changes without becoming unresponsive.
