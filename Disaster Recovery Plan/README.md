# Disaster Recovery Plan 

**Disaster recovery plan (DRP)** identifies how to recover critical
systems and data after a disaster. Disaster recovery is a part of an
overall business continuity plan. Often, the organization will use the
business impact analysis to identify the critical systems and
components and then develop disaster recovery strategies and DRPs
to address the systems hosting these functions.

In some cases, an organization will have multiple DRPs within a BCP,
and in other cases, the organization will have a single DRP. For
example, it’s possible to have individual DRPs that identify the steps
to recover individual critical servers and other DRPs that detail the
recovery steps after different disasters such as hurricanes or
tornadoes. A smaller organization might have a single DRP that
simply identifies all the steps used to respond to any disruption.

A DRP or a BCP will include a hierarchical list of critical systems. This
list identifies what systems to restore after a disaster and in what
order. For example, should a server hosting an online website be
restored first, or a server hosting an internal application? The
answer is dependent on how the organization values and uses these
servers. In some cases, systems have interdependencies requiring
administrators to restore systems in a specific order.

If the DRP doesn’t prioritize the systems, individuals restoring the
systems will use their own judgment, which might not meet the
organization’s overall needs. For example, Nicky New Guy might not
realize that a web server is generating $5,000 an hour in revenue
but does know that he’s responsible for keeping a generic file server
operational. Without an ordered list of critical systems, he might
spend his time restoring the file server and not the web server.

This hierarchical list is valuable when using alternate sites such as
warm or cold sites, too. When the organization needs to move
operations to an alternate site, the organization will want the most
important systems and functions restored first.


Similarly, the DRP often prioritizes the services to restore after an
outage. As a rule, critical business functions and security services
are restored first. Support services are restored last. The different
phases of a disaster recovery process typically include the following
steps:

* **Activate the disaster recovery plan**. Some disasters,
such as earthquakes or tornadoes, occur without much
warning, and a DRP is activated after the disaster. Other
disasters, such as hurricanes, provide a warning, and the
DRP is activated when the disaster is imminent.

* **Implement contingencies**. If the recovery plan requires
the implementation of an alternate site, critical functions are
moved to these sites. If the disaster destroyed on-site
backups, this step retrieves the off-site backups from the
off-site location.

* **Recover critical systems**. After the disaster has passed,
the organization begins recovering critical systems using the
prioritization listed in the DRP. This also includes reviewing
change management documentation to ensure that
recovered systems include approved changes.

* **Test recovered systems**. Before bringing systems online,
administrators test and verify them. This may include
comparing the restored system with a performance baseline
to verify functionality.

* **After-action report**. The final phase of disaster recovery
includes a review of the disaster, sometimes called an afteraction review. This often includes a lessons learned review
to identify what went right and what went wrong. After
reviewing the after-action report, the organization often
updates the plan to incorporate any lessons learned.

## Fail Over Tests
**Fail over tests** are the ultimate test of a disaster recovery plan.
Also known as full interruption tests, these tests work by actually
shutting down the primary site and testing whether the recovery site
properly handles the load. Of course, a failed fail over test can be
incredibly disruptive to the organization, so they should be planned
and scheduled with care. Remember, though, that a self-inflicted
wound from a failed fail over test is probably not as bad as
discovering that your recovery site doesn’t work during an actual
disaster!
