[rundeck-archive](../../index.html)
# apitoken-list 

List the API tokens.

## SYNOPSIS

    rerun rundeck-archive:apitoken-list --password <> --url <> --user <>

### OPTIONS

* [    --password <>: the login password](../../options/password/index.html)
* [    --url <>: rundeck server url](../../options/url/index.html)
* [    --user <>: the login user name](../../options/user/index.html)

## README

Example
-------

List the API tokens for the "admin" user:

    rerun rundeck-archive: apitoken-list --url http://localhost:4440 --user admin --password admin
    
Each token is printed on a separate line.
In this example there are 3:
    
    V1pKunEs3scEc5Ke4v84ddU34DkO0Cdp
    R4OdEDKkkdVnDN8p05Dd9C1Doe2507ru
    5EsCDCrcDpUoPoNrSS4U2R0v071P9DDS

## TESTS

Use the `stubbs:test` command to to run test plans.

    rerun stubbs:test -m rundeck-archive -p apitoken-list

*Test plan sources*

* [apitoken-list-1](../../tests/apitoken-list-1.html)
  * it fails without a real test

## SCRIPT

To edit the command script for the rundeck-archive:apitoken-list command, 
use the `stubbs:edit`
command. It will open the command script in your shell EDITOR.

    rerun stubbs:edit -m rundeck-archive -c apitoken-list

*Script source*

* [script](script.html): `RERUN_MODULE_DIR/commands/apitoken-list/script`

## METADATA

* `NAME` = apitoken-list
* `DESCRIPTION` = "List the API tokens."
* `OPTIONS` = "password url user"

----

*Generated by stubbs:docs Wed May 22 19:51:18 PDT 2013*
