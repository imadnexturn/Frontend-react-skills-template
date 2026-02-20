I have updated the Rules File to include the Universal "Hard Stop" Policy:

Strict Circuit Breaker Rules:

Universal Hard Stop: Execution must STOP IMMEDIATELY if ANY command (npm, git, npx, etc.) fails with an error code, system error, or crash.
Valid vs Invalid Red:
Invalid Red (STOP): Test runner crashes, file not found, compilation error.
Valid Red (PROCEED): Test runner executes successfully and reports specific Assertion Failures (e.g., "Expected X but found Y").
Prohibition: It is strictly FORBIDDEN to write implementation code if the previous command failed to execute properly.
This ensures the agent will never proceed on a broken or unstable foundation. All key TDD enforcement tasks are now complete.