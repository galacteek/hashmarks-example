.. _hashmarks-format:

Hashmarks YAML format
----------------------

Your hashmarks must be stored in the *hashmarks*
folder, in YAML files. All files ending with *.yaml*
are imported. The format is as follows::

    hashmarks:
      - url: /ipfs/bafybeidlrwhpvr5nfbeqnga4luhrh6gk7sa7g4sj2gxo37sxvqvj5tc2gq
        title: Title
        description: Description
        datecreated: '2020-04-23T18:00:00-00:00'
        category: my/category
        tags:
          - '@Earth#dapp'
          - '#ipfs'

The only mandatory fields for an hashmark definition are
*url* (which can be an ENS URL like ens://ethereum.eth
or a path to an IPFS object) and *title*.

Tags are in the format *@Planet#tag* or just *#tag* (in which
case it is treated as *@Earth#tag*. Using a tag such as
*@Mars#climate* to tag the wikipedia article of Mars's climate
is appropriate for example. Creation dates, if specified, must be
in the rfc3339 format.

The *infos.yaml* just contains information about the source (name
and UID)
