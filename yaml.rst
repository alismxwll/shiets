YAML
====

YAML syntax
-----------

A value::

    good

A value named "pie"::

    pie: good

A list::

    - 111
    - 222
    - 'string'

A list named "pie"::

    pie:
      - 111
      - 222
      - 'string'

Alternate list syntax::

    pie: [111, 222, 'string']

A dictionary::

    pie: tasty
    tea: tasty
    poo: 'not tasty'

A dictionary named "pie"::

    pie:
      type: pickle
      size: large
      shape: round

Alternative dictionary style::

    pie: {type: pickle, size: large, shape: round}

List of dictionaries::

    pies:
        -   type: pickle
            size: large
        -   type: yam
            size: small

