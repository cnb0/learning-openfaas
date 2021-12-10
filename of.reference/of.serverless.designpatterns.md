Introduction

            What is serverless computing?
            No servers to manage
            Pay-per-invocation billing model
            Ability to automatically scale with usage
            Built-in availability and fault tolerance
            Design patterns
            When to use serverless
            The sweet spot
            Classes of serverless pattern
            Three-tier web application patterns
            ETL patterns
            Big data patterns
            Automation and deployment patterns
            Serverless frameworks
        
A Three-Tier Web Application Using REST

            Serverless tooling
            System architecture
            Presentation layer
            Logic layer
            Data layer
            Logic layer
            Application code and function layout
            Organization of the Lambda functions
            Organization of the application code
            Configuration with environment variables
            Code structure
            Function layout
            Presentation layer
            File storage with S3
            CDN with CloudFront
            Data layer
            Writing our logic layer
            Application entrypoint
            Application logic
            Wiring handler.py to Lambda via API Gateway
            Deploying the REST API
            Deploying the Postgres database
            Setting up static assets
            Viewing the deployed web application
            Running tests
            Iteration and deployment
            Deploying the entire stack
            Deploying the application code
        
A Three-Tier Web Application Pattern With GraphQL

            Introduction to GraphQL
            System architecture
            Logic layer
            Organization of the Lambda functions
            Organization of the application code
            Function layout
            Presentation layer
            Writing the logic layer
            Implementing the entry point
            Implementing GraphQL queries
            Implementing GraphQL mutations
            Deployment
            Viewing the deployed application
            Iteration and deployment
        
Integrating Legacy APIs With The Proxy Pattern

            AWS API Gateway introduction
            Simple proxy to a legacy API
            Setting up a pass-through proxy
            Deploying a pass-through proxy
            Transforming responses from a modern API
            Method execution flow
            Setting up example
            Setting up a new resource and method
            Setting up Integration Request
            Setting up Integration Response
            Complex integration using a Lambda function
            Implementing the application code
            Setting up a new resource and method
            Migration techniques
            Staged migration
            Migrating URLs
        
Scaling Out With The Fan-Out Pattern

            System architecture
            Synchronous versus asynchronous invocation
            Resizing images in parallel
            Setting up the project
            Setting up trigger and worker functions
            Setting up permissions
            Implementing the application code
            Testing our code
            Alternate Implementations
            Using notifications with subscriptions
            Using notifications with       s
        
Asynchronous Processing With The Messaging Pattern

            Basics of queuing systems
            Choosing a   queue     service
            queues versus streams
            Asynchronous processing of Twitter streams
            System architecture
            Data producer
            Mimicking daemon processes with serverless functions
            Data consumers
            Viewing results
            Alternate Implementations
            Using the Fan-out and Messaging Patterns together
            Using a queue as a rate-limiter
            Using a dead-letter       
        
Data Processing Using The Lambda Pattern

            Introducing the lambda architecture
            Batch layer
            Speed layer
            Lambda serverless architecture
            Streaming data producers
            Data storage
            Computation in the speed layer
            Computation in the batch layer
            Processing cryptocurrency prices using lambda architecture
            System architecture
            Data producer
            Speed layer
            Batch layer
            AWS resources
            Data producer
            Speed layer
            Batch layer
            Results
        
The MapReduce Pattern

            Introduction to MapReduce
            MapReduce example
            Role of the mapper
            Role of the reducer
            MapReduce architecture
            MapReduce serverless architecture
            Processing Enron emails with serverless MapReduce
            Driver function
            Mapper implementation
            Reducer implementation
            Understanding the limitations of serverless MapReduce
            Memory limits
            Storage limits
            Time limits
            Exploring alternate implementations
            AWS Athena
            Using a data store for results
            Using Elastic MapReduce
        
Deployment And CI/CD Patterns

            Introduction to CI/CD
            CI
            CD
            Setting up unit tests
            Code organization
            Setting up unit tests
            Setting up CI with CircleCI
            Configuring CircleCI builds
            Setting up environment variables
            Setting up CD and deployments with CircleCI
            Setting up Slack notifications
            Setting up a CircleCI badge
            Setting up deployments
            Setting up AWS credentials
            Setting up environment variables
            Executing deployments
        
Error Handling And Best Practices

            Error tracking
            Integrating Sentry for error tracking
            Integrating Rollbar
            Logging
            Structuring log messages
            Digesting structured logs
            Cold starts
            Keeping cloud functions warm
            AWS Lambda functions and VPCs
            Start-up times for different languages
            Allocating more memory
            Local development and testing
            Local development
            Learning about testing locally
            Managing different environments
            Securing sensitive configuration
            Encrypting variables
            Decrypting variables
            Trimming AWS Lambda versions
