# Site Reliability Engineering

## 1 Introduction

* split between dev and ops is pathological and costly
* operations teams and development are in conflict over how quickly software can be released
* dev teams want to launch new features and see them adopted by users
* ops teams want to make sure the service doesn't break
* ops and devs are in tension because most outages are caused by change - new config, feature launch, user traffic

* SREs design and implement automation with software to replace human labor
* services that basically run and repair themselves
* the number of SREs needed to run, maintain, and improve a system scales sublinearly with the size of the system

* SRE team is responsible for:
  * availability
  * latency
  * performance
  * efficiency
  * change management
  * monitoring
  * emergency responsible
  * capacity planning

* cap operational work for SREs at 50% of their time
* remaining time should be spent on project work
* this is accomplished by monitoring the amount of operational work done by SREs and redirecting excess operational work to the product development teams:
  * reassigning bugs and tickets to dev managers
  * integrating devs into on-call pager rotations
* the redirection ends when the operational load drops back to 50% or lower
* provides a feedback mechanism - guides devs to build systems that don't need manual intervention
* reduce the app's operational load
* postmortems should be documented
* postmortems that did not trigger a page are valuable because they point to clear monitoring gaps
* investigation should:
  * establish what happened in detail
  * find all root causes
  * assign actions to correct the problem or improve how it's addressed

* attempt to automate everything
* playbook for responding to errors improves the amount of time for resolving issues

## 2 The Production Environment at Google, from the Viewpoint of an SRE

* a bunch of stuff about google proprietary software and infrastructure
* all of google's services communicate using Remote Procedure Call (RPC)

## 3 Embracing Risk
