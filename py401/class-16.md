# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 16 - Serverless Functions

## [What is Serverless Computing?](https://www.ibm.com/cloud/learn/serverless)
> Serverless is a cloud execution model that enables a simpler, more cost-effective way to build and operate cloud-native applications.

- automatically provides computer with required data
- Automatically scales recources
- Automatically scales resources to zero when the application stops
- offloads all management responsibility in backend to make room for front end

### Serverless vs. FaaS (function as a service)
- FaaS is actually a subset of serverless
- . Serverless includes FaaS plus all the other associated resources in the code

## Serverless pros and cons
| Pros | Cons |
|---|---|
| focus on writing code, not managing infrastructure | Stable or predictable workloads |
| pay for execution only | Cold starts |
| polyglot environment, code in any language or framework | Monitoring and debugging, move serverless architecture exacerbates complexity |
| simplifies deployment | Vendor lock-in |
| faster and more cost-effective |  |
| ear-total visibility into system and user times |  |

## Understanding the serverless stack
- Functions as a Service (FaaS)
- Databases (SQL and NoSQL) are the foundation
- well-suited for event-driven and stream-processing workloads
- API gateways act as proxies

## Comparing FaaS to PaaS, containers, and VMs

|  | FaaS |  |
|---|---|---|
| Provisioning time: | milliseconds | minutes to hours |
| Ongoing administrative burden: | None | continuum from light to heavy |
| Elastic scaling: |  Instant and inherent, with auto-scaling to zero | automatic but slow scaling, no zero scaling |
| Capacity planning: | None | require a mix of automatic scalability and capacity planning |
| Persistent connections and state: | Limited | more flexible |
| Maintenance: | Managed by the provider | Managed by the provider with significant more maintenance |
| High availability (HA) and disaster recovery (DR): | Inherent no extra cost | require additional cost and management |
| Resource utilization: | 100% efficient | some degree of idle capacity |
| Charging granularity and billing:  | units of 100 milliseconds | by the hour |

## Use cases
- supporting microservices architectures
- can be turned into a HTTP endpoint
- well-suited to working with structured text
- Any kind of parallel task
- Stream processing workloads

## Additional Resources
- [venv - Creation of Virtual Environments](https://docs.python.org/3/library/venv.html)
- [Vercel - Get Started](https://vercel.com/docs/get-started)
- [http.server](https://pymotw.com/3/http.server/index.html)
- [Requests](https://docs.python-requests.org/en/latest/)
- [Python & APIs](https://realpython.com/python-api/)

- [Video: What is Serverless?](https://www.youtube.com/watch?v=vxJobGtqKVM)

## Bookmark and Review
- [Serverless Functions](https://vercel.com/docs/concepts/functions/serverless-functions)