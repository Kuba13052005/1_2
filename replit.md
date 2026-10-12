# Imported Java/Maven project

## Run on Replit

This project is a Java console application. Its entry point is
`src/main/java/Main.java`, which prints a greeting and then exits.

- Click **Run** to execute the configured `Start application` console workflow.
  Expected output: `Hello world JPWP2!`. The program then exits normally;
  it does not serve a web page.
- Build and test manually with `mvn test`. The build succeeds, but there are
  currently no active tests.
- Run the entry point directly with `javac -d . src/main/java/Main.java && java -cp . Main`.

The `java-graalvm22.3` Replit module provides Java, Maven, and Java editor tools.
Keep those tools in the module rather than adding duplicate legacy Java
packages to `replit.nix`; the imported legacy package references prevented
the environment from loading.
No secrets or external services are required.
