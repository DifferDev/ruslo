# RuSLo
PHP **Ru**ntime **S**uperglobals **Lo**ader: a project to put legacy PHP on Runtime executions.

* Runtime > _POST _GET _FILES _SERVER _SESSION _COOKIES
* OutputBuffer > Runtime - this could be dificult!

## Proposal

This project is a reverse of the Symfony/Runtime component, in case when we need the PHP SuperGlobals working on a runtime environment.

I decided to create this component to help legacy PHP code to run as CLI Runtime, without changing the base code.

It'll help to migrate your app to performant async servers using libs like: PHPReact, RoadRunner, AWS Lambda and etc...

## Starter

Here's a list of the implementantions that we need:

Boot:
- Create RuSLo\Loader\Bootstrap
- Create RuSLo\Loader\Interface\Input
- Create RuSLo\Loader\Interface\GlobalsLoader
- Code RuSLo\Loader\AWSLambdaToSuperGlobals

Result:
- Create RuSLo\Result\Interface\Output

Execution:
- Create RuSLo\Executor

Features target for future implementantions:

- RuSLo\Loader\PSR7ToSuperGlobals
- RuSLo\Loader\PHPReactToSuperGlobals
- RuSLo\Loader\SwooleToSuperGlobals
- RuSLo\Loader\RoadRunnerToSuperGlobals

**This is an experimental component, please report any bug or problem, everyone is free to colaborate, thank you.**

This is a start, so there is only the branch **main** yet.

Author @leoqbc
