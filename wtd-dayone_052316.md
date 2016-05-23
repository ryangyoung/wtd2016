# Write the Docs NA 2016 - Day One

## State of the Docs

Speaker: Eric Holscher

"Documentarian" is the word WTD came up with to define not only technical writers, but also developers, programmers, UX designers, tech support and QA engineers etc etc who contribute to and care about documentation.

Eric envisions a whole series of speakers on different stages talking about the importance of documentation. For instance, he encouraged the crowd to invite people with different job titles to next year's event.

Next year might be split into two different events: one for the east coast and one for the west coast.

## [Technical Writing as a Public Service](http://www.writethedocs.org/conf/na/2016/speakers/#speaker-britta-gustafson)

Speaker: [Britta Gustafson](https://twitter.com/brittagus)

18F is human-centered, Agile, iterative, and open source (FOSS) and is a part of the Federal Government, specifically the [General Services Adminstration (GSA)](http://www.gsa.gov/portal/category/100000).

18F has a team of about 180 people. It's a tiny piece of the government. Part of its mission is to make "of the people, by the people, for the people" more of a reality. Software is a core part f how government works, so the software that government uses should be open, accessible, and modifiable (through pull requests, and within reason). "The people should be able to reuse and adapt the work the public paid for."   

Making government software more accessible and open-source-like, it could attract more participants in the government.

One thing that Britta worked on was [eRegulations](http://www.consumerfinance.gov/eregulations/).

Another was the government's [Source Code Policy](https://sourcecode.cio.gov/). Part of this involved writing bug reports on [the White House's GitHub repo](https://github.com/whitehouse/source-code-policy/issues).

Yet another was writing a blog post about the tools that the government, and specifically 18F, uses.

"Public service + open source + documentation = of the people, by the people, for the people"  

If you want to learn more:

- <https://18f.gsa.gov>

- <https://github.com/18F>

## [Two Great Teams that Work Great Together: Bridging the Gap Between Documentation and Customer Support](http://www.writethedocs.org/conf/na/2016/speakers/#speaker-neal-kaplan)

Speaker: [Neal Kaplan](https://twitter.com/NealKaplan)

Neal works at a startup and is the only tech writer. For part of his career, he ran a support group. When "software came in boxes," his doc team was based in Menlo Park and the support team was based in Dublin. The software offered a way to provide customer comments, but the comments were not really cataloged. They were hard to find and often lost.

Documentation should promote "ticket deflection" and be "self-service." Neal feels that "ticket direction" is a better term because interaction with customers is good, as long as that interaction is good.

Neal was at a meetup where a customer support person presented and said, proudly, that they have a knowledge base. A doc person also presented and said they had a help site. The two teams did not share content. The reason for this, they said, was that documentation was "prescriptive" and the support content was "descriptive." This was a bad idea because it forces customers to choose between two sets of information. How are the users expected to know which information to choose? This mentality leads to frustrated customers.

Neal's suggestions:

- Meet your support team. Know who they are and what their expertise is.

- Review support tickets. Especially the tickets that ask how to do something or mention that they've read the docs and still don't understand.

- Set up automated processes. If the support team gets a doc-related ticket, have it automatically assigned to you (or the docs team).

- Review difficult and interesting cases. For example, after talking to an engineer about a difficuly use case, Neal realized that the instructions would benefit from a diagram, which he subsequently added a  diagram.

- Learn about your customers and understand their skill level. Understand their vocabulary. If the terms they're using don't match the docs, maybe you should update your terminology.

- Review ticket metrics. And keep reviewing them. Look for changes.

- Join forces with support! Have one source of truth.

- Have the support team write docs! Give them credit and show them where their efforts ended up.

- Don't train: make templates.

- Make support part of the doc review process.

- Share knowledge. Have the support team come to you with new procedures.

- Use the input from support to reprioritize.

## [So You Need to Document an API](http://www.writethedocs.org/conf/na/2016/speakers/#speaker-allison-reinheimer-moore)

Speaker: [Allison Reinheimer Moore](https://twitter.com/schmalliso)

Allison has an MS in Library Sciences and previously worked for Oracle. She works for MongoDB now.

### A Very Short Introduction to APIs

"APIs are sets of requirements that govern how different systems can talk to each other."

MongoDB has APIs. They use RESTful APIs. REST is an architectural style.

RESTful APIs typically:

- Communicate over HTTP

- Use HTTP verbs, i.e. GET, POST, PUT, DELETE, etc

### Questions to Ask When You're Documenting an API

About the users:

- Who are your users?

- What are your users' motivations?

- What do people want to do with your API?

- What programming languages are popular among your users? This is important for code samples. Doesn't make sense to provide Java examples if your users are writing applications in Node.js, for example.

About the API:

- What does the API let people do? Why does the API exist?

- How does this API relate to other APIs provided by the company?

- How does Auth/access work? Are you using OAuth? 1.0 or 2.0?

About you:

- Where do you come in? What are you responsible for? What are the developers responsible for?

- Who will write the code examples? You or the devs?

- Who is going to review what your write? Devs? Support?

### Concepts to Cover in API Documentation

- API call pattern (i.e., <someurl/asset/asset_id>)

- Common URI parameters

- Asset descriptions (i.e., descriptions of the data objects; what are you trying to get from the API?)

- Terminology (what words mean in the API)

- Tutorials are also important. Especially for authentication, because OAuth is hard.

- References are important. Descriptions of request and response fields are *very* important.

### API Documentation Tools

MongoDB uses Sphinx, which builds PDF, HTML, ePub and more.

Slate is another tool that might be useful. It's what Stripe uses. Has a Markdown backbone.

You *can* use Flare for API docs, but it's far from ideal.

## [Crossing the Streams: Enabling Collaboration Between Products and Upstreams](Crossing the Streams: Enabling Collaboration Between Products and Upstreams)

Speaker: [Shaun McCance](https://twitter.com/shaunm), RedHat

Shaun got his start with the Gnome project. He noticed that each Linux distro had a slightly different version of Gnome that had been tweaked by the different maintainers. For example, Fedora might have added a date and time config. He needed a way to develop a global help system that accounted for all these different versions. The solution was Project Mallard. It allowed the team to create a help system from a disparate set of topics.

All of RedHat's products are built from open source projects. They focus on the upstream first, meaning that they modify at the source.

Shaun:

- Makes upstream, open source docs great.

- Builds docs communities around upstream.

- Makes upstream docs reusable by downstream. This is friendly for downstream developers.

### What are all these streams?

- RedHat Gluster storage is a downstream from the gluster project.

- RedHat OpenStack Platform is a downstream of ~dozen open-source projects, including Glance, Horizon, Swift, Neutron, Heat, Nova, Trove, Cinder, Ironic, Keystone. RH created the RDO project for packaging and integration, which is the immediate upstream of the enterprise product. OpenStack is an upstream of RDO, and all the other listed projects are upstreams of OpenStack. They all need documentation.

- Fedora is another upstream, from RHEL and CentOS. These streams go both ways, from Fedora to RHEL, to CentOS, and then back to Fedora and some upstreams.

### Thinking in Topics

Shaun's advice on how to manage all these interdependent streams—up, down, side, left, and right—is: Stop Writing Books. Start writing Topics. And thining in Topics:

- Write only what's necessary

- Be upfront about required background.

- Cross-link to other topics.

- Do not  expect a linear reading.

-  Every page is page one.

### Types of Topics

There are different types, but it's not necessary to

### How Product teams can Upstream

- Community is a good source of piecemeal content.

- Help organize and curate content.

- Help from content strategy and plan.

- Connect writers to SMEs.

- Don't do it by yourself! Create a community. But:

    - Don'y treat your community as unpaid workers.

### Content Strategy in a Box

You can devise a strategy in a doc sprint.

Analyze your audience:

- Split your audience into 3-5 segments. Segments should cover every reader. e.g., administrators, 3rd-party developers, contributors to the project, etc

- In each segment, define 3-5 samples:

    - Talk about specific needs and circumstances

    - Samples can't possibly cover every reader

User stories can be helpful, e.g. "As a ________, I want to _______ so I can _______." Shaun started [@jediuserstories](https://twitter.com/jediuserstories).

From user stories, you can assemble the documentation from the bottom up.

- Create topics from user stories.

- Do card sorts and other exercises to put topics in categories.

- Categories, not linear narrative.

- You will always need to add more topics than your user stories.

- Remember that topics will be reassembled downstream.

Shaun's Twitter handles:

@shaunm

@openhelpconf

@gnome

@projectmallard
