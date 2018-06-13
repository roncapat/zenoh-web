---
title: "The Proposal"
date: 2017-12-08T13:21:08+01:00
draft: false
---
Dear all,

I wanted to share with the ROS community the proposal we made
yesterday afternoon to other DDS vendors, the OMG MARS Taskforce and
the XRCE evaluation team on a possible way forward.

Before articulating the proposal let me give some context.

As a result of the XRCE standardisation process we need to select one
of the proposals (our proposal is available [here](http://zenoh.io/public/resources/pdf/zenoh.pdf)). On the ROS mailing list we have discussed few
aspects of the protocol and [@gbiggs]([@gbiggs](https://discourse.ros.org/u/gbiggs/summary)) provides
[here](https://discourse.ros.org/t/ipc-in-ros2/2619/23) above a good
and independent analysis on the two proposals with Erik and myself
clarifying a few points
[here](https://discourse.ros.org/t/ipc-in-ros2/2619/24) and  [here](https://discourse.ros.org/t/ipc-in-ros2/2619/25)
respectively. Thus if you have not read those I suggest you do before
continuing reading things.

With reference to
[@gbiggs](https://discourse.ros.org/u/gbiggs/summary) analysis, we
have one proposal (ours) that is perceived as being slightly more
complex but that supports peer-to-peer as well as client-to-broker and
is more suited for constrained environments. The other (RTIandCo)
which appears to be simpler but only supports client-to-broker and
carries more overhead.

If along with this information, we take into account that  we (ADLINK):

1.  have made available our XRCE implementation as Open Source under
Apache 2 as part of the project [zenoh.io](http://zenoh.io), and

2. are going to release a C++ broker by the end of the year (we
already have a Swift and a Scala broker implemented -- some folks have
seen these in actions at various demonstrations), and

3. are committed to make [zenoh.io](http://zenoh.io) the XRCE
reference implementation, both in terms of standards as well as
quality

Now that the context is given I can enunciate the proposal I made to
other vendors, task force & co:

**_Adopt our proposal and join forces, around the newly established
  open source project (zenoh), to accelerate the establishment of the
  XRCE standard in constrained environments._**

The advantages of my proposal are several:

1. End-users such as the ROS community would get access to an
implementation of the standard much more quickly -- essentially now.

2. Other DDS vendors could have immediately constrained connectivity
by simply integrating their DDS implementation on the
[zenoh.io](http://zenoh.io) broker.

3. We would have an open source implementation of XRCE supported by
all DDS vendors, which means no interoperability issues, faster
evolution, and faster adoption.

4. We would have a protocol that can do peer-to-peer as well as
brokered communication, which is good for some use cases -- most
notably in robotics.

5. We would have a protocol that could be deployed down to the
sensors. Imagine for a moment having ROS-enabled sensors talking XRCE
via low-power protocols or anything else that suits them.

6. As the one protocol everyone uses and supports is open-source we
would facilitate adoption immensely.

Collaboration can bring us much more further away than
competition. What has made humans excel is our ability to collaborate
not so much that to compete... Thus, why not in this case?

I am looking forward to hear comments  from the ROS community. Please speak-up.

-- Angelo Corsaro
