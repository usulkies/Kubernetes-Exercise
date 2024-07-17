# Kubernetes-Exercise

In this exercise, you are required to create a small event-driven application, while displaying knowledge of event-driven architecture, Kubernetes and observability

Prerequisites:

1. A Kubernetes cluster (you can use a local cluster or if you have access to a more mature installation, that is also great, just make sure you have the proper permissions required)
2. Knowledge of Kubernetes and Argo Workflows

Tasks:
1. Using ArgoWorkflows and ArgoEvents, create an eventsource that triggers a workflow. This worklow should receive an input from the eventsource, printing the message sent to the screen.
2. Add another step to the workflow, it should return the number of namespaces in the cluster you are currently using.
3. The workflow should have 2 more steps, one running if the message from the first task contained the word elden, the other running if it didn't. They both print 1 or 2 (doesn't really matter)
4. Now you are required to add a new event, that is triggered at the same time as the first step. This new event executes a different workflow. This workflow runs the same step as task 2.
5. Add a small tracing mechanism to allow us to track requests between the 2 different workflows. You do not need to use a third party app.


