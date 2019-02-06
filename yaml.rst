YAML
====

YAML syntax
-----------

A value::

    value

A value named "pie"::

    pie: value

A list::

    - 1
    - 2
    - 'a string'

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

