<h2>2022 SLSA “Specification” Meeting Notes  </h2>


<h2>Meeting Info:</h2>

* When: every Monday at 12-1pm Eastern (OSSF Public Calendar)

* Video Call:	LFX Zoom

* Mailing list:	slsa-specification

* Discussion:	#slsa-specification (for invite, see slack.openssf.org)

* Repository:[SLSA](https://github.com/slsa-framework/slsa)

* Leads:Mark Lodato Joshua Lock



<h2>Legal / Code of Conduct</h2>


<p align="justify">Foundation meetings involve participation by industry competitors, and it is the intention of the Linux Foundation to conduct all of its activities in accordance with applicable antitrust and competition laws. It is therefore extremely important that attendees adhere to meeting agendas, and be aware of, and not participate in, any activities that are prohibited under applicable US state, federal or foreign antitrust and competition laws. Examples of types of actions that are prohibited at Linux Foundation meetings and in connection with Linux Foundation activities are described in the Linux Foundation Antitrust Policy available at www.linuxfoundation.org. If you have questions about these matters, please contact your company counsel, or if you are a member of the Linux Foundation, feel free to contact Andrew Updegrove of the firm of Gesmer Updegrove LLP, which provides legal counsel to the Linux Foundation.</p> 

All meeting attendees must follow SLSA Code of Conduct.

[SLSA’s code of conduct](https://github.com/slsa-framework/governance/blob/main/8._Code_of_Conduct.md)  

<h2>Meeting notes</h2>


Most recent on top.

<h3>2-26 (CANCELED)</h3>


<h3>2022-12-19 (CANCELED)</h3>


<h3>2022-12-12</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Fridolín Pokorný(Datadog)
* Kathleen Goeschel (Red Hat)
* Tracy Miranda (Chainguard)
* Brandon Mitchell (IBM)
* Aaron Bacchi (Verizon)
* Arnaud Le Hors (IBM)

Notes:



* Mark Lodato: Meeting schedule for the rest of the year?
    * Cancel next three weeks for holiday, resume on Jan 9
* Arnaud: “Specification Stages” PR out now, next step is adding the tags on existing pages
* Kris K put out draft of threat model and verifying systems doc:  [#508](https://github.com/slsa-framework/slsa/issues/508). Comments welcome
    * [SLSA Builder Spec](https://docs.google.com/document/d/1CdSi1qF-uYM00_LYO-216NKLi4Hu6teCKRLmc23g9IE/edit?usp=sharing)
* Website work is ongoing, if you see PRs, that’s why
* Tracy: no significant progress on conformance program, looking forward to making progress next year
    * Looking to speak to others in CNCF, LF, etc about their experience running similar programs

<h3>2022-12-05</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Shaun Lowry(ActiveState)
* Kris K (Google)
* Brandon Mitchell (IBM)
* Joshua Lock (VMware)
* Melba Lopez (IBM)
* Arnaud Le Hors (IBM)
* Jay WHite (Microsoft)
* Fridolín Pokorný(Datadog)
* Brian Cook (Red Hat)
* Marcela Melara (Intel)

Notes:



* Mark Lodato: Spec v1.0 - #536 submitted
* Mark Lodato: Provenance v1.0 - [#525](https://github.com/slsa-framework/slsa/pull/525) - small iteration on format, no significant progress, plan to spend more time later in month
    * Feedback appreciated on the designs for formatting inputs (parameters and artifacts) [https://github.com/slsa-framework/slsa/pull/525#discussion_r1022249070](https://github.com/slsa-framework/slsa/pull/525#discussion_r1022249070) 
* Kris K: Verifying build systems - [#508](https://github.com/slsa-framework/slsa/issues/508) - putting finishing touches on draft doc, posting to issue this afternoon
    * Documenting how to verify build L3 build systems
* Specification stages: [Link](https://github.com/slsa-framework/slsa/pull/543/files/c6f506dc6ba0c9d4dbffac6798f55413de96e923#diff-7c171f8b7090fd1b7664142370552f44039799f394fb0b126292c3fa16205580)
    * Discussion around abandoned and outdated vs. retired
    * Want to differentiate “this is the latest version” from “this is an old version, it is valid, but new implementations SHOULD use the newer version, and we don’t plan to maintain this old version”.
    * Suggestion: call out that a new version is in progress to give a signal for people that this is coming, even if they’re not following along closely to development
    * Should we connect version numbers with a date?
    * Alternative terms for “retired”: “superseded” (formerly used by Python PEP), “replaced” (new PEP term)
        * [https://peps.python.org/pep-0001/#pep-review-resolution](https://peps.python.org/pep-0001/#pep-review-resolution) 
    * Next step: comment on PR within next day or two, Arnaud to make decision based on feedback

<h3>2022-11-28</h3>


Attendees (please add yourself):



* Shaun Lowry(ActiveState)
* Mark Lodato (Google)
* Brandon Mitchell (IBM)
* Joshua Lock (VMware)
* Arnaud Le Hors (IBM)
* Aaron Bacchi (Verizon) 

Notes:



* Mark Lodato: Provenance v1.0 - #525 - will address comments, haven’t had time to work on it
* Mark Lodato: Spec v1.0 - #536 sent out for review
    * Proposal to merge and iterate in tree. Please indicate intent to comment/review.
* Mark Lodato: When do we “unhide” the spec?
* Arnaud: Add a “status” section to the top of each page, not just the popup, that clearly explains everything we want to say, what to expect, how to review, we’re inviting comments, etc. Suggestion: follow w3c convention [maturity levels](https://www.w3.org/2021/Process-20211102/#maturity-levels), e.g. “working draft”
    * Terms:
        * Working Draft
        * Proposed Specification
        * Specification
    * Where to document: /spec/lifecycle, /maturity-levels, ?
    * Include status in URL? Add a query parameter (e.g. “?draft”)
    * Do we want versioned URLs?
        * W3C is moving away from that towards “living specifications” so that you can fix issues and everyone picks that up
    * Also note that newer version is available?
    * **AI(Arnaud):** Create a GitHub Issue for this.
* Joshua Lock: FYI comments are invited on “[Is there a better term than "packaging ecosystem" that is more obvious to most readers?](https://github.com/slsa-framework/slsa/issues/538)” which has been posted to various OpenSSF Slack channels.
    * “Distribution ecosystem”?
        * “Distribution” is overloaded too: “Linux distribution”, “python distribution”
* Joshua Lock: Package ecosystem diagram, expectations, etc. - early draft
    * Consider data flow diagrams? These are discussed for security use in [https://shostack.org/books/threat-modeling-book](https://shostack.org/books/threat-modeling-book) 

<h3>2022-11-21</h3>


Attendees (please add yourself):



* Shaun Lowry(ActiveState)
* Mark Lodato (Google)
* Mike Lieberman (Kusari)
* Brandon Mitchell (IBM)
* Zach Steindler (GitHub)
* Joshua Lock (VMware)
* Fridolín Pokorný (Datadog)
* Marcela Melara (Intel Labs)
* Justin Cappos (NYU)
* Roy Williams (Microsoft)
* Sebastien Awwad (Anaconda)
* Kris K (Google)
* Leyon Thampi
* Jomcy Pappachen(Google)
* David Zendzian (VMware)
* David A. Wheeler (Linux Foundation)

Agenda:



* Zach Steindler: SLSA Source requirements - what time period do they cover and how do you verify them?
    * What features should we be talking about today that can be delivered in the next 6-12 months?
    * How would you attest to source properties? Walk through every commit? SCM attests to security controls being enabled? Something else?
    * In the interface, could render how long the project has met the source properties. Hopefully monotonically increasing.
    * In future releases, you can show that it has been enabled since the previous release.
    * Considering authenticated pushes?
    * Spec shouldn’t be implementation/system specific - each system is going to have its own implementation of security controls
    * Desirable to align with Scorecards and the checks they are running against SCM ([https://github.com/ossf/scorecard#scorecard-checks](https://github.com/ossf/scorecard#scorecard-checks)) – SLSA can provide additional value because a Scorecard score is a snapshot
    * A way to track that a dependency / risk that you’ve accepted in the past hasn’t increased in risk - i.e. commits were reviewed in a previous release, but they were not going forward
    * Difficult to boil down to reviewed vs. not reviewed, and that becomes even harder in open source where you can’t map strong auth to an individual person.
        * Have been using “two-person reviewed” as a proxy, requires two actors in order to make a change to a system
        * Two-person approval is a good principle to extend throughout SLSA requirements
    * How strong does the assurance need to be? There’s a difference between strong auth of an identity vs. ensuring an account isn’t a sock puppet
    * Identity need not be public, just that the org attests to it
    * Two party review is a means to the end. Ultimately we want to measure risk, and perhaps alternate solutions could be other means to that end of reducing risk
    * Big discussion on sock puppets
    * For OSS we could just represent the increased risk of one-person review as a lower slsa level
* Mark Lodato: Check-in on v1.0 requirements rewrite
    * Types of packages: system, language ecosystem, containers (e.g., OCI), virtual machine images
    * SLSA should cover formal repo systems, as well as direct installs/downloads from websites etc.
    * Need to make sure SLSA & SBOMs aren’t just overlapping
      

<h3>2022-11-14</h3>


Attendees (please add yourself):



* Shaun Lowry(ActiveState)
* Mark Lodato (Google)
* David A. Wheeler (Linux Foundation)
* Melba Lopez (IBM)
* Aaron Bacchi (Verizon)
* Arnaud Le Hors (IBM)
* John Speed Meyers (Chainguard)
* Mike Lieberman (Kusari)
* Brandon Mitchell (IBM)
* Kris K (Google)
* David Zendzian (VMware)
* Joshua Lock (VMware)
* Marcela Melara (Intel Labs)
* Preston Moore(Anaconda)
* Joshua Mulliken(Red Hat)
* Emmy Eide (Red Hat)
* Tracy Miranda (Chainguard)
* Luke Hinds (Red Hat)

Agenda:



* Shaun: signatures for [bundles](https://github.com/in-toto/attestation/blob/main/spec/bundle.md)?
    * See: [https://github.com/in-toto/attestation/blob/main/spec/bundle.md](https://github.com/in-toto/attestation/blob/main/spec/bundle.md)
    * We don’t require bundles, but that means it could be subverted.
    * GUAC is doing this
    * Maybe this is beyond the scope of SLSA?
    * In-toto layouts working on this
* Mark: Build model (early draft, looking for thoughts)
    * Discussed and simplified the model for what a build is. Presented the diagram (not published yet).
    * Maybe look at Data Flow Diagrams (DFDs) as used in threat modeling [https://threatmodeler.com/data-flow-diagrams-process-flow-diagrams/](https://threatmodeler.com/data-flow-diagrams-process-flow-diagrams/) they have a visual notation for security/trust boundaries
* David: Continue discussion on [#321: How strong of a guarantee is required for Isolated and Ephemeral Environment at SLSA 3?](https://github.com/slsa-framework/slsa/issues/321)
    * NOT necessarily personal ID, must be *possible* to automate
    * How far do we go in SLSA 3, what gets pushed to SLSA 4?
    * PR: [https://github.com/slsa-framework/slsa/pull/532](https://github.com/slsa-framework/slsa/pull/532)
        * Simple proposal to merge the two reqs based on the discussion in the issue.
    * Concern- isolated being confused with hermetic. 
    * Mark: presented a possible table with two rows:
        * Provenance guarantees: Exists (L1), Authenticated (L2), Non-forgeable (L3)
        * Isolation strength: None (L1), Hosted (L2), Fully isolated (L3)
    * Terms are little confusing. E.g., hosted vs. fully isolated vs. hermetic, etc. Maybe need better terms in “build system” table
    * Switch from checkbox to labels has mixed feedback:
        * On the one hand, checkboxes have visual appeal and make it more achievable
        * On the other, checkboxes don’t show the progression along axes and maybe make it seem too simple
    * Should we put a potential “L4” be listed in the table? We already have the “potential future level” clickable boxes, but putting it on might show what L3 does **not** require, particularly hermetic
        * Or just “beyond L3”. That implies what’s not required at L3.
    * Idea: should we define “hermetic”, so that we can define the “one less than hermetic” better?
    * There is a concern of all-or-nothing. If you can’t reach the top level (e.g. L4), it’s not worth doing at all.
    * Perhaps just list what’s **not** required for L3?
        * Recommended term: *Future higher levels*
    * AI: Mark will send out a PR so we can discuss this.
* Josh M: [Conformance program](https://github.com/slsa-framework/slsa/issues/515) self-assessment survey and scope of program
    * Proposed scope is to initially target build systems – “can this system meet my SLSA goals?”
    * Kubernetes Checklist: [SLSA Compliance Assessment](https://docs.google.com/spreadsheets/d/1fNdJJZZdEJAJU0ZaCnYcIlZA3L-bwT7vY7ZesqW3WEs/edit#gid=0)
    * Ideally two-way link between requirements and survey questions
    * Similar self-certification programs: [Best Practices](https://bestpractices.coreinfrastructure.org/en), PCI/QSA, Cloud Security Alliance STAR
    * Probably make a public registry of the self-certification
    * **<span style="text-decoration:underline;">Decision:</span>** Initially limit the scope to build systems

<h3>2022-11-07</h3>


Attendees (please add yourself):



* Joshua Lock (VMware)
* Aaron Bacchi (Verizon)
* Mark Lodato (Google)
* Shaun Lowry (ActiveState)
* Jason Lutz (Chainguard)
* Mike Lieberman (Kusari)
* Jay White (Microsoft)
* Brandon Mitchell (IBM)
* Tracy Miranda (Chainguard)
* Melba Lopez (IBM)
* Sunny Yip (Kusari)
* Kris K (Google)
* Jomcy Pappachen (Google)
* Preston Moore (Anaconda)
* Alessandro Mantovani (Qualcomm)
* Josh Dolitsky (Chainguard)
* Leyon Thampi 
* Emmy Eide (Red Hat)

Agenda:



* Mike Lieberman: Making workload identity vs. build service signing distinction clearer
    * Multiple people seem to be confused that workload identity is all you need to to hit SLSA 3’s non-falsifiable provenance. I believe this to be inaccurate as a build workload signing its own provenance means a compromised build environment could still sign whatever it wants.
    * This is different from how I think it was originally intended where you are doing the signing and recording in a different trust domain. This means that a compromised build can never sign its own provenance, have access to the signing secrets, etc.
    * The Tekton Chains approach of a separate system in a separate trust domain “observing” what the build is doing means you get increased confidence that even if the build lied to you, you can compare inputs to outputs as part of an audit or rebuild and have more to go after.
    * I think mechanisms like Github reusable workflows with a restricted set of actions are suitable.
    * Compare this with a build that generates its own provenance. It can lie about its own inputs and there would be a discrepancy between the build pipeline and the provenance.
    * Workload identities, or build derived identities might still be valuable as a requirement or recommendation as they make it much easier to revoke trust on a single signing rather than having to potentially revoke a long lived key.
    * Workload identities also help secure against compromise during the build.
    * Related: [#321: How strong of a guarantee is required for Isolated and Ephemeral Environment at SLSA 3?](https://github.com/slsa-framework/slsa/issues/321)
    * What would be level 2 vs 3?
        * Example: using secrets that are locked down to only be accessible to the CI job, but no guarantee that users can’t extract those secrets
    * Conclusion: If everything required by L3 is embedded in the workload identity, then that would be fine. Otherwise it’s just L2.
        * Example: Sigstore GitHub integration could meet L3 because all of the required fields of SLSA are present in the x.509 certificate and cannot be faked, but it requires the client to verify all of them.
    * Ideally we would clarify this in the spec since there is a lot of confusion here. This ambiguity is undesirable.
* Mark: SLSA v1.0 updates
    * [#529: frame levels around tamper protection](https://github.com/slsa-framework/slsa/pull/529) (submitted)
    * [#528: key principles](https://github.com/slsa-framework/slsa/pull/528) (submitted)
    * [#525: draft of provenance v1.0](https://github.com/slsa-framework/slsa/pull/525) (draft)
        * Should be enough information in the predicate that they should be able to rebuild if they have access to all artifacts
        * At what level do we require “all of the inputs are recorded”? Previously this was L4, now that’s kind of L3. Does L2 not require it?
        * Devil’s advocate: what if you took a snapshot of the container right before the build and listed that as the sole input. Is that sufficient?
            * Raises the question of the provenance of that container - transitive SLSA question
    * Working on split of maintainer vs implementer now
* Tracy: [SLSA Conformance Program](https://github.com/slsa-framework/slsa/issues/515)
    * There’s value in splitting tier 1 (self assessment) from tier 2 and pursuing the self assessment in the first instance
    * Would like to have someone from the conformance proposal attend the tooling meeting and share progress and insights
    * We should determine in this group what is a blocker for 1.0
        * Having a survey in place and defining the split of requirements on projects, services, etc.
    * Let’s work out how to do this in an iterative manner, we won’t get it right the first time
    * There’s a defacto list of “conformant” services in what is accepted by [https://github.com/slsa-framework/slsa-verifier](https://github.com/slsa-framework/slsa-verifier) 

<h3>2022-10-31</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Jeremy Rickard (Microsoft)
* Aaron Bacchi (Verizon)
* Melba Lopez (IBM)
* Shaun Lowry (ActiveState)
* Mike Lieberman (Kusari)
* Brandon Mitchell (IBM)
* Arnaud Le Hors (IBM)
* Tony Loehr (Cycode)
* Preston Moore(Anaconda)
* Emmy Eide (red hat)
* Kris K (Google)
* John Speed Meyers (Chainguard)
* Marcela Melara (Intel Labs)
* Jay White (Microsoft)

Regrets:



* Joshua Lock (VMware) – personal

Agenda:



* No updates on SLSA v1.0 spec
* Aaron -Does this body of work include updating the attestation spec?
    * Great conversation in this issue- [https://github.com/slsa-framework/slsa/issues/508](https://github.com/slsa-framework/slsa/issues/508)
    * Some action items out of it are to 
        * Add fields for attestations to invocation and buildConfig.
        * Rename buildConfig to buildService.
    * Mark’s proposal (very draft): [https://github.com/MarkLodato/slsa/blob/provenance-refactor/docs/provenance/v1.0.proto](https://github.com/MarkLodato/slsa/blob/provenance-refactor/docs/provenance/v1.0.proto)
        * [examples](https://github.com/MarkLodato/slsa/blob/provenance-refactor/docs/provenance/examples.md)
        * Provide guidance to actually define a schema.
        * Might be prohibitive to make everyone define their own type. Might want to define a default schema that works in most cases, e.g. “run a command”, to lower the barrier to entry.
        * Is there some subset of fields that are common to most/all build types?
        * Should we split out buildDefinition to a separate file and include the hash in runDetails. This is basically what Nix does.
            * Con: would be more difficult to propagate two files instead of one
            * So far erred on the side of simplicity. If we had a concrete use case for where we want it split or hashed, that could make the argument stronger.
                * Discussion of logs with provenance, relates to separating files
* Melba - [Build L1 discrepancies ](https://github.com/slsa-framework/slsa/issues/523)- Git Issue# 523
    * [https://deploy-preview-512--slsa.netlify.app/spec/v1.0/requirements#build-track](https://deploy-preview-512--slsa.netlify.app/spec/v1.0/requirements#build-track)
        * L1 - All build steps were fully defined in some sort of “build script”. The only manual command, if any, was to invoke the build script.
        * L2 - All build steps ran using some build service, **not on a developer’s workstation.**
    * [https://github.com/slsa-framework/slsa/blob/main/docs/spec/v1.0/levels.md#levels-and-tracks](https://github.com/slsa-framework/slsa/blob/main/docs/spec/v1.0/levels.md#levels-and-tracks)
        * L1 Benefits:_ Prevents mistakes during the release process, such as building from a client with local modifications._
    * Mark: “client from local modifications” was meant more of a version control thing - did you build from an identical copy of the verison that was uploaded to version control? For example, `cargo publish` blocks this by default unless you pass `--allow-dirty` (or similar).
        * We’d need a requirement that, to call something Build L1, you need a roadblock somewhere in the publication step that stops someone from making a mistake of uploading an unpublished source.
        * The term “local” is probably what’s confusing. It’s “local to the build”. Need better term.
    * Next steps: update levels.md to use more clear language and requirements.md to add a requirement where this is checked
* Mark: [SLSA "Package" Terminology for v1.0](https://docs.google.com/document/u/0/d/1yHc3Bcq8fV5sthCcOhhQBd5UC6xfH9UV-NTry56ocD0/edit)
    * Michael Lieberman: Various folks at KubeCon discussed need for common terminology. Will start a thread.
    * Jay White: Also trying to get folks in Best Practices WG working on a glossary to come here but they couldn’t attend.

<h3>2022-10-24</h3>


Attendees (please add yourself):



* Mark Lodato
* Kris K (Google)
* Wietse Z Venema (Google)
* Shaun Lowry (ActiveState)
* Emmy Eide (Red Hat)
* Melba Lopez (IBM)
* Brandon Mitchell (IBM)
* David Zendzian (VMware)
* Aaron Bacchi (Verizon)
* Arnaud Le Hors (IBM)
* Alessandro Mantovani (Qualcomm)
* ?

Regrets:



* Joshua Lock(KubeCon)
* Marcela Melara (conflict)

Agenda:



* SLSA v1.0
    * Outstanding PRs:
        * [#512](https://github.com/slsa-framework/slsa/pull/512) - update requirements.md to Source vs Build, undefine L4
        * [#514](https://github.com/slsa-framework/slsa/pull/514) - move faq.md (minor)
        * [#516](https://github.com/slsa-framework/slsa/pull/516) - delete most of index.md
    * [Project board](https://github.com/orgs/slsa-framework/projects/1)
    * Terminology
        * Should sync with OpenSSF Best Practices Working Group. Can have that be done in that WG, though perhaps not blocking (not same timeline).
            * AI: Jay White to put us in contact
            * AI: Mark Lodato to put out a proposed starting doc
* To be added to the slsa-foundation org so that you can assign yourself issues, ask Mark Lodato on Slack
* Mark Lodato: Provenance v1.0 format
    * Working on a draft version, looking for early reviews

<h3>2022-10-17</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Joshua Lock (VMware)
* Brandon Mitchell (IBM)
* Jay White (Microsoft)
* Saundra Monroe (Anaconda)
* Sebastien Awwad (Anaconda)
* Preston Moore (Anaconda)
* Alessandro Mantovani (Qualcomm)
* Emmy Eide (Red Hat)
* David A. Wheeler (Linux Foundation)
* Wietse Z Venema (Google)
* Arnaud Le Hors (IBM)
* Kris K (Google)
* Marcela Melara (Intel Labs)
* Aaron Bacchi
* John Speed Meyers (Chainguard)

Regrets:



* Mike Lieberman (Kusari)

Agenda:



* Mark Lodato: SLSA v1.0
    * FYI, submitted [PR #502](https://github.com/slsa-framework/slsa/pull/502): rewrite of levels.md. No requirement changes intended. Expect further rewording around signatures in a subsequent PR.
    * Sent [PR #503](https://github.com/slsa-framework/slsa/pull/503) for review: shift emphasis to expectations + verification in levels.md. PTAL - this is a requirement change! (Will update requirements.md in the future.)
    * Verification
        * [Issue #130](https://github.com/slsa-framework/slsa/issues/130) covers the explanation of automatic (artifacts) vs manual (systems) verification
        * [Issue #46](https://github.com/slsa-framework/slsa/issues/46) covers automatic verification of artifacts
        * [Issue #508](https://github.com/slsa-framework/slsa/issues/508) covers manual verification of systems
* How can we get more contributions?
    * Process going forward - if only done by Mark, it will not finish before end of year
    * Can write PRs, review PRs, comment on issues, even just a thumbs up - all very valuable!
    * How can we make it easier for folks to contribute?
        * Having a clear list of who owns which task - don’t want to work on something that someone else is already working on
        * Having assigned tasks with clear deadlines
        * Making it more clear where contributions are easier
        * Smaller blocks, e.g. PR #502 was massive making hard to review in an available block of time
        * Having a priority list of what we want to tackle
        * Collectively go through to avoid the hesitancy to jump in, build up confidence
    * Could just inch an issue forward by posting a comment on a rough idea, even if not worded carefully
    * Prioritize for v1.0
        * Meta - categorizing issues
        * P0: Splitting up Build vs Source [lodato]
            * Update requirements.md
            * Update index.md
        * P0: Verification - more gathering consensus and figuring out concepts, writing will come later
            * [Issue #130](https://github.com/slsa-framework/slsa/issues/130) covers the explanation of automatic (artifacts) vs manual (systems) verification
            * [Issue #46](https://github.com/slsa-framework/slsa/issues/46) covers automatic verification of artifacts
            * [Issue #508](https://github.com/slsa-framework/slsa/issues/508) covers manual verification of systems
                * Evidence of build service security claims
        * P0 Fix specific issues that are blocking adopters of v0.1
            * (???)
        * P1: Model & Terminology - shovel ready, more explanation than gathering consensus
            * [Better define source](https://github.com/slsa-framework/slsa/issues/129)
            * Define “package”, “ecosystem”, etc.  (needs issue?)
            * Diagram of how builds emit provenance which is the consumed downstream (existing issue - need to find)
            * [Simplify terminology](https://github.com/slsa-framework/slsa/issues/306)
            * [define trusted control plane](https://github.com/slsa-framework/slsa/issues/367)
            * ["build service"](https://github.com/slsa-framework/slsa/issues/369)
            * [maintainer package vs distribution package](https://github.com/slsa-framework/slsa/issues/235)
        * P1: Clarifications & improved wording
            * TODOs in the [1.0 specification](https://github.com/slsa-framework/slsa/tree/main/docs/spec/v1.0) around being less prescriptive on digital signatures
            * A lot of specific issues, e.g. ["service generated"](https://github.com/slsa-framework/slsa/issues/362)
    * AI(Mark Lodato) Create a spreadsheet that gives priorities and hierarchy to issues
        * [https://github.com/orgs/slsa-framework/projects/1/views/1](https://github.com/orgs/slsa-framework/projects/1/views/1)
* Joshua Lock: FYI KubeCon NA next week (Joshua, possibly others, absent)

<h3>2022-10-10</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Kris K (Google)
* Wietse Z Venema (Google)
* Arnaud Le Hors (IBM)
* Jay White (Microsoft)
* Mike Lieberman (Kusari)
* Brandon Mitchell (IBM)
* Marcela Melara (Intel Labs)
* Álvaro Figueroa (Microsoft)

Regrets:



* Melba Lopez
* Joshua Lock (VMware): sick
* Alessandro Mantovani (Qualcomm): personal

Agenda:



* Mark Lodato: Going to submit [SLSA Proposal 3](https://github.com/slsa-framework/slsa-proposals/pull/7) (v1.0 plan)
* Mark Lodato: Review of new levels doc
    * Preview: [https://marklodato-slsa.netlify.app/spec/v1.0/levels](https://marklodato-slsa.netlify.app/spec/v1.0/levels)
    * Source: [https://github.com/MarkLodato/slsa/tree/v1-refactor](https://github.com/MarkLodato/slsa/tree/v1-refactor)
    * (1) use term “evidence” to explain purpose of provenance
        * negative reaction, confusion with other uses of the term (e.g. evidence that the build system was implemented correctly)
    * (2) add expectations and verification
        * no significant comments
    * Will send out a proper PR later this week
* Mark Lodato: v1.0 issue discussion
    * [#498](https://github.com/slsa-framework/slsa/issues/498): Drop “scripted build” requirement (at L1)?
        * Gilbert: If we keep, perhaps call it “blueprint on every run”? Goal is to ensure repeatability
        * Alvaro: in favor of keeping it. Slackware doesn’t have a build service, so L2 is difficult (would have to jump straight to L3). Requiring the script adds value. All builds run on machine of main maintainer (Patrick) for legacy reasons, other maintainers try to replicate.
        * Mike: Confusion between “Scripted build” vs “Build as code”. Not sure keep it vs don’t keep it. Take a step back and say what are the goals here? Difference between running arbitrary commands vs invoking the build itself vs build service. +1 to goal being repeatability. Still confusing between what happens inside build script vs at build service level.
        * Mark: What about transforming the “Scripted build” into defining expectations for what the build should look like, e.g. run this command or series of commands. Ties to the (2) in previous topic.
        * Arnaud: Feels like we lose something if we drop scripted build. What if we have in the README that you just run “go install” or “gcc” and no script exists per se. Does that satisfy?
            * Mark: Yes, I think that would satisfy, which hints to me that it’s really about setting the expectation about how to build.
        * Marcela: +1 to expectations, but expectation also includes how we should verify. Separate out those two requirements? Provenance points to README? Is in-toto layout sufficient?
        * Mark: Yes to in-toto, skeptical about README. Want to focus on automatic verification. Could be explicit (e.g. in-toto layout) or implicit (e.g. trust on first use - same build process as previous version).
        * Mike: Should be sufficient information to reproduce (“repeat?”) the build, though not necessarily bit-for-bit. At higher levels, that includes all of the inputs.
        * Next step: Mark to summarize conversation on Issue and to propose concrete wording, which we can then review and discuss.

<h3>2022-10-03</h3>


Attendees (please add yourself):



* Joshua Lock (VMware)
* Shaun Lowry(ActiveState)
* Melba Lopez (IBM)
* Jay White (Microsoft)
* Emmy Eide (Red Hat)
* Sebastien Awwad (Anaconda)
* Preston Moore(Anaconda)
* Mike Lieberman (Kusari)
* Kris K (Google)
* Mark Lodato (Google) - Have to leave early
* Joshua Mulliken (Red Hat)
* Marcela Melara (Intel Labs)
* Alessandro Mantovani (Qualcomm)
* Jeremy Rickard (Microsoft - sorry for being late)

Regrets:



* Laura Seay (Red Hat) - dr appt

Agenda:



* Mark Lodato (in absentia): [slsa-proposals/pull/7](https://github.com/slsa-framework/slsa-proposals/pull/7) copies the v1.0 proposal to Markdown
    * Please review [via GitHub](https://github.com/slsa-framework/slsa-proposals/pull/7/files?short_path=edd7dd8#diff-edd7dd874321ad9dc14216e4e7448a8b9ecb55b511fdd336a23cdb1a0e2dae9c) (view [with working links](https://github.com/MarkLodato/slsa-proposals/tree/prop-3-slsa-v1.0/0003))
* Joshua Lock: getting more reviewers for v1.0 changes
    * Proposal: one reviewer for v1.0 PRs (contrary to current requirement of 2 approvals), plus a broad review before marking v1.0 as final
    * Thoughts on easing review of 1.0 changes prior to marking them final
    * One challenge is time to review the changes that are proposed, which requires a block of time to review.
    * Mark: in favor of reducing barrier for 1.0 while it’s in draft, book several weeks in November for this group to review the document as a whole in its near final-form
    * Could have no reviews for the draft, then review it all in bulk at the end.
        * Generally not in favor. Having a single reviewer catches a lot and gets people in sync.
    * Most important item for review right now is proposal 3, to ensure it reflects group consensus
    * Mark will have another PR this week updating levels page
    * Proposed convention: if you’re reviewing a PR and it will take some time (more than an hour or so from starting) please comment to let the author and other reviewers know you are doing the work. That way the author knows there’s eyes on it and reviewers know to hold off on merging.
    * Shaun: should we label PRs for 1.0 to ensure they are getting appropriate attention?
        * Let’s use a “SLSA v1.0:” prefix on PR titles?
* Proposal to reduce the number of required reviews from 2 to 1 on PRs to versions that are in draft.
    * Seven “ayes” (Shaun Lowry, Mark Lodato, Emmy Eide, Kris K, Sebastien Awwad, Preston Moore, Alessandro Mantovani) and an abstain (Mike Lieberman) for reducing required reviewers from 2 to 1 for v1.0 changes while v1.0 remains “draft”.
* Mike L: SLSA builder spec.
    * Most metadata about a build using SLSA provenance comes from invocation. There seems to be no standardization even within a builder.
        * Are dependencies and source ~= for SLSA provenance?
        * When builders are providing rich communication through builder specific provenance fields, how do they communicate that to a verifier to be able to leverage? Can they?
        * Shaun: may be implementer specific? Currently no real consensus.
            * Can we codify a convention of the TypeURI being resolvable?
            * Joshua: I think this is already recommended for TypeURI somewhere in the suite of specifications used by the attestation model
            * Can we provide more/stronger guidance around resolving TypeURI and what’s hosted there?
            * V1.0 spec should make intentions clear here; do we intend to have machine verifiable definitions that verifiers can leverage?
        * Mike to put together a proposal.
* Shaun: Ephemeral/Isolated/Hermetic distinctions [#321](https://github.com/slsa-framework/slsa/issues/321) [#230](https://github.com/slsa-framework/slsa/issues/230)
    * Overlap in understanding – we need to provide more actionable guidance and clarity so that implementers are interpreting the requirements as we intend.
    * Spec needs to be firmer about distinctions, but specific technologies should only be recommended in supplementary guidance documentation.
* Mike: we’ve slipped our original schedule, do we have a new estimated window for when 1.0 will be complete as a draft?
    * Shaun: I think we need at least another week or two of work before we can begin to estimate.
    * Good to keep in mind that we should aim to communicate a window for folks to be able to schedule time to review
* Review [maybe-1.0](https://github.com/slsa-framework/slsa/labels/maybe-1.0) ?

<h3>2022-09-26</h3>


Attendees (please add yourself):



* Mike Lieberman (Kusari)
* Shaun Lowry (ActiveState)
* Alessandro Mantovani (Qualcomm)
* Arnaud Le Hors (IBM)
* Wietse Z Venema (Google)
* Preston Moore(Anaconda)
* Fridolin Pokorny (Datadog)
* Marcela Melara (Intel Labs)
* Laura Seay (Red Hat)
* Sebastien Awwad (Anaconda)
* Emmy Eide (Red Hat)
* Jay White (Microsoft)
* Joshua Mulliken (Red Hat)
* Jeremy Rickard (Microsoft)
* Mark Lodato (Google)
* Melba Lopez (IBM)
* Nisha Kumar (Oracle)
* Kris K (Google)

Regrets:



* Jay White (Microsoft) - competing meeting
* Joshua Lock (VMware) – personal conflict

Agenda:



* SLSA v1.0
    * [PR #486](https://github.com/slsa-framework/slsa/pull/486) creates new v1.0 directory, hidden by default
        * Reviews appreciated
        * This new directory will be where we can send PRs to for v1.0 issues
    * Mark started implementing the proposal to split build vs source, call them “tracks”?
        * [lseay] the word "track" sounds optional like you could go down the source "track" OR build "track". 
    * Q: are we going to still define a “source” track but say details TBD?
        * Tentatively yes. Basic idea is to share that this is coming
    * Need to better define “source” either way
    * Also better define “package”, some other OSSF work in this area
        * Also SPDX, CycloneDX, and maybe OWASP etc. have definitions, can at least use as prior art
    * Cleanup of [maybe-1.0 tag](https://github.com/slsa-framework/slsa/issues?q=is%3Aissue+is%3Aopen+label%3Amaybe-1.0)
* Shaun Lowry(ActiveState): Discussion: should we update the DSSE envelope spec to allow for certificates to be embedded in signature blocks?  Seems like it’s common practice already.  See [https://github.com/secure-systems-lab/dsse/pull/50](https://github.com/secure-systems-lab/dsse/pull/50) 
    * Good idea, getting bogged down in the details.
        * When / for what purpose is it OK to put trust chain info in an unauthenticated portion of a signature?  IMO (Seb), it's okay to do it for search efficiency ("check these first", not "check these only"), or alternatively if there is a good, established way for tooling that evaluates the signature to make judgments about the acceptability of the provided trust chain, with the information provided.
    * Mark will ping the author.
* mlieberman85@gmail.com: Define “source” term w.r.t. build requirements (“source” included in the provenance) - [#129](https://github.com/slsa-framework/slsa/issues/129)
    * Shaun’s suggestion:
        * One definition of the inputs to a build:
            * Source(s): that which is acted upon, e.g. unpacked tarball
            * Build script: the actor in the build, that which is executed
            * Dependencies: essentially passive within the build but required for build to complete
    * Mark’s suggestion:
        * Build configuration, config-as-code e.g. GitHub Actions workflow definition file
        * Build parameters, non-config-as-code, e.g. GHA “input” parameter for workflow_dispatch
        * “Source” - artifact that “should” be input, hard to define, maybe drop?
        * Dependencies - artifacts fetched during the build
        * “Environment” - VM/container chosen by the builder, maybe user can select among environments, but not an arbitrary package/VM/container/file
    * Nisha: just call everything that goes into a build “inputs”?
    * Shaun: Useful to identify one or more artifacts as the “source”, meaning the thing that is intended to be built. Otherwise it’s hard to pick out it among dependencies.
    * Mike’s suggestion:
        * Shaun’s suggestion mostly
    * Mark: Agreed on Shaun’s suggestion to identify “source” even if there is no technical control that that was the thing that was actually built.
    * Mark: “Dependencies” here means build-time dependencies = things (and only those things) needed at build time. For example, if you need a container image, just list the container image, not the things inside the container image.
    * Melba: “Direct” are the ones needed by your code, “transitive” are all the other build-time things needed but that came long, so to speak. (declaring it explicitly it in the source code — during build it will grab the non-declared dependencies)
        * Nisha: “Declared” vs “implicit”?
        * Mark: Kind of mirrors the “source” notion above - it is provided by the tenant, with no way for the build system to verify
    * Shaun: Only build-time deps, not runtime deps
    * Recap:
        * Build Configuration - artifact that the build system read
        * Input Artifacts - artifacts that were fetched during the build. Sub-categorization provided by the tenant, with no real way for the build system to verify.
            * “Source” - the nominal thing that is being built
            * “Direct Dependency” - things declared in the build configuration
            * “Indirect Dependency” - things not declared in the build configuration
    * Mark: Assuming above, what should be required at what level?
        * Direct & Indirect deps are Build L4 or later
        * Build config - L2?
        * Source - L2?
        * Undecided - something to think about for the future

<h3>2022-09-19</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Mike Lieberman (Kusari)
* Shaun Lowry (ActiveState)
* Alessandro Mantovani (Qualcomm)
* Arnaud Le Hors (IBM)
* Preston Moore(Anaconda)
* Fridolin Pokorny (Datadog)
* Marcela Melara (Intel Labs)
* Laura Seay (Red Hat)
* Sebastien Awwad (Anaconda)
* Emmy Eide (Red Hat)
* Jay White (Microsoft)

Regrets:



* Joshua Lock (VMware) – sick

Agenda:



* Mark Lodato [10 min]: More explicitly call out the three [use cases](https://slsa.dev/use-cases) (first party, open source, vendor)?
    * Might be good to put more in spec
* Marcela Melara: Roadmap
    * When might the draft of 1.0 be ready?
    * Potential Milestones
        * Branch for 1.0 (or similar) - next week (Mark)
        * Development work of the draft [shoot for mid October]
            * High-level reorgs from the 1.0 proposal (defer slsa 4, rename levels, etc.)
            * Low-level changes from the issue tracker
        * Ratification process [shoot for mid November]
    * Might be good to mention that 1.0 is coming down the line at Kubecon (mid October)
* Triage on open issues for 1.0
    * First-pass label: [maybe-1.0](https://github.com/slsa-framework/slsa/issues?q=is%3Aissue+is%3Aopen+label%3Amaybe-1.0)
    * Decided: [spec 1.0 milestone](https://github.com/slsa-framework/slsa/milestone/2) (currently Mark’s suggestion)
    * Issue issue tracker complete?
        * Please add known missing
        * Mark will add ones for the proposal doc
* Plan to implement
    * Create new v1.0 directory, with a big visible banner that says it’s draft
    * PRs for most issue can go there
    * The major refactor from the proposal can happen in a branch and then merge later
* Action items
    * Everyone: Go through the [maybe-1.0](https://github.com/slsa-framework/slsa/issues?q=is%3Aissue+is%3Aopen+label%3Amaybe-1.0) and [spec 1.0 milestone](https://github.com/slsa-framework/slsa/milestone/2) and comment:
        * If it should or should not go in 1.0
        * Any thoughts/ideas for resolution
    * Mark: Create the v1.0 directory with banner
    * Mark: Will take on the proposal refactor

<h3>2022-09-12</h3>


Attendees (please add yourself):



* Mark Lodato (Google)
* Isaac Hepworth (Google)
* Alessandro Mantovani (Qualcomm)
* Melba Lopez (IBM)
* Laura Seay (Red Hat)
* Preston Moore (Anaconda)
* Sebastien Awwad  (Anaconda)
* John Speed Meyers (Chainguard)
* Joshua Mulliken (Red Hat)
* Marcela Melara (Intel Labs)
* Jay White (Microsoft)

Regrets



* Joshua Lock (OSS EU)

Agenda:



* Joshua Lock [5 min]: rules of engagement: identifying areas and agreeing on high-level approach before assigning work items
* Emmy Eide, Joshua Mulliken, or Laura Seay [10 min]: Trademark SLSA? Licensing? Goes back to the “rejected topic” of Corroboration of security claims
    * Potentially we could produce a set of badges that are specially licensed so that it can only be used if requirements are met. Organizations would have to sign some sort of “license agreement” to be able to use a badge
    * That wouldn’t necessitate that independent audits occur but it would give legal power to revoke the badge if it was discovered that they were not fully complying
    * In the absence of a badge that people can display, the SLSA brand will be diluted.
    * Should be moved to Positioning meeting.
* Sebastien AwwadPreston Moore: [Level 2 Provenance:"Authenticated"](https://slsa.dev/spec/v0.1/requirements#authenticated) criterion's SHOULD clause clarifications
    * Key access rule can readily be interpreted as either too loose or too difficult (maintenance access, key rotation access).
    * Access to a private key can be seen as meaning visibility of the raw key value (exfiltration risk) or ability to use the key during compromise (use risk).
    * Similar issue: [https://github.com/slsa-framework/slsa/issues/187](https://github.com/slsa-framework/slsa/issues/187)
    * Please file issue or [append to the existing issue](https://github.com/slsa-framework/slsa/issues/187). Should be resolved for v1.0.
* Mark Lodato: [SLSA v1.0 Proposal [PUBLIC]](https://docs.google.com/document/u/0/d/13i2f-1SPogsuOCRDBFqQVRx0ieMBc7B-XxHsST-tx5c/edit?resourcekey=0-PRIrYGqLqLfqzEmx2eQ5_Q)
    * Evidence of build service security claims → mark as decided
    * Redefine levels as outcomes, not requirements → defer
        * Too high level to discuss in this venue. We can optionally come up with a concrete proposal and see what people think. Not worth getting caught up in this meeting.
    * Policy - Mark’s suggested path forward:
        * (1) Supplemental guidelines/docs that are not the “requirements” checkboxes that talk about the model, generating provenance, verifying against a policy, etc.
        * (2) In the “requirements”, require a canonical source location at some level. Leave room for interpretation, e.g. whole git repo vs specific branch vs build target. Can be trust-on-first-use. The important thing is that the pointer itself is resistant to tampering.
        * (3) Find a word other than “policy” or “verification.” Leave for the implementation.
        * Need to better define what we mean here
            * "The way I interpret what I think we're trying to talk about with 'policy' is:  information from some authority (maybe it's the authors, maybe it's the builders, maybe it's a third party auditor, etc.) about what to expect from the provenance evidence / attestations."
            * expected source location?  expected signing keys for various attestations?
        * Next step is to sketch a quick requirement wording for "policy" (or whatever we'll call it) and iterate on it.
    * Start implementing?
        * Have unreviewed “draft” branch and publish to a different URL.
* Melba/Shaun/Gilbert/Marcela **(If there’s time)** - Hybrid OSS + Proprietary Scenario

<h3>2022-09-05</h3>


Canceled: US Labor Day holiday.

<h3>2022-08-29</h3>


Canceled: Both leads are absent.

<h3>2022-08-22 </h3>


Attendees (please add yourself):



* Joshua Lock (VMware)
* Melba Lopez (IBM)
* Jeremy Rickard (Microsoft)
* Cameron Banowsky (SHE BASH)
* Saundra Monroe (Anaconda)
* Emmy Eide (Red Hat)
* David A. Wheeler (Linux Foundation)
* Marcela Melara (Intel Labs)
* Michael Scovetta (Microsoft)
* Kris (Google)
* Mike Lieberman (Kusari)
* Keanan McArthur
* Roy Williams (Microsoft)

Regrets:



* Mark Lodato: On leave

Agenda:



* Melba Lopez [5-10 min]:  Review Source vs Build Diagram _(related to evidence of security) _[https://github.com/slsa-framework/slsa/issues/463](https://github.com/slsa-framework/slsa/issues/463) 
    * Draft attempt to visualize the “why” of separating build vs. source
    * If a provider hosts the build, etc., & own everything, they can claim SLSA.
    * But what if they don’t? E.g., a public OSS repo - they don’t know how the code is vetting code, so it’s unknown trust.
    * Discussion around endorsements without access to all attestations to verify. [VSA](https://slsa.dev/verification_summary/v0.1) covers this.
        * There are two different avenues to discuss.  The first is the binding between SLSA claim and its evidence where if one is visible then both are, or is there a model where that is not true.
        * In a SCITT world, there is a concept of endorsement that is based on the SLSA\SSDF claims.  The endorsement can be put onto another instance from the one where the “evidence\claims” are.  Thus allowing for reviewers to bridge between public and internal data.  When it comes to auditing of both the signed content and then with the claims to evidence these need further work.
    * Future topics:
        * discuss hybrid OSS & not model
        * Discuss how that interops with SCITT?
* Joshua Lock: [SLSA v1.0 Proposal [PUBLIC]](https://docs.google.com/document/u/0/d/13i2f-1SPogsuOCRDBFqQVRx0ieMBc7B-XxHsST-tx5c/edit?resourcekey=0-PRIrYGqLqLfqzEmx2eQ5_Q)
    * Evidence of security claims—decided?
        * Heads up: Mark refactored the section without changing content, except for adding #2 - keeping the common requirements (instead of dropping them) and renaming them to “recommendations”. Please take a look.
        * Otherwise, it seems like we’re in agreement? OK to resolve comments?
    * Redefine levels as outcomes—needs more discussion
    * Policy verification
        * How do we incorporate the notion of policy into the specification?
    * Roy: we need to flesh out source requirements and levels
        * have a hard time disentangling source provenance in current build requirements and “source” requirements wrt storage duration, two-party review, etc.
* More generally: How to reveal some information without revealing what should not be revealed? This is a bigger issue for closed source software.
    * I like this example "logs": [
    *     {
    *         "uri": "scheme://some/path",
    *         "digest": {
    *             "sha256": "eb158a15263554e65cab9dfd6f2a640b434d17e7e6af8f40435707662f88234a"
    *         }
    *     }
    * ]
    * you don't share the details within the logs..but u can show where it is and the sha …
    * DAW: That's fine, but then you need to define how the hash is created, and how authorized individuals can use the hash to get the rest of the data.
    * DAW: (I guess technically you need to ensure that the log entries are long enough that identical entries don't reveal things and they can't be brute-forced. I'll be honest, I've never seen that as a *real* problem for log entries :-) ).
    * Michael Scovetta: We'll also need the uri be globally unique.
* Joshua Lock: cancel meeting on US Labor Day (September 5) and UK national holiday next week (August 29)?
    * No objection to canceling both of these meetings
* Mike Lieberman [5 min]: Conformance – What expectations are there for folks claiming to be compliant with the spec?
    * Does a builder meet SLSA requirements?
    * Is the project configured in a SLSA conformant way?
* Areas to develop/model:
    * Hybrid OSS & proprietary (Melba to take a stab)
    * Source code requirements & leveling
    * How we publicly distribute SLSA claims (overlap with discussion in tooling meeting last week [Attestation Distribution and Discovery Design Doc](https://docs.google.com/document/d/163H4cCeT7JaeZGYzkM2yxhavGigIirQjNxfbH3daVwo/edit))

<h3>2022-08-15</h3>


Attendees (please add yourself)



* Joshua Lock (VMware)
* Jeremy Rickard (Microsoft)
* Wietse Z Venema (Google)
* Emmy Eide (Red Hat)
* Mark Lodato (Google)
* Mike Lieberman (Kusari)
* Josiah Bruner (Cisco)
* Brandon Lum (Google)
* Marcela Melara (Intel Labs)
* John Speed Meyers(Chainguard)

Regrets:



* Melba Lopez (will add comments to doc regarding Build vs Source levels)

Agenda:



* Mark Lodato: [SLSA v1.0 Proposal [PUBLIC]](https://docs.google.com/document/u/0/d/13i2f-1SPogsuOCRDBFqQVRx0ieMBc7B-XxHsST-tx5c/edit?resourcekey=0-PRIrYGqLqLfqzEmx2eQ5_Q)
    * Reviews—I added a “Reviews” line to each section to record opinions to record to make sure we have consensus. (Won’t publish that to github, but it’s helpful now to keep track without having to dig through comments and meeting notes.)
        * Request: please add your name if you have an opinion or are reviewing. It’s ok to disagree, e.g. 👎 or 🤔.
    * Postpone definition of SLSA 4—in agreement?
        * Yes. Decided.
    * Separate “build” levels vs “source” levels—in agreement? what term to use?
        * Seems like the best options among what’s available.
        * Would allow “Build L3 Source L1” which is complex.
        * Discussed alternative of “SLSA 3 + two-party review”. Generally negative sentiment - most people want levels.
        * What about a source-only distribution, e.g. a tarball of source code? Still a “build” with a SLSA Build level, since the tarball is not the original form in which modifications are made (e.g. git).
            * Need to be clear on what SLSA Build does and doesn’t buy you.
        * Name “source” isn’t super accurate.
    * Evidence of security claims—next steps to reach agreement?
    * Provenance format v1.0—blocker? [comment from Emmy Eide]
        * Not a hard blocker
* Wietse: Policy model from last week, now written as a [short text document](https://docs.google.com/document/d/1X30O8jlxNP-_n0oTQo_b-c-VwmGeX8y7cHhmw075D04/edit?usp=sharing) for easier discussion.
    * Please comment on doc.
    * Related: would be valuable to have a “What does SLSA do and not do?”
* [Yes, the zoom call ended early for everyone. We’ll just call that a day I guess!]
* Action Items (for next meeting)
    * All: review “Evidence of security claims" section of SLSA v1.0 Proposal
    * All: review and comment on Wietse’s [policy model text document](https://docs.google.com/document/d/1X30O8jlxNP-_n0oTQo_b-c-VwmGeX8y7cHhmw075D04/edit?usp=sharing)
        * Next step: how do we incorporate this into slsa.dev?

<h3>2022-08-08</h3>


Attendees (please add yourself)



* Melba Lopez (IBM)
* Mike Lieberman (Kusari)
* Joshua Lock (VMware)
* Simon Kent(Google)
* Mark Lodato (Google)
* David A. Wheeler (Linux Foundation)
* Marcela Melara (Intel Labs)
* Emmy Eide (Red Hat)
* Jory Burson (Linux Foundation)
* Jeremy Rickard (Microsoft)
* Wietse Z Venema (Google)
* Roy Williams (Microsoft)

Agenda



* Melba: Can a pure scripting approach claim SLSA Level 3?
    * Question:
        * SLSA L2 seems to require the build service to sign, not the pipeline definition itself
        * [GitHub Actions](https://github.com/features/actions) - [slsa-github-generator](https://github.com/slsa-framework/slsa-github-generator)  scripted in the pipeline vs the runner underneath
        * Does the SLSA attestation come from the infrastructure or the pipeline? **(need clarity)**
        * Responsibility chart - pipeline, runner, infrastructure (who can attest to what) (Positioning sig?)
    * Intention of SLSA 3 is that the developer can’t generate/modify the provenance. It’s in the control of some central “infrastructure”.
    * In other words, the goal is to reduce the size of the trust base. Instead of having to trust thousands of projects all configuring their CI/CD system correctly and securely, we can place our trust in a handful of “infrastructure” systems.
    * David A. Wheeler: This really needs clarification, it’s not clear enough.
    * Mike L. : L3 - yes for pure scripting approach --- whatever is running the script that is recording it…it can’t be modified by an end user..must go through some sort of approval process for changes
    * AI: Melba to file an issue for 1.0 milestone (label “Clarification”)
    * Melba: ​​"must prevent” is pretty harsh language ---- “reduces the likelihood of exploitation" --- you can't prevent 100% unless its in the desert disconnected from the world 🙂
* Mark Lodato [5 min]: Roadmap: [0002: for 1.0 require verification for highest level](https://github.com/slsa-framework/slsa-proposals/pull/6)
    * We’re not sure what this means. Is this about reproducible builds? Something else?
    * Mark will reject, we can discuss the idea in this meeting though
* Mark Lodato [20 min]: [SLSA v1.0 Proposal [PUBLIC]](https://docs.google.com/document/u/0/d/13i2f-1SPogsuOCRDBFqQVRx0ieMBc7B-XxHsST-tx5c/edit?resourcekey=0-PRIrYGqLqLfqzEmx2eQ5_Q)
    * Corroboration of security claims: reject -> yes
    * Mark L4 as “draft” but still communicate the requirements that are likely to come down the road: hermeticity, two-party review, etc. -> general agreement
    * Remove “verified history”, retention, etc. from SLSA 1-3, so that SLSA 1-3 is purely about the build process
        * Value in separating source from build requirements
        * Not always the same people responsible for the two systems
        * Idea: splitting source vs build ladders. [Done by Mark]
* Mark Lodato [20 min]: inclusion of policy in v1.0, [SLSA policy model for OSS packages](https://docs.google.com/presentation/d/16MnZt4S2tprgGlS5JZssGN22wZLvZoiSvc7QnFdQVOw/edit?usp=sharing)
    * Policy: corroborate that the claims in provenance match “user’s” expectations
        * A collection of expectations
        * Provenance provides source→artifact mapping, describes what was built and how
    * Not sufficient to just list expected source repo, must also have a “trust policy” listing trusted builders
    * AI: attendees review and add comments to that presentation -[SLSA policy model for OSS packages](https://docs.google.com/presentation/d/16MnZt4S2tprgGlS5JZssGN22wZLvZoiSvc7QnFdQVOw/edit?usp=sharing) - by next week

<h3>2022-08-01</h3>


Attendees (please add yourself)



* Mark Lodato (Google)
* Alessandro Mantovani
* John Speed Meyers (Chainguard)
* Brandon Lum(Google)
* Mike Lieberman (Kusari)
* Emmy Eide (Red Hat)
* Marcela Melara (Intel Labs)

Regrets



* Joshua Lock (VMware) – on PTO 

Agenda:



* [SLSA v1.0 Proposal [PUBLIC]](https://docs.google.com/document/u/0/d/13i2f-1SPogsuOCRDBFqQVRx0ieMBc7B-XxHsST-tx5c/edit?resourcekey=0-PRIrYGqLqLfqzEmx2eQ5_Q)
    * Versioning
        * Agreement on the “Hybrid” approach. We agree to not change the high-level meaning of each level. If we want to renumber, we give them new names.
        * Also would be good to cover specific attacks that they’re covering.
        * For notation, “version” and “revision” are the two main contenders. SSDF uses “version”, 800-53 uses “revision”. Sometimes “rev”, sometimes “r”.
            * Majority opinion for “version”.
            * “SLSA 3 (v1.0)”
        * **To be discussed later:** how often and under what conditions we bump revision numbers. E.g. do we submit on branch then “release” to the main site, or do we always publsh on the site the “head” version? Or call it “errata”?
        * Next step: propose wording to be included in the spec / site.
    * Lock down levels 1 and 2 first, then 3, then 4. List the “draft” ideas of higher levels but with clear warning that it’s up in the air.
        * Discuss “Redefine levels as outcomes, not requirements” proposal, for levels 1 and 2
        * Maybe level 1 means this for hardening and this for provenance, level 2 means this for hardening and this for provenance, etc.
        * SBOM and provenance are covering slightly different things, do we want to include Vulnerability Management into SLSA?
            * There is interest in possibly expanding to those areas, perhaps as different names, but for v1.0 we probably want to stick to just provenance to stay focused
        * At previous company, there was need to define the value of SLSA at each level.
            * SLSA 1 has value in retaining records for auditing. It doesn’t prevent tampering.
            * SLSA 2 starts to deter tampering.
        * Might be helpful to provide definition of what even falls under provenance. E.g. has to be SLSA format vs SBOM.
            * Should make that clearer. Intention is not to require a specific format, just _suggest_ the one.
            * Also need to make it more clear in the docs for the recommended predicate format what goes in at what level.
            * Perhaps not calling it “SLSA provenance” would avoid confusion
        * Agreement on:
            * SLSA 1 = provide provenance
            * SLSA 2 = build service, signed by build service
        * Question: do we include a requirement about establishing a “canonical” (or expected) source repository, or do we leave that out of SLSA 2 (either for SLSA 3+ or out entirely)?
            * Some cases a distro might want to build from a fork, some might not.
                * Would be different packages, with different policies
            * Provenance says “artifact with this hash was built from source with that hash”, while a policy is a “matcher” saying “any artifact to be called package X must be built from a source at location Y”
            * Is SLSA an arbiter of truth on the sources of truth?
        * Consensus: Move to higher level (if at all), not part of level 2. Still don’t have a clear shared mental model for how it works, let alone clear wording. Plus it might be too big a jump from 1 to 2.
* Minor logistic notes
    * OSSF calendar still missing cal for breakouts? Or am i calendaring wrong?

<h3>2022-07-25</h3>


Attendees (please add yourself)



* Mark Lodato (Google)
* Alessandro Mantovani (Qualcomm)
* John Speed Meyers (Chainguard)
* Joshua Lock (VMware)
* Shaun Lowry (ActiveState)
* Melba Lopez (IBM)
* Jeremy Rickard (Microsoft)
* Emmy Eide (Red Hat)
* Marcela Melara (Intel Labs)
* Isaac Hepworth (Google)

Agenda:



* Mark Lodato:
    * Priorities for workstream
        * Rename to “Special Interest Group (SIG)” --per Brian B. [https://github.com/slsa-framework/governance/issues/11](https://github.com/slsa-framework/governance/issues/11) 
        * Alignment on what we want to get out of 1.0 proposal
            * Do we even agree on 1.0 being the next release? We’d like to indicate stability and maturity.
        * What are priorities? What’s deferred?
        * Melba: Do we focus on levels 1 & 2 for 1.0?
            * Mark: feel like 1, 2, & 3 are well defined. Level 4 is less well defined with hermeticity, reproducibility, etc.
            * Melba: lot of confusion even on 1 and 2 w.r.t. terms, concepts, ambiguity
            * Shaun: keep requirements succinct but have more clarifications, also +1 for v1.0 (as opposed to another v0.x release)
* Mark Lodato: [SLSA v1.0 proposal](https://docs.google.com/document/d/13i2f-1SPogsuOCRDBFqQVRx0ieMBc7B-XxHsST-tx5c/edit?usp=sharing&resourcekey=0-PRIrYGqLqLfqzEmx2eQ5_Q)
    * Hard problems we should tackle:
        * Versioning
        * Evidence of claims (i.e. common requirements)
            * Shaun: Common security requirements blows up the scope of what an auditor must do, e.g. SOC-2, try to keep these out of scope for v1.0
            * Marcela: Still valuable to provide guidance on techniques or how you can qualify, readers can have a goalpost to work toward
                * Mark: e.g. SUSE found it valuable
            * Michael: Can look to see community best practices around this
        * Corroboration of evidence
            * Michael, Isaac, John: Third party auditor
            * Michael, Mark: separate builder requirements vs artifact/tenant requirements
            * Marcela: may want to introduce notion of reputation
        * Reframing in terms of benefits
            * Michael: +1, valuable to do this ASAP, common source of confusion, what do I get from SLSA X
            * Joshua: torn, might make it more confusing
            * Emmy: user stories for each levels, cautious on what types of attacks we’re preventing, who might be targeting level 1
            * John: could have some additional documentation to explain what each level achieves but doesn’t require redefining each level
            * Shaun: can make it more measurable, opens to more implementations
            * Mark: both documents are valuable, which is the “specification” and which is the ancillary document? Is the levels document the spec and the requirements the normative document?
        * Policy verification
            * Mark: MUST work this in to the spec somehow
        * Drop source integrity?
            * Mark: torn on this, could split out and call it something else that is verified under a separate label
            * Shaun: in favor at the moment, when multiple parties in the chain then it’s hard for a build service to enforce back up the chain. Makes 
            * Melba: would like to keep review requirement, could list known-unknowns
            * John: +1 on keeping, but not strong opinion
            * Joshua: torn, could postpone this problem if we focus on SLSA 1 & 2. Also need to clarify just recipe or all of the source code
            * Marcela: not sure yet, but note that build service certification is different from source system certification
            * Michael: 
            * Mark: maybe next step is to come up with concrete proposals and see which we like
            * Shaun: also speaks to transitive levels, is the source code considered a separate artifact with its own SLSA level?
            * Mark: having level apply only to built artifact, not the source from which it’s built, has some appeal
            * Mark: +1 on just defining lower levels first
* Collaboration model [10 min] - meetings, docs, slack, etc.
    * Other topics that were not in Mark’s doc?
        * Joshua: relationship to SCITT ⇒ Positioning SIG?
        * Joshua: reviewing the doc is a good next step
