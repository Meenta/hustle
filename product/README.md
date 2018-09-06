# Product Owner Test
This hustle test is for product owners. This is a real problem. There is
no `right` answer. Unlike the UI and Server tests this is more of thought
and presentation challenge.

We are moving our stack to a `micro-features` pattern. This means that
each feature in our application resided in its own git repo, and contains
a suite of web components and services that support it. These `features`
a design to allow a product owner to mix and max features within a range
of single page applications (SPA).

Currently we are building out a suite of `search` related web components
that we can combine with landing pages, copy and usage cases to learn
how our customers approach finding the sequencing resources they need to
solve their research objectives.

The link below points to a prototype SPA that is designed to help a `newbie`
users by providing them with an NGS (Next Generation Sequencing) calculator.
The `calculator` component allows a scientists to enter the specifics of
their experiment. The application then allows them see recommendations for
instruments that will meet their requirements.

The SPA contains four components; `search form`, `profile`, `quotes` and `results table`.

https://meenta.io/search

#### Happy Path
A user visits this page, enters in their experimental requirements. The user
reviews the results, and selects an individual instrument. The SPA allows the
user to see details, and add a given instrument to a quote. Quotes can be
reviewed and downloaded. A user needs to have an account (use the following to
test.)

Username: john.doe@meenta.io Password: meenta123

#### Tasks and Deliverables
The task is to review the SPA and explore how this product should be managed,
tested and deployed. We know that there is a lot of subject matter expertise
needed to build and manage. The goal is to move this out of a developer lead
POC into a product that has its own roadmap, customer feedback, marketing
and ROI.

Questions:
- How would you think about this product and its components?
- How would you approach vetting the copy and features?
- How have you approached new features?
- What resources would you need to provide a roadmap?

There is no right answer. We want to understand how you think about features,
applications and testing customer assumptions.

#### Reference Materials
- [UI Micro Frontend](https://micro-frontends.org)
- [Illumina NGS Calculator](https://support.illumina.com/downloads/sequencing_coverage_calculator.html)
