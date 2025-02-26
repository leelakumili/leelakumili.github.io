# Building the Baseline – The Foundation of Observability

## Are You Really Prepared for the Unexpected?

When building a platform, how do you know you're truly prepared for the sudden spikes or increases in demand? How can you be sure your system is behaving as it should when traffic surges or an incident strikes? 

The key is having a baseline - a clear definition of what ‘normal’ looks like. With it, you can quickly spot anomalies, notify the right people, and empower on-call engineers with the confidence to take action. Let’s explore how to build that baseline and ensure your team is ready for anything.

## Why a Baseline Matters

How do you know when something is truly wrong with your system? Without a baseline, it’s nearly impossible to distinguish between normal fluctuations and serious problems.

A baseline defines what “normal” looks like. It helps you identify anomalies, notify the right people, and empower on-call engineers to act quickly and confidently.

Think of your system as a car—you know its usual speed, fuel consumption, and engine sounds. When the engine overheats, you notice immediately and take action before it gets worse. Without a baseline, you’re driving blind, unsure if rising temperature is a minor hiccup or a critical failure.

But remember, defining “normal” isn’t a one-time task. As systems evolve and traffic patterns change, your baseline must adapt. Monitoring and refining it is an ongoing process that ensures accuracy over time.

## How to Build the Baseline

Building a solid baseline is a strategic step toward ensuring your system can handle the unexpected. Here’s how I approach it:

### Monitor Core Metrics
Start with the fundamentals. Track key metrics such as latency, throughput, error rates, and resource utilization. These are the building blocks of observability and help you measure system performance against known, healthy values.

### Track System Behavior Over Time
Observe how your system behaves under various conditions—during traffic surges, deployments, and idle periods. This helps you understand what "normal" looks like at different times. It’s also crucial to capture how your system reacts to stress so you can anticipate performance issues before they turn into full-blown problems.

### Map System Dependencies
Understand how your services interact with each other. Use distributed tracing to visualize dependencies and pinpoint potential bottlenecks. Knowing how each component communicates will help you troubleshoot more effectively when things go wrong.

### Analyze Historical Data
Past incidents are powerful learning tools. Review the data from previous outages or performance issues to identify common thresholds for anomalies. For example, you might discover that high CPU usage typically precedes a failure, or that response times exceed acceptable limits during a traffic spike.

### Define Alert Thresholds
Create dynamic, adaptive alerting systems based on your baseline. Avoid static thresholds that are out of sync with real-world fluctuations. Your alerts should be flexible enough to account for expected variations while still providing early warnings for genuine issues.

### Visualize and Centralize
A good baseline isn’t just about tracking metrics—it’s about making them accessible. Build dashboards that offer centralized, intuitive views of your system’s health. These dashboards should be easy for your team to understand and should allow them to respond quickly in case of anomalies.

## Who’s Responsible for the Baseline?

Building and maintaining a baseline isn’t the sole responsibility of SREs or DevOps engineers; it’s a collaborative effort that spans across multiple teams. In a complex environment like a platform composed of multiple microservices, various teams take ownership of different parts of the baseline. Here’s how responsibilities can be divided:

- **Service Teams:** Focus on defining and monitoring service-level metrics, such as response times, Kafka lag, CPU and memory utilization, and success vs. failure response rates. Monitor pod-level health if using Kubernetes.
- **Gateway Teams:** Monitor public API baselines to ensure external interfaces are healthy and responsive.
- **SRE Teams:** Ensure system-wide health, including clusters, shared infrastructure, Kafka, and databases.

This collaborative approach ensures that the baseline is defined in a way that covers all areas of the system, from microservices to infrastructure. By making this a team-wide responsibility, everyone is invested in understanding what "normal" looks like, and the system can evolve as it grows. When everyone has a clear understanding of the baseline, you create a culture of ownership and shared accountability. This means that when incidents occur, each team member is equipped to respond with the same clarity and confidence.

## Empowering Your Team

A clear baseline empowers on-call engineers to take action swiftly. They can diagnose issues before they escalate, reducing downtime and avoiding unnecessary panic. With the right data and context, your team can focus on continuous improvement rather than firefighting.

By investing in a strong baseline, you enable your team to:

- Respond confidently to incidents.
- Diagnose and resolve issues faster.
- Focus on building a more robust system.

## Closing Call to Action

Do you have a baseline for your system? How do you define "normal" for your platform, and what practices help you spot anomalies early? Share your thoughts in the comments—I’d love to hear how you're building resilience into your systems!

## Next Article Preview

In the next article, we’ll explore how to transform your baseline into a resilient system—one that not only detects anomalies but also recovers gracefully and continues to perform under stress. Stay tuned!
