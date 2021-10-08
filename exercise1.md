
# CI/CD pipeline for an API built with Python and FastAPI

## Linting

It's an important step since it allows us to write code that is easier to read, maintain and modify, especially after some time of not working with a codebase. It also checks for errors so we can guarantee things like using the right types when passing data around. This last task is easier now because Python added static typing in version 3.5.

Some popular linters for Python that check both for logical and stylistic errors are Flake8 and Pylama. Personally, for automatic and consistent code styling, I like to use the standalone Black formatter.

## Testing

This step executes our code and checks that the results obtained are the same as the expected ones. If our modifications to the codebase don't change the output, the tests should be able to run and pass without any modification.

The basic tool for this is "unittest", a testing framework already bundle with the Python language. An alternative (they are not mutually exclusive) is "doctest", which also comes with the language itself and allows us to write the tests directly into the documentation strings.

## Building

An API built with Python and FastAPI doesn't need building, since it is an interpreted language and is deployed directly.

## Github Actions alternatives (cloud CI/CD solutions):

-   Gitlab CI: the CI offering directly from one of, if not the, biggest Github competitors.
-   CircleCI: offers cloud and self-hosted options, with a basic free tier for the cloud service. I see their ads ofter on YouTube. Can be integrated with Github.
-   Travis CI: one of the first services to offer a free tier for cloud-hosted CI/CD, according to Wikipedia. Can be integrated with Github.
-     
    

## Jenkins alternatives (self-hosted CI/CD solutions):

-   CircleCI can be self-hosted but requires a paid plan.
-   Travis CI: self-hosted option only for the enterprise tier.
-   Buddy: free and paid tiers.
-   Final builder: free and paid tiers.
-   CruiseControl: free and open source.
-   Integrity: free and open-source, but seems abandoned.
-   GoCD: free and open source.

## What to use in this case

In this case, I would suggest just using a cloud CI/CD solution, because it should be more than enough with the free tier of the mentioned services.
