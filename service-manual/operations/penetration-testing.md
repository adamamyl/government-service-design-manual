---
layout: detailed-guidance
title: Vulnerability and penetration testing
subtitle: Identifying insecurities in your service
category: operations
type: guide
audience:
  primary: 
  secondary: developers, tech-archs
status: draft
breadcrumbs:
  -
    title: Home
    url: /service-manual
  -
    title: Operations
    url: /service-manual/operations
---

Ensuring web based systems and applications are secure requires more than just good design and development. In order to identify vulnerabilities it is often a good idea to involve an independent body to help find potential security problems before releasing to the public.

Sometimes referred to as **pen testing**, vulnerability and penetration testing is the act of analysing and testing a service for security problems. This is often a specialist activity done via a third party.

It's often a good idea to view security testing as an ongoing activity for any project, not as a final check.

## Involve the right people

Security is important to both a product and technical audience. It's essential that vulnerability testing reports and the risks they identify are understood by non-technical audiences as well a developer audience. 

Security is rarely binary, in that it's not generally a matter of being secure or not, rather reducing the risks of a wide range of potential issues.

### Liaise with CESG

[CESG](http://www.cesg.gov.uk/Pages/homepage.aspx) are the National Technical Authority for Information Assurance. Based at Cheltenham they provide both standards and advice for information security. 

For any sizable project it is wise to engage with them as early as possible. They can provide guidance and expertise on potential problems and help you make sure the right things are tested.

### Use in-house expertise as well as external services

Testing for security issues should be done throughout the development of a service, as well as regularly when it's up and running. Having third parties do this testing is a good way of introducing genuine experts and getting a different view on something. However it's also important to make sure the team building the software know that security is the responsibility of the team, and not something that is outsourced.

## Not just software

Remember that when testing for vulnerability to look at the whole system, not just the software involved. 

An obvious example would be physical security (where is the equipment housed and how secure is it?) but a more interesting example is often the interplay between an online system and a call centre. 

It may be that by using information available from a call centre you can exploit the software system in some way. For instance, [getting a call-centre team to change an email address on record for someone else, and then using a forgotten password facility which relies on the email address being trusted](http://www.emptyage.com/post/28679875595/yes-i-was-hacked-hard-here).

## Automate where possible

Although some level of exploratory manual testing is always a good idea when looking for vulnerabilities this is time-consuming and expensive. Having some level of automation can often be a good idea.

This may take the form of tests written or tools used specifically to test the security of a feature. For instance [static analysis](http://en.wikipedia.org/wiki/Static_program_analysis) or [input fuzz testing](http://en.wikipedia.org/wiki/Fuzz_testing).

## Why we do this

The web is a hostile environment, and the nature of Government services means they can be targets for a wide range of different threats; from financially motivated criminals and online activists up to nation states. Even where personal or sensitive information is not at risk the reputation of government can be damaged by even the smallest issues.

Web application exploits tend to follow a relatively small number of common patterns, which means automated and manual testing, as well as awareness of these common problems can have a drastic effect on the security of the system.

[The Government Accreditation processes](http://www.cesg.gov.uk/servicecatalogue/PGAS/Pages/PGAS.aspx) mandate some form of vulnerability testing, often working with [CHECK approved suppliers](http://www.cesg.gov.uk/finda/Pages/CHECKSearch.aspx). This should be viewed as the minimum effort required. 

## Further reading

* [OWASP Top 10](https://www.owasp.org/index.php/Top_10_2010)
* [CESG](http://www.cesg.gov.uk/)
* [CHECK provider search](http://www.cesg.gov.uk/finda/Pages/CHECKSearch.aspx)
* [Fuzz testing](http://en.wikipedia.org/wiki/Fuzz_testing)
