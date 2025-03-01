---
title: EXID-TYPE
permalink: /terms/v7/EXID-TYPE.html
layout: none
redirect-from:
  - /terms/v7/EXID-TYPE
...

```

%YAML 1.2
---
lang: en-US

type: structure

uri: https://gedcom.io/terms/v7/EXID-TYPE

standard tag: TYPE

specification:
  - Type
  - |
    The authority issuing the `EXID`, represented as a URI. It is recommended that
    this be a URL.
    
    If the authority maintains stable URLs for each identifier it issues, it is
    recommended that the `TYPE` payload be selected such that appending the `EXID`
    payload to it yields that URL. However, this is not required and a different
    URI for the set of issued identifiers may be used instead.
    
    Registered URIs are listed in [exid-types.json], where fields include:
    
    - "label": a short string suitable for display in a user interface.
    - "type": The URI representing the authority issuing the `EXID`.
    - "description": A description of the meaning of the `EXID`.
    - "contact": A contact email address for the person or organization registering
      the URI.
    - "change-controller": The name or contact information for the person or
      organization authorized to update the registration.
    - "fragment": If present, indicates a short string that can be used as a label
      for a fragment identifier appended to the URI. If absent, indicates that
      fragment identifiers are not used with the URI.
    - "reference": A URL with more information about the meaning of the `EXID`.
      Such information should explain the uniqueness and expected durability of the
      identifier.
    
    Additional type URIs can be registered by filing a [GitHub pull request].

label: 'Type'

payload: http://www.w3.org/2001/XMLSchema#string

substructures: {}

superstructures:
  "https://gedcom.io/terms/v7/EXID": "{0:1}"
...

```
