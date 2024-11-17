Capstone-Project-Peer-Review

**Are there unit tests for the API?**
Unit Testing:-
API Unit Tests: Verifies the reliability and expected functionality of API endpoints. Test cases may include:
Valid requests (e.g., correct inputs and outputs).
Edge cases (e.g., malformed requests or missing data).
Error handling and response times.

**Are there unit tests for the model?**
Model Unit Tests: Checks the internal logic of the model:

Does the model handle inputs of varying types and sizes gracefully?
Are predictions reasonable across edge cases and normal inputs?

**Are there unit tests for the logging?**
Logging Unit Tests: Ensures:

Errors, warnings, and events are correctly logged.
Logging adheres to required formats and contains useful information for debugging.
Run All Tests Together: A single script to run all unit tests efficiently:

**Can all of the unit tests be run with a single script and do all of the unit tests pass?**
Ensures consistency.
Confirms all tests pass in a clean state.

**Is there a mechanism to monitor performance?**
Performance Monitoring
Validates whether tools are implemented to track model performance in production.
Examples might include:
Response times.
Accuracy drift over time.
Alerts for anomalies in API usage or model outputs.

**Was there an attempt to isolate the read/write unit tests from production models and logs?**
Read/Write Test Isolation
Assesses whether tests that interact with production models or logs are isolated to prevent unintended consequences:
Sandboxed environments.
Use of mock data for testing.

**Does the API work as expected? For example, can you get predictions for a specific country as well as for all countries combined?**
API Functionality
Evaluates the API’s usability and versatility:
Can it return predictions for both specific and aggregated inputs (e.g., specific countries or global data)?
Does it support scalability?

**Does the data ingestion exists as a function or script to facilitate automation?**
Automated Data Ingestion
Confirms the existence of scripts or functions to automate data ingestion:
Does it handle varying data formats or types?
Is it robust to common issues like missing or corrupt data?

**Were multiple models compared?**
Model Comparison
Assesses whether multiple models were evaluated before finalizing one:
Were baseline models (e.g., linear regression) compared against advanced models?
Were metrics used to make comparisons clear?

**Did the EDA investigation use visualizations?**
Exploratory Data Analysis (EDA)
Checks if EDA included relevant visualizations:
Correlation matrices.
Histograms, box plots, or scatter plots.
Time series trends, if applicable.

**Is everything containerized within a working Docker image?**
Containerization with Docker
Confirms the workflow is fully containerized:
Is the Docker image complete and functional?
Can it be used to deploy the project seamlessly in different environments?

**Did they use a visualization to compare their model to the baseline model?**
Model vs. Baseline Comparison (Visualization)
Verifies the inclusion of visual tools to compare the chosen model with the baseline:
Example: A bar chart or ROC curve showing performance improvements.
Should provide clarity to non-technical stakeholders.
