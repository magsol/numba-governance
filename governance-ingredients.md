# Numba Governance

## The Project (numba)

A definition of the numba project and its goals, principles, and design philosophy. License, Code of Conduct, other institutional affiliations, and high-level participation and contribution guidelines can also go here. e.g., from pandas:

> The Project is developed by a team of distributed developers, called Contributors. Contributors are individuals who have contributed code, documentation, designs or other work to one or more Project repositories. Anyone can be a Contributor. Contributors can be affiliated with any legal entity or none. Contributors participate in the project by submitting, reviewing and discussing GitHub Pull Requests and Issues and participating in open and public Project discussions on GitHub, mailing lists, and elsewhere. The foundation of Project participation is openness and transparency.

(along with a list of current contributors)

## Governance Structure

A high-level definition of the structure of governance around numba, as well as the goals of the governance structure (e.g., pandas specifically highlights "openness and transparency, active contribution, and institutional neutrality" as its governance goals; the latter would be interesting for numba to adopt!).

In terms of the governance structure itself:

 - PyTorch has a hierarchical governance model: at the lowest level, you have *contributors*, then *module maintainers*, then *core maintainers*, then *lead core maintainer* at the highest level (BDFL)
 - Pandas has only the upper two levels in its governance structure
 - Jupyter's model is flatter, consisting of two disjoint bodies with some amount of overlap: an Executive Council (EC) and a Software Steering Council (SSC), the former of which focuses mostly on non-technical concerns while the latter deals primarily with software decisions
 - conda is a mix: there are "external contributors" and "project teams" of core maintainers, with a "steering council" at the top that has representation from every project, as well as an "emeritus steering" which is exclusively former steering council members

Basically: **who is involved in the decision-making process**. It's interesting to me that PyTorch includes external contributors in its governance hierarchy, but conda/pandas/Jupyter do not. This is not to say that external contributors have no pull at all in those latter projects, but it's worth considering and explicitly noting if that is the case here.

Numba likely falls closest to pandas, with governance stakeholders consisting of (e.g.): external contributors, core maintainers, and maybe a BDFL (the PyTorch governance document makes a good case for this role in the case of "controversial decisions").

### Roles

Whatever roles are enumerated in the governance structure, here they are explained in terms of their responsibilities and privileges, as well as the processes for being considered a member of the given role (e.g., how to become a core maintainer).

 - Both pandas and PyTorch go great lengths to identify the BDFL as a special role primarily meant for breaking ties or stalemates during the regular business of the core maintainers, and as such is envisioned as rarely exercising their full authority; a "ceremonial+" type role. PyTorch specifically mentions the utility of this role in the case of "controversial decisions / changes", like backwards-incompatibility, removal of core features or support, additions to the core library, or semantic/syntactic changes to the core framework.
 - conda and Jupyter have no BDFL, but instead have a top-level steering/executive committee that fulfill the same role as the BDFL+core maintainers.
 - Neither pandas nor PyTorch have explicit term limits on the BDFL, but allow for their removal (PyTorch) or direct appointment of a successor (pandas) in consultation with the core maintainers. Neither explicitly mentions eligibility criteria for BDFL (i.e., do they need to already be a core maintainer, or can they be anyone at all).
 - The core maintainers / Core Team / EC / Project Team exercise the same authority that the numba dev team already does

Interestingly:
 - PyTorch goes great lengths to divorce itself from specific insitutions, insisting on an individual/merit-based governance structure.
 - conda, on the other hand, defines a "Provisional Steering Council Member" position to organizations that fund at least one FTE contributing to the conda ecosystem.

There are a lot of limitations / expectations on provisional steering council members, and this likely ties back to PyTorch still being ostensibly a Meta project (and therefore not short on resources), but something to consider nonetheless: **is diverisfying the core numba maintainer base beyond Anaconda an explicit goal?**

### Decision making

If not spelled out in the previous section, this is where the process for decision making would be enumerated. PyTorch does a great job of this, especially in separating out "uncontroversial changes" from "controversial" ones and providing examples of each.

### Partners and Funding

If there are any institutional partners and/or external funding sources, this is where they would be enumerated and the specifics of their roles defined, as well as explanations for how other future opportunities could fit in.

For example: if numba became a NumFOCUS sponsored project, this is where the details of that would be spelled out (though any role that NumFOCUS has in the day-to-day decision-making would be in the previous section).

### FAQ / Non-compliance / Other components 

Any final items to wrap things up.