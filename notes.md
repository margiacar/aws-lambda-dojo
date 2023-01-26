# Good Points - (Programming Model)

- To save processing time on subsequent events, create reusable resources like AWS SDK clients during initialization. Once initialized, each instance of your function can process thousands of requests.

- Your function also has access to local storage in the /tmp directory. The directory content remains when the execution environment is frozen, providing a transient cache that can be used for multiple invocations.

- Use local storage and class-level objects to increase performance, but keep to a minimum the size of your deployment package and the amount of data that you transfer onto the execution environment.
