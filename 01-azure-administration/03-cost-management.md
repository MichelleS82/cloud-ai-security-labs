# 03 - Cost Management

## Objective

Implement Azure cost controls for the Contoso Legal environment to prevent unexpected expenditure and demonstrate responsible cloud administration.

## Budget

A monthly Azure budget has been configured for the lab environment.

| Setting | Configuration |
|---|---|
| Budget scope | Contoso Legal resource group |
| Monthly budget | £20 |
| Warning threshold | 80% |
| Critical threshold | 100% |
| Purpose | Prevent unexpected lab expenditure |

## Cost Management Strategy

The lab uses the following controls:

- Monthly budget monitoring
- Threshold-based alerts
- Resource tagging
- Resource group organisation
- Regular review of deployed resources
- Removal of unused resources
- Avoidance of unnecessary public-facing resources

## Resource Tagging

Resources are tagged consistently to support cost attribution and administration.

| Tag | Value |
|---|---|
| Environment | Production |
| Company | ContosoLegal |
| Owner | IT |
| Project | CloudLab |

## Operational Controls

The lab environment is designed to minimise unnecessary Azure costs.

Before deploying a resource, the following questions should be considered:

1. Is the resource required?
2. Is the selected SKU appropriate for the lab?
3. Does the resource need to run continuously?
4. Can the resource be stopped when not required?
5. Is there a lower-cost configuration suitable for the workload?
6. Is the resource correctly tagged?

## Cost Monitoring

Azure Cost Management will be used to review:

- Current expenditure
- Forecast expenditure
- Resource-level costs
- Budget utilisation
- Unexpected cost increases

## Production Considerations

In a real enterprise environment, cost management would also include:

- Management-group or subscription-level budgets
- Cost allocation by department
- Chargeback or showback
- Reserved instances or savings plans where appropriate
- Azure Policy controls
- Resource lifecycle management
- Regular cost optimisation reviews

## Evidence

- Budget configuration
- Budget threshold configuration
- Cost analysis
- Resource tags
- Resource group resource inventory

## Status

Day 1 - Cost management configuration completed.
