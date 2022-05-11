# java-add-SSL-cert-to-trusted.example

Sometimes you build java microservice, and calling https endpoint returns error like:Ж
    ```
    PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
    ```

This is example how to retrieve certificate, and add it into trusted for the java application.

# How to

## Compile class:

    ```shell
    javac SSLPoke.java
    ```

## Scripts
1. `DEV.ssl.build-full-cacerts` - main script to build certificates file
2. `DEV.ssl.check` - very simple java-application to check connection to the server


# Useful links
- http://confluence.atlassian.com/display/JIRA/Connecting+to+SSL+services
- https://gist.github.com/4ndrej/4547029 one more `SSLPoke` java class source??
