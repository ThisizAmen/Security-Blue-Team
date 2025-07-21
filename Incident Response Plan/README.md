# Incident Response Plan

### Incident Response Process
 Incident response includes multiple phases. It starts with creating an
 incident response policy and an incident response plan. With the
 plan in place, personnel are trained and given the tools necessary to
handle incidents. Incident response preparation will help an
 organization prevent or effectively contain and recover from
 incidents.

 The phases of an incident response process are:

 * Preparation. 

 This phase occurs before an incident and
 provides guidance to personnel on how to respond to an
 incident. It includes establishing and maintaining an incident
 response plan and incident response procedures. It also
 includes establishing procedures to prevent incidents. For
 example, preparation includes implementing security
 controls to prevent malware infections.
 
 * Detection. 
 
 During normal operations, the security team
 monitors network, system, application, and user behavior,
 watching for unusual activity. This is normally coordinated
 by an organization’s security operations center (SOC)
 through the use of tools like security information and event
 management (SIEM) systems, security orchestration,
 automation and response (SOAR) systems, extended
 detection and response (XDR) systems, network detection
 and response (NDR) systems, intrusion detection and
 prevention systems (IDS/IPS), data loss prevention (DLP)
 systems, and related technologies such as user and entity
 behavior analytics (UEBA) systems.
 
 * Analysis.
 
  All detected events aren’t security incidents, so
 when a potential incident is reported, personnel take the
 time to verify it is an actual incident. For example, intrusion
 detection systems (IDSs) might falsely report an intrusion,
 but administrators would investigate it and verify if it is a
 false positive or an incident. After confirming an incident,
personnel might try to isolate the system based on
 established procedures.
 
 * Containment.
 
  After an incident analysis and verification,
 security personnel attempt to isolate or contain it. This
 protects critical systems while maintaining business
 operations. Containment might include quarantining a
 device or removing it from the network. This can be as
 simple as unplugging the system’s network interface card to
 ensure it can’t communicate on the network. Similarly, you
 can isolate a network from the Internet by modifying access
 control lists on a router or a network firewall. This is similar
 to how you’d respond to water spilling from an overflowing
 sink. You wouldn’t start cleaning up the water until you first
 turn off the faucet. The goal of isolation is to prevent the
 problem from spreading to other areas or other computers
 in your network or to simply stop the attack.
 
 * Eradication.
 
  After containing the incident, it’s often
 necessary to remove components from the attack. For
 example, if attackers installed malware on systems, it’s
 important to remove all remnants of the malware on all
 hosts within the organization. Similarly, an attack might
 have been launched from one or more compromised
 accounts. Eradication would include deleting or disabling
 these accounts.

 * Recovery.
 
  During the recovery process, administrators
 return all affected systems to normal operation and verify
 they are operating normally. This might include rebuilding
 systems from images, restoring data from backups, and
 installing updates. Additionally, if administrators have
identified the vulnerabilities that caused the incident, they
 typically take steps to remove the vulnerabilities.
 
 * Lessons learned.
 
  After handling an incident, security
 personnel perform a lessons-learned review. The incident
 may provide some valuable lessons, and the organization
 might modify procedures or add additional controls to
 prevent a reoccurrence of the incident. Part of this process
 normally includes a root cause analysis that tries to
 identify what initially went wrong that allowed an incident to
 occur. The lessons-learned review might indicate a need to
 provide additional training to users or indicate a need to
 update the incident response policy. The goal is to learn
 from the incident and prevent a future reoccurrence of a
 similar incident.


 # Training & Testing

 Training and testing play important roles in ensuring the
effectiveness of incident response plans. This includes both tabletop
exercises and simulations, both of which provide different yet
complementary aspects of training.


**Tabletop exercises**  are a type of scenario-based training where
participants discuss and analyze a hypothetical incident in a nonthreatening environment. This is like a game of chess where you
anticipate your opponent’s moves and plan your strategy
accordingly. In a cybersecurity context, a tabletop exercise could
involve a simulated phishing attack or data breach. The incident
response team would then discuss the steps they would take to
respond to the incident based on the existing incident response plan.
The goal is to identify gaps in the plan and refine it based on the
insights gained from the exercise.


**Simulations**, on the other hand, are a more hands-on form of
training. Instead of discussing hypothetical situations, simulations
involve recreating real-world incidents as closely as possible. This
provides the incident response team with practical experience in
responding to an incident. Simulations are particularly valuable for
training personnel on complex or unusual incidents that can’t be
easily replicated in a live environment.

Both tabletop exercises and simulations are critical in ensuring an
effective incident response. Tabletop exercises allow teams to
discuss strategies and refine their plans, while simulations give
teams the opportunity to apply their plans in practice. By conducting
regular training and testing, organizations can better prepare
themselves for the real-world incidents they will inevitably face.


# Threat Hunting

**Threat hunting** is like being a detective in the digital world. It’s
when skilled computer security experts actively search for sneaky
cyber threats that might have slipped past regular security systems.
Instead of just waiting for an alarm to go off, these experts go out
and look for clues that might suggest a cyber invader is up to no
good.

The aim of threat hunting is to catch these cyber invaders as quickly
as possible. The quicker you find them, the less damage they can
do. This is important because sometimes these cyber invaders can
sneak into a network and hide there, causing problems without
being noticed for a long time.

To track down these hidden threats, threat hunters use a mix of
special tools and techniques. They may use things like threat
intelligence feeds which provide regularly updated ‘most wanted’ lists
of cyber threats. They also use smart systems that can spot when
users or computers are behaving oddly, which might suggest a cyber
invader is at work.
