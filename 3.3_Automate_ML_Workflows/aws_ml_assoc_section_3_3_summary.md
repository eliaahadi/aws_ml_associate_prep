# AWS ML Associate --- Section 3.3: Automate ML Workflows

This section covers automating end-to-end ML workflows for
repeatability, scalability, and MLOps integration. It includes SageMaker
Pipelines, Step Functions, and CI/CD with CodePipeline.

# Automation Tools

• SageMaker Pipelines --- native CI/CD for ML workflows (data prep →
training → deployment)

• Step Functions --- orchestrates workflows across AWS services,
integrates ML steps into larger business processes

• CodePipeline / CodeBuild --- standard CI/CD tools for integration with
ML deployments

# Best Practices

• Automate retraining when new data arrives or drift is detected

• Version datasets, code, and models for reproducibility

• Integrate with CloudWatch/Model Monitor for alerts and triggers

# Exam Tips

• SageMaker Pipelines = ML-native automation

• Step Functions = service orchestration beyond ML

• CI/CD with CodePipeline + CodeBuild supports production ML at scale
