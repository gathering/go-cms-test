# Gathering.org CMS tests

A collection of CMS demo setups on systems we are considering for new Gathering.org.

Each demo lives in a separate folder aptly named by which CMS and what type (mostly needed if we have multiple of same system) of demo it is.

Feel free to add more examples and documentation as needed.

## Current Content Management Systems being evaluated

- [Wagtail](https://wagtail.org/) - Python and Django - [Go to Bakery demo](./wagtail-bakery/README.md)
- [Payload](https://payloadcms.com/) - Typescript - [Go to Website demo](./payload-website/README.md) (Runs v2 which was just released, PG support was not yet stable during testing so using Mongo DB)

## Relevant notes

- What we are looking for
    - Something that "any" developer can figure out (but specifically the ones in TG crew)
    - Headless CMS. Ie. they "only" provide admin pages and an API (Preferably REST or GraphQL)
    - Something that is developer centric. Ie. we want it to be as easy as possible for a developer to adjust models and similar, and harder/impossible for users.
    - A solution that allows us to create any content types and relations TG might come up with
    - A solution that allows us to create new workflows for certain content types (ex. an article has to be approved by an editor before publishing)
    - Ability to extend CMS itself with new functionality if needed
    - Something that allows login via login providers (ex. SAML, OpenID Connect)
    - Preferably something that integrates well with known/common frontend frameworks (does it have a simple starting package?)
    - ...?
- Things to look out for
  - How easy are admin pages to use?
  - How easily can existing content types be modified?
  - How easily can new content types and settings pages be added?
  - What type of "extensions" are available (and how hard are they to make)?
- Demo sites will generally include some frontend component in order to display contents. Keep this in mind when evaluating, and try to ignore the non-cms parts.
