# Business Continuity Plan

Business continuity planning helps an organization predict and plan
for potential outages of critical services or functions. The goal is to
ensure that critical business operations continue and the
organization can survive the outage. Organizations often create a
**business continuity plan (BCP)**. This plan includes disaster
recovery elements that provide the steps used to return critical
functions to operation after an outage. Disasters and outages can
come from many sources, including:

* **Environmental**. This can include natural disasters, such as
hurricanes, floods, tornadoes, and earthquakes. It can also
include things like fires caused by lightning strikes rather
than by humans. On a larger scale, it can include major
environmental disasters such as the Fukushima Daiichi
Nuclear Power Plant’s nuclear meltdown after an earthquake
and tsunami in 2011.

* **Human-made**. Human-made disasters refer to those
caused by human activity. This includes fires (caused by
people) and train wrecks caused by human error, such as
the May 2015 Amtrak derailment. Within an organization,
human error can cause hardware and software failures, and
data loss. Attacks are also human-made.

* **Internal versus external**. An internal disaster occurs
within an organization. For example, a fire within an
organization’s data center is an internal disaster that may
result in hardware failure and data loss. In contrast, an
external disaster is a disaster that occurs outside of an
organization but still impacts the organization. As an
example, a wildfire near an organization may damage utility
lines impacting the stability of power or communication
lines.


## Business Impact Analysis Concepts

**Business impact analysis (BIA)** is an important part of a BCP.
It helps an organization identify critical systems and components
that are essential to the organization’s success. These critical
systems support mission-essential functions. Mission-essential
functions are the activities that must continue or be restored quickly
after a disaster. The BIA also helps identify vulnerable business
processes, which are the processes that support mission-essential
functions.

As an example, imagine an organization that has an online ecommerce business. Some basic mission-essential functions might
include serving webpages, providing a shopping cart path, accepting
purchases, sending email confirmations, and shipping purchases to
customers. The shopping cart path alone is a business process.
Because it is essential to the mission of e-commerce sales,
management will likely consider it a vulnerable business process to
protect. The customer needs to view products, select a product,
enter customer information, enter credit card data, and complete the
purchase. Some critical systems that support the website are web
servers and a back-end database application hosted on one or more
database servers.

If critical systems and components fail and cannot be restored
quickly, it impacts mission-essential functions. If this lasts too long,
the organization may not be able to survive the disaster.

For example, if a disaster such as a hurricane hits, which services
must the organization restore to stay in business? Imagine a
financial institution. It might decide that customers must have
uninterrupted access to account data through an online site. If
customers can’t access their funds online, they might lose faith with
the company and leave in droves.

However, the company might decide to implement alternate business
practices in other elements of the business. For example,
management might decide that accepting and processing loan
applications is not important enough to continue during a disaster.
Loan processing is still important to the company’s bottom line, but a
delay will not seriously affect its ability to stay in business. In this
scenario, continuous online access is a mission-essential function,
but processing loan applications during a disaster is not missionessential.

The time to make these decisions is not during a crisis. Instead, the
organization completes a BIA in advance. The BIA involves collecting
information from throughout the organization and documenting the
results. This documentation identifies core business or mission
requirements. The BIA does not recommend solutions. However, it
provides management with valuable information so that they can
focus on critical business functions. It helps them address some of
the following questions:

* What are the critical systems and functions?
* Are there any dependencies related to these critical systems
and functions?
* What is the maximum downtime limit of these critical
systems and functions?
* What scenarios are most likely to impact these critical
systems and functions?
* What is the potential loss from these scenarios?

As an example, imagine an organization earns an average of $5,000
an hour through online sales. In this scenario, management might
consider online sales to be a mission-essential function, and all
systems that support online sales are critical systems. This includes
web servers and back-end database servers. These servers depend
on the network infrastructure connecting them, Internet access, and
access to payment gateways for credit card charges.

After analysis, they might determine that the maximum allowable
outage for online sales is five hours. Identifying the maximum
downtime limit is extremely important. It drives decisions related to
recovery objectives and helps an organization identify various
contingency plans and policies.

# Key Aspects About BCP

## Recovery Time Objective
The **recovery time objective (RTO)** identifies the maximum
amount of time it can take to restore a system after an outage.
Many BIAs identify the maximum acceptable outage or maximum
tolerable outage time for mission-essential functions and critical
systems. If an outage lasts longer than this maximum time, the
impact is unacceptable to the organization.

For example, imagine an organization that sells products via a
website that generates $10,000 in revenue an hour via online sales.
It might decide that the maximum acceptable outage for the web
server is five minutes. This results in an RTO of five minutes,
indicating any outage must be limited to no more than five minutes.

Imagine that the organization has a database server only used by
internal employees, not online sales. Although the database server
may be valuable, it is not critical. Management might decide they
can accept an outage for as long as 24 hours, resulting in an RTO of
24 hours.

## Recovery Point Objective
A **recovery point objective (RPO)** identifies a point in time where
data loss is acceptable. Imagine a server hosting archived data that
has very few changes weekly. Management might decide that some
data loss is acceptable, but they always want to recover data from at
least the previous week. In this case, the RPO is one week.

With an RPO of one week, administrators would ensure that they
have at least weekly backups. In the event of a failure, they will be
able to restore recent backups and meet the RPO.

In some cases, the RPO is up to the minute of the failure. For
example, any data loss from an online database recording customer
transactions might be unacceptable. In this case, the organization
can use various techniques to ensure administrators can restore data
up to the moment of failure.

## MTBF and MTTR
When working with a BIA, experts often attempt to predict the
possibility of a failure. For example, what is the likelihood that a hard
disk within a RAID configuration will fail? The following two terms
are often used to predict potential failures:

* **Mean time between failures (MTBF)**. The MTBF
provides a measure of a system’s reliability and is usually
represented in hours. More specifically, the MTBF identifies
the average (the arithmetic mean) time between failures.
Higher MTBF numbers indicate higher reliability of a product
or system. Administrators and security experts attempt to
identify the MTBF for critical systems with the goal of
predicting potential outages.

* **Mean time to repair (MTTR)**. The MTTR identifies the
average (the arithmetic mean) time it takes to restore a
failed system. In some cases, people interpret MTTR as the
mean time to recover, and both mean essentially the same
thing. Organizations that have maintenance contracts often
specify the MTTR as a part of the contract. The supplier
agrees that it will, on average, restore a failed system within
the MTTR time. The MTTR does not provide a guarantee
that it will restore the system within the MTTR every time.
Sometimes, it might take a little longer, and sometimes it
might be a little quicker, with the average defined by the
MTTR.
