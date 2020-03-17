---

layout: col-sidebar
title: OWASP Glue Tool
tags: example-tag
level: 0
type: tool
pitch: The OWASP Glue Tool Project is a tools based project intended to make security automation easier. It is essentially a ruby gem that co-ordinates the running of different analysis tools and reporting from those tools.
---

[![Twitter Follow](https://img.shields.io/twitter/follow/glue?style=social)](https://twitter.com/owaspglue)

The OWASP Glue Tool Project is a tools based project intended to make security automation easier. It is essentially a ruby gem that co-ordinates the running of different analysis tools and reporting from those tools.
The purpose of the project is to make it easy to integrate security tools (like static or dynamic analysis) into the CI/CD pipeline.

# FAQs

## What does Glue do?

The OWASP Glue tool attempts to make it very easy to run different types
of security tools at various stages of the software development process
and produce unified issues that can be used in other contexts to track
or remediate issues.

## Why would I use Glue?

To help get security feedback into your developers hands faster.

## How can I participate in your project?

Reach out to matt.konda@owasp.org with any questions or ideas or ideas
about how to participate. We are welcoming input. We are following
standard github workflow so you can fork the code and submit a pull
request if you prefer. Alternatively, you can get more deeply involved
and talk with us about roadmap and other items. And finally, you are
always invited to our Slack channel.

## If I am not a programmer can I participate in your project?

Yes, you can certainly participate in the project if you are not a
programmer or technical. The project needs different skills and
expertise and different times during its development. Currently, we are
looking for researchers, writers, graphic designers, and a project
administrator. See the Road Map and Getting Involved tab for more
details.

# Acknowledgements

## Contributors

To this point, project contributors include:

  - [Matt Konda](https://www.owasp.org/index.php/User:Matt_Konda)
  - Rafael Zambrano
  - Alex Lock
  - Omer Levi Hevroni

# Road Map and Getting Involved

Deliverable: Glue is delivered as a ruby gem (executable binary) and in
a docker image with required tools already bundled.

## Roadmap

Allows extending the tool more without changing code. Currently, it’s
possible to integrate new tools without changing code, in the future we
would like to add a similar support for reports and filters. Check out
the open issues on GitHub. This is what we hope to achieve in future
releases.

## Getting Involved

Involvement in the development and promotion of <strong>Glue</strong> is
actively encouraged\! You do not have to be a security expert or a
programmer to contribute. Some of the ways you can help are as follows:

### Coding

We could implement some of the later items on the roadmap sooner if
someone wanted to help out with a unit or automated regression tests

### Localization

Are you fluent in another language? Can you help translate the text
strings in the <strong>Tool Project Template</strong> into that
language?

### Testing

Do you have a flair for finding bugs in software? We want to produce a
high-quality product, so any help with Quality Assurance would be
greatly appreciated. Let us know if you can offer your help.

### Feedback

Please use the [Tool Project Template project mailing
list](https://lists.owasp.org/mailman/listinfo/OWASP_Tool_Project_Template)
for feedback about:

  - What do like?
  - What don't you like?
  - What features would you like to see prioritized on the roadmap?

Alternativly, you can also use our Slack channel on OWASP slack.

# Minimum Viable Product

## Pipeline needs

1\. Pull from github or a specified location on the file system 2. Run
tools like brakeman, bundler-audit and owasp-dependency-check on the
code. 3. Standardizes the format of results then reports them in text,
csv, json or via JIRA's REST API. 4. Detect duplicates and won't report
the same thing more than once.

It also needs to be easy to set up the security tools and digest
results. Hence a focus on docker.
