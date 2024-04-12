# EC2 Instance Purchasing Options
- **On Demand Instances** :- short workload, predictable pricing, pay by second
- **Reserved (1 & 3 years)**
    * **Reserved Instances** Long Workloads
    *  **Convertable Reserved Instances** :- Long workloads with flexible instances

- **Savings Plans (1 & 3 years)** :- Commitment to an amount of usage, long workload
- **Spot Instances** :- Short workloads, cheap, can lose instances (less reliable)
- **Dedicated Hosts** :- Book an entire physical server, control instance placement
- **Dedicated Instances** :- No other customers will share your hardware
- **Capicity Reservation** :- reserve capacity in a specific AZ for any duration.


## EC2 On Demand
- Pay for what you use:
    * Linux or windows :- billing per second, after the first minute
    * All other operating systems :- billing per hour
- Has the highest cost but no upfront payment
- No long-term commitment 
- Recommended for short-term and un-interrupted workloads, where you can't predict how the application will behave.

## EC2 Reserved Instances
- Up to 72% discount compared to On-demand 
- You reserve a specific instance attributes (Instance Type, Region, Tenancy, OS)
- Reservation Period :- 1 year (+ discount) 3 years (+++ discount)
- Payment Options :- No Upfront (+), Partial Upfront (++), All Upfront (+++)
- Reserved Instance's Scope :- Regional or Zonal (Reserve capacity in an AZ)
- Recommended for steady-state usage applications (think database)
- You can buy or sell in the Reserved Instance Marketplace

- Convertible Reserved Instance
    * Can change the EC2 instance type, instance family, OS, scope and tenancy 
    * upto 66% discount.


## EC2 Savings Plans 
- Get a discount based on long-term usage (up to 72% - same as RIs)
- Commit to a certain type of usage ($10/hour for 1 or 3 years)
- Usage beyond EC2 savings plans is billed at the On-Demand price
- Locked to a specific instance family & AWS region (e.g., M5 in us-east-1)
- Flexible across:
    * Instance Size (e.g., M5.xlarge,m5.2xlarge)
    * OS (e.g., Linux, Windows)
    * Tenancy (Host, Dedicated. Default)

## EC2 Spot Instances 
-  Can get a discount of up to 90% compared to On-demand 
- Instances that you can *"lose"* at any point of tme if your max pprice is less than the currenct spot price
- The MOST cost-efficient instance in AWS
- Usefull for workloads that are resilient to failure
    * Batch jobs
    * data analysis
    * Image processing
    * Any **distributed** workloads
    * Workloads with a flexibble start and endtime
- Not suitable for critical jobs or databases.

## EC2 Dedicated Hosts
- A physical server with EC2 instance capacity fully dedicated to your use
- Allows you address compliance requirements and use your existing server-bound software licences (per-socket, per-core, per VM software Licences)
- Purchasing Options:
    * On-demand :- Pay per second for active Dedicated host
    * Reserved :- 1 or 3 years (No Upfront, partial Upfront, All Upfront)
- The most expensive option
- Useful for software that have complicated licensing model (BYOL - Bring your own license)
- Or for companies that have strong regulatory or compliance needs

## EC2 Dedicated Instances 
- instances run on hardware that's dedicated to you
- May share hardware with other instances in same account
- No control over instance placement (can move hardware after Stop/Start)

## EC2 Capacity Reservations 
- Reserve On-demand instances capacity in a specific AZ for any duration
- You always have access to EC2 capacity when you need it
- No time commitment (create/cancle anytime), no billing discounts
- Combine with Rigional Reserved Instances and savings plans to benefit from billing discounts
- You are charged at On-Demand rate whether you run instances or not
- Suitable for short-term, uninterrupted workloads that needs to be in a specific AZ


# Which purchasing option is right for me?

- **On demand:** coming and staying in resort whenever we like, we pay the full price
- **Reserved:** Like planning ahead and if we plan to stay for long time, we may get a good discount
- **Savings Plans:** Pay a certain amount per hour for certain period and stay in any room type (e.g., King, Suite, Sea View, ...)
- **Spot instances:** The hotel allows people to bid for the empty rooms and the highest bidder keeps the rooms. You can get kicked out at any time.
- **Dedicated Hosts:** We book an entire building of the resort
- **Capacity Reservations:** You book a room for a period with full price even you don't stay in it. 

