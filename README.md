### 1. Project Overview

EcoTrack Vision is an AI-powered campus sustainability monitoring prototype designed to promote a cleaner, greener, and more resource-efficient campus. The system aims to identify visible environmental issues, manage campus maintenance reports, and encourage the responsible use of essential resources such as water and electricity.

The platform provides a centralized dashboard where students, faculty members, maintenance staff, and administrators can interact with the system according to their roles. By combining camera-based object detection, issue reporting, resource readings, and maintenance status tracking, EcoTrack Vision demonstrates how technology can support sustainable campus management.

### 2. AI Camera and Object Detection

One of the main features of EcoTrack Vision is its AI Monitoring Centre. It allows users to activate a camera in authorized common campus areas, such as classrooms, computer laboratories, corridors, canteen common areas, and gardens.

The system uses TensorFlow.js and the COCO-SSD object detection model to identify common objects visible through the camera. When an object is detected, the system displays a bounding box around it, along with its predicted label and confidence score.

For example, the AI model may recognize objects such as bottles and cups. If a detected object might indicate a waste-related issue, the user can create a report for maintenance staff to inspect.

However, object detection alone cannot confirm whether an object is litter or whether a dustbin is overflowing. Therefore, human verification is required before taking action.

### 3. Campus Issue Reporting System

EcoTrack Vision allows users to report environmental and maintenance-related issues by selecting a campus location, choosing the suspected problem, uploading a photograph, and providing additional details.

The prototype supports reports related to:

* Water leakage and water wastage.
* Taps that may have been left running.
* Overflowing dustbins and litter.
* Lights and fans that may have been left on.
* Other visible campus maintenance issues.

After submission, the system generates a demonstration analysis result and adds the issue to the recent reports section. Each report includes the location, issue description, priority, and current status.

### 4. Maintenance and Report Management

The dashboard includes a report management section that helps track reported issues. Reports can be marked as Open, In Progress, or Resolved.

This feature helps demonstrate how maintenance staff can prioritize problems, monitor pending complaints, and update their progress. The dashboard also displays summary statistics, including total reports, open alerts, and resolved issues.

### 5. Water and Electricity Resource Monitoring

The Resource Readings section allows users to record water consumption readings in litres and electricity readings in kilowatt-hours (kWh).

These readings can help maintain a basic record of resource usage. In a real-world implementation, the system could be extended to receive readings from smart meters or IoT sensors installed in campus buildings, hostels, canteens, laboratories, and other departments.

The current prototype records readings entered by the user. It does not automatically measure electricity or water consumption.

### 6. User Roles and Access

The website provides a role-selection interface for three types of users:

* **User:** Students and faculty members who can report campus issues.
* **Maintenance:** Staff responsible for monitoring reports and updating issue statuses.
* **Admin:** An administrator role intended for system management.

The prototype demonstrates login and registration interfaces. However, its current authentication system stores account information in the browser rather than using a secure backend server.

### 7. Data Storage and Technology

EcoTrack Vision is implemented as a single HTML file containing HTML, CSS, and JavaScript.

Its main technologies include:

* **HTML:** Structures the website and its dashboard.
* **CSS:** Provides the visual design and responsive layout.
* **JavaScript:** Controls authentication interfaces, reporting, dashboard statistics, and camera functionality.
* **TensorFlow.js:** Enables machine-learning functionality directly in the browser.
* **COCO-SSD:** Detects common objects in camera frames.
* **LocalStorage:** Stores demonstration data, including user accounts, issue reports, and resource readings, in the current browser.

Because this is a browser-based prototype, its stored data is not automatically shared across different devices or users.

### 8. Future Scope

EcoTrack Vision can be expanded into a more comprehensive campus sustainability platform by integrating:

* IoT-enabled electricity and water meters.
* AI-based waste classification models trained specifically for campus environments.
* Automated alerts for maintenance staff.
* Historical resource consumption reports and analytics.
* Campus building-wise and department-wise monitoring.
* Secure user authentication and centralized database storage.
* Authorized camera installations in suitable common areas.
* Separate modules for washroom cleanliness and odour monitoring using appropriate sensors and manual inspection.

These improvements could help transform the prototype into a practical campus resource management system.

### 9. Conclusion

EcoTrack Vision demonstrates how artificial intelligence, browser-based object detection, digital reporting, and resource monitoring can contribute to campus sustainability.

Its primary objective is to make environmental issues easier to report, improve maintenance coordination, encourage responsible resource usage, and support data-informed decisions.

The current version is a functional demonstration prototype rather than a fully deployed campus monitoring system. With secure backend development, real sensor integrations, suitable AI models, and centralized data storage, it could be developed further into a real-world campus sustainability solution.

