---
description: >-
  A service-level agreement (SLA) is an agreement between a service provider and
  a service consumer in which the service provider commits to a standard of
  service based on measurable metrics and defined
---

# Service-level agreements \(SLAs\)

#### Determine the service-level agreement of your application <a id="determine-the-service-level-agreement-of-your-application"></a>

SLAs can be strict, legally bound, contractual agreements, or assumed expectations of availability by customers. Service metrics typically focus on service throughput, capacity, and availability, all of which can be measured in various ways. Regardless of the specific metrics that make up the SLA, failure to meet the SLA can have serious financial ramifications for the service provider. A common component of service agreements is guaranteed financial reimbursement for missed SLAs.

Service-level objectives \(SLO\) are the values of target metrics that are used to measure performance, reliability, or availability. These could be metrics defining the performance of request processing in milliseconds, the availability of services in minutes per month, or the number of requests processed per hour. By evaluating the metrics exposed by your application and understanding what customers use as a measure of quality, you can define the acceptable and unacceptable ranges for these SLOs. By defining these objectives, you clearly set goals and expectations with both the teams supporting the services and customers who are consuming these services. These SLOs will be used to determine if your overall SLA is being met.

The following table shows the potential cumulative downtime for various SLA levels.

| SLA | Downtime per week | Downtime per month | Downtime per year |
| :--- | :--- | :--- | :--- |
| 99% | 1.68 hours | 7.2 hours | 3.65 days |
| 99.9% | 10.1 minutes | 43.2 minutes | 8.76 hours |
| 99.95% | 5 minutes | 21.6 minutes | 4.38 hours |
| 99.99% | 1.01 minutes | 4.32 minutes | 52.56 minutes |
| 99.999% | 6 seconds | 25.9 seconds | 5.26 minutes |

Of course, higher availability is better, everything else being equal. But as you strive for more 9s, the cost and complexity to achieve that level of availability grows. An uptime of 99.99% translates to about 5 minutes of total downtime per month. Is it worth the additional complexity and cost to reach five 9s? The answer depends on the business requirements.

Here are some other considerations when defining an SLA:

* To achieve four 9's \(99.99%\), you probably can't rely on manual intervention to recover from failures. The application must be self-diagnosing and self-healing.
* Beyond four 9's, it is challenging to detect outages quickly enough to meet the SLA.
* Think about the time window that your SLA is measured against. The smaller the window, the tighter the tolerances. It probably doesn't make sense to define your SLA in terms of hourly or daily uptime.

Identifying SLAs is an important first step when determining the high availability capabilities that your architecture will require. These will help shape the methods you'll use to make your application highly available.

