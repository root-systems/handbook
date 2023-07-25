> This is version two of our financial agreement. We learned a **lot** from the first and overall deem it a success.
>
> Things that worked:
>
> - We never had to negotiate. We all knew the same calculation determined how much we each got paid.
> - When Greg joined, all he had to do was read our agreement and say he agreed... that easy!
> - Our pay went up and down based on how well our business was going.
>
> Things that didn't go so well:
>
> - We built the system to reward software development, but other activity types were not financially valued.
> - The base salary assumed we were all working full-time. In reality, we get sick and want to take leave.
> - As we paid people based on what they did rather than what they intended to do, we had to make relatively large assumptions about our outgoings when looking at cash flow forecasts.
>
> In our next iteration of the model, we want to experiment with the idea of paying members based on what they **say** they will do, rather than what they actually do. This may sound strange - but it's precisely what a salary is! We allow members to define a granular collection of activity types to determine their pay. We hypothesise that this gives us the benefits of having people on salary  (predictable outgoings and intent) while maintaining the flexibility of our current model (pay increases with company success).
>
> At least that's the idea ;)

# Financial Agreement

## Dependencies
This agreement is dependent on three others:

 - [Activity Types Agreement](/internal/activity-types)
 - [Self Management Agreement](/internal/self-management)
 - [Buffer Agreement](/internal/buffer-agreement)

## Member Remuneration
Our simplified formula for a month's pay can be described as:

**Base Income + Business Viability Bonus + Performance Bonus**

 - **Base Income:** This is the monthly amount a core member will always receive, no matter what number of hours they work.
 - **Business Viability Bonus:** A top up amount that is based on how sustainable we perceive our business to be.
 - **Performance Bonus:** A top up based on work that brings money to organisation.

How we generate these different amounts is a little more complex as it depends on two factors:

 - Our current Buffer Level
 - Activity Types conducted during the month

We use Activity Types and Buffer Levels to determine what amounts are added to these three components:

Variables:

 - COR - Charge-out rate: How much a member costs per hour to the client
 - BH - Billable hours: Number of billable hours a member billed to a client in a month
 - COM - Commission = 20%
 - Day Activity Types:
    - Personal: Covered by monthly basic income
    - Team: Days the member is acting/working for the team - paid a day rate based on buffer
    - Contracting: Top up for hours worked on Team days that bring money to the group -  BH \* COR \* COM
 - Buffer:
    - Level 1
    - Level 2
    - Level 3
    - Level 4

#### Summary
![The Formula](https://github.com/root-systems/agreement-financial/blob/master/indivdual-emuneration-formula.png)


### The Formula
To calculate the amount someone recieves, take their active days for a month and refer to the table below.

### Calculating daily amounts
| Buffer Level 	| Day Rate	    | Contracting Rate  |
| :---         	| ---:    		  | ---:			        |
| Level 0  	    | 100    		    | COM * COR * BH	  |
| Level 1       | 150        		| COM * COR * BH	  |
| Level 2       | 200	      		| COM * COR * BH	  |
| Level 3       | 250        		| COM * COR * BH    |
| Level 4       | 300        		| COM * COR * BH	  |

### Day rate adjustment
To provide members flexibility we ask members to self-describe how much they feel they worked according to team expectations. Members book in and update "day descriptions" to denote their intent and actual work::

 - **Short day:** 0.5
 - **Full day:** 1.0
 - **Long day:** 1.25

 Members will denote what type of day they plan to work and update it to what was actually worked.

### Forcasting example
Given we are planning for February of a non-leap year (28 days, 20 weekdays, 8 weekend days)
And we are at Buffer Level 2
And a member has booked in:

 - 4 Personal days
 - 16 Team days

And we can estimate:

 - 6 billable hours per day for 10 of the days
 - a charge out rate of $140

When we run a cashflow forecast
Then we can calculate the member will recieve:


                     1 * $1500
            +        16 * $200
            +  60 * 0.2 * $140
              ----------------
                  Total: $6380

### End of Month
At the end of a month we produce the invoices for our members. This follows the same process as forecasting except that we substitute in the actual billable hours worked, and the charge out rate.

It is the job of the [Coordinators](https://www.rootsystems.nz/roles/coordinator.html) to keep an eye on this overtime and checkin with the group and members about how things are going. A transparent monthly report will be shared to all members.

### Buffer as control lever (What's the point of all this?)
By coupling several factors to buffer events we can create a self-regulating system. The intent is that as the buffer increases, so too does the money flowing away from the pod. These are the scaling money outflows and do not include fixed costs such as space hire and SaaS tools.

### Buffer level amount
A buffer level is defined as $4,000 per person as per the [buffer agreement](https://www.rootsystems.nz/agreements/buffer-agreement.html)

## Contribution to a commons
Contribution to a commons is done as a percentage of total revenue of the pod per month. Unless agreed otherwise this is a scaling amount of between 0-8% depending on the Buffer Level.

## Collaborative funding
Giving individuals control over a discretionary amount of organisation funds that they (by themselves or with others) can use for a business expense they identify. e.g. new computer, desk, coffee machine, plants etc...

## Invoicing
Invoices to our customers are sent within the first 5 days of the month following the billing month. Invoices are sent via Xero.

## Reporting
A cashflow report is published at the end of each month.

# Glossary

## Income
The pod's funds come from the following sources:

#### Contracting/Bodyshopping
We sell our time to work as directed - often augmenting an existing team. We charge by the hour.

#### Brownfields project work
We manage and deliver a project that is extending/refining an existing code base. May be charged by the hour or by negotiated value.

#### Greenfields project work
We manage and deliver a project with a new code base.

#### Technical Discovery workshops/Code audits
Typically a day's work, these are tools we use to deepen ours and the client's understanding of the requirements.

#### Retainers/Maintenance Agreements
A fixed monthly sum paying for us to update, refactor and slowly develop the code base.

## Expenses
Money flowing away from the pod happens as follows:

#### Fixed costs
Paying for our operation cost has the highest priority and happens before paying individuals.

#### Payment for services rendered
Paying for contractors by the hour.

#### Livelihood
Eating together

#### Basic Income
All members recieve $100 a day (5 days/week) all year. Regardless of what activities they conduct.



# Archived agreements

 - [Financial V01](archive/financial-agreement-1.0.0.md)
