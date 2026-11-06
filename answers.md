# Assignment: Build and Call Your Own MCP Tool

## 1. How many tools were available?

- Part 1: The MCP server initially provided **8 tools**.
- Part 3: After adding the `predict_both` tool, the server provided **9 tools**.

## 2. How many disagreements occurred?

The Logistic Regression and KNN models disagreed on **8 out of 114 test patients**.

## 3. Which model was correct for each disagreement?

| Patient | True Diagnosis | Logistic Regression | KNN | Correct Model |
|---|---|---|---|---|
| 3 | Benign | Benign | Malignant | Logistic Regression |
| 25 | Benign | Benign | Malignant | Logistic Regression |
| 48 | Benign | Benign | Malignant | Logistic Regression |
| 53 | Malignant | Benign | Malignant | KNN |
| 76 | Malignant | Malignant | Benign | Logistic Regression |
| 80 | Benign | Benign | Malignant | Logistic Regression |
| 99 | Benign | Benign | Malignant | Logistic Regression |
| 102 | Malignant | Malignant | Benign | Logistic Regression |

## 4. Which model was right more often?

Among the 8 disagreement cases:

- Logistic Regression was correct in 7 cases.
- KNN was correct in 1 case.

Therefore, Logistic Regression performed better on the disagreement cases.

## 5. Why are triple-quoted descriptions important?

Triple-quoted descriptions provide information about what a tool does, its purpose, and how it should be used. They help developers and MCP clients understand the tool's functionality.

## 6. Why should we log tool calls?

Logging tool calls helps track which tools were used, when they were called, and whether they succeeded or failed. It is useful for debugging, monitoring, auditing, and troubleshooting.