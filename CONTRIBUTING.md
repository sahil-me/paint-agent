<!---
Copyright 2026 Sahíl Sharma. All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# Contribute to Paint Agent

Everyone is welcome to contribute, and we value every contribution. Code contributions are not the only way to support the project. Improving AI agent behavior, paint-product search, room planning, coverage calculations, user experience, performance, architecture, security, testing, Google Cloud integration, or documentation are all valuable ways to contribute to **Paint Agent**.

If you find this project helpful, consider sharing it with others, referencing it in your blogs or projects, discussing it on social platforms, or simply giving the repository a ⭐️ to support the project and the community.

**However you choose to contribute, please be mindful and respect our [Code of Conduct](https://github.com/sahil-me/paint-agent/blob/main/CODE_OF_CONDUCT.md).**

## Ways to contribute

There are several ways you can contribute to **Paint Agent**.

* **AI Agent Improvements:** Improve the agent's ability to understand paint-related questions, guide users through product selection, collect room details, and provide helpful responses.
* **Paint Product Search Improvements:** Improve retrieval of paint-product information, including product descriptions, prices, coverage rates, and other details available in the configured datasheets.
* **Room Planning Improvements:** Improve the process of collecting room names, dimensions, color preferences, doors, windows, and the number of paint coats.
* **Coverage Calculation Improvements:** Improve paint-coverage calculations, input validation, calculation accuracy, rounding, and explanations of estimated paint requirements.
* **Google ADK Improvements:** Improve agent instructions, tool usage, sub-agent integration, orchestration, session state, callbacks, and error handling.
* **Gemini and Vertex AI Improvements:** Improve model configuration, response quality, reliability, and integration with Google Cloud AI services.
* **Agent Search Improvements:** Improve search configuration, retrieval quality, relevance, and handling of missing or incomplete product information.
* **Agent Runtime Improvements:** Improve deployment configuration, reliability, permissions, authentication, and troubleshooting documentation.
* **UI/UX Improvements:** Improve the Chainlit interface, accessibility, usability, responsive behavior, conversation flow, loading states, and error messages.
* **Performance Optimization:** Improve response handling, tool execution, search performance, startup time, and overall application efficiency.
* **Security Improvements:** Help identify and address issues involving credentials, Google Cloud permissions, environment variables, data access, and configuration.
* **Documentation:** Improve the README, setup instructions, architecture documentation, deployment guidance, troubleshooting information, and examples.
* **Testing:** Add or improve tests for agent behavior, product retrieval, room planning, coverage calculations, session state, and application integration.

> All contributions are valuable to the project and its learning community. 🥰

## Submitting a bug-related issue or feature request

Feel free to open an issue when you encounter a bug or have an idea for improving **Paint Agent**. Include relevant error logs, screenshots, Python and dependency versions, environment details, or Google Cloud service information when appropriate.

Please check the existing issues before creating a new one. This helps avoid duplicate reports and makes it easier to track existing problems.

### Did you find a bug?

**Paint Agent** becomes more reliable through community feedback, issue reporting, testing, and meaningful contributions.

Before reporting an issue, please make sure the bug has not already been reported under the repository's **Issues** section.

When submitting a bug report, please include the following information:

* Your **operating system** and version.
* Your **browser** and version, if the issue relates to the Chainlit interface.
* Steps to reproduce the issue.
* A short description of the expected behavior and what actually happened.
* Relevant error messages or application logs.
* Python version and relevant dependency versions.
* The affected component, such as the root agent, search agent, room planner, or coverage calculator.
* Google Cloud service or deployment information, if applicable.
* Screenshots or screen recordings, if applicable.
* Any other information that may help reproduce or understand the issue.

Please **do not include API keys, passwords, authentication tokens, service-account credentials, `.env` files, temporary lab credentials, or other sensitive information** in an issue.

### Do you want a new feature?

If there is a new feature you'd like to see in **Paint Agent**, please open an issue and describe:

1. **Motivation**

   Explain the problem, limitation, or use case that the feature would address.

2. **Feature Description**

   Describe the proposed feature and how you would expect it to work.

3. **AI Agent Behavior**

   If the feature affects the AI agent, explain how it should influence product selection, tool usage, room planning, calculations, or responses.

4. **Paint Product Data**

   If the feature depends on paint-product information, explain what information is needed and how it should be retrieved or validated.

5. **Room Planning and Calculations**

   If the feature affects room dimensions, paint coverage, number of coats, or cost estimation, explain the expected behavior and relevant assumptions.

6. **User Experience**

   Explain how the feature would improve the user's painting-planning experience.

7. **Implementation Details**

   If you have an implementation idea, architecture suggestion, or code example, feel free to include it.

8. **Additional References**

   If the feature is inspired by an external project, article, design, or technical reference, please include the relevant link.

A clear and well-written feature request makes it easier to evaluate and discuss the proposal.

## Do you want to improve paint-product search?

Paint-product information is an important part of the agent's decision-making workflow.

You can contribute by:

* Improving the retrieval of paint-product information.
* Improving the relevance of search results.
* Improving how the agent uses product datasheets.
* Improving retrieval of product prices and coverage rates.
* Improving handling of missing or incomplete product information.
* Improving the accuracy of product comparisons.
* Improving the clarity of product descriptions.
* Improving error handling when search services are unavailable.
* Improving the agent's ability to distinguish retrieved facts from unsupported assumptions.

When modifying search behavior, ensure that product-related responses are grounded in available information. Avoid inventing prices, coverage rates, product specifications, or other details that are not supported by the configured source.

## Do you want to improve AI agent behavior?

Contributions that improve the agent's behavior are especially welcome.

Examples include:

* Improving agent instructions.
* Improving the understanding of user requests.
* Improving root-agent and sub-agent coordination.
* Improving tool selection and tool usage.
* Improving paint-product selection conversations.
* Improving follow-up questions.
* Improving room-detail collection.
* Improving session-state handling.
* Improving coverage-calculation workflows.
* Reducing hallucinations and unsupported claims.
* Improving conversational responses and explanations.
* Improving error handling.
* Improving the agent's ability to handle missing information.
* Improving callback logging and troubleshooting.
* Improving the transition between product selection and room planning.

Changes to AI behavior should be tested against representative painting scenarios to ensure that existing functionality is not unintentionally affected.

## Do you want to improve room planning or paint coverage calculations?

Room planning and coverage calculations are important parts of the Paint Agent workflow.

You can contribute by:

* Improving the collection and validation of room dimensions.
* Improving the handling of multiple rooms.
* Improving the handling of length, width, and height.
* Improving the handling of doors and windows where supported by the calculation logic.
* Improving the calculation of paintable surface area.
* Improving paint-coverage estimates.
* Improving calculations for multiple coats.
* Improving rounding and container-quantity estimates.
* Improving cost estimates when reliable product pricing is available.
* Improving explanations of calculation results.
* Adding tests for normal, boundary, and invalid inputs.
* Improving error handling when required room details are missing.

When modifying calculation logic, document the assumptions being used. For example, estimates can depend on room dimensions, openings, paint coverage rates, number of coats, and container sizes.

Any change to the calculation method should be tested against known examples to help verify that the results are correct.

## Do you want to improve Google ADK, Gemini, or Agent Runtime integration?

The project uses Google Agent Development Kit (ADK) and Google Cloud services to build and deploy the agent.

You can contribute by:

* Improving root-agent and sub-agent configuration.
* Improving agent instructions and tool integration.
* Improving session-state management.
* Improving callback handling and logging.
* Improving Gemini model configuration.
* Improving Vertex AI integration.
* Improving Agent Search integration.
* Improving Agent Runtime deployment instructions.
* Improving authentication and permissions documentation.
* Improving error handling for Google Cloud services.
* Improving configuration validation.
* Improving local development and troubleshooting guidance.

Infrastructure and permission changes should be reviewed carefully and tested in an appropriate development environment before being submitted.

Do not include temporary Google Skills lab credentials, project-specific secrets, or private configuration files in your changes.

## Do you want to improve the Chainlit interface?

The Chainlit interface provides a conversational way for users to interact with Paint Agent.

You can contribute by:

* Improving the layout and visual consistency.
* Improving accessibility and usability.
* Improving the conversation flow.
* Improving the presentation of paint-product information.
* Improving the presentation of room-planning questions.
* Improving the readability of coverage and cost estimates.
* Improving loading indicators and error messages.
* Improving responsive behavior across screen sizes.
* Improving documentation for running the interface.
* Adding screenshots or examples to explain user interactions.

Interface changes should be tested to ensure that users can continue to interact with the agent correctly.

## Do you want to add documentation?

We're always looking for improvements that make **Paint Agent** clearer and easier to understand.

You can contribute by:

* Fixing typos or grammatical errors.
* Improving the README.
* Improving setup instructions.
* Clarifying environment-variable configuration.
* Improving local development instructions.
* Documenting the agent architecture.
* Documenting the responsibilities of individual sub-agents.
* Documenting paint-product search.
* Documenting room-planning and coverage-calculation logic.
* Improving Google Cloud deployment instructions.
* Adding troubleshooting guidance.
* Adding examples of supported conversations.
* Improving testing instructions.
* Adding or improving screenshots and demo references.

Documentation contributions are especially appreciated when they help new contributors understand the project and get started safely.

## Fixing outstanding issues

If you notice an existing issue and have a fix in mind, feel free to **[start contributing](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)** and open a Pull Request.

### Making code changes

<details>
<summary><strong>Step-by-step contribution workflow</strong></summary>

#### 1. Fork the repository

Go to the [Paint Agent repository](https://github.com/sahil-me/paint-agent) on GitHub and click the **Fork** button.

#### 2. Clone your forked repository

Replace `<username>` with your GitHub username.

```bash
git clone https://github.com/<username>/paint-agent.git
```

Navigate into the project directory:

```bash
cd paint-agent
```

#### 3. Create a new branch

Create a separate branch for your feature or bug fix.

```bash
git checkout -b feature/your-feature-name
```

For a bug fix, you can use a name such as:

```bash
git checkout -b fix/issue-description
```

#### 4. Set up the Python environment

Make sure Python is installed. Create a virtual environment from the repository root:

```bash
python -m venv .venv
```

Activate the environment.

**Windows PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux:**

```bash
source .venv/bin/activate
```

#### 5. Install dependencies

Navigate into the project directory containing the agent and its dependency files:

```bash
cd adk_agent
```

Install the main project dependencies:

```bash
python -m pip install -r requirements.txt
```

If you are working on the Chainlit interface, install its dependencies as well:

```bash
python -m pip install -r chainlit_ui/requirements.txt
```

If a change affects a component with its own `requirements.txt`, install the dependencies required by that component.

> Dependency installation commands may need to be adjusted if the repository's dependency files change.

#### 6. Configure Google Cloud

Configure the Google Cloud project, region, authentication, required APIs, permissions, and other services needed for the component you are working on.

Follow the current project README and official Google Cloud documentation.

Some workflows may require access to Google Cloud services or a separately configured search application and data store. Contributors are responsible for using an appropriately authorized development environment.

> Never commit API keys, service-account credentials, access tokens, temporary lab credentials, or other secrets to the repository.

#### 7. Configure environment variables

Configure the required environment variables for your development environment. These may include values for:

- Google Cloud project.
- Google Cloud location.
- Model configuration.
- Resource bucket.
- Search application or engine configuration.

Use your own authorized development resources and follow the project's configuration instructions.

> Do not commit `.env` files or other files containing sensitive configuration. Keep secrets out of logs, screenshots, and Pull Request descriptions.

#### 8. Run the application locally

Follow the current README instructions to run the agent or launch the Chainlit interface.

For example, the project may be started using the appropriate Chainlit command from the directory containing the UI application:

```bash
chainlit run app.py
```

Verify the working directory and the project's current configuration before running the command. If your change only affects an individual agent component, use the appropriate ADK development or testing workflow instead.

Make sure the relevant component starts successfully before making or testing changes.

#### 9. Make your changes

- Develop the feature or fix the issue.
- Follow the existing project structure and coding conventions.
- Keep changes focused and maintainable.
- Avoid unrelated modifications.
- Document important assumptions.
- Test your changes locally before submitting a Pull Request.

#### 10. Run and test agent behavior

If your changes affect the agent or its tools, test representative scenarios such as:

- Greeting the user and explaining the agent's purpose.
- Asking about available paint products.
- Retrieving product prices and coverage information.
- Selecting a paint product.
- Collecting room names, dimensions, and color preferences.
- Calculating paint requirements for a room.
- Handling multiple coats or room details where supported.
- Handling missing or invalid inputs.
- Handling missing search results or unavailable services.
- Preserving relevant session state across conversation steps.

Verify that the agent uses the available product information and calculation logic correctly. Do not assume that a plausible-looking AI response is necessarily accurate.

#### 11. Commit your changes

From the repository root, review the files you have changed and stage only the intended changes.

```bash
git status
git add <file-or-directory>
git commit -m "Describe your change"
```

Avoid committing credentials, local configuration files, generated files, or unrelated modifications.

#### 12. Push to your fork

```bash
git push origin feature/your-feature-name
```

Replace the branch name if you used a different one.

#### 13. Create a Pull Request

Open your fork on GitHub and create a Pull Request targeting the original **Paint Agent** repository.

In your Pull Request description:

- Explain what you changed.
- Explain why the change was needed.
- Reference any related issue.
- Include screenshots for UI changes when appropriate.
- Describe changes to agent behavior or orchestration.
- Explain changes to search or calculation logic.
- Mention Google Cloud or deployment changes, if applicable.
- Describe the tests you performed.
- Mention any setup requirements or limitations.

#### 14. Address feedback

If the project maintainer leaves comments or requests changes, address the feedback and push the required updates to your branch.

Thank you for taking the time to review and improve the project!

</details>

## Contribution Guidelines

To keep the project maintainable and welcoming:

- Keep Pull Requests focused on a single feature, fix, or improvement whenever possible.
- Avoid unnecessary changes to unrelated files.
- Follow the existing code style and project structure.
- Test changes before submitting a Pull Request.
- Test AI-agent behavior when modifying agent logic.
- Verify calculation changes against known examples.
- Keep product-related responses grounded in available information.
- Document assumptions that affect coverage or cost estimates.
- Avoid introducing unsupported product specifications or prices.
- Do not commit secrets, API keys, credentials, `.env` files, or service-account files.
- Do not make unverified claims about deployment status or cloud resources.
- Provide clear commit messages and Pull Request descriptions.
- Include relevant screenshots, logs, or test results when appropriate.
- Be respectful and constructive when reviewing or discussing contributions.

## I want to become a maintainer of the project. How do I get there?

**Paint Agent** is a learning and demonstration project that explores AI-powered paint selection, room planning, paint-coverage calculations, and multi-agent development using Google ADK.

Contributors interested in improving AI agent behavior, Google ADK, Gemini, Vertex AI, Agent Search, room planning, calculation logic, Chainlit, performance, testing, security, documentation, and Google Cloud deployment are welcome.

If you are interested in contributing at a deeper level, consistently submitting meaningful improvements, reviewing Pull Requests, improving documentation, or helping maintain the project, feel free to get involved and collaborate.

Thank you for contributing to **Paint Agent**! 🖌

