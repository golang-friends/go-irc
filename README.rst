======================================================
Draft for Roadmap for a Internet Relay Chat(IRC) in Go
======================================================

.. contents:: Table of Contents
.. section-numbering::


Introduction
============

Internet Relay Chat (IRC_) is an application that facilitates communication between two parties primarily via text. Traditionally the chat process has worked on a client/server networking model. IRC clients are computer programs that users can install on their system or web based applications running either locally in the browser or on a 3rd party server. These clients communicate with chat servers to transfer messages to other clients. IRC is mainly designed for group communication in discussion forums, called channels, but also allows one-on-one communication via private messages as well as chat and data transfer, including file sharing.(see more Wikipedia_)

..  _IRC: https://tools.ietf.org/html/rfc1459
.. _Wikipedia: https://en.wikipedia.org/wiki/Internet_Relay_Chat


Definition and Terms
--------------------

Server
******

The main component of the entire system, providing a point to which clients may connect to to talk to each other, and a point for other servers to connect to, forming an network of servers.

Client
******

A client is anything connecting to a server that is not another server. A user uses this client to connect to the server to consume the services provided. The client can be a web base client, which can be accessed using a web browser or a desktop application which the user installs on their machine. Services offered by the server will be platform independent.


What is this document for?
==========================

A project roadmap is a high-level overview of a project. Typically represented on a visual form with timeline, a roadmap consists of:

* **Project scope**: Project scope represents the big-picture vision of what you wish to achieve at the end of the project.
* **Deliverables**: Deliverables are the output or the end results of a project’s activities.
* **High-level project schedule**: The schedule describes the chronological order in which project activities are done and milestones achieved.
* **Project milestones**: Milestones are events on the project timeline that indicate a change in the project’s phase.
* **Risks**: Risks are challenges with project activities, team members, resources, or external factors that may cause the project to veer off its schedule or budget.

Project Scope
-------------

This project aims to create a Internet Relay Chat(IRC_) in Go_. This project aims to be a collaboration between like minded Go_ enthusiasts to create something that would drive learning and gain valuable experience in enterprise grade application development.

This project under the `GNU General Public License v3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_, will ensure anyone can use/extend the project and it will still remains free.


.. _Go: https://golang.org

Deliverables
------------

* Create a server which can handle communication between via text.
* Create a web based client that users can connect to and initiate a communication between other user(s).

High-level project schedule
---------------------------

Since this project is a collaboration between individual who would be volunteering their time for this project, it will be unreasonable to set a hard deadline. There is another side to this argument that if we don't have a time milestone the project risks fizzling out.

This roadmap propose a delivery schedule for alpha to be around fall of 2021, beta to be around winter 2021. These are extremely stretched timeline, but this will give enough space to experiment and try out new things, and there is nothing wrong with getting it done early :stuck_out_tongue_winking_eye:.

Project milestone
-----------------

The completion of server and making the APIs available, would be a major milestone for this project as a whole. This will allow the client to connect to it and build services on top of these APIs.


Risks
-----

Fundamentally, risk management involves making an exhaustive list of all the risks to the project. This involves identifying the risks, their probability of occurrence, their impact on the success of the project, and the proposed action. By devising the right strategies, you are well on your way to executing a successful project.

We identify some of the risks here, this list by no means is exhaustive but its a start. The goal is identify and create plans so that they don't effect the project's success.

*Anadequate design*:

What?
    Since we all are learning we run a high risk of getting into a sub-optimal software structure.

Possible actions
    Create a governance group to approve all designs.

*Shortchanged quality*:

What?
    This would mean delivering a feature/issue which is less than what was expected in terms of quality.(`Definition: Shortchanged <https://www.merriam-webster.com/dictionary/shortchange>`_).

Possible actions
    Create a code review and merge requests policy.Limit the number of reviewers.

*Feature creep*:

What?
    Feature creep is the excessive ongoing expansion or addition of new features in a product, especially in computer software, videogames and consumer and business electronics(`wiki <https://en.wikipedia.org/wiki/Feature_creep>`_). In our context, this would be new features being proposed and worked before completion of existing issues.

Possible actions:
    Create a space for new feature requests. Create a space for people to vote for specific features. Limit the number of features per version.

*Overly optimistic schedules*:

What?
    Self defining

Possible actions:
    Reevaluate project timeliness on regular intervals.

*Friction between developers*:

What?
    This project will involve individuals from across the globe(hopefully), everyone with different level of skill sets and their own opinion. There will more than a few disagreements in the course of the project. Conflicts have a way of derailing a projects.

Possible actions:
    Create a space where all opinions can be heard and taken into account.
