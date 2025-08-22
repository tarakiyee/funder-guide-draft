---
title: " Evaluating Technical Standards in the Public Interest: A Guide for Public Funding Organizations"
abbrev: "public-funder-guide"
category: info

docname: draft-tarakiyee-funder-guide-latest
submissiontype: "independent"
number:
date:
v: 3
keyword:
 - funder guide
 - standards evaluation
 - public interest
venue:
  github: "tarakiyee/funder-guide-draft"
  latest: "https://tarakiyee.github.io/funder-guide-draft/draft-tarakiyee-funder-guide.html"

author:
 -
    fullname: "Tara Tarakiyee"
    organization: Sovereign Tech Agency
    email: "me@tarakiyee.com"

normative:
  RFC2026:
  RFC3935:
  RFC6852:
  RFC7282:
  RFC7942:
  RFC8179:
  RFC8890:

informative:
  RFC1958:
  RFC3552:
  RFC5321:
  RFC5322:
  RFC5657:
  RFC6410:
  RFC6576:
  RFC6973:
  RFC7258:
  RFC7704:
  RFC8170:
  RFC8280:
  RFC9501:
  RFC9620:

--- abstract

Technical standards are agreements that make the Internet and digital technologies work. This document helps public funding organizations understand and evaluate opportunities to invest in standards development. Drawing from decades of Internet Engineering Task Force (IETF) experience documented across numerous RFCs, it explains key concepts like interoperability, rough consensus, and running code while providing practical frameworks for assessment. The guide emphasizes that successful standards require not just technical excellence but also open processes, real implementations, and consideration of human rights and social impact. It tries to provide concrete evaluation criteria while remaining accessible to funders new to standards work.

--- middle

# Introduction

Technical standards shape our digital world. They enable that your phone can connect to any WiFi network your email reaches its destination regardless of provider, and websites look the same across different browsers. For public funding organizations, understanding standards is important  because standards decisions made today affect digital infrastructure for decades and can often have societal implications beyond technical correctness.

This guide synthesizes lessons from the Internet Engineering Task Force (IETF). The IETF's approach, which is documented across thousands of documents called RFCs (Requests for Comments), offers practical principles that can be useful for evaluating whether a standards project merits public investment.

## Why Public Funding for Standards Matters

Public funding plays two critical roles in standards development:

**Ensuring Public Interest Representation**: Even commercially viable standards need public interest voices. Industry participants naturally focus on their business needs, but standards affect everyone, from everyday users, civil society, researchers, and most importantly communities who may lack resources or proximity to technical standard production to participate. Public funding can:

- Support participation by public interest advocates
- Fund privacy and human rights impact assessments
- Enable attendance at crucial in-person meetings
- Ensure accessibility and internationalization reviews
- Bring in voices from underserved communities

**Addressing Market Failures**: Some essential standards lack commercial incentives entirely:

- **Public goods**: Standards that benefit everyone but generate no direct revenue (like security protocols that protect personal privacy)
- **Coordination problems**: Standards requiring simultaneous adoption by competitors not willing to work with each other.
- **Long-term infrastructure**: Standards whose benefits appear over decades rather than quarterly earnings cycles.
- **Underserved communities**: Standards addressing needs of users who lack market power.

Strategic public investment ensures standards serve society's needs, not just commercial interests.

## Document Structure and Approach

This document provides:

- Core concepts essential for understanding standards ({{concepts}})
- The IETF model and its key principles ({{ietf-model}})
- Practical evaluation criteria for funding decisions ({{evaluation}})
- Human rights and social considerations ({{human-rights}})
- Methods for following standards development ({{followingwork}})
- Common pitfalls and how to avoid them ({{pitfalls}})
- Concrete recommendations for funders ({{recommendations}})

I tried to reference specific RFCs when possible, not to overwhelm with citations but to show that these principles emerge from the decades of practical experience documented by the IETF.

# Understanding Technical Standards {#concepts}

## What Standards Actually Do

Technical standards are documented agreements about how technology should work. They're not software or hardware themselves, but rather the specifications that allow different implementations to work together. Consider email: {{RFC5321}} defines how email servers transfer messages, while {{RFC5322}} defines the message format. Any software following these specifications can exchange email with any other conforming software.

This **interoperability** is the fundamental purpose of standards. It is absolutely neccesary for a global internet to work.

## The Standards Development Lifecycle

Standards typically evolve through several phases:

1. **Problem Identification**: Recognition that standardization could solve a coordination problem or enable new capabilities

2. **Experimentation**: Building prototypes and testing different approaches (what the IETF calls "running code")

3. **Specification**: Writing down how the technology works in sufficient detail for independent implementation

4. **Implementation and Testing**: Multiple parties build implementations and verify they work together

5. **Deployment**: Real-world adoption, revealing issues that need refinement

6. **Maintenance**: Updating the standard based on experience, fixing errors, adding needed features

The IETF formalizes this in {{RFC2026}} "The Internet Standards Process," which requires demonstrating "sufficient successful operational experience" before advancing standards. This means standards must prove themselves in reality, not just theory.

## Standards Organizations and Their Approaches

There are several technical standards organisations and they don't all operate the same way. It's important for funders to understand this to determine the most effective way to engage with the standards process. While this guide primarily focuses on the IETF, it's important to note this here to give the full picture.

- **IETF**: Emphasizes "rough consensus and running code," open participation, and voluntary adoption.
- **W3C**: A vendor forum focused on web standards, strong industry membership and stringent patent policies.
- **IEEE**: Develops standards through formal balloting processes with strict membership rules.
- **ISO**: Creates international standards through national body representation.

Understanding an organization's approach is important to help determine the appropriate engagement mechanisms (if any) to align their proccesses with public interest goals.

# The IETF Model {#ietf-model}

## The Mission: Making the Internet Work Better

{{RFC3935}} defines the IETF's mission: "to make the Internet work better by producing high quality, relevant technical and engineering documents that influence the way people design, use, and manage the Internet."
- **"Work better"** points to the incremental approach of the IETF, not waiting for perfection.
- **Quality and relevance** point to how IETF standards must be both technically sound and actually used in the real world.
- **Influence, not mandate** highlights an important part of how IETF Standards work. They often succeed through voluntary adoption, however this doesn't stop national and international regulatory bodies from voluntarily adopting IETF standards in their regulation.

## Rough Consensus and Running Code

This foundational IETF principle, examined in {{RFC7282}} "On Consensus and Humming in the IETF," means:

**Rough Consensus**: Decisions aren't made by voting but by addressing technical objections until most participants agree the result is acceptable. This prevents both single-party veto power and tyranny of the majority. As {{RFC7282}} explains, consensus means "everyone has had their issues addressed, not necessarily accommodated."

**Running Code**: Ideas must be validated through acutal software or hardware implementations. {{RFC7942}} "Improving Awareness of Running Code" established practices for documenting implementation status, recognizing that standards developed without implementation experience often fail.

Together, these principles ensure standards are both technically sound (through implementation experience) and broadly acceptable (through inclusive consensus building).

## Open Process and Participation

{{RFC2026}} Section 6.5 establishes that IETF processes must be "open and fair" with "no more than a reasonable and non-discriminatory fee" for participation. {{RFC9501}} strengthened this in 2023 by requiring free remote participation options, recognizing that economic barriers prevent global participation.

However, openness in principle doesn't guarantee participation in practice. Despite free remote options, critical discussions often happen in person - during meeting breaks, over dinner, side meetings, or in hallway conversations. The IETF meets three times yearly in different global locations, and attending costs thousands of dollars per meeting, and that doesn't include interim meetings for specific work that happen in-between. This creates an invisible barrier where well-funded corporate participants have advantages over public interest advocates.

The openness is meant to serve multiple purposes:

- Enables participation by affected stakeholders worldwide.
- Acts as a bulwark against capture by special interests
- Improves quality through diverse perspectives
- Builds legitimacy through inclusive processes

However achieving these benefits meaningfully and in practice requires concentrated effort, and for the purposes of this guide, adequtete funding.

## The End-to-End Principle and User Focus

{{RFC1958}} "Architectural Principles of the Internet" established that intelligence belongs at the network edges, not in the middle. This "end-to-end principle" means the network should be a simple, neutral pipe that doesn't constrain what users do with it.

{{RFC8890}} "The Internet is for End Users" made this explicit: when different parties' interests conflict, standards should prioritize end users over intermediaries like network operators or vendors. This principle helps resolve difficult trade-offs by asking "what serves users best?"

# Evaluating Standards: A Practical Framework {#evaluation}

## Technical Excellence

### Implementation Requirements

Following {{RFC2026}}'s advancement criteria, evaluate:

**Running Code**: Are there working implementations? {{RFC7942}} provides a framework for documenting implementation status:

- Research prototypes (proof of concept)
- Production implementations (deployed systems)
- Multiple independent implementations (true interoperability)

Without running code, you're funding research, not standardization.

**Interoperability Testing**: {{RFC5657}} "Guidance on Interoperation and Implementation Reports" describes how to verify that independent implementations actually work together. Look for:

- Documented test results between implementations
- Public interoperability events
- Clear problem reports and resolutions

**Technical Quality**: Does the specification demonstrate the technical excellence {{RFC2026}} requires? Consider:

- Clarity and completeness of specification
- Appropriate complexity for the problem
- Security integrated from the beginning ({{RFC3552}})
- Scalability for anticipated deployment

### Deployment Feasibility

{{RFC8170}} "Planning for Protocol Adoption and Subsequent Transitions" identifies key factors for successful deployment:

- **Incremental Deployability**: Can the standard be adopted gradually, or does it require everyone to switch simultaneously?
- **Clear Benefits**: Do early adopters gain value even before widespread deployment?
- **Transition Mechanisms**: How do systems migrate from current practice?
- **Cost-Benefit Analysis**: Are implementation costs justified by expected benefits?

## Process Openness

### The OpenStand Principles

{{RFC6852}} "Affirmation of the Modern Paradigm for Standards" established five fundamental principles that public funders should verify:

1. **Due Process**: Decisions through defined processes with appeals
2. **Broad Consensus**: Agreement across diverse stakeholders
3. **Transparency**: Public access to proceedings and documents
4. **Balance**: No domination by particular interests
5. **Openness**: Participation available to all interested parties


### Consensus Building

{{RFC7282}} explains how genuine consensus works. Warning signs of problematic processes include:

- Decision by voting rather than addressing objections
- Single organization dominating discussions
- Technical concerns dismissed for business reasons
- Rushed timelines preventing thorough review

## Intellectual Property Considerations

{{RFC8179}} "Intellectual Property Rights in IETF Technology" establishes a clear preference hierarchy:

1. No patent claims (ideal)
2. Royalty-free licensing to everyone
3. Reasonable and non-discriminatory (RAND) terms with reciprocity
4. RAND with fees (least desirable)

Critically, {{RFC8179}} requires that security mechanisms must be royalty-free, recognizing that patent barriers to security implementation harm everyone. Public funders should similarly prioritize royalty-free standards that maximize public benefit.

# Human Rights and Social Impact {#human-rights}

Standards that seem purely technical often have profound social implications. A protocol's design choices can enable surveillance or protect privacy, facilitate censorship or preserve free expression, include or exclude marginalized communities. Even commercially successful standards may optimize for business needs while ignoring public interest concerns.

Public funding can ensure these impacts are assessed and addressed, even in standards with strong commercial backing.

## The Evolution Toward Human Rights Considerations

The IETF's approach to standards has evolved from purely technical considerations to recognizing broader impacts. {{RFC8280}} "Research into Human Rights Protocol Considerations" pioneered systematic analysis of how technical choices affect human rights. {{RFC9620}} "Guidelines for Human Rights Protocol Considerations" (2024) provides practical assessment tools.

However, current frameworks show a bias toward civil and political rights such as privacy, freedom of expression, freedom from surveillance. While these are crucial, the full spectrum of human rights includes economic, social, and cultural rights that remain underexamined in standards work:

- **Economic rights**: How do standards affect access to work, fair wages, and economic participation? Do they enable or prevent economic exploitation?
- **Social rights**: Do standards support rights to education, health, and social security? How do they affect community participation?
- **Cultural rights**: Do standards respect cultural diversity, linguistic rights, and traditional knowledge? Do they impose particular cultural assumptions?

As a global network serving diverse populations, the Internet's standards must consider all human rights. Public funders can support development of more comprehensive assessment frameworks that address this gap.

## Privacy as a Fundamental Consideration

{{RFC6973}} "Privacy Considerations for Internet Protocols" established that privacy analysis must be integral to standards development, not an afterthought. Key considerations include:

- **Data Minimization**: Protocols should reveal minimum necessary information
- **User Control**: Users should understand and control information disclosure
- **Anonymity and Pseudonymity**: Support for users who need to protect their identity
- **Confidentiality**: Protection of communication content and metadata

{{RFC7258}} went further, declaring "Pervasive Monitoring Is an Attack" that protocols should mitigate. This transformed privacy from a feature to a security requirement.

## Accessibility and Inclusion

{{RFC7704}} "An IETF with Much Diversity and Professional Conduct" documents that diverse participation improves standards quality. Standards should be evaluated for:

- **Accessibility**: Can people with disabilities use the technology?
- **Internationalization**: Does it work for all languages and cultures?
- **Digital Divide**: Does it function in low-bandwidth or high-latency environments?
- **Economic Barriers**: Can it be implemented without expensive licenses or hardware?

Beyond these technical considerations, standards affect broader social and economic inclusion:

- **Economic Participation**: Do standards enable or restrict economic opportunities? For example, payment protocols that require bank accounts exclude the unbanked.
- **Educational Access**: Can standards support diverse learning environments and pedagogical approaches? Do they require expensive infrastructure that limits educational access?
- **Cultural Preservation**: Do standards allow communities to maintain their languages, scripts, and cultural practices online?
- **Social Services**: How do standards affect delivery of healthcare, social support, and public services?

Public funders should support research into these broader impacts and development of assessment tools that capture the full range of human rights considerations.

## Practical Assessment Questions

When evaluating human rights impacts, consider:

- Could this standard enable censorship or surveillance?
- Does it protect privacy and freedom of expression?
- Does it support freedom of association and assembly online?
- Does this standard affect people's ability to work or access economic opportunities?
- How does it impact access to education, healthcare, or social services?
- Does it respect linguistic diversity and cultural practices?
- Will it widen or narrow global digital divides?
- Does it enable local innovation or require dependence on foreign technology?

These broader assessments are often completely absent from standards work. Industry participants may not see them as relevant. Public funding can support more Human Rights and Privacy assesments to be done.

# Following Standards Work {#followingwork}

## Understanding IETF Documentation

The IETF's work is documented in RFCs, but not all RFCs are standards. {{RFC2026}} defines several categories:

- **Standards Track**: Specifications intended for Internet standards
- **Informational**: General information for the community
- **Experimental**: Research or early-stage work
- **Best Current Practice (BCP)**: Operational guidance

Within Standards Track, documents progress through maturity levels:

- **Proposed Standard**: Stable specification ready for deployment
- **Internet Standard**: Demonstrated widespread deployment and interoperability

## Information Sources

### Official IETF Resources

- **IETF Datatracker** (datatracker.ietf.org): Real-time status of all IETF documents
- **RFC Editor** (rfc-editor.org): Published RFCs and errata
- **Mail Archives** (mailarchive.ietf.org): Complete discussion history
- **Meeting Materials**: Agendas, presentations, recordings from triannual meetings

### Key Documents to Review

For any standards project, examine:

- **Charter**: Working group scope and deliverables
- **Internet-Drafts**: Works in progress showing current thinking
- **Implementation Status**: Following {{RFC7942}} format
- **Mailing List Activity**: Quality and breadth of technical discussion
- **Meeting Minutes**: Decisions and consensus points

## Engagement Strategies

Funders can engage with standards development through:

- **Monitoring**: Following relevant working groups and documents
- **Participation Support**: Funding public interest advocates to engage deeply in standards work, including travel to key meetings
- **Supporting Implementations**: Funding reference implementations that demonstrate public interest features
- **Research**: Supporting studies on deployment and impact
- **Capacity Building**: Training new participants from underrepresented communities
- **Coalition Building**: Bringing together public interest groups to coordinate standards engagement

Remember that meaningful participation requires sustained engagement. A single comment or meeting attendance rarely influences outcomes. Public interest advocates need support for the long-term commitment that effective standards work requires.

# Common Pitfalls and How to Avoid Them {#pitfalls}

## The "Build It and They Will Come" Fallacy

**Pitfall**: Assuming that creating a standard guarantees adoption.

**Reality**: Standards succeed through voluntary adoption based on clear value propositions. {{RFC8170}} documents many technically excellent standards that failed due to lack of adoption incentives.

**Avoidance**: Require clear analysis of adoption incentives, transition costs, and deployment strategies. Fund implementation and deployment support, not just specification development.

## Vendor Capture

**Pitfall**: Standards that appear open but actually lock in a single vendor's approach.

**Reality**: Some organizations use standards to legitimize proprietary technology. True standards enable competitive implementations.

**Avoidance**: Verify multiple independent implementations are possible. Check who participates in development and whether processes follow {{RFC6852}}'s OpenStand principles.

## Complexity Creep

**Pitfall**: Standards that try to solve every possible problem become too complex to implement correctly.

**Reality**: As {{RFC1958}} notes, "Keep it simple. When in doubt, use the simplest solution." Complex standards often fail or result in incompatible partial implementations.

**Avoidance**: Favor incremental approaches that solve immediate problems while enabling future extension. Require evidence that complexity is necessary, not just potentially useful.

## Ignoring Existing Practice

**Pitfall**: Creating "clean slate" standards that require abandoning working systems.

**Reality**: The Internet's success comes from evolutionary improvement, not revolutionary replacement. Standards must work with existing infrastructure.

**Avoidance**: Require clear migration paths from current practice. Fund standards that enhance rather than replace existing systems.

## Premature Standardization

**Pitfall**: Standardizing before understanding the problem space.

**Reality**: {{RFC2026}} requires "sufficient successful operational experience" because standards created without deployment experience often standardize the wrong things.

**Avoidance**: Fund experimentation and prototype development before formal standardization. Look for evidence of real deployment experience, not just laboratory testing.

# Recommendations for Public Funders {#recommendations}

## Essential Requirements

Based on IETF experience, public funders should require:

1. **Working Implementations**: Following {{RFC7942}}, require documented implementation status before significant funding.

2. **Open Process**: Verify adherence to {{RFC6852}}'s OpenStand principles

3. **Multiple Implementers**: Ensure genuine interoperability per {{RFC5657}} guidelines. Often it is good to have a diversity of implementations, such as a reference implementation that is faithful to the specification, and an opinionated one that maintainas interoperability while focusing on a specific use case for the standard.

4. **Human Rights Assessment**: Apply {{RFC9620}}'s evaluation framework

5. **Royalty-Free Licensing**: Especially for security features, per {{RFC8179}}

## Evaluation Process

A systematic evaluation should include:

1. **Problem Validation**: Is there a real problem that standardization can solve?

2. **Technical Assessment**: Does the approach demonstrate technical excellence per {{RFC2026}}?

3. **Implementation Verification**: Is there running code and interoperability testing?

4. **Process Review**: Are development processes open and inclusive?

5. **Impact Analysis**: What are the human rights and social implications?

6. **Deployment Planning**: Is there a realistic path to adoption per {{RFC8170}}?

## Investment Strategies

### Supporting Public Interest Participation

Even in commercially viable standards, public funding should ensure public interest representation:

**Travel and Participation Support**:

- Fund attendance at critical IETF meetings and interim sessions
- Support long-term engagement, not just one-time participation
- Enable participation in multiple working groups when issues intersect
- Cover costs for preparatory work and follow-up activities

**Impact Assessments**:

- Fund independent privacy impact assessments per {{RFC6973}}
- Support human rights reviews following {{RFC9620}}
- Enable accessibility evaluations
- Document impacts on marginalized communities

**Capacity Building**:

- Train public interest technologists in standards processes
- Support fellowships for underrepresented participants
- Create mentorship programs pairing newcomers with experienced participants
- Fund time for advocates to engage deeply with technical details

### Direct Standards Development

When funding standards development directly:

- Support multiple independent implementations, not just specifications
- Require public documentation of decisions and rationales
- Fund long-term maintenance, not just initial development
- Include support for interoperability testing events
- Ensure public interest voices are resourced throughout the process

### Ecosystem Support

Beyond direct development, consider funding:

- **Conformance Tools**: Test suites verifying correct implementation
- **Community Building**: Supporting participation from underrepresented groups
- **Research and Assessment**: Studies on deployment barriers, comprehensive human rights impacts, and lessons learned

## Success Metrics

TODO

# Conclusion

Technical standards shape our digital infrastructure in ways that affect billions of people. While industry drives much standards development, commercial incentives alone don't ensure public interest considerations. Even highly commercial standards need public interest voices to address privacy, human rights, accessibility, and impacts on marginalized communities.

Public funders have two essential roles: supporting standards that markets won't produce, and ensuring public interest representation in all standards work. This includes funding participation by civil society advocates, supporting impact assessments that industry might skip, and ensuring diverse voices can engage despite economic barriers.

The IETF's decades of experience, documented in thousands of RFCs, provide proven principles for public funders to evaluate effective and open standards work. While the IETF process is nominally open, meaningful participation requires resources, such as travel to meetings, time for deep technical engagement, expertise development. Public funding can level this playing field.

Key insights from IETF experience:

- Successful standards emerge from practical experience, not theoretical design
- Running code and multiple implementations are essential
- Open processes need active support to achieve diverse participation
- Human rights and social impacts require dedicated assessment
- Standards embedding public values need public investment

Most importantly, remember that standards are means, not ends. The goal isn't to create standards but to solve problems that improve people's lives. Public investment ensures these solutions serve everyone, not just those with the loudest voices or deepest pockets.

# Security Considerations

This document describes evaluation frameworks that inherently improve security by:

- Requiring security consideration from initial design
- Mandating royalty-free security mechanisms
- Evaluating privacy and surveillance resistance
- Supporting transparent processes that enable security review

Funders should recognize that security cannot be added after standardization - it must be designed in from the beginning.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
