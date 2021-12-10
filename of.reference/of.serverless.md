Introduction To Serverless
     
            What Is Serverless?
            History of Serverless
            The Cloud Provider Landscape
            Reliability, Availability, Disaster Recovery
            Strengths of Serverless
            Increased Scalability, Security, and Reliability
            You Only Pay for What You Use
            Saving Time and Money on Managing Servers
            Improved Developer Productivity
            Decreased Management Responsibilities
            Convenient Integrations
            Weaknesses of Serverless
            The Cold (Start) War
            Compute Time
            VPC/Network Issues
            Application Size
            Potential to Be More Expensive
            Vendor Lock-In
            Complex Debugging
            When Does It Make Sense to Use Serverless?
            When Is Serverless Compute Not Right for You?

I. The Path To Production
     
1. Distributed Systems
     
            What Is a Distributed System?
            Why Do We Want a Distributed System?
            The Harsh Realities of Distributed Systems
            The Physical World
            Missing Messages
            Unreliable Clocks
            Cascading Failures
            Unexpected Ordering
            Idempotency
            What Am I Responsible For?
            What Do You Need to Consider When Designing a Distributed System?
            Loose Coupling (or Decoupling)
            Fault Tolerance
            Generating Unique (Primary) Keys
            Planning for Idempotency
            Two-Phase Changes
   
2. Microservices
     
            Why Do You Want to Use Microservices?
            Improved Developer Velocity
            Increased Developer Freedom
            Issues with Microservices
            Increased Complexity
            Proper DevOps Practices and Resources Needed
            Challenges with Local Development and Testing
            How Do You Use Microservices Effectively?
            Consistent Interfaces
            Loosely Coupled
            How Micro Is a Microservice?
            Choosing Between Monoliths and Microservices
            When Should You Use a Monolith?
            When Do You Want to Use Microservices?
   
3. Serverless Architecture And Patterns
     
            The Role of an Architect
            What Do You Need to Know to Be an Architect?
            Making Decisions
            What Kinds of Decisions?
            Documenting Your Decisions
            How Do We Make Decisions?
            When Do We Make Decisions?
            Cloud Provider Components
            Streams
            Queues    s
            Buckets
            Compute
            Datastores
            Identity Service
            API Gateways
            GraphQL
            Networking
            State Machines
            Logging
            Monitoring and Alerting
            Events from Your Cloud Provider
            Periodic Invocations
            Patterns
            Example 1: Serverless Monolith
            Example 2: Incoming Webhook
            Example 3: Using Your Cloud Provider for User Authentication
            Example 4: Generic Background Task Pattern
            Example 5: Streaming Extract, Transform, Load
            Example 6: Create Your Own Polling Integration
            Example 7: Processing Files and Images
            Example 8: Migration Service Pattern
            Example 9: Fanning Out
   
4. Interfaces
     
            Interfaces: Some Assembly Required
            The Message
            The Protocol
            The Contract
            Serverless Interfaces
            Automatic Retries and Dead Letter      s
            Finite Versus Infinite Scale
            Designing Your Interfaces
            Messages/Payloads
            Sessions and Users/Auth
            Avoid Unbounded Requests
            Interface Versus Implementation
            Lines with Logic
            Designing the Unhappy Path
            Validating Input
            Failures
            Strategies for Integrating with Other Services
            Time-Outs
            Retries
            Exponential Backoff
            Webhooks
            Evaluating External Services
            Rate Limits
   
II. The Tools
     
5. The Serverless Framework
     
            Why Use the Serverless Framework?
            When the Serverless Framework Isn’t for You
            AWS Is the Only First-Class Citizen
            AWS CloudFormation Is Not Perfect
            Relying on Strangers for Your Infrastructure
            What to Know Before You Start
            YAML
            Node.js
            Cloud Resources and Permissions
            Infrastructure Templates
            Production Secrets
            .gitignore
            The Components of a serverless.yml File
            Provider
            Environment
            Functions
            Resources
            Package
            Plug-Ins
            Custom
            Namespacing for Sanity and Security
            Using the serverless Command
            Installing Serverless
            Setting Up Serverless with Credentials
            Pulling in Templates Using serverless install
            Inspecting the Package of Our Sample Project (What’s Inside)
            Deployment
            Invoking the Function, and Viewing Logs
            Rollbacks
            Destroying the Service
            Deployment Packages
            Real-World serverless.yml
            Setting Environment Variables
            Modify Permissions
   
6. Monitoring, Observability, And Alerting
     
            What Is Monitoring?
            Why Do We Need Monitoring?
            How Does Monitoring Relate to Serverless?
            The On-Ramp to Automation
            What Are My Options?
            Hosted SaaS Offerings
            Self-Hosted and Open Source
            Components of Monitoring
            Metrics
            Charts/Graphs
            Dashboards
            Alerts/Alarms
            A Selection of Advanced Practices
            Heartbeats
            Smoke Testing and/or Canaries
            The Most Important Metric in the World
            Avoiding Vendor Lock-In
            Cleaning Up Metrics and Alerts over Time
   
7. Logging
     
            What Does It Mean to Log?
            Why Log?
            When to Rely on Logs Instead of Metrics
            What Should You Log?
            What Shouldn’t You Log?
            How Does Logging Work?
            Ensuring Your Logs Scale
            Structured Logging
            More Effective Debugging with Logs
            Searching Logs
            Exception Logging (Sentry)
            Collecting Other Logs
            Compliance
            Distributed Tracing
            Encrypting Logs for Privacy and Compliance
            Encrypt Only the Values of Sensitive Fields
            Encrypt the Entire Log Statement
   
8. Changes, Automation, And Deployment Pipelines
     
            Dealing with Change
            The Role of Automation
            What Do We Automate?
            Getting Your Code Ready for Production
            Infrastructure as Code
            Database Changes (Migrations)
            Configuration Management
            What Is a Pipeline?
            Decisions to Make Regarding Your Pipeline
            Canaries and Blue/Green Deployments
            Pipeline Permissions
            Why Do You Need a Pipeline?
            Key Phases of a Deployment Pipeline
            Step 1. Enforce Standards
            Step 2. Build and Package
            Step 3. Test
            Step 4. Publish the Artifact
            Step 5. Deploy to the Target Environment
            Step 6. Validate Deployment
            Step 7. Roll Back if Necessary (and Possible)
            Handling Pipeline Failures
   
III. Concepts
     
9. Security, Permissions, And Privacy
     
            Everyone Is Responsible, but You Are Especially Responsible
            Prepare to Be Hacked
            Understanding Your Threats and Your Attackers
            Design for Security
            Limit, Track, and Review All Secrets and Access
            Be Ready to Roll
            Defense in Depth
            Limit Blast Radius
            Trust but Verify
            Validate All User Input and Double-Check Those Settings
            Monitoring Your System for Anomalies
            Test Your Security
            Select Dependencies Carefully and Keep Your Software Up to Date
            Prioritize Privacy for Your Data and Your Customers’ Data
            Don’t Mess with Production
            Keep Your Machine Secure

   
10. Quality, Testing, And Staging
     
            The Role of Code Quality
            Code Style
            Linting
            Testing
            What to Test and What Not to Test
            Types of Testing
            Code Coverage
            Power Up Your Testing
            Staging
   
11. Planning For Failure
     
            Introduction: Understand It, Even if You Don’t Manage It
            Identify Risks
            Exercise: Finding Your Failure Points
            Be Prepared
            Making a Runbook
            Planning for Outages
            On-Call/Escalation Plan
            Monitor Your Cloud Provider
            Know Your (Service) Limits
   
12.Summary    
     
Deciding among Vendors
Community
Gather the Advice of Others
What to Do When You Get Stuck
Taking the Next Step in Your Career