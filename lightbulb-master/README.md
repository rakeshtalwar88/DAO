# Ansible Lightbulb

The Ansible Lightbulb project is an effort to provide a content toolkit and educational reference for effectively communicating and teaching Ansible topics.

Lightbulb began life as the content that supported Ansible's training program before it joined the Red Hat family focused solely on Linux server automation.

This content is now taking on a new life as a multi-purpose toolkit for effectively demonstrating Ansible's capabilities or providing informal workshop training in various forms -- instructor-led, hands-on or self-paced. 

Over time lightbulb will be expanded to include advanced and developer topics in addition to expanding beyond linux server automation and into Windows and network automation.

To support these objectives, the project provides a lab provisiover tool for creating an environment to present and work with lightbulb content. 

**NOTE:** Lightbulb "v2" is currenly a work in progress and still has not met all of its intended goals. 

### What's Provided

The Ansible Lightbulb project has been designed to be used as a toolkit and best practices reference for Ansible presentations ranging from demos thru self-paced learning thru hands-on workshops. Here you will find:

* Examples
* Workshops
* Presentation Decks
* Lab Provisioner
* Facilitator Guide

#### Examples

The content in `examples/` is the heart of what lightbulb has to offer. They are a complete Ansible playbooks that demonstrate the most fundamental features and most common use patterns. 

These examples are an excellent educational reference for communicating how Ansible works in a clear, focused and consistent manner using recommended best practices.

This content is a great source for canned demos or something you can walk-thru to illustrate automating with Ansible to a group. Some of the examples are serve as the solutions to the workshops.

#### Workshops

The content of `workshops/` are a collection of Markdown documents and applicable resources for providing hands-on assignments for learning how to automate with Ansible. 

Instructor notes on the execution and solution to all workshops can be found in `facilitator/solutions/`. 

#### Presentation Decks

The content of `decks/` are collection of presentation decks using the [reveal.js framework](http://lab.hakim.se/reveal-js/) for delivering instructor-led or hands-on instruction. 

#### Lab Provisioner

Lightbulb provides a lab provisioner utility for creating a personal lab environment for each student. Currently only Amazon Web Services (AWS) is supported in us-east-1 and us-west-1 with the foundation to support other regions in place.

**Coming Soon.** Vagrant support for self-paced learning is planned. Legacy support from the previous generation of lightbulb remains, but is in need of an overhaul. 

#### Facilitator Guide

`facilitator/` includes documentation on recommended ways Lightbulb content can be assembled and used for a wide range of purposes and scenarios. 

If you are planning on using lightbulb for some sort of informal training on automating with Ansible [this documentation](facilitator/README.md) should be your next stop.

### Requirements

True to it's philosophy and The Ansible Way, Lightbulb has been develop so that using lightbulb is as simple and low-overhead as possible. Requirements depend on the format and delivery of the lightbulb content. 

* Modern HTML5 Standard Compliant Web Browser
* A recent stable version of Python 2.7 and the latest stable version of the boto libraries.
* The latest stable versions of Ansible.
* A SSH client such as PuTTY or Mac OSX Terminal.
* An AWS account or local Vagrant setup.

#### Assumed Knowledge

For hands-on or self-paced training, students should have working knowledge of using SSH and command line shell (BASH). The ability to SSH from their personal laptop to a lab environment hosted in a public cloud can also be required based dependent on the format and presentation of the context. 

For demos and instrcutor-led exercises, conceptual understanding of linux system admin, DevOps and distributed application architecture is all that is required.

### Reference

* [Ansible Documentation](http://docs.ansible.com)
* [Ansible Best Practices: The Essentials](https://www.ansible.com/blog/ansible-best-practices-essentials)

### License

Red Hat, the Shadowman logo, Ansible, and Ansible Tower are trademarks or registered trademarks of Red Hat, Inc. or its subsidiaries in the United States and other countries.

All other parts of Ansible Lightbulb are made available under the terms of the [MIT License](LICENSE).
